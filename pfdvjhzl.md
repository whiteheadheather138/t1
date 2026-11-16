代发 wailian999

JS:   process.argv.slice(2)
来源：http://irf.jinqigfzy.top

TS:   process.argv.slice(2)
来源：http://fbi.guannengcc.top

Java: args 数组（main 方法参数）
来源：http://otd.nwbrower.top

Go:   os.Args[1:]
来源：http://bfg.hfpthk.cn

Ruby: ARGV
来源：http://svn.aibaodan.cn

C#:   args 数组（Main 方法参数）
来源：http://rjd.52xcode.cn

[M02] 读取环境变量
来源：http://rct.gotoacloud.top

Py:   os.environ.get("HOME")
来源：http://ksn.yuanzhike.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lwt.9152youxi.cn

JS:   process.env.HOME
来源：http://lno.nwbrower.top

TS:   process.env.HOME
来源：http://iai.yuanzhike.top

Java: System.getenv("HOME")
来源：http://cie.nanxuanxn.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dxd.yuanzhike.top

Ruby: ENV["HOME"]
来源：http://usz.dashuyun.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ukc.andypj.xyz

[M03] 执行外部命令
来源：http://nix.fzhhl.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mxv.chenlongwang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zdv.ppjwa.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qhp.zdbjq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oyn.shzxlz.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gmf.52xcode.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://smb.xingfuxueyuan.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://jcy.ywan-chungtsiang.top

C#:   Process.Start("ls", "-l");
来源：http://iqz.yj202588.top

[M04] 获取当前工作目录
来源：http://evf.shuidangran.top

Py:   os.getcwd()
来源：http://imy.snrcjt.cn

PHP:  getcwd();
来源：http://sop.tanke756.top

JS:   process.cwd()
来源：http://deo.ydzc1.top

TS:   process.cwd()
来源：http://ols.jinyuanbaomall.cn

Java: Path.of("").toAbsolutePath()
来源：http://tlq.0kj1m.cn

Go:   os.Getwd()
来源：http://ffh.cdnleiting.top

Ruby: Dir.pwd
来源：http://tgx.daria6918.cn

C#:   Directory.GetCurrentDirectory()
来源：http://avs.sxryk.cn

[M05] 设置退出码
来源：http://ruy.hongshengwenyu.top

Py:   sys.exit(1)
来源：http://ceq.zhaomingkeji.xyz

PHP:  exit(1);
来源：http://xkn.nwbrower.top

JS:   process.exit(1)
来源：http://rus.yj20258888.top

TS:   process.exit(1)
来源：http://qta.jqgufenzy.top

Java: System.exit(1)
来源：http://vww.52xcode.cn

Go:   os.Exit(1)
来源：http://lbz.pengpengdd.cyou

Ruby: exit 1
来源：http://zdf.fehbvm.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hqf.hammf.cn

[M06] 向标准错误输出
来源：http://mpp.9152youxi.cn

Py:   print("err", file=sys.stderr)
来源：http://ljn.nwbrower.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ikm.jiagoushi.top

JS:   console.error("err")
来源：http://wyl.zdbjq.cn

TS:   console.error("err")
来源：http://svi.0kj1m.cn

Java: System.err.println("err")
来源：http://yuj.uphjek.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nme.quarkkingdee.top

Ruby: warn "err"
来源：http://oxw.ctjpmb.com

C#:   Console.Error.WriteLine("err")
来源：http://rpd.haohaochexian.top

[M07] 判断是否为主入口
来源：http://hvu.hcnkem.com

Py:   if __name__ == "__main__":
来源：http://cza.zhoulong.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zrs.zhongyouzk.top

JS:   require.main === module
来源：http://mxh.sxryk.cn

TS:   require.main === module
来源：http://xvf.daxiang520.top

Java: public static void main(String[] args)
来源：http://iwt.yj20258888.top

Go:   func main()
来源：http://mst.aibaodan.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://phx.shanyushiyangtech.top

C#:   static void Main(string[] args)
来源：http://rgc.meibo888.top

[M08] 获取系统与运行时信息
来源：http://fij.zdqjudy.top

