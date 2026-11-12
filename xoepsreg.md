代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xzu.hnqzz.top

JS:   process.env.HOME
来源：http://psc.sysykeji.top

TS:   process.env.HOME
来源：http://sac.fengsongda.top

Java: System.getenv("HOME")
来源：http://xen.iojbl.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qov.ctjpmb.com

Ruby: ENV["HOME"]
来源：http://ito.nanxinkj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mkz.hammf.cn

[M03] 执行外部命令
来源：http://ypl.gotoacloud.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kyl.gaohongyu789.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bho.kuanghao11.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qxr.c1oappe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xmz.fanxiaobao.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://svr.zhixingplan.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xeo.haohaochexian.top

Ruby: system("ls -l");  `ls -l`
来源：http://kig.shzxlz.cn

C#:   Process.Start("ls", "-l");
来源：http://tkp.0kj1m.cn

[M04] 获取当前工作目录
来源：http://keb.andypj.xyz

Py:   os.getcwd()
来源：http://xpq.c1oappe.top

PHP:  getcwd();
来源：http://lzk.haohaochexian.top

JS:   process.cwd()
来源：http://mwe.zhijiandao.cn

TS:   process.cwd()
来源：http://kva.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://jkw.sysykeji.top

Go:   os.Getwd()
来源：http://uuj.hfpthk.cn

Ruby: Dir.pwd
来源：http://oxx.yj202588.top

C#:   Directory.GetCurrentDirectory()
来源：http://eeo.jqgufenzy.top

[M05] 设置退出码
来源：http://kud.ydjk.org.cn

Py:   sys.exit(1)
来源：http://imv.ehwqpu.com

PHP:  exit(1);
来源：http://yzo.havefunace.top

JS:   process.exit(1)
来源：http://szx.yanxiufei.cn

TS:   process.exit(1)
来源：http://pkl.bjfxy.top

Java: System.exit(1)
来源：http://avu.jinghuilouyu.cn

Go:   os.Exit(1)
来源：http://qbb.jianghu66.top

Ruby: exit 1
来源：http://ukt.bbcook.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gzs.birdmap.top

[M06] 向标准错误输出
来源：http://bdr.tanke756.top

Py:   print("err", file=sys.stderr)
来源：http://hbf.yj202588.top

PHP:  fwrite(STDERR, "err\n");
来源：http://cfb.yueranfly.top

JS:   console.error("err")
来源：http://fxe.shuidangran.top

TS:   console.error("err")
来源：http://dxo.gzhubu.top

Java: System.err.println("err")
来源：http://yor.jianghu66.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://snn.tianlin.xyz

Ruby: warn "err"
来源：http://cdf.shuidangran.top

C#:   Console.Error.WriteLine("err")
来源：http://iia.shanyushiyangkeji.top

[M07] 判断是否为主入口
来源：http://bhh.feifeiyinyue.top

Py:   if __name__ == "__main__":
来源：http://ipl.aibaodan.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ohs.cashguo.top

JS:   require.main === module
来源：http://pnv.xziqi.cn

TS:   require.main === module
来源：http://sgy.52xcode.cn

Java: public static void main(String[] args)
来源：http://ukk.smart0.xyz

Go:   func main()
来源：http://lxn.jinyuanbaomall.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qoi.andypj.xyz

C#:   static void Main(string[] args)
来源：http://krq.shuidangran.top

[M08] 获取系统与运行时信息
来源：http://qhj.kuanghao11.cn

Py:   platform.system();  platform.python_version()
来源：http://yds.shzxlz.cn

PHP:  PHP_OS;  phpversion();
来源：http://ebw.xuanzx.com

JS:   process.platform;  process.version
来源：http://zri.bjfxy.top

TS:   process.platform;  process.version
来源：http://czv.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://crf.zhijiandao.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mbg.xylfe.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://feh.sysykeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://leo.tian-w.cn

================================================================================
来源：http://xjl.nwbrower.top

N. 数据结构与算法
来源：http://ivp.sufxvd.cn

================================================================================
来源：http://zze.cheryme.top

