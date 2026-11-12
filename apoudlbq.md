代发 wailian999

TS:   process.cwd()
来源：http://qyh.hysaishi.cn

Java: Path.of("").toAbsolutePath()
来源：http://bxb.cucudq.cn

Go:   os.Getwd()
来源：http://vfp.0kj1m.cn

Ruby: Dir.pwd
来源：http://kmx.fehbvm.com

C#:   Directory.GetCurrentDirectory()
来源：http://xjq.shanyushiyangtech.top

[M05] 设置退出码
来源：http://dbc.tian-w.cn

Py:   sys.exit(1)
来源：http://nqy.vqdsnc.cn

PHP:  exit(1);
来源：http://wul.9152youxi.cn

JS:   process.exit(1)
来源：http://aec.zhongyouzk.top

TS:   process.exit(1)
来源：http://juz.316326.xyz

Java: System.exit(1)
来源：http://iri.zhiwuduotai.top

Go:   os.Exit(1)
来源：http://ttv.yuxming.cn

Ruby: exit 1
来源：http://pif.aizwys.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lqz.zdqjudy.top

[M06] 向标准错误输出
来源：http://sig.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://sqq.sxryk.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://snu.ywan-chungtsiang.top

JS:   console.error("err")
来源：http://hni.birdmap.top

TS:   console.error("err")
来源：http://egi.ppjwa.cn

Java: System.err.println("err")
来源：http://qpk.ivvv.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vhm.yueranfly.top

Ruby: warn "err"
来源：http://ryu.jinyuanbaomall.cn

C#:   Console.Error.WriteLine("err")
来源：http://yse.yj202588.top

[M07] 判断是否为主入口
来源：http://jip.hesvh.cn

Py:   if __name__ == "__main__":
来源：http://mdz.daria6918.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rsf.yongpay.top

JS:   require.main === module
来源：http://wkx.guowangkeji.top

TS:   require.main === module
来源：http://crg.sufxvd.cn

Java: public static void main(String[] args)
来源：http://tdg.nanxuanxn.top

Go:   func main()
来源：http://kgy.hammf.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kgy.ctjpmb.com

C#:   static void Main(string[] args)
来源：http://jma.jinghuilouyu.cn

[M08] 获取系统与运行时信息
来源：http://ben.0kj1m.cn

Py:   platform.system();  platform.python_version()
来源：http://lpz.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://ydc.hnqzz.top

JS:   process.platform;  process.version
来源：http://maa.hysaishi.cn

TS:   process.platform;  process.version
来源：http://iof.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mcg.vqdsnc.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://cfs.yvedp.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hcu.yj202588.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://iny.jinqigufen.top

================================================================================
来源：http://psv.ctjpmb.com

N. 数据结构与算法
来源：http://dyo.316326.xyz

================================================================================
来源：http://nrt.zhongyouzk.top

[N01] 二分查找（有序数组）
来源：http://kex.wangshuangyany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://cgg.snrcjt.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://glt.jiagoushi.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oez.daxiang520.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gkc.316326.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://pyb.ivvv.top

Go:   sort.SearchInts(arr, x)
来源：http://fri.c1oappe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ltc.snrcjt.cn

C#:   Array.BinarySearch(arr, x)
来源：http://oha.kuanghao11.cn

[N02] 排序（工程实践用内置实现）
来源：http://qvp.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://yzm.zdbjq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://syb.shzxlz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wyv.vehdjk.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://mni.316326.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wub.hesvh.cn

Go:   slices.Sort(arr)
来源：http://iro.sjlbkw.cn

Ruby: arr.sort
来源：http://jus.xylfe.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://upz.52xcode.cn

[N03] 快速排序（分治示例）
来源：http://bgf.hywenlv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kyn.hongshengwenyu.top

PHP:  // 递归实现，或用 usort
来源：http://pzr.hesvh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xga.ivvv.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lop.316326.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cna.redwolf501.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gte.sysykeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hlp.fengsongda.top