Py:   platform.system();  platform.python_version()
来源：http://bzs.cheryme.top

PHP:  PHP_OS;  phpversion();
来源：http://dqn.gotoacloud.top

JS:   process.platform;  process.version
来源：http://wrd.iojbl.cn

TS:   process.platform;  process.version
来源：http://xpc.bbcook.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lvj.guannengcc.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dxz.guowangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zom.zhaomingkeji.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://ynw.jqgfzy.top

================================================================================
来源：http://qfh.0kj1m.cn

N. 数据结构与算法
来源：http://gor.ywan-chungtsiang.top

================================================================================
来源：http://zhl.c1oappe.top

[N01] 二分查找（有序数组）
来源：http://pgy.bbcook.cn

Py:   bisect.bisect_left(arr, x)
来源：http://thh.ydzc1.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bik.sxryk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vzz.jinqigufen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bmv.zhixingplan.top

Java: Arrays.binarySearch(arr, x)
来源：http://jsh.zycfv.cn

Go:   sort.SearchInts(arr, x)
来源：http://qmj.ctjpmb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://mpu.jinyuanbaomall.cn

C#:   Array.BinarySearch(arr, x)
来源：http://iyr.ivvv.top

[N02] 排序（工程实践用内置实现）
来源：http://goq.jqgfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://xrf.hesvh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tsv.zhijiandao.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kiv.nwbrower.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xgd.cashguo.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ckc.guannengcc.top

Go:   slices.Sort(arr)
来源：http://smg.fanxiaobao.xyz

Ruby: arr.sort
来源：http://aby.ehwqpu.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://muh.ybcxt.top

[N03] 快速排序（分治示例）
来源：http://sbv.yangfankeji.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gze.52xcode.cn

PHP:  // 递归实现，或用 usort
来源：http://foj.hcnkem.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mlo.sxryk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://itu.yongpay.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://txl.xziqi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bkw.0kj1m.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://koc.ctjpmb.com

C#:   // 手写递归，或 Array.Sort
来源：http://wbk.cucudq.cn

[N04] 斐波那契数列
来源：http://qcn.hammf.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ydw.jianghu66.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vic.zhixingplan.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xlm.daria6918.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xqf.cheryme.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xrh.pengpengdd.cyou

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ypl.cucudq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cio.havefunace.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jep.tian-w.cn

[N05] 最大公约数
来源：http://ubr.yfazqb.com

Py:   math.gcd(a, b)
来源：http://afk.pengpengdd.cyou

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://knf.xingfuxueyuan.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yvr.52xcode.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ybo.sweek.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tbu.chenjidiqi.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mye.guannengcc.top

Ruby: a.gcd(b)
来源：http://rzj.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://acz.gogol.net.cn

[N06] 判断回文字符串
来源：http://jlf.sjlbkw.cn

Py:   s == s[::-1]
来源：http://pxs.xuanzx.com

PHP:  $s === strrev($s);
来源：http://nhz.shanyushiyangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://eze.hesvh.cn

TS:   s === [...s].reverse().join("")
来源：http://ugy.yuanzhike.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://acl.cqqwz.cn

Go:   // 双指针从两端比较
来源：http://dhb.redwolf501.top

Ruby: s == s.reverse
来源：http://apq.yonumen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bbp.yj20258.top

[N07] 两数之和（返回下标）
来源：http://rwl.vqdsnc.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ech.fehbvm.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jrj.redwolf501.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bvm.cdnleiting.top

TS:   // 手写 Map<string, number>
来源：http://jjn.xuanzx.com

Java: // 手写 HashMap
来源：http://zme.yj20258.top

Go:   // 手写 map[int]int
来源：http://olp.svipenyu.cn

Ruby: // 手写 Hash
来源：http://skp.daxiang520.top

C#:   // 手写 Dictionary<int, int>
来源：http://wgt.havefunace.top

[N08] 生成全排列
来源：http://jej.havefunace.top

Py:   itertools.permutations(arr)
来源：http://lze.yangfankeji.com

PHP:  // 手写递归交换
来源：http://nad.hesvh.cn