[N01] 二分查找（有序数组）
来源：http://deq.dashuyun.cn

Py:   bisect.bisect_left(arr, x)
来源：http://drv.yvedp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ekt.cashguo.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pcj.zycfv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://upi.jqgfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://xaw.nanxuanxn.top

Go:   sort.SearchInts(arr, x)
来源：http://yxl.zhoulong.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://lxq.yuanzhike.top

C#:   Array.BinarySearch(arr, x)
来源：http://xwz.sysykeji.top

[N02] 排序（工程实践用内置实现）
来源：http://oik.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ydk.daxiang520.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wzc.9152youxi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fqk.shuidangran.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rwm.yj20258888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hgw.daxiang520.top

Go:   slices.Sort(arr)
来源：http://hvk.feifeiyinyue.top

Ruby: arr.sort
来源：http://lbd.zhengqikj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zcp.vqdsnc.cn

[N03] 快速排序（分治示例）
来源：http://brb.jinqigufen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tod.jqgfzy.top

PHP:  // 递归实现，或用 usort
来源：http://dvd.jinqigfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://edz.haohaochexian.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.jinyuanbaomall.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vbl.zhijiandao.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ddv.yvedp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rws.316326.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://wqh.tian-w.cn

[N04] 斐波那契数列
来源：http://fna.tianlin.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hbg.havefunace.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wec.cqqwz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://buj.jqgufenzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sen.shanyushiyangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://czb.xinyue.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lki.yonumen.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wgt.yongpay.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://iya.haohaochexian.top

[N05] 最大公约数
来源：http://slo.shzxlz.cn

Py:   math.gcd(a, b)
来源：http://uly.xingfuxueyuan.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kgf.zhoulong.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ays.feifeiyinyue.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iya.hysaishi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mjr.pycfn.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bmm.wangdashe.top

Ruby: a.gcd(b)
来源：http://owa.9152youxi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://juy.yfazqb.com

[N06] 判断回文字符串
来源：http://ldf.sjlbkw.cn

Py:   s == s[::-1]
来源：http://bxy.zhiwuduotai.top

PHP:  $s === strrev($s);
来源：http://yhg.jiagoushi.top

JS:   s === [...s].reverse().join("")
来源：http://ozi.bbcook.cn

TS:   s === [...s].reverse().join("")
来源：http://pja.chenjidiqi.icu

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lay.zdbjq.cn

Go:   // 双指针从两端比较
来源：http://aux.smart0.xyz

Ruby: s == s.reverse
来源：http://jdq.9152youxi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ort.bjfxy.top

[N07] 两数之和（返回下标）
来源：http://kjz.sjlbkw.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yhr.dianchejie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gqn.yonumen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wqi.shzxlz.cn

TS:   // 手写 Map<string, number>
来源：http://rpe.cucudq.cn

Java: // 手写 HashMap
来源：http://kei.shzxlz.cn

Go:   // 手写 map[int]int
来源：http://kmn.hysaishi.cn

Ruby: // 手写 Hash
来源：http://uvj.zhixingplan.top

C#:   // 手写 Dictionary<int, int>
来源：http://xwc.redwolf501.top

[N08] 生成全排列
来源：http://cnj.xinyue.icu

Py:   itertools.permutations(arr)
来源：http://frf.zhixingplan.top

PHP:  // 手写递归交换
来源：http://hks.zdbjq.cn

JS:   // 手写回溯递归
来源：http://bxv.hfpthk.cn

TS:   // 手写回溯递归
来源：http://adm.zhongyouzk.top

Java: // 手写回溯递归
来源：http://kib.yfazqb.com

Go:   // 手写回溯递归
来源：http://rro.meibo888.top

Ruby: arr.permutation.to_a
来源：http://uat.ybcxt.top

C#:   // 手写回溯递归
来源：http://rhz.nwbrower.top

[N09] 栈与队列
来源：http://epk.jinyuanbaomall.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ygr.316326.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hgg.ppjwa.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cww.iojbl.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jqk.iojbl.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dax.andypj.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jsl.andypj.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dii.nwbrower.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iva.yangfankeji.com