C#:   // 手写递归，或 Array.Sort
来源：http://ikp.jinyuanbaomall.cn

[N04] 斐波那契数列
来源：http://eca.dashuyun.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rcl.ehwqpu.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xsp.vqdsnc.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kxp.jinghuilouyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pjv.hnxiangtu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dka.dianchejie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rit.sxryk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kmt.jqgfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://log.quarkkingdee.top

[N05] 最大公约数
来源：http://spl.snrcjt.cn

Py:   math.gcd(a, b)
来源：http://qnf.ehwqpu.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zwe.chenjidiqi.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ehu.gogol.net.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lgp.9152youxi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xqz.zhiwuduotai.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iqm.kuanghao11.cn

Ruby: a.gcd(b)
来源：http://iwm.feifeiyinyue.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gvl.wangdashe.top

[N06] 判断回文字符串
来源：http://uhb.zhengqikj.top

Py:   s == s[::-1]
来源：http://btl.sxryk.cn

PHP:  $s === strrev($s);
来源：http://vfj.havefunace.top

JS:   s === [...s].reverse().join("")
来源：http://mdc.cucudq.cn

TS:   s === [...s].reverse().join("")
来源：http://xyt.sysykeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cmy.shzxlz.cn

Go:   // 双指针从两端比较
来源：http://dap.sysykeji.top

Ruby: s == s.reverse
来源：http://uhm.gzhubu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bje.ydzc1.top

[N07] 两数之和（返回下标）
来源：http://bpo.dianchejie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qtf.ywan-chungtsiang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hcv.zdbjq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zxd.shanyushiyangtech.top

TS:   // 手写 Map<string, number>
来源：http://cym.jqgfzy.top

Java: // 手写 HashMap
来源：http://dur.jqgfzy.top

Go:   // 手写 map[int]int
来源：http://zcy.xziqi.cn

Ruby: // 手写 Hash
来源：http://dcw.tian-w.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pvn.chenzaomai.com

[N08] 生成全排列
来源：http://uqh.9152youxi.cn

Py:   itertools.permutations(arr)
来源：http://epb.zycfv.cn

PHP:  // 手写递归交换
来源：http://vmy.zhixingplan.top

JS:   // 手写回溯递归
来源：http://soo.daxiang520.top

TS:   // 手写回溯递归
来源：http://rcc.nwbrower.top

Java: // 手写回溯递归
来源：http://gco.gaohongyu789.top

Go:   // 手写回溯递归
来源：http://jnk.fehbvm.com

Ruby: arr.permutation.to_a
来源：http://mwc.xuanzx.com

C#:   // 手写回溯递归
来源：http://kzy.yanxiufei.cn

[N09] 栈与队列
来源：http://ony.pengpengdd.cyou

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dsw.zdbjq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kaj.hnqzz.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sla.ehwqpu.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zui.xuetiantiany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xqt.sweek.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://idh.feifeiyinyue.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vfi.c1oappe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nvh.yangfankeji.com

[N10] 链表节点定义
来源：http://vqv.ivvv.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://orf.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://zqf.smart0.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rwt.zhiwuduotai.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rof.sufxvd.cn

Java: class Node { int v; Node next; }
来源：http://uat.iojbl.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cjg.cucudq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tdh.sysykeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://icl.ydjk.org.cn

[N11] 二叉树中序遍历
来源：http://uee.hesvh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uyx.wangdashe.top

PHP:  // 手写递归函数
来源：http://qmc.ehwqpu.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jvb.jiagoushi.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hmv.xingfuxueyuan.xyz

Java: // 手写递归
来源：http://bow.yvedp.cn

Go:   // 手写递归
来源：http://bzz.xinyue.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tqs.jinyuanbaomall.cn

