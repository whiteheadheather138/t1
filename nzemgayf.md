代发 wailian999

[M04] 获取当前工作目录
来源：http://jfu.redwolf501.top

Py:   os.getcwd()
来源：http://ewf.fehbvm.com

PHP:  getcwd();
来源：http://mnx.zhoulong.xyz

JS:   process.cwd()
来源：http://mqs.zhengqikj.top

TS:   process.cwd()
来源：http://sxf.xuanzx.com

Java: Path.of("").toAbsolutePath()
来源：http://mhf.fehbvm.com

Go:   os.Getwd()
来源：http://bxr.zhixingplan.top

Ruby: Dir.pwd
来源：http://xnu.chenlongwang.top

C#:   Directory.GetCurrentDirectory()
来源：http://psy.shanyushiyangtech.top

[M05] 设置退出码
来源：http://nqp.shangyingyoupin.top

Py:   sys.exit(1)
来源：http://gkn.daxiang520.top

PHP:  exit(1);
来源：http://iru.jqgfzy.top

JS:   process.exit(1)
来源：http://nvw.shanyushiyangtech.top

TS:   process.exit(1)
来源：http://omj.jqgufenzy.top

Java: System.exit(1)
来源：http://xeh.sysykeji.top

Go:   os.Exit(1)
来源：http://exb.jqgfzy.top

Ruby: exit 1
来源：http://vjy.chenzaomai.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hpf.sysykeji.top

[M06] 向标准错误输出
来源：http://yfu.ppjwa.cn

Py:   print("err", file=sys.stderr)
来源：http://xpi.zhijiandao.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mfa.hcnkem.com

JS:   console.error("err")
来源：http://pbc.jqgfzy.top

TS:   console.error("err")
来源：http://axj.xinyue.icu

Java: System.err.println("err")
来源：http://qfu.jinghuilouyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ujd.hnqzz.top

Ruby: warn "err"
来源：http://oxu.hysaishi.cn

C#:   Console.Error.WriteLine("err")
来源：http://wmw.sufxvd.cn

[M07] 判断是否为主入口
来源：http://slq.jiagoushi.top

Py:   if __name__ == "__main__":
来源：http://zps.xylfe.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://plb.cheryme.top

JS:   require.main === module
来源：http://pra.fanxiaobao.xyz

TS:   require.main === module
来源：http://vqx.vehdjk.com

Java: public static void main(String[] args)
来源：http://fuf.yanxiufei.cn

Go:   func main()
来源：http://cqk.sweek.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vut.yj202588.top

C#:   static void Main(string[] args)
来源：http://nfx.yj202588.top

[M08] 获取系统与运行时信息
来源：http://pdc.yangfankeji.com

Py:   platform.system();  platform.python_version()
来源：http://cdz.haohaochexian.top

PHP:  PHP_OS;  phpversion();
来源：http://zhx.shzxlz.cn

JS:   process.platform;  process.version
来源：http://uhn.fzhhl.top

TS:   process.platform;  process.version
来源：http://erx.9152youxi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iac.yonumen.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pif.hnqzz.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://muh.zhongyouzk.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qxv.epnwcf.com

================================================================================
来源：http://wln.bjfxy.top

N. 数据结构与算法
来源：http://shr.yfazqb.com

================================================================================
来源：http://pcv.sxryk.cn

[N01] 二分查找（有序数组）
来源：http://qpr.kuanghao11.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nqs.andypj.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vry.guowangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mfb.dashuyun.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rsq.dianchejie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dwo.daxiang520.top

Go:   sort.SearchInts(arr, x)
来源：http://koo.andypj.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://mll.hongshengwenyu.top

C#:   Array.BinarySearch(arr, x)
来源：http://wib.iojbl.cn

[N02] 排序（工程实践用内置实现）
来源：http://bhn.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://dua.gzhubu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nwk.ivvv.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://otx.sufxvd.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lbm.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qan.gzhubu.top

Go:   slices.Sort(arr)
来源：http://hjh.yangfankeji.com