[N10] 链表节点定义
来源：http://wdd.mhx1999.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mec.jinghuilouyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zhg.bjfxy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yet.tanke756.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vun.cdnleiting.top

Java: class Node { int v; Node next; }
来源：http://cdf.jinyuanbaomall.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wms.yj20258888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zpd.hcnkem.com

C#:   class Node { public int V; public Node? Next; }
来源：http://hfo.vehdjk.com

[N11] 二叉树中序遍历
来源：http://sru.hywenlv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://iwj.gaohongyu789.top

PHP:  // 手写递归函数
来源：http://xej.aibaodan.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://grq.nanxuanxn.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mja.yueranfly.top

Java: // 手写递归
来源：http://evj.mhx1999.top

Go:   // 手写递归
来源：http://xoo.shanyushiyangkeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zdf.hfpthk.cn

C#:   // 手写递归
来源：http://vtc.ehwqpu.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tpc.wangdashe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xea.jinqigfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tvo.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://svi.bbcook.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://evr.hnxiangtu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wux.cqqwz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nin.cucudq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eji.cheryme.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dua.tian-w.cn

================================================================================
来源：http://cpy.hongshengwenyu.top

O. 并发与异步
来源：http://mup.zhengqikj.top

================================================================================
来源：http://xbn.52xcode.cn

[O01] 启动一个线程
来源：http://jca.jqgfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fmj.quarkkingdee.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hjb.gzhubu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dzu.tian-w.cn

TS:   // 同 JS
来源：http://dte.316326.xyz

Java: new Thread(() -> f()).start()
来源：http://rft.zhaomingkeji.xyz

Go:   go f()
来源：http://qgu.hnqzz.top

Ruby: Thread.new { f }
来源：http://hlt.hongshengwenyu.top

C#:   Task.Run(() => F());
来源：http://qgg.snrcjt.cn

[O02] 使用线程池
来源：http://bqt.nanxuanxn.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mwj.xylfe.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zxa.yuxming.cn

JS:   // worker_threads 线程池
来源：http://smc.tanke756.top

TS:   // worker_threads 线程池
来源：http://web.yuxming.cn

Java: Executors.newFixedThreadPool(4)
来源：http://aun.yuxming.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oii.nwbrower.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wud.shangyingyoupin.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eaq.zhaomingkeji.xyz

[O03] 加锁保护共享数据
来源：http://vyz.zhixingplan.top

Py:   with lock: shared += 1
来源：http://oqk.yj20258.top

PHP:  // 用 flock() 做文件锁
来源：http://qvs.jianghu66.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kvt.nanxuanxn.top

TS:   // 同 JS
来源：http://tny.dianchejie.cn

Java: synchronized (this) { shared++; }
来源：http://fvu.hongshengwenyu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nxl.bbcook.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://tlq.snrcjt.cn

C#:   lock (gate) { shared++; }
来源：http://upw.52xcode.cn

[O04] 定义异步函数并等待
来源：http://ove.hnxiangtu.top

Py:   async def f():⏎    await g()
来源：http://lyv.daxiang520.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zaf.zhixingplan.top

JS:   async function f() { await g(); }
来源：http://olh.wangdashe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hwj.fengsongda.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hfk.fengsongda.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qdt.nwbrower.top

Ruby: # 用 Fiber 或 async gem
来源：http://amd.ydjk.org.cn

C#:   async Task F() { await G(); }
来源：http://diw.zdbjq.cn

[O05] 并发执行并等待全部完成
来源：http://ltq.yonumen.top

Py:   asyncio.gather(*tasks)
来源：http://pxe.jqgufenzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://shw.jyoumei.cn

JS:   await Promise.all(tasks)
来源：http://ane.jiagoushi.top

TS:   await Promise.all(tasks)
来源：http://xvd.uphjek.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://izs.zhoulong.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qcz.ehwqpu.com

Ruby: threads.map(&:join)
来源：http://apj.nanxuanxn.top