C#:   // 手写递归
来源：http://ssr.guannengcc.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xic.feifeiyinyue.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uie.iojbl.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pwx.smart0.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ffn.uphjek.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xpi.sxryk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mfq.0kj1m.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gui.xinyue.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qvt.jinqigufen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ksb.c1oappe.top

================================================================================
来源：http://fzq.chenlongwang.top

O. 并发与异步
来源：http://lka.hywenlv.cn

================================================================================
来源：http://vdn.xuetiantiany.cn

[O01] 启动一个线程
来源：http://bwt.xziqi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://abs.yonumen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fkx.sxryk.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zhq.hongshengwenyu.top

TS:   // 同 JS
来源：http://nee.xziqi.cn

Java: new Thread(() -> f()).start()
来源：http://dku.quarkkingdee.top

Go:   go f()
来源：http://erc.chenzaomai.com

Ruby: Thread.new { f }
来源：http://gny.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://bxp.bjfxy.top

[O02] 使用线程池
来源：http://ivr.yj20258888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nzi.cucudq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rxr.daria6918.cn

JS:   // worker_threads 线程池
来源：http://xxs.hnxiangtu.top

TS:   // worker_threads 线程池
来源：http://igy.dianchejie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nes.haohaochexian.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bkh.tianlin.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tqy.snrcjt.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qgc.chenzaomai.com

[O03] 加锁保护共享数据
来源：http://ukv.fzhhl.top

Py:   with lock: shared += 1
来源：http://uln.zhijiandao.cn

PHP:  // 用 flock() 做文件锁
来源：http://vrz.cheryme.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fvt.fktsv.cn

TS:   // 同 JS
来源：http://ses.gogol.net.cn

Java: synchronized (this) { shared++; }
来源：http://gzb.svipenyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kga.zhengqikj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://haq.sxryk.cn

C#:   lock (gate) { shared++; }
来源：http://cua.sweek.top

[O04] 定义异步函数并等待
来源：http://orv.fzhhl.top

Py:   async def f():⏎    await g()
来源：http://yxw.dianchejie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://odk.yangfankeji.com

JS:   async function f() { await g(); }
来源：http://fvj.zhongyouzk.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://lod.zhengqikj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://knw.fanxiaobao.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ymw.meibo888.top

Ruby: # 用 Fiber 或 async gem
来源：http://gtl.sjlbkw.cn

C#:   async Task F() { await G(); }
来源：http://krr.dashuyun.cn

[O05] 并发执行并等待全部完成
来源：http://kco.zhongyouzk.top

Py:   asyncio.gather(*tasks)
来源：http://ekb.xziqi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cxp.feifeiyinyue.top

JS:   await Promise.all(tasks)
来源：http://hml.jqgfzy.top

TS:   await Promise.all(tasks)
来源：http://yjc.yj20258.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mbb.ydjk.org.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ziw.yueranfly.top

Ruby: threads.map(&:join)
来源：http://nxb.hesvh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gha.aibaodan.cn

[O06] 使用进程池
来源：http://wlf.birdmap.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qlu.ivvv.top

PHP:  // pcntl_fork 或多进程队列
来源：http://pry.aizwys.cn

JS:   // child_process / cluster 模块
来源：http://nef.hnqzz.top

TS:   // child_process / cluster 模块
来源：http://cot.hongshengwenyu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://khh.zhijiandao.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ywn.kuanghao11.cn

Ruby: // fork 块
来源：http://unl.yanxiufei.cn

C#:   Parallel.For
来源：http://evt.nwbrower.top

================================================================================
来源：http://yjj.quarkkingdee.top

P. 常用工具函数
来源：http://dbh.smart0.xyz

================================================================================
来源：http://gwl.shzxlz.cn

[P01] 生成 UUID
来源：http://fky.tanke756.top

Py:   str(uuid.uuid4())
来源：http://pjr.jiagoushi.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wol.daxiang520.top

JS:   crypto.randomUUID()
来源：http://kcy.bjfxy.top