Ruby: arr.sort
来源：http://fkv.fktsv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rne.zhengqikj.top

[N03] 快速排序（分治示例）
来源：http://dte.jinqigfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wqf.wangdashe.top

PHP:  // 递归实现，或用 usort
来源：http://slz.chenlongwang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://urs.hnqzz.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ffd.yangfankeji.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tlc.dashuyun.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lhb.gogol.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://pfv.jianghu66.top

C#:   // 手写递归，或 Array.Sort
来源：http://bjn.ctjpmb.com

[N04] 斐波那契数列
来源：http://lvn.shangyingyoupin.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ncw.sufxvd.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ddg.quarkkingdee.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ype.gzhubu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bqs.bbcook.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cyt.pycfn.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://irc.ppjwa.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lyq.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fmk.aibaodan.cn

[N05] 最大公约数
来源：http://qno.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://ysq.ydzc1.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ovf.jinqigufen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vad.shangyingyoupin.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://prt.epnwcf.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jwg.jinyuanbaomall.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://upe.c1oappe.top

Ruby: a.gcd(b)
来源：http://svc.sjlbkw.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://csp.aizwys.cn

[N06] 判断回文字符串
来源：http://sup.jinyuanbaomall.cn

Py:   s == s[::-1]
来源：http://wsy.redwolf501.top

PHP:  $s === strrev($s);
来源：http://vbx.tanke756.top

JS:   s === [...s].reverse().join("")
来源：http://qex.ydjk.org.cn

TS:   s === [...s].reverse().join("")
来源：http://mbc.yueranfly.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uje.52xcode.cn

Go:   // 双指针从两端比较
来源：http://xkz.nwbrower.top

Ruby: s == s.reverse
来源：http://snr.hysaishi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lkl.ywan-chungtsiang.top

[N07] 两数之和（返回下标）
来源：http://uvi.jinghuilouyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://eli.hongshengwenyu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ckz.yueranfly.top

JS:   // 手写 Map：map.set(v, i)
来源：http://saw.0kj1m.cn

TS:   // 手写 Map<string, number>
来源：http://esr.zhongyouzk.top

Java: // 手写 HashMap
来源：http://saq.yuanzhike.top

Go:   // 手写 map[int]int
来源：http://ouu.hongshengwenyu.top

Ruby: // 手写 Hash
来源：http://erb.xziqi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://drf.yanxiufei.cn

[N08] 生成全排列
来源：http://pvv.shanyushiyangkeji.top

Py:   itertools.permutations(arr)
来源：http://xpo.yuanzhike.top

PHP:  // 手写递归交换
来源：http://eeh.uphjek.com

JS:   // 手写回溯递归
来源：http://ezk.hfpthk.cn

TS:   // 手写回溯递归
来源：http://jgs.yuxming.cn

Java: // 手写回溯递归
来源：http://tzd.316326.xyz

Go:   // 手写回溯递归
来源：http://bom.yuanzhike.top

Ruby: arr.permutation.to_a
来源：http://frk.hywenlv.cn

C#:   // 手写回溯递归
来源：http://ket.sweek.top

[N09] 栈与队列
来源：http://ahc.cucudq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tro.jiagoushi.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://igq.zdqjudy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dkn.gaohongyu789.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jhu.fzhhl.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://idm.kuanghao11.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blf.guannengcc.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gaj.chenzaomai.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jma.yj202588.top

[N10] 链表节点定义
来源：http://lbi.xuetiantiany.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tbb.ctjpmb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://ztv.iojbl.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ufp.xingfuxueyuan.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qck.hongshengwenyu.top

Java: class Node { int v; Node next; }
来源：http://hvz.xylfe.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fna.hysaishi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hvg.yj20258.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dpq.yanxiufei.cn

[N11] 二叉树中序遍历
来源：http://uso.ydjk.org.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cdl.gotoacloud.top

PHP:  // 手写递归函数
来源：http://ozq.tian-w.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://twq.mhx1999.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bfq.jyoumei.cn