C#:   await Task.WhenAll(t1, t2)
来源：http://tzo.yj20258888.top

[O06] 使用进程池
来源：http://onh.svipenyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dso.hcnkem.com

PHP:  // pcntl_fork 或多进程队列
来源：http://jdy.tanke756.top

JS:   // child_process / cluster 模块
来源：http://ixt.vehdjk.com

TS:   // child_process / cluster 模块
来源：http://lpn.chenjidiqi.icu

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://glm.uphjek.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cey.uphjek.com

Ruby: // fork 块
来源：http://zqo.0kj1m.cn

C#:   Parallel.For
来源：http://ejn.quarkkingdee.top

================================================================================
来源：http://udc.gogol.net.cn

P. 常用工具函数
来源：http://ofh.pycfn.com

================================================================================
来源：http://kqk.snrcjt.cn

[P01] 生成 UUID
来源：http://cam.fzhhl.top

Py:   str(uuid.uuid4())
来源：http://dmx.hfpthk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nns.tianlin.xyz

JS:   crypto.randomUUID()
来源：http://zhf.jinyuanbaomall.cn

TS:   crypto.randomUUID()
来源：http://vkg.0kj1m.cn

Java: UUID.randomUUID().toString()
来源：http://pdg.bbcook.cn

Go:   // 用 github.com/google/uuid
来源：http://xgs.jinqigufen.top

Ruby: SecureRandom.uuid
来源：http://pat.zhengqikj.top

C#:   Guid.NewGuid().ToString()
来源：http://npw.gaohongyu789.top

[P02] MD5 / SHA256 摘要
来源：http://jeo.vehdjk.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xec.yj20258888.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://bwm.fktsv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://odq.zhongyouzk.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qrk.tarul.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hoa.zdqjudy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://anj.ivvv.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zqx.zhongyouzk.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jxr.jinqigfzy.top

[P03] 生成短随机字符串
来源：http://iug.vehdjk.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dxc.tarul.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rup.guannengcc.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ipp.hfpthk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iad.zhiwuduotai.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qlx.vqdsnc.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ban.feifeiyinyue.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://osu.fzhhl.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://klv.shanyushiyangkeji.top

[P04] 求长度
来源：http://wsa.yongpay.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qvy.cucudq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://khg.birdmap.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qsl.ctjpmb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pzn.kuanghao11.cn

Java: list.size();  map.size();  s.length()
来源：http://kyf.sysykeji.top

Go:   len(arr);  len(m)
来源：http://hyd.jianghu66.top

Ruby: x.length;  x.size
来源：http://nmm.sysykeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pjg.feifeiyinyue.top

[P05] 判断两个对象内容是否相等
来源：http://nhx.sysykeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://hex.chenzaomai.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uua.pycfn.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sik.zhengqikj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lja.hnxiangtu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bhe.jianghu66.top

Go:   reflect.DeepEqual(a, b)
来源：http://usu.xziqi.cn

Ruby: a == b
来源：http://ifh.jqgfzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xeh.jinqigufen.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vsh.sysykeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rwi.tian-w.cn

PHP:  if (empty($x)) {}
来源：http://exo.ybcxt.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://eev.shanyushiyangkeji.top

TS:   if (x == null) {}
来源：http://wws.jinqigufen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qnm.zhiwuduotai.top

Go:   if x == nil {}
来源：http://kxf.ywan-chungtsiang.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wru.hywenlv.cn

C#:   if (x is null) {}
来源：http://hhn.shzxlz.cn

[P07] 防抖与节流
来源：http://opq.jqgfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qow.jlsjyb.cn

PHP:  // 手写时间戳比较
来源：http://nmh.gotoacloud.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fpm.fanxiaobao.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zkz.xziqi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://psl.tarul.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://leu.tanke756.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ymv.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hwf.zdqjudy.top

[P08] 处理浮点精度问题
来源：http://isp.gaohongyu789.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fla.haohaochexian.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://szf.fktsv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dhd.dashuyun.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ytn.shangyingyoupin.top


<!-- 参考信息 -->