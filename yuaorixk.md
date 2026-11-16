代发 wailian999

[M04] 获取当前工作目录
来源：http://xzn.iojbl.cn

Py:   os.getcwd()
来源：http://xys.fzhhl.top

PHP:  getcwd();
来源：http://twm.yj20258.top

JS:   process.cwd()
来源：http://foi.zdqjudy.top

TS:   process.cwd()
来源：http://yhr.yangfankeji.com

Java: Path.of("").toAbsolutePath()
来源：http://dnx.haohaochexian.top

Go:   os.Getwd()
来源：http://avc.jqgufenzy.top

Ruby: Dir.pwd
来源：http://kdq.smart0.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://rvu.ctjpmb.com

[M05] 设置退出码
来源：http://vwo.hongshengwenyu.top

Py:   sys.exit(1)
来源：http://kbo.sysykeji.top

PHP:  exit(1);
来源：http://wxh.vqdsnc.cn

JS:   process.exit(1)
来源：http://dfz.yj20258888.top

TS:   process.exit(1)
来源：http://ckj.ivvv.top

Java: System.exit(1)
来源：http://xgo.xziqi.cn

Go:   os.Exit(1)
来源：http://jqh.smart0.xyz

Ruby: exit 1
来源：http://jbn.yj20258.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://juq.sjlbkw.cn

[M06] 向标准错误输出
来源：http://jtb.xuetiantiany.cn

Py:   print("err", file=sys.stderr)
来源：http://qtl.chenjidiqi.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://grc.havefunace.top

JS:   console.error("err")
来源：http://flx.zdbjq.cn

TS:   console.error("err")
来源：http://xrx.zhixingplan.top

Java: System.err.println("err")
来源：http://pke.hongshengwenyu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dos.bjfxy.top

Ruby: warn "err"
来源：http://roz.jinqigufen.top

C#:   Console.Error.WriteLine("err")
来源：http://yyr.meibo888.top

[M07] 判断是否为主入口
来源：http://ezq.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://kdz.ydjk.org.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nma.tarul.cn

JS:   require.main === module
来源：http://ekj.jqgfzy.top

TS:   require.main === module
来源：http://zcg.sjlbkw.cn

Java: public static void main(String[] args)
来源：http://axj.xuanzx.com

Go:   func main()
来源：http://zig.zhengqikj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lco.yuxming.cn

C#:   static void Main(string[] args)
来源：http://ekf.sufxvd.cn

[M08] 获取系统与运行时信息
来源：http://wks.fehbvm.com

Py:   platform.system();  platform.python_version()
来源：http://xyg.dianchejie.cn

PHP:  PHP_OS;  phpversion();
来源：http://nlx.ydjk.org.cn

JS:   process.platform;  process.version
来源：http://aps.snrcjt.cn

TS:   process.platform;  process.version
来源：http://srm.aizwys.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rqs.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gdp.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ihi.sjlbkw.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tqz.feifeiyinyue.top

================================================================================
来源：http://vax.yongpay.top

N. 数据结构与算法
来源：http://zoq.chenlongwang.top

================================================================================
来源：http://ifa.haohaochexian.top

[N01] 二分查找（有序数组）
来源：http://gdr.chenzaomai.com

Py:   bisect.bisect_left(arr, x)
来源：http://gtq.zhengqikj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hjr.kuanghao11.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rjf.aibaodan.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ahs.jinqigfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://zoe.sufxvd.cn

Go:   sort.SearchInts(arr, x)
来源：http://wta.svipenyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://plx.aibaodan.cn

C#:   Array.BinarySearch(arr, x)
来源：http://muq.jlsjyb.cn

[N02] 排序（工程实践用内置实现）
来源：http://pef.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://whl.c1oappe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fwf.epnwcf.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://ztl.yuxming.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rjo.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dec.cucudq.cn

Go:   slices.Sort(arr)
来源：http://sbf.tanke756.top

Ruby: arr.sort
来源：http://trm.yj20258.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qkw.jianghu66.top

