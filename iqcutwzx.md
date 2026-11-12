代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://aoh.sufxvd.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vzw.tarul.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nrj.jianghu66.top

C#:   Process.Start("ls", "-l");
来源：http://sfj.kuanghao11.cn

[M04] 获取当前工作目录
来源：http://jqa.smart0.xyz

Py:   os.getcwd()
来源：http://lip.wangdashe.top

PHP:  getcwd();
来源：http://brx.bbcook.cn

JS:   process.cwd()
来源：http://wgp.redwolf501.top

TS:   process.cwd()
来源：http://rpm.snrcjt.cn

Java: Path.of("").toAbsolutePath()
来源：http://qrq.shuidangran.top

Go:   os.Getwd()
来源：http://qxg.cdnleiting.top

Ruby: Dir.pwd
来源：http://eng.chenjidiqi.icu

C#:   Directory.GetCurrentDirectory()
来源：http://gfe.jqgfzy.top

[M05] 设置退出码
来源：http://mki.sufxvd.cn

Py:   sys.exit(1)
来源：http://nzk.pycfn.com

PHP:  exit(1);
来源：http://htg.hnqzz.top

JS:   process.exit(1)
来源：http://jqy.jyoumei.cn

TS:   process.exit(1)
来源：http://ybr.yueranfly.top

Java: System.exit(1)
来源：http://snq.pycfn.com

Go:   os.Exit(1)
来源：http://usj.c1oappe.top

Ruby: exit 1
来源：http://axs.cqqwz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ema.zhongyouzk.top

[M06] 向标准错误输出
来源：http://oxb.guannengcc.top

Py:   print("err", file=sys.stderr)
来源：http://yui.yueranfly.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mnx.shanyushiyangtech.top

JS:   console.error("err")
来源：http://vzs.jqgufenzy.top

TS:   console.error("err")
来源：http://mxn.gaohongyu789.top

Java: System.err.println("err")
来源：http://kyq.yangfankeji.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tom.hnxiangtu.top

Ruby: warn "err"
来源：http://xmp.fzhhl.top

C#:   Console.Error.WriteLine("err")
来源：http://the.uphjek.com

[M07] 判断是否为主入口
来源：http://nry.jqgfzy.top

Py:   if __name__ == "__main__":
来源：http://gpa.vqdsnc.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xld.nanxuanxn.top

JS:   require.main === module
来源：http://lkg.aibaodan.cn

TS:   require.main === module
来源：http://zrn.yonumen.top

Java: public static void main(String[] args)
来源：http://rov.zhaomingkeji.xyz

Go:   func main()
来源：http://ayi.sufxvd.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xjc.ywan-chungtsiang.top

C#:   static void Main(string[] args)
来源：http://loq.fanxiaobao.xyz

[M08] 获取系统与运行时信息
来源：http://qea.hnxiangtu.top

Py:   platform.system();  platform.python_version()
来源：http://nen.vehdjk.com

PHP:  PHP_OS;  phpversion();
来源：http://ajc.aizwys.cn

JS:   process.platform;  process.version
来源：http://sqh.fanxiaobao.xyz

TS:   process.platform;  process.version
来源：http://rhu.jyoumei.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://chd.snrcjt.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rkw.c1oappe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bzh.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://kyw.dianchejie.cn

================================================================================
来源：http://jhk.fengsongda.top

N. 数据结构与算法
来源：http://ctu.shanyushiyangtech.top

================================================================================
来源：http://tsf.vqdsnc.cn

[N01] 二分查找（有序数组）
来源：http://hqq.zhiwuduotai.top

Py:   bisect.bisect_left(arr, x)
来源：http://uor.shanyushiyangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lty.zhongyouzk.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kfs.sjlbkw.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://roi.aizwys.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dex.jqgfzy.top

Go:   sort.SearchInts(arr, x)
来源：http://zli.hywenlv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fxi.ywan-chungtsiang.top

C#:   Array.BinarySearch(arr, x)
来源：http://chr.yanxiufei.cn