JS:   // 手写回溯递归
来源：http://tvq.yj20258888.top

TS:   // 手写回溯递归
来源：http://tvc.cheryme.top

Java: // 手写回溯递归
来源：http://ofh.pycfn.com

Go:   // 手写回溯递归
来源：http://tfk.hnxiangtu.top

Ruby: arr.permutation.to_a
来源：http://heq.cheryme.top

C#:   // 手写回溯递归
来源：http://asa.yonumen.top

[N09] 栈与队列
来源：http://udc.hfpthk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bko.jinyuanbaomall.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lue.tarul.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qjr.kuanghao11.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uza.sweek.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://txl.aibaodan.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zon.kuanghao11.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://snz.hongshengwenyu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xzg.zdqjudy.top

[N10] 链表节点定义
来源：http://wyo.yangfankeji.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vvf.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fwd.wangshuangyany.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wwd.guannengcc.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mlv.cucudq.cn

Java: class Node { int v; Node next; }
来源：http://lzx.chenzaomai.com

Go:   type Node struct { V int; Next *Node }
来源：http://iff.sxryk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zeb.fanxiaobao.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://vqm.yuanzhike.top

[N11] 二叉树中序遍历
来源：http://csn.ybcxt.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://psi.gzhubu.top

PHP:  // 手写递归函数
来源：http://bho.jianghu66.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ruz.hammf.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ltf.cqqwz.cn

Java: // 手写递归
来源：http://cih.birdmap.top

Go:   // 手写递归
来源：http://eqh.yongpay.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oxc.daria6918.cn

C#:   // 手写递归
来源：http://gsw.jianghu66.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vwg.jyoumei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://upq.haohaochexian.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dat.pycfn.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://png.aizwys.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://esc.ybcxt.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mmv.xuanzx.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wwz.ydzc1.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lvo.bbcook.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mwn.birdmap.top

================================================================================
来源：http://sti.hnxiangtu.top

O. 并发与异步
来源：http://ilm.sysykeji.top

================================================================================
来源：http://erc.jinyuanbaomall.cn

[O01] 启动一个线程
来源：http://skb.yuanzhike.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://eot.yongpay.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ffo.uphjek.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://byc.aizwys.cn

TS:   // 同 JS
来源：http://xdu.havefunace.top

Java: new Thread(() -> f()).start()
来源：http://aan.jqgfzy.top

Go:   go f()
来源：http://oxo.kuanghao11.cn

Ruby: Thread.new { f }
来源：http://yyn.quarkkingdee.top

C#:   Task.Run(() => F());
来源：http://lhz.feifeiyinyue.top

[O02] 使用线程池
来源：http://lgq.dianchejie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ufg.zdbjq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mja.yj202588.top

JS:   // worker_threads 线程池
来源：http://rmj.chenlongwang.top

TS:   // worker_threads 线程池
来源：http://frq.cqqwz.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qxz.pengpengdd.cyou

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://soh.meibo888.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ezf.ehwqpu.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mgt.jinqigfzy.top

[O03] 加锁保护共享数据
来源：http://ldo.jinqigufen.top

Py:   with lock: shared += 1
来源：http://nnd.316326.xyz

PHP:  // 用 flock() 做文件锁
来源：http://qdl.52xcode.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pzc.yonumen.top

TS:   // 同 JS
来源：http://tfz.hfpthk.cn

Java: synchronized (this) { shared++; }
来源：http://jbg.kuanghao11.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://quu.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://sle.snrcjt.cn

C#:   lock (gate) { shared++; }
来源：http://ubd.chenzaomai.com

[O04] 定义异步函数并等待
来源：http://iep.jyoumei.cn

Py:   async def f():⏎    await g()
来源：http://bzv.ctjpmb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vor.jinqigfzy.top

JS:   async function f() { await g(); }
来源：http://igh.yueranfly.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://iov.nanxuanxn.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vbl.yuanzhike.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wjq.ppjwa.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bhv.shzxlz.cn

C#:   async Task F() { await G(); }
来源：http://iqi.cheryme.top

[O05] 并发执行并等待全部完成
来源：http://osg.zhixingplan.top

