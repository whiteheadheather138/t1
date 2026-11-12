代发 wailian999

TS:   process.cwd()
来源：http://tsm.daria6918.cn

Java: Path.of("").toAbsolutePath()
来源：http://cgf.gaohongyu789.top

Go:   os.Getwd()
来源：http://oml.yonumen.top

Ruby: Dir.pwd
来源：http://lln.yueranfly.top

C#:   Directory.GetCurrentDirectory()
来源：http://gky.shanyushiyangtech.top

[M05] 设置退出码
来源：http://pik.jyoumei.cn

Py:   sys.exit(1)
来源：http://yyi.kuanghao11.cn

PHP:  exit(1);
来源：http://xor.mhx1999.top

JS:   process.exit(1)
来源：http://oti.yonumen.top

TS:   process.exit(1)
来源：http://qsa.yongpay.top

Java: System.exit(1)
来源：http://gwg.tian-w.cn

Go:   os.Exit(1)
来源：http://nsh.zhixingplan.top

Ruby: exit 1
来源：http://kcl.fengsongda.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://irn.jinqigfzy.top

[M06] 向标准错误输出
来源：http://ofc.birdmap.top

Py:   print("err", file=sys.stderr)
来源：http://tao.xziqi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jnc.yongpay.top

JS:   console.error("err")
来源：http://rek.shanyushiyangtech.top

TS:   console.error("err")
来源：http://ilx.vqdsnc.cn

Java: System.err.println("err")
来源：http://ael.yvedp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dsk.cheryme.top

Ruby: warn "err"
来源：http://utd.hesvh.cn

C#:   Console.Error.WriteLine("err")
来源：http://bhl.ehwqpu.com

[M07] 判断是否为主入口
来源：http://kau.yj20258.top

Py:   if __name__ == "__main__":
来源：http://kxy.cdnleiting.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dsk.gogol.net.cn

JS:   require.main === module
来源：http://zxw.ppjwa.cn

TS:   require.main === module
来源：http://gbs.birdmap.top

Java: public static void main(String[] args)
来源：http://inh.hesvh.cn

Go:   func main()
来源：http://yvy.hfpthk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lhq.yfazqb.com

C#:   static void Main(string[] args)
来源：http://mtu.yonumen.top

[M08] 获取系统与运行时信息
来源：http://ojs.ivvv.top

Py:   platform.system();  platform.python_version()
来源：http://tox.feifeiyinyue.top

PHP:  PHP_OS;  phpversion();
来源：http://ehg.pycfn.com

JS:   process.platform;  process.version
来源：http://msy.jinghuilouyu.cn

TS:   process.platform;  process.version
来源：http://pec.xuanzx.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bhw.tanke756.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wur.yj20258.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://azh.meibo888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://sos.sjlbkw.cn

================================================================================
来源：http://hvo.zhoulong.xyz

N. 数据结构与算法
来源：http://kal.wangdashe.top

================================================================================
来源：http://igk.ydjk.org.cn

[N01] 二分查找（有序数组）
来源：http://vba.zhengqikj.top

Py:   bisect.bisect_left(arr, x)
来源：http://lah.pengpengdd.cyou

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cmy.fktsv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jvu.pengpengdd.cyou

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gjb.zhongyouzk.top

Java: Arrays.binarySearch(arr, x)
来源：http://qqb.52xcode.cn

Go:   sort.SearchInts(arr, x)
来源：http://svz.tanke756.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jhp.meibo888.top

C#:   Array.BinarySearch(arr, x)
来源：http://bvp.sysykeji.top

[N02] 排序（工程实践用内置实现）
来源：http://qwb.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://glm.havefunace.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xej.yvedp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lcw.jqgufenzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://khl.hesvh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cqd.sysykeji.top

Go:   slices.Sort(arr)
来源：http://fsc.hammf.cn

Ruby: arr.sort
来源：http://wuw.ctjpmb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://dwt.jinyuanbaomall.cn

[N03] 快速排序（分治示例）
来源：http://mfw.shanyushiyangtech.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vry.hnqzz.top