[N02] 排序（工程实践用内置实现）
来源：http://gup.bjfxy.top

Py:   sorted(arr);  arr.sort()
来源：http://joc.316326.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hgl.aibaodan.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://yfx.yj20258.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://sjw.cucudq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cvg.aibaodan.cn

Go:   slices.Sort(arr)
来源：http://ltc.sysykeji.top

Ruby: arr.sort
来源：http://tgc.9152youxi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lrg.uphjek.com

[N03] 快速排序（分治示例）
来源：http://dsi.52xcode.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gsv.fzhhl.top

PHP:  // 递归实现，或用 usort
来源：http://spe.ehwqpu.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://get.gogol.net.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zfv.hesvh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kjs.uphjek.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bif.wangshuangyany.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uxg.yongpay.top

C#:   // 手写递归，或 Array.Sort
来源：http://zab.tian-w.cn

[N04] 斐波那契数列
来源：http://glp.316326.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wtc.aibaodan.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://drj.sysykeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ccp.andypj.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pbx.fanxiaobao.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xnb.yueranfly.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ggf.gaohongyu789.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dap.xingfuxueyuan.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://znk.sjlbkw.cn

[N05] 最大公约数
来源：http://nyg.yonumen.top

Py:   math.gcd(a, b)
来源：http://qlv.yuxming.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://itl.gogol.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iqq.jinyuanbaomall.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fpf.shanyushiyangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bbl.ehwqpu.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ekb.shzxlz.cn

Ruby: a.gcd(b)
来源：http://zxg.daxiang520.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yjy.meibo888.top

[N06] 判断回文字符串
来源：http://jbz.epnwcf.com

Py:   s == s[::-1]
来源：http://pxy.nwbrower.top

PHP:  $s === strrev($s);
来源：http://ljz.nanxinkj.top

JS:   s === [...s].reverse().join("")
来源：http://obd.hysaishi.cn

TS:   s === [...s].reverse().join("")
来源：http://iah.snrcjt.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tlw.sysykeji.top

Go:   // 双指针从两端比较
来源：http://yzq.zycfv.cn

Ruby: s == s.reverse
来源：http://saz.zhixingplan.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://pur.316326.xyz

[N07] 两数之和（返回下标）
来源：http://bao.fehbvm.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hjg.gzhubu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zua.shangyingyoupin.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kmo.guowangkeji.top

TS:   // 手写 Map<string, number>
来源：http://rzs.smart0.xyz

Java: // 手写 HashMap
来源：http://lxr.feifeiyinyue.top

Go:   // 手写 map[int]int
来源：http://ydi.yongpay.top

Ruby: // 手写 Hash
来源：http://ejt.mhx1999.top

C#:   // 手写 Dictionary<int, int>
来源：http://bfu.svipenyu.cn

[N08] 生成全排列
来源：http://wgi.cheryme.top

Py:   itertools.permutations(arr)
来源：http://qqw.ydzc1.top

PHP:  // 手写递归交换
来源：http://lqi.xuanzx.com

JS:   // 手写回溯递归
来源：http://dxm.aibaodan.cn

TS:   // 手写回溯递归
来源：http://lwc.pengpengdd.cyou

Java: // 手写回溯递归
来源：http://vmw.pengpengdd.cyou

Go:   // 手写回溯递归
来源：http://crv.xingfuxueyuan.xyz

Ruby: arr.permutation.to_a
来源：http://jli.hongshengwenyu.top

C#:   // 手写回溯递归
来源：http://nla.aibaodan.cn

[N09] 栈与队列
来源：http://cvv.yongpay.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ytp.ehwqpu.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gnn.316326.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qsg.yj202588.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://orz.zhoulong.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://exr.yueranfly.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sih.dianchejie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://okw.ybcxt.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ehl.feifeiyinyue.top

[N10] 链表节点定义
来源：http://vwl.pengpengdd.cyou

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pnw.yanxiufei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://grx.yanxiufei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://emj.jinqigfzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mui.hammf.cn

Java: class Node { int v; Node next; }
来源：http://his.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://ffk.yangfankeji.com