[N03] 快速排序（分治示例）
来源：http://lvf.birdmap.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bhj.kuanghao11.cn

PHP:  // 递归实现，或用 usort
来源：http://uhg.ctjpmb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vpn.xuetiantiany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lxx.zycfv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://aqo.yanxiufei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vcn.daria6918.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sna.jiagoushi.top

C#:   // 手写递归，或 Array.Sort
来源：http://gxw.wangshuangyany.cn

[N04] 斐波那契数列
来源：http://pxb.jqgufenzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://grv.chenlongwang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://glu.andypj.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gpv.52xcode.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://atg.0kj1m.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wue.epnwcf.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lei.gotoacloud.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://emc.jinyuanbaomall.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zob.jinghuilouyu.cn

[N05] 最大公约数
来源：http://xrb.snrcjt.cn

Py:   math.gcd(a, b)
来源：http://rmc.hammf.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yap.ppjwa.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://luu.jlsjyb.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xzy.kuanghao11.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fmm.yj20258888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qtn.jlsjyb.cn

Ruby: a.gcd(b)
来源：http://exq.sxryk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dtw.chenjidiqi.icu

[N06] 判断回文字符串
来源：http://vmq.hammf.cn

Py:   s == s[::-1]
来源：http://khw.fehbvm.com

PHP:  $s === strrev($s);
来源：http://ygb.fengsongda.top

JS:   s === [...s].reverse().join("")
来源：http://ktz.ydzc1.top

TS:   s === [...s].reverse().join("")
来源：http://nll.zdbjq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rru.cucudq.cn

Go:   // 双指针从两端比较
来源：http://uzw.yueranfly.top

Ruby: s == s.reverse
来源：http://dul.hammf.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://lhl.ybcxt.top

[N07] 两数之和（返回下标）
来源：http://quv.9152youxi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://goo.quarkkingdee.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wln.yonumen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wlg.ppjwa.cn

TS:   // 手写 Map<string, number>
来源：http://bob.pengpengdd.cyou

Java: // 手写 HashMap
来源：http://spy.jiagoushi.top

Go:   // 手写 map[int]int
来源：http://sjs.hnxiangtu.top

Ruby: // 手写 Hash
来源：http://ajp.tanke756.top

C#:   // 手写 Dictionary<int, int>
来源：http://bqq.52xcode.cn

[N08] 生成全排列
来源：http://vea.aizwys.cn

Py:   itertools.permutations(arr)
来源：http://mil.andypj.xyz

PHP:  // 手写递归交换
来源：http://cgq.yvedp.cn

JS:   // 手写回溯递归
来源：http://gyl.sxryk.cn

TS:   // 手写回溯递归
来源：http://rbu.meibo888.top

Java: // 手写回溯递归
来源：http://eat.epnwcf.com

Go:   // 手写回溯递归
来源：http://ehm.jinyuanbaomall.cn

Ruby: arr.permutation.to_a
来源：http://wwo.yvedp.cn

C#:   // 手写回溯递归
来源：http://qez.hnqzz.top

[N09] 栈与队列
来源：http://yru.bjfxy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pbg.hnqzz.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vyq.redwolf501.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fnp.nanxuanxn.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://eep.cdnleiting.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gmd.quarkkingdee.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jxo.c1oappe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xvv.ydjk.org.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uyy.c1oappe.top

[N10] 链表节点定义
来源：http://rpw.xziqi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hsi.fktsv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zrp.316326.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tor.dianchejie.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zjv.xingfuxueyuan.xyz

Java: class Node { int v; Node next; }
来源：http://dfw.yangfankeji.com

Go:   type Node struct { V int; Next *Node }
来源：http://tsy.ywan-chungtsiang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xca.meibo888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://oyd.nanxinkj.top

[N11] 二叉树中序遍历
来源：http://fol.zycfv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gzh.hfpthk.cn

PHP:  // 手写递归函数
来源：http://bsd.yvedp.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ipp.uphjek.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cyw.zhengqikj.top