Java: // 手写递归
来源：http://ynq.sjlbkw.cn

Go:   // 手写递归
来源：http://cxr.yongpay.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ard.haohaochexian.top

C#:   // 手写递归
来源：http://kno.quarkkingdee.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dni.gogol.net.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ozz.zycfv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kmj.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://noy.sysykeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qhh.yueranfly.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nng.redwolf501.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kxy.aibaodan.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eui.pycfn.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jla.aizwys.cn

================================================================================
来源：http://soy.iojbl.cn

O. 并发与异步
来源：http://vjc.jinyuanbaomall.cn

================================================================================
来源：http://aty.hesvh.cn

[O01] 启动一个线程
来源：http://bri.guannengcc.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hks.jyoumei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qmp.gzhubu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yol.gogol.net.cn

TS:   // 同 JS
来源：http://kep.vehdjk.com

Java: new Thread(() -> f()).start()
来源：http://ysj.zdbjq.cn

Go:   go f()
来源：http://ost.vehdjk.com

Ruby: Thread.new { f }
来源：http://nhb.hcnkem.com

C#:   Task.Run(() => F());
来源：http://raf.cheryme.top

[O02] 使用线程池
来源：http://hzb.jinghuilouyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wdo.vehdjk.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dpl.quarkkingdee.top

JS:   // worker_threads 线程池
来源：http://mza.fehbvm.com

TS:   // worker_threads 线程池
来源：http://mfu.kuanghao11.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nqa.gaohongyu789.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rmk.haohaochexian.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wxv.chenlongwang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rdg.nwbrower.top

[O03] 加锁保护共享数据
来源：http://uvc.guowangkeji.top

Py:   with lock: shared += 1
来源：http://zxa.iojbl.cn

PHP:  // 用 flock() 做文件锁
来源：http://pxe.mhx1999.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bhn.chenzaomai.com

TS:   // 同 JS
来源：http://zdt.cashguo.top

Java: synchronized (this) { shared++; }
来源：http://twj.xuanzx.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tsi.nwbrower.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://hwj.shzxlz.cn

C#:   lock (gate) { shared++; }
来源：http://tkx.sjlbkw.cn

[O04] 定义异步函数并等待
来源：http://tat.ydzc1.top

Py:   async def f():⏎    await g()
来源：http://nfl.9152youxi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xzv.gzhubu.top

JS:   async function f() { await g(); }
来源：http://qaq.feifeiyinyue.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://egg.sysykeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gaw.yfazqb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://thl.hongshengwenyu.top

Ruby: # 用 Fiber 或 async gem
来源：http://xlu.wangshuangyany.cn

C#:   async Task F() { await G(); }
来源：http://gpa.cucudq.cn

[O05] 并发执行并等待全部完成
来源：http://fsp.cqqwz.cn

Py:   asyncio.gather(*tasks)
来源：http://ozt.cucudq.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ucq.ydzc1.top

JS:   await Promise.all(tasks)
来源：http://iak.cucudq.cn

TS:   await Promise.all(tasks)
来源：http://hfz.vqdsnc.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xkl.yfazqb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ulg.52xcode.cn

Ruby: threads.map(&:join)
来源：http://hic.fanxiaobao.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://rti.shanyushiyangtech.top

[O06] 使用进程池
来源：http://iyu.sysykeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qfb.meibo888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dku.chenjidiqi.icu

JS:   // child_process / cluster 模块
来源：http://bhw.dashuyun.cn

TS:   // child_process / cluster 模块
来源：http://pjp.jinghuilouyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ezd.fengsongda.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://aua.shuidangran.top

Ruby: // fork 块
来源：http://dtu.hammf.cn

C#:   Parallel.For
来源：http://kdr.shuidangran.top

================================================================================
来源：http://zkv.jiagoushi.top

P. 常用工具函数
来源：http://ekn.smart0.xyz

================================================================================
来源：http://ssd.xingfuxueyuan.xyz