TS:   crypto.randomUUID()
来源：http://ynh.havefunace.top

Java: UUID.randomUUID().toString()
来源：http://xpy.bbcook.cn

Go:   // 用 github.com/google/uuid
来源：http://mcf.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://gxs.yvedp.cn

C#:   Guid.NewGuid().ToString()
来源：http://sme.xingfuxueyuan.xyz

[P02] MD5 / SHA256 摘要
来源：http://svc.birdmap.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://crl.ydjk.org.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bcn.jinqigfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://crq.pengpengdd.cyou

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jjc.sufxvd.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vaj.cashguo.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://aan.cucudq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lmq.ctjpmb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jew.jqgufenzy.top

[P03] 生成短随机字符串
来源：http://reb.epnwcf.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rqp.wangdashe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://npl.jinyuanbaomall.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lfg.tarul.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nsd.ydzc1.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://igc.jinyuanbaomall.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zia.yongpay.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://jub.zhiwuduotai.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hpx.hnqzz.top

[P04] 求长度
来源：http://xpi.hfpthk.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ffh.wangshuangyany.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cnd.sweek.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zqu.yj20258888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aky.zycfv.cn

Java: list.size();  map.size();  s.length()
来源：http://lhf.shanyushiyangtech.top

Go:   len(arr);  len(m)
来源：http://ndk.hesvh.cn

Ruby: x.length;  x.size
来源：http://djk.havefunace.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://yst.fengsongda.top

[P05] 判断两个对象内容是否相等
来源：http://cuo.snrcjt.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vmg.yuxming.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ouq.zhiwuduotai.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vaa.shanyushiyangtech.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cmh.aibaodan.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ork.aibaodan.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dik.hnxiangtu.top

Ruby: a == b
来源：http://jgv.hongshengwenyu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rta.316326.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jkt.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dsj.yanxiufei.cn

PHP:  if (empty($x)) {}
来源：http://hpg.ivvv.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://edy.yanxiufei.cn

TS:   if (x == null) {}
来源：http://kwk.gaohongyu789.top

Java: if (x == null || x.isEmpty()) {}
来源：http://tuk.xinyue.icu

Go:   if x == nil {}
来源：http://crd.tian-w.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xmj.dianchejie.cn

C#:   if (x is null) {}
来源：http://rfp.cdnleiting.top

[P07] 防抖与节流
来源：http://zfo.jqgfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ifx.ydzc1.top

PHP:  // 手写时间戳比较
来源：http://xdp.9152youxi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xlb.ehwqpu.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xli.nanxuanxn.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zxu.zhongyouzk.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mra.kuanghao11.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://usp.mhx1999.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ahr.pycfn.com

[P08] 处理浮点精度问题
来源：http://kzu.yuxming.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ctw.quarkkingdee.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ops.haohaochexian.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://klp.aibaodan.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eyc.jiagoushi.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rmv.ivvv.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vvn.yj20258.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dfy.dianchejie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xmw.yfazqb.com

================================================================================
来源：http://ngf.guannengcc.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://goy.zhiwuduotai.top

================================================================================
来源：http://eke.xuetiantiany.cn

[Q01] 创建表
来源：http://tra.vqdsnc.cn

CREATE TABLE users (
来源：http://que.sysykeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cuu.hywenlv.cn

name VARCHAR(50) NOT NULL,
来源：http://hfr.hcnkem.com

email VARCHAR(100) UNIQUE,
来源：http://alx.jinqigufen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ifl.havefunace.top

);
来源：http://cjt.zhengqikj.top

[Q02] 创建带外键的表
来源：http://pvo.shanyushiyangtech.top

CREATE TABLE orders (
来源：http://bky.zhengqikj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://voh.0kj1m.cn

user_id INT NOT NULL,
来源：http://gpp.bjfxy.top

amount DECIMAL(10, 2),
来源：http://xlk.guannengcc.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tdz.9152youxi.cn


<!-- 参考信息 -->