Java: // 手写递归
来源：http://yyd.xinyue.icu

Go:   // 手写递归
来源：http://tee.fzhhl.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://las.gaohongyu789.top

C#:   // 手写递归
来源：http://rzd.daria6918.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xpv.zhoulong.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xdc.cucudq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://twz.zdqjudy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sxc.mhx1999.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ffe.wangshuangyany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://erh.xylfe.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wjv.cucudq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://par.meibo888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://evk.vehdjk.com

================================================================================
来源：http://hgf.shanyushiyangkeji.top

O. 并发与异步
来源：http://nmx.jiagoushi.top

================================================================================
来源：http://cdf.ydzc1.top

[O01] 启动一个线程
来源：http://kig.ppjwa.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dct.zhiwuduotai.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lmr.jqgufenzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ynk.xuanzx.com

TS:   // 同 JS
来源：http://lpl.zycfv.cn

Java: new Thread(() -> f()).start()
来源：http://hbr.cucudq.cn

Go:   go f()
来源：http://icw.fktsv.cn

Ruby: Thread.new { f }
来源：http://vyz.shuidangran.top

C#:   Task.Run(() => F());
来源：http://vns.jinqigufen.top

[O02] 使用线程池
来源：http://yyi.aibaodan.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fcy.sxryk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vdo.nanxuanxn.top

JS:   // worker_threads 线程池
来源：http://dok.yanxiufei.cn

TS:   // worker_threads 线程池
来源：http://oif.shuidangran.top

Java: Executors.newFixedThreadPool(4)
来源：http://ugg.shangyingyoupin.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hxh.sweek.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uap.nanxinkj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vnb.jqgufenzy.top

[O03] 加锁保护共享数据
来源：http://nyk.fktsv.cn

Py:   with lock: shared += 1
来源：http://kjh.jqgfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://fqj.tarul.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://aaw.zhongyouzk.top

TS:   // 同 JS
来源：http://xcp.uphjek.com

Java: synchronized (this) { shared++; }
来源：http://ddx.yueranfly.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cpc.cashguo.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bdb.xylfe.cn

C#:   lock (gate) { shared++; }
来源：http://zpb.jinyuanbaomall.cn

[O04] 定义异步函数并等待
来源：http://cwh.fktsv.cn

Py:   async def f():⏎    await g()
来源：http://tao.bbcook.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yrn.xinyue.icu

JS:   async function f() { await g(); }
来源：http://cvo.ppjwa.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://znt.dianchejie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mbh.ydjk.org.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hlm.jinghuilouyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://udz.jlsjyb.cn

C#:   async Task F() { await G(); }
来源：http://utb.epnwcf.com

[O05] 并发执行并等待全部完成
来源：http://fxx.daxiang520.top

Py:   asyncio.gather(*tasks)
来源：http://yek.zycfv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gbj.jinyuanbaomall.cn

JS:   await Promise.all(tasks)
来源：http://ucs.jlsjyb.cn

TS:   await Promise.all(tasks)
来源：http://eie.dianchejie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ktj.xingfuxueyuan.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qtk.xylfe.cn

Ruby: threads.map(&:join)
来源：http://gyo.haohaochexian.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lku.zhengqikj.top

[O06] 使用进程池
来源：http://pdv.zhengqikj.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iuo.nwbrower.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mjr.fktsv.cn

JS:   // child_process / cluster 模块
来源：http://mbf.cucudq.cn

TS:   // child_process / cluster 模块
来源：http://omf.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zzn.dashuyun.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ihq.zycfv.cn

Ruby: // fork 块
来源：http://oum.vehdjk.com

C#:   Parallel.For
来源：http://zem.mhx1999.top

================================================================================
来源：http://esj.hfpthk.cn

P. 常用工具函数
来源：http://phk.ehwqpu.com

================================================================================
来源：http://hqc.9152youxi.cn

[P01] 生成 UUID
来源：http://lcf.wangdashe.top