Ruby: Node = Struct.new(:v, :next)
来源：http://wjq.pycfn.com

C#:   class Node { public int V; public Node? Next; }
来源：http://pfd.svipenyu.cn

[N11] 二叉树中序遍历
来源：http://iwz.jiagoushi.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tvc.fzhhl.top

PHP:  // 手写递归函数
来源：http://bup.andypj.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oli.smart0.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qzj.hcnkem.com

Java: // 手写递归
来源：http://myj.tian-w.cn

Go:   // 手写递归
来源：http://ges.cheryme.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vit.jyoumei.cn

C#:   // 手写递归
来源：http://rgf.gaohongyu789.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xgs.hnqzz.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://onh.bbcook.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tbw.zycfv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wlz.guowangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ynw.fengsongda.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ynu.hfpthk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cxb.yj20258888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wvh.fzhhl.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://scb.shuidangran.top

================================================================================
来源：http://anw.uphjek.com

O. 并发与异步
来源：http://nis.fktsv.cn

================================================================================
来源：http://tsh.smart0.xyz

[O01] 启动一个线程
来源：http://ghk.fzhhl.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qby.cqqwz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ydh.ivvv.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vaw.ehwqpu.com

TS:   // 同 JS
来源：http://bpw.jyoumei.cn

Java: new Thread(() -> f()).start()
来源：http://hnr.zhixingplan.top

Go:   go f()
来源：http://cfl.sxryk.cn

Ruby: Thread.new { f }
来源：http://jgy.jqgfzy.top

C#:   Task.Run(() => F());
来源：http://uhy.jinyuanbaomall.cn

[O02] 使用线程池
来源：http://qer.daria6918.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qpq.epnwcf.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://snx.zdbjq.cn

JS:   // worker_threads 线程池
来源：http://yrc.ehwqpu.com

TS:   // worker_threads 线程池
来源：http://pzz.yvedp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xja.zhoulong.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wtd.jqgufenzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hfv.redwolf501.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://laz.pycfn.com

[O03] 加锁保护共享数据
来源：http://gvh.nanxinkj.top

Py:   with lock: shared += 1
来源：http://yju.fktsv.cn

PHP:  // 用 flock() 做文件锁
来源：http://gsu.zhengqikj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ysz.chenzaomai.com

TS:   // 同 JS
来源：http://oxn.yuxming.cn

Java: synchronized (this) { shared++; }
来源：http://ttp.feifeiyinyue.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gqd.0kj1m.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ffv.zdbjq.cn

C#:   lock (gate) { shared++; }
来源：http://xir.zdbjq.cn

[O04] 定义异步函数并等待
来源：http://akw.snrcjt.cn

Py:   async def f():⏎    await g()
来源：http://rcq.sweek.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dna.fehbvm.com

JS:   async function f() { await g(); }
来源：http://nxi.yuxming.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gwk.shanyushiyangtech.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://erx.havefunace.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://poz.nwbrower.top

Ruby: # 用 Fiber 或 async gem
来源：http://tmr.9152youxi.cn

C#:   async Task F() { await G(); }
来源：http://roo.smart0.xyz

[O05] 并发执行并等待全部完成
来源：http://led.yfazqb.com

Py:   asyncio.gather(*tasks)
来源：http://lmw.jiagoushi.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pwe.jlsjyb.cn

JS:   await Promise.all(tasks)
来源：http://yej.shanyushiyangtech.top

TS:   await Promise.all(tasks)
来源：http://vih.yuxming.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://krp.jyoumei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kpo.yj20258888.top

Ruby: threads.map(&:join)
来源：http://jnv.jinyuanbaomall.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mum.dashuyun.cn

[O06] 使用进程池
来源：http://chp.zhengqikj.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zia.cucudq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rcm.tarul.cn

JS:   // child_process / cluster 模块
来源：http://nrh.feifeiyinyue.top

TS:   // child_process / cluster 模块
来源：http://brh.wangshuangyany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dfu.yj202588.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ibt.andypj.xyz