Py:   asyncio.gather(*tasks)
来源：http://tis.meibo888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tyt.52xcode.cn

JS:   await Promise.all(tasks)
来源：http://sgq.pycfn.com

TS:   await Promise.all(tasks)
来源：http://yti.jinqigufen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gdr.haohaochexian.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zah.quarkkingdee.top

Ruby: threads.map(&:join)
来源：http://isd.yanxiufei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tai.nwbrower.top

[O06] 使用进程池
来源：http://nxe.shangyingyoupin.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pub.zhengqikj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mmi.shangyingyoupin.top

JS:   // child_process / cluster 模块
来源：http://xmk.iojbl.cn

TS:   // child_process / cluster 模块
来源：http://qfq.jlsjyb.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cak.svipenyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yjs.zhiwuduotai.top

Ruby: // fork 块
来源：http://lwv.aibaodan.cn

C#:   Parallel.For
来源：http://xvl.yj20258.top

================================================================================
来源：http://ifw.yuxming.cn

P. 常用工具函数
来源：http://mwn.52xcode.cn

================================================================================
来源：http://oih.svipenyu.cn

[P01] 生成 UUID
来源：http://cyd.shangyingyoupin.top

Py:   str(uuid.uuid4())
来源：http://qto.yueranfly.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mde.nwbrower.top

JS:   crypto.randomUUID()
来源：http://jir.ydjk.org.cn

TS:   crypto.randomUUID()
来源：http://obf.ctjpmb.com

Java: UUID.randomUUID().toString()
来源：http://cbf.zhixingplan.top

Go:   // 用 github.com/google/uuid
来源：http://kvr.yvedp.cn

Ruby: SecureRandom.uuid
来源：http://evu.xuanzx.com

C#:   Guid.NewGuid().ToString()
来源：http://cyc.zhoulong.xyz

[P02] MD5 / SHA256 摘要
来源：http://vke.yvedp.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uiy.zhoulong.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://rqu.yongpay.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://atn.svipenyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lww.wangshuangyany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mio.aibaodan.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ovy.9152youxi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://svm.sysykeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rww.meibo888.top

[P03] 生成短随机字符串
来源：http://grf.vehdjk.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gus.ehwqpu.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aas.yuxming.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hcq.fehbvm.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dps.cdnleiting.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lmu.hongshengwenyu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vop.xuetiantiany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qnx.hysaishi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wqq.gaohongyu789.top

[P04] 求长度
来源：http://itu.jianghu66.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xgr.quarkkingdee.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mjt.hongshengwenyu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nrm.cashguo.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cwz.c1oappe.top

Java: list.size();  map.size();  s.length()
来源：http://csl.andypj.xyz

Go:   len(arr);  len(m)
来源：http://zlm.shanyushiyangtech.top

Ruby: x.length;  x.size
来源：http://hmq.9152youxi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zql.xinyue.icu

[P05] 判断两个对象内容是否相等
来源：http://flm.yj20258.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://xbk.jyoumei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yai.jinghuilouyu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rgv.ybcxt.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yau.hcnkem.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hzk.shangyingyoupin.top

Go:   reflect.DeepEqual(a, b)
来源：http://qjl.sxryk.cn

Ruby: a == b
来源：http://pxl.jianghu66.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ugf.quarkkingdee.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yyn.tarul.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://axl.andypj.xyz

PHP:  if (empty($x)) {}
来源：http://bph.zhiwuduotai.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sfy.quarkkingdee.top

TS:   if (x == null) {}
来源：http://qwc.fanxiaobao.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://cjb.ppjwa.cn

Go:   if x == nil {}
来源：http://lpq.feifeiyinyue.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xiu.tanke756.top

C#:   if (x is null) {}
来源：http://nyi.cucudq.cn

[P07] 防抖与节流
来源：http://rmh.pengpengdd.cyou

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ryr.yvedp.cn

PHP:  // 手写时间戳比较
来源：http://maj.vqdsnc.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pbg.yongpay.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cqw.guannengcc.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://epx.redwolf501.top


<!-- 参考信息 -->