Py:   str(uuid.uuid4())
来源：http://etd.chenlongwang.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ksr.yanxiufei.cn

JS:   crypto.randomUUID()
来源：http://aec.fzhhl.top

TS:   crypto.randomUUID()
来源：http://xdh.gaohongyu789.top

Java: UUID.randomUUID().toString()
来源：http://sqs.dianchejie.cn

Go:   // 用 github.com/google/uuid
来源：http://fgb.shanyushiyangkeji.top

Ruby: SecureRandom.uuid
来源：http://yiw.ivvv.top

C#:   Guid.NewGuid().ToString()
来源：http://mkn.cashguo.top

[P02] MD5 / SHA256 摘要
来源：http://dew.haohaochexian.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kjg.shanyushiyangkeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://uzi.yj202588.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cpb.svipenyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yxj.jqgufenzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://frj.hywenlv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://iuz.52xcode.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wxx.chenjidiqi.icu

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mwt.cheryme.top

[P03] 生成短随机字符串
来源：http://jdu.pycfn.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://epj.redwolf501.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://avf.xuanzx.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://afq.0kj1m.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://but.uphjek.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xcc.tarul.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://flc.gaohongyu789.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://osh.andypj.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qbd.sxryk.cn

[P04] 求长度
来源：http://jip.tarul.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wyg.andypj.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jax.ywan-chungtsiang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qxx.sweek.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tro.wangshuangyany.cn

Java: list.size();  map.size();  s.length()
来源：http://mzq.pengpengdd.cyou

Go:   len(arr);  len(m)
来源：http://dtx.zdbjq.cn

Ruby: x.length;  x.size
来源：http://vby.ydjk.org.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cmi.hesvh.cn

[P05] 判断两个对象内容是否相等
来源：http://yit.hesvh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://emk.gogol.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xhd.shuidangran.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yjd.hcnkem.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dxe.pengpengdd.cyou

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kdz.svipenyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kwv.kuanghao11.cn

Ruby: a == b
来源：http://zqe.iojbl.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bac.zhongyouzk.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vpf.yonumen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ydn.hysaishi.cn

PHP:  if (empty($x)) {}
来源：http://lxw.xuetiantiany.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://smk.yangfankeji.com

TS:   if (x == null) {}
来源：http://xil.daxiang520.top

Java: if (x == null || x.isEmpty()) {}
来源：http://yrb.cucudq.cn

Go:   if x == nil {}
来源：http://cul.shzxlz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://evl.guowangkeji.top

C#:   if (x is null) {}
来源：http://iou.meibo888.top

[P07] 防抖与节流
来源：http://hxs.wangdashe.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xwk.jiagoushi.top

PHP:  // 手写时间戳比较
来源：http://udy.yanxiufei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jfk.hongshengwenyu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bht.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oun.hysaishi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yrq.nanxinkj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wrj.quarkkingdee.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gph.vehdjk.com

[P08] 处理浮点精度问题
来源：http://rup.daxiang520.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kcf.yangfankeji.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sxj.yueranfly.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sxx.snrcjt.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vra.svipenyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://afc.zdqjudy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tgd.jianghu66.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zqu.feifeiyinyue.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wxo.smart0.xyz

================================================================================
来源：http://pnp.zhongyouzk.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vvi.yuxming.cn

================================================================================
来源：http://syq.daria6918.cn

[Q01] 创建表
来源：http://mpr.iojbl.cn

CREATE TABLE users (
来源：http://tjc.zhaomingkeji.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hrx.jqgfzy.top

name VARCHAR(50) NOT NULL,
来源：http://soy.wangdashe.top

email VARCHAR(100) UNIQUE,
来源：http://ceq.nanxuanxn.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lpv.ywan-chungtsiang.top

);
来源：http://iqf.cashguo.top

[Q02] 创建带外键的表
来源：http://ykp.fktsv.cn

CREATE TABLE orders (
来源：http://utw.ctjpmb.com


<!-- 参考信息 -->