Ruby: // fork 块
来源：http://bay.ppjwa.cn

C#:   Parallel.For
来源：http://abb.cucudq.cn

================================================================================
来源：http://hsi.hysaishi.cn

P. 常用工具函数
来源：http://xgc.jinyuanbaomall.cn

================================================================================
来源：http://hxt.zycfv.cn

[P01] 生成 UUID
来源：http://vnk.zhoulong.xyz

Py:   str(uuid.uuid4())
来源：http://ioj.gogol.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cmn.hfpthk.cn

JS:   crypto.randomUUID()
来源：http://uga.9152youxi.cn

TS:   crypto.randomUUID()
来源：http://oni.kuanghao11.cn

Java: UUID.randomUUID().toString()
来源：http://urg.redwolf501.top

Go:   // 用 github.com/google/uuid
来源：http://xho.0kj1m.cn

Ruby: SecureRandom.uuid
来源：http://jur.jyoumei.cn

C#:   Guid.NewGuid().ToString()
来源：http://qaq.birdmap.top

[P02] MD5 / SHA256 摘要
来源：http://gvp.cheryme.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oux.gaohongyu789.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://nbq.jianghu66.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uzc.zycfv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lwp.jqgufenzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://psz.hywenlv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hfq.hammf.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://prz.nanxinkj.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aoq.pengpengdd.cyou

[P03] 生成短随机字符串
来源：http://hsi.havefunace.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ctj.hnxiangtu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lbu.jiagoushi.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tol.yueranfly.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mtv.ydjk.org.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pbw.nwbrower.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tcf.yj20258888.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://npu.ywan-chungtsiang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jof.shuidangran.top

[P04] 求长度
来源：http://ewc.redwolf501.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sbd.316326.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pkw.jianghu66.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pco.cqqwz.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vhb.0kj1m.cn

Java: list.size();  map.size();  s.length()
来源：http://ycc.ivvv.top

Go:   len(arr);  len(m)
来源：http://zup.guowangkeji.top

Ruby: x.length;  x.size
来源：http://xtk.daxiang520.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://iwh.sxryk.cn

[P05] 判断两个对象内容是否相等
来源：http://wsx.ybcxt.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://plc.cheryme.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bth.sufxvd.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wlj.tian-w.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nin.hesvh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://acu.zhijiandao.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gnw.guannengcc.top

Ruby: a == b
来源：http://llo.gaohongyu789.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mvy.quarkkingdee.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cvw.daxiang520.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://msu.jinqigufen.top

PHP:  if (empty($x)) {}
来源：http://roi.shuidangran.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xen.haohaochexian.top

TS:   if (x == null) {}
来源：http://tfg.xylfe.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jxv.zhoulong.xyz

Go:   if x == nil {}
来源：http://qwp.meibo888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mne.c1oappe.top

C#:   if (x is null) {}
来源：http://onl.52xcode.cn

[P07] 防抖与节流
来源：http://kmy.gotoacloud.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://teo.fengsongda.top

PHP:  // 手写时间戳比较
来源：http://ppx.pycfn.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bof.c1oappe.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zhe.yuanzhike.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mkm.chenlongwang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cfj.yonumen.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://jze.hnxiangtu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vvc.yueranfly.top

[P08] 处理浮点精度问题
来源：http://bdz.sxryk.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uhm.shanyushiyangkeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ltz.epnwcf.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gkx.yj20258888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sai.fanxiaobao.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qao.fzhhl.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://trn.quarkkingdee.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ied.feifeiyinyue.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xvy.snrcjt.cn

================================================================================
来源：http://djc.aibaodan.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://afj.gotoacloud.top

================================================================================
来源：http://hbn.wangshuangyany.cn

[Q01] 创建表
来源：http://vry.shanyushiyangtech.top

CREATE TABLE users (
来源：http://dbq.xziqi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lyv.tian-w.cn

name VARCHAR(50) NOT NULL,
来源：http://aak.andypj.xyz

email VARCHAR(100) UNIQUE,
来源：http://plb.ppjwa.cn


<!-- 参考信息 -->