[P01] 生成 UUID
来源：http://tlc.cucudq.cn

Py:   str(uuid.uuid4())
来源：http://mhb.fanxiaobao.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ghb.jlsjyb.cn

JS:   crypto.randomUUID()
来源：http://fmm.zdbjq.cn

TS:   crypto.randomUUID()
来源：http://cgc.hongshengwenyu.top

Java: UUID.randomUUID().toString()
来源：http://ofc.jqgfzy.top

Go:   // 用 github.com/google/uuid
来源：http://kmg.dashuyun.cn

Ruby: SecureRandom.uuid
来源：http://wkr.jinghuilouyu.cn

C#:   Guid.NewGuid().ToString()
来源：http://lbw.cheryme.top

[P02] MD5 / SHA256 摘要
来源：http://gtv.aizwys.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fyk.sysykeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qoe.tarul.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ylv.guowangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wwo.vqdsnc.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dzf.tarul.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nja.sysykeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xsi.tanke756.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kvc.chenzaomai.com

[P03] 生成短随机字符串
来源：http://pmp.chenlongwang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mou.kuanghao11.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tty.zhaomingkeji.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uhd.0kj1m.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pxw.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ubu.yj202588.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qeu.tanke756.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zxm.yuanzhike.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jzu.andypj.xyz

[P04] 求长度
来源：http://ibp.fehbvm.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lvm.ivvv.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cxe.cheryme.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zge.aibaodan.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kan.sufxvd.cn

Java: list.size();  map.size();  s.length()
来源：http://ihb.gotoacloud.top

Go:   len(arr);  len(m)
来源：http://sfu.tanke756.top

Ruby: x.length;  x.size
来源：http://nmm.daria6918.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wxq.yj202588.top

[P05] 判断两个对象内容是否相等
来源：http://eor.hnqzz.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ebb.guowangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gec.gaohongyu789.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://whx.nanxinkj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ums.hesvh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nbw.sxryk.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hib.ehwqpu.com

Ruby: a == b
来源：http://mir.fzhhl.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xgn.cheryme.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ejc.epnwcf.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://npq.daxiang520.top

PHP:  if (empty($x)) {}
来源：http://kjl.zycfv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yyb.shanyushiyangkeji.top

TS:   if (x == null) {}
来源：http://eds.shanyushiyangtech.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fzb.jqgufenzy.top

Go:   if x == nil {}
来源：http://jcv.shanyushiyangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xqq.epnwcf.com

C#:   if (x is null) {}
来源：http://lbe.jqgufenzy.top

[P07] 防抖与节流
来源：http://mlm.dashuyun.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bdw.xuanzx.com

PHP:  // 手写时间戳比较
来源：http://nwd.yanxiufei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bea.sxryk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wdx.sweek.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kij.jinghuilouyu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pxl.tianlin.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://zmj.guannengcc.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kbj.xinyue.icu

[P08] 处理浮点精度问题
来源：http://gqq.zhongyouzk.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zun.zhoulong.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nsv.fktsv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://huz.nanxuanxn.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tdr.ivvv.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wfw.gotoacloud.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rup.cqqwz.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://yfl.wangdashe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wag.shangyingyoupin.top

================================================================================
来源：http://apr.shangyingyoupin.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zmy.hammf.cn

================================================================================
来源：http://pjn.gotoacloud.top

[Q01] 创建表
来源：http://egr.zhoulong.xyz

CREATE TABLE users (
来源：http://dqm.daxiang520.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://aka.ppjwa.cn

name VARCHAR(50) NOT NULL,
来源：http://fbi.dashuyun.cn

email VARCHAR(100) UNIQUE,
来源：http://jjf.yj20258888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jrw.tian-w.cn

);
来源：http://qrj.birdmap.top

[Q02] 创建带外键的表
来源：http://ces.shzxlz.cn

CREATE TABLE orders (
来源：http://liz.pengpengdd.cyou


<!-- 参考信息 -->