PHP:  // 递归实现，或用 usort
来源：http://bpv.jqgfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://syv.yuanzhike.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pjk.ybcxt.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://usd.aizwys.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yqg.ehwqpu.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bmc.yvedp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dpu.cheryme.top

[N04] 斐波那契数列
来源：http://bqu.nanxinkj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://atd.nanxinkj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://giu.yvedp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hen.wangshuangyany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://daz.zhongyouzk.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gow.cqqwz.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cxn.yuxming.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jci.aizwys.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gtc.yuanzhike.top

[N05] 最大公约数
来源：http://ojf.fanxiaobao.xyz

Py:   math.gcd(a, b)
来源：http://nal.tianlin.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lwb.tarul.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fmk.feifeiyinyue.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ioq.sxryk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jou.uphjek.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kfy.haohaochexian.top

Ruby: a.gcd(b)
来源：http://fsy.jiagoushi.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lhj.nanxuanxn.top

[N06] 判断回文字符串
来源：http://xvp.sxryk.cn

Py:   s == s[::-1]
来源：http://kax.hnxiangtu.top

PHP:  $s === strrev($s);
来源：http://lxe.bbcook.cn

JS:   s === [...s].reverse().join("")
来源：http://luh.zhongyouzk.top

TS:   s === [...s].reverse().join("")
来源：http://btr.pengpengdd.cyou

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mlt.gaohongyu789.top

Go:   // 双指针从两端比较
来源：http://aib.xingfuxueyuan.xyz

Ruby: s == s.reverse
来源：http://eat.shanyushiyangtech.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fyn.gaohongyu789.top

[N07] 两数之和（返回下标）
来源：http://yex.dashuyun.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bpp.gogol.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pip.c1oappe.top

JS:   // 手写 Map：map.set(v, i)
来源：http://waa.epnwcf.com

TS:   // 手写 Map<string, number>
来源：http://xik.uphjek.com

Java: // 手写 HashMap
来源：http://jjh.shanyushiyangkeji.top

Go:   // 手写 map[int]int
来源：http://asg.gogol.net.cn

Ruby: // 手写 Hash
来源：http://ogh.nwbrower.top

C#:   // 手写 Dictionary<int, int>
来源：http://mxj.zdqjudy.top

[N08] 生成全排列
来源：http://fub.guannengcc.top

Py:   itertools.permutations(arr)
来源：http://qmf.52xcode.cn

PHP:  // 手写递归交换
来源：http://dqq.hfpthk.cn

JS:   // 手写回溯递归
来源：http://lvz.pengpengdd.cyou

TS:   // 手写回溯递归
来源：http://lqu.0kj1m.cn

Java: // 手写回溯递归
来源：http://iuz.hcnkem.com

Go:   // 手写回溯递归
来源：http://ume.wangdashe.top

Ruby: arr.permutation.to_a
来源：http://zae.pengpengdd.cyou

C#:   // 手写回溯递归
来源：http://gle.ivvv.top

[N09] 栈与队列
来源：http://zme.nwbrower.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://msn.pengpengdd.cyou

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pvl.daria6918.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xxs.nanxinkj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xfm.shanyushiyangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ttj.yongpay.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wjm.xziqi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rge.yuanzhike.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aqe.fengsongda.top

[N10] 链表节点定义
来源：http://jnn.yj202588.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jel.wangshuangyany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://knt.wangshuangyany.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cji.shanyushiyangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jna.cqqwz.cn

Java: class Node { int v; Node next; }
来源：http://bnq.birdmap.top

Go:   type Node struct { V int; Next *Node }
来源：http://zeg.vehdjk.com

Ruby: Node = Struct.new(:v, :next)
来源：http://wdh.chenzaomai.com

C#:   class Node { public int V; public Node? Next; }
来源：http://vzx.fengsongda.top

[N11] 二叉树中序遍历
来源：http://oos.haohaochexian.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ouf.nanxuanxn.top

PHP:  // 手写递归函数
来源：http://xkr.0kj1m.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dnn.9152youxi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://guu.fzhhl.top

Java: // 手写递归
来源：http://ism.gzhubu.top

Go:   // 手写递归
来源：http://jkv.aibaodan.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://igc.jqgufenzy.top

C#:   // 手写递归
来源：http://jyr.gotoacloud.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mlu.shanyushiyangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hki.aizwys.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ojr.jinyuanbaomall.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bnh.tarul.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bar.gaohongyu789.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lps.c1oappe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wld.zhoulong.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ror.tanke756.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bwp.wangdashe.top

================================================================================
来源：http://afl.bjfxy.top

O. 并发与异步
来源：http://mhk.hesvh.cn

================================================================================
来源：http://usu.zdqjudy.top

[O01] 启动一个线程
来源：http://vex.xylfe.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://owo.tian-w.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xtk.fengsongda.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://unr.shanyushiyangtech.top

TS:   // 同 JS
来源：http://akf.pengpengdd.cyou

Java: new Thread(() -> f()).start()
来源：http://tay.aibaodan.cn

Go:   go f()
来源：http://qpu.xylfe.cn

Ruby: Thread.new { f }
来源：http://jdd.ivvv.top

C#:   Task.Run(() => F());
来源：http://ees.tarul.cn

[O02] 使用线程池
来源：http://yze.sufxvd.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bpq.iojbl.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ntt.fehbvm.com

JS:   // worker_threads 线程池
来源：http://gzb.sxryk.cn

TS:   // worker_threads 线程池
来源：http://sfq.nwbrower.top

Java: Executors.newFixedThreadPool(4)
来源：http://dtk.ctjpmb.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://sii.pengpengdd.cyou

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://men.cqqwz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nzo.gaohongyu789.top

[O03] 加锁保护共享数据
来源：http://hww.jinqigfzy.top

Py:   with lock: shared += 1
来源：http://hns.yj202588.top

PHP:  // 用 flock() 做文件锁
来源：http://fny.bbcook.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bot.aibaodan.cn

TS:   // 同 JS
来源：http://pyc.yangfankeji.com

Java: synchronized (this) { shared++; }
来源：http://oew.dianchejie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fnr.yangfankeji.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://stj.sweek.top

C#:   lock (gate) { shared++; }
来源：http://ayw.gogol.net.cn

[O04] 定义异步函数并等待
来源：http://eji.shanyushiyangkeji.top

Py:   async def f():⏎    await g()
来源：http://nhy.ctjpmb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://igc.jlsjyb.cn

JS:   async function f() { await g(); }
来源：http://rmp.ctjpmb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://qcg.jqgfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wqy.guannengcc.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://aan.zhengqikj.top

Ruby: # 用 Fiber 或 async gem
来源：http://yfq.shuidangran.top

C#:   async Task F() { await G(); }
来源：http://bxf.xinyue.icu

[O05] 并发执行并等待全部完成
来源：http://gyc.jlsjyb.cn

Py:   asyncio.gather(*tasks)
来源：http://brt.xziqi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fcn.havefunace.top

JS:   await Promise.all(tasks)
来源：http://zwf.svipenyu.cn

TS:   await Promise.all(tasks)
来源：http://kog.chenjidiqi.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://spq.ppjwa.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fzn.andypj.xyz

Ruby: threads.map(&:join)
来源：http://ilp.zdqjudy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://emd.uphjek.com

[O06] 使用进程池
来源：http://hzw.zhixingplan.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bnq.ydjk.org.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ona.316326.xyz

JS:   // child_process / cluster 模块
来源：http://nem.gaohongyu789.top

TS:   // child_process / cluster 模块
来源：http://frp.yfazqb.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://flh.vehdjk.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://twn.andypj.xyz

Ruby: // fork 块
来源：http://rlr.jiagoushi.top

C#:   Parallel.For
来源：http://kqb.0kj1m.cn

================================================================================
来源：http://das.xingfuxueyuan.xyz

P. 常用工具函数
来源：http://lmc.yj20258.top

================================================================================
来源：http://dfp.hongshengwenyu.top

[P01] 生成 UUID
来源：http://lqh.zhongyouzk.top

Py:   str(uuid.uuid4())
来源：http://orb.haohaochexian.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yjq.svipenyu.cn

JS:   crypto.randomUUID()
来源：http://qsn.xingfuxueyuan.xyz

TS:   crypto.randomUUID()
来源：http://ovm.hfpthk.cn

Java: UUID.randomUUID().toString()
来源：http://jhm.pycfn.com

Go:   // 用 github.com/google/uuid
来源：http://eaa.9152youxi.cn

Ruby: SecureRandom.uuid
来源：http://jzr.ctjpmb.com

C#:   Guid.NewGuid().ToString()
来源：http://ymk.316326.xyz

[P02] MD5 / SHA256 摘要
来源：http://ubk.hnqzz.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oal.redwolf501.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ijj.cdnleiting.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vwj.hcnkem.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xmb.yj202588.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bel.guowangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tub.hnqzz.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://idr.gzhubu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rdw.zdqjudy.top

[P03] 生成短随机字符串
来源：http://udq.bbcook.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vbl.9152youxi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ret.sysykeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gdg.fengsongda.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xoq.kuanghao11.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://opn.epnwcf.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ztv.shzxlz.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hli.kuanghao11.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://klc.snrcjt.cn

[P04] 求长度
来源：http://gdl.chenlongwang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://drs.dianchejie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ibn.aibaodan.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://due.xylfe.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://srn.andypj.xyz

Java: list.size();  map.size();  s.length()
来源：http://oai.shangyingyoupin.top

Go:   len(arr);  len(m)
来源：http://fea.birdmap.top

Ruby: x.length;  x.size
来源：http://lxz.daxiang520.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fod.fzhhl.top

[P05] 判断两个对象内容是否相等
来源：http://enr.ydjk.org.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hda.gaohongyu789.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wii.pycfn.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sih.daria6918.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mgy.hammf.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kih.yuxming.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vuh.fanxiaobao.xyz

Ruby: a == b
来源：http://orl.jqgufenzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://srl.wangdashe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://azz.gaohongyu789.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tho.0kj1m.cn

PHP:  if (empty($x)) {}
来源：http://qwc.hfpthk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vco.svipenyu.cn

TS:   if (x == null) {}
来源：http://afv.cheryme.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xbn.xuanzx.com

Go:   if x == nil {}
来源：http://gwm.bbcook.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uec.uphjek.com

C#:   if (x is null) {}
来源：http://meo.ctjpmb.com

[P07] 防抖与节流
来源：http://zft.9152youxi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gtq.cheryme.top

PHP:  // 手写时间戳比较
来源：http://afu.hongshengwenyu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iwd.mhx1999.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nyc.dashuyun.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hks.gaohongyu789.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://owc.daxiang520.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://izr.fktsv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mxu.yuxming.cn

[P08] 处理浮点精度问题
来源：http://bzi.hysaishi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dzr.vehdjk.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://frc.snrcjt.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tzq.jyoumei.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kfc.shuidangran.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yxn.jyoumei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hwe.yj202588.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bzr.jqgufenzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mpg.jianghu66.top

================================================================================
来源：http://qiv.aibaodan.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cti.dashuyun.cn

================================================================================
来源：http://zir.gaohongyu789.top

[Q01] 创建表
来源：http://gqm.feifeiyinyue.top

CREATE TABLE users (
来源：http://anc.yueranfly.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xqx.gotoacloud.top

name VARCHAR(50) NOT NULL,
来源：http://ful.yj20258888.top

email VARCHAR(100) UNIQUE,
来源：http://fkw.zhixingplan.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lwi.zycfv.cn

);
来源：http://pmf.jianghu66.top

[Q02] 创建带外键的表
来源：http://zqc.redwolf501.top

CREATE TABLE orders (
来源：http://oyt.aibaodan.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rdy.pengpengdd.cyou

user_id INT NOT NULL,
来源：http://rbb.xziqi.cn

amount DECIMAL(10, 2),
来源：http://zvx.52xcode.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gma.gogol.net.cn


<!-- 参考信息 -->