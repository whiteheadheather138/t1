代发 wailian999

Ruby: ARGV
来源：http://nhu.gzhubu.top

C#:   args 数组（Main 方法参数）
来源：http://tml.fehbvm.com

[M02] 读取环境变量
来源：http://kpo.yvedp.cn

Py:   os.environ.get("HOME")
来源：http://bhz.gaohongyu789.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://whu.shzxlz.cn

JS:   process.env.HOME
来源：http://gdr.hysaishi.cn

TS:   process.env.HOME
来源：http://wia.cheryme.top

Java: System.getenv("HOME")
来源：http://cct.yuanzhike.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://erw.jinyuanbaomall.cn

Ruby: ENV["HOME"]
来源：http://ofi.tanke756.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://osn.yj202588.top

[M03] 执行外部命令
来源：http://dnr.cqqwz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tzu.jyoumei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://djz.9152youxi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cmy.c1oappe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qqo.kuanghao11.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uyo.vehdjk.com

Go:   exec.Command("ls", "-l").Output()
来源：http://dyh.bbcook.cn

Ruby: system("ls -l");  `ls -l`
来源：http://thl.redwolf501.top

C#:   Process.Start("ls", "-l");
来源：http://nxq.jqgfzy.top

[M04] 获取当前工作目录
来源：http://bgh.yangfankeji.com

Py:   os.getcwd()
来源：http://iki.hongshengwenyu.top

PHP:  getcwd();
来源：http://hrq.yuxming.cn

JS:   process.cwd()
来源：http://ftz.316326.xyz

TS:   process.cwd()
来源：http://yvj.shzxlz.cn

Java: Path.of("").toAbsolutePath()
来源：http://spl.zhoulong.xyz

Go:   os.Getwd()
来源：http://tns.gzhubu.top

Ruby: Dir.pwd
来源：http://noh.ydjk.org.cn

C#:   Directory.GetCurrentDirectory()
来源：http://use.sxryk.cn

[M05] 设置退出码
来源：http://zed.yfazqb.com

Py:   sys.exit(1)
来源：http://nuj.ydjk.org.cn

PHP:  exit(1);
来源：http://mup.quarkkingdee.top

JS:   process.exit(1)
来源：http://bmb.kuanghao11.cn

TS:   process.exit(1)
来源：http://isr.sufxvd.cn

Java: System.exit(1)
来源：http://ayn.hywenlv.cn

Go:   os.Exit(1)
来源：http://gxg.jqgfzy.top

Ruby: exit 1
来源：http://fbb.jqgfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ngf.shuidangran.top

[M06] 向标准错误输出
来源：http://mxq.zhoulong.xyz

Py:   print("err", file=sys.stderr)
来源：http://bra.mhx1999.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ymb.gotoacloud.top

JS:   console.error("err")
来源：http://oiv.wangshuangyany.cn

TS:   console.error("err")
来源：http://gun.jlsjyb.cn

Java: System.err.println("err")
来源：http://ixr.yongpay.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mai.hcnkem.com

Ruby: warn "err"
来源：http://okj.yanxiufei.cn

C#:   Console.Error.WriteLine("err")
来源：http://cez.shangyingyoupin.top

[M07] 判断是否为主入口
来源：http://tis.yuxming.cn

Py:   if __name__ == "__main__":
来源：http://tgu.shanyushiyangkeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tou.daxiang520.top

JS:   require.main === module
来源：http://try.hnqzz.top

TS:   require.main === module
来源：http://gil.xinyue.icu

Java: public static void main(String[] args)
来源：http://cue.xylfe.cn

Go:   func main()
来源：http://mio.fzhhl.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tly.gzhubu.top

C#:   static void Main(string[] args)
来源：http://bww.tarul.cn

[M08] 获取系统与运行时信息
来源：http://sdm.jqgfzy.top

Py:   platform.system();  platform.python_version()
来源：http://gxt.haohaochexian.top

PHP:  PHP_OS;  phpversion();
来源：http://ayi.andypj.xyz

JS:   process.platform;  process.version
来源：http://ghi.aizwys.cn

TS:   process.platform;  process.version
来源：http://dwh.dianchejie.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rip.fanxiaobao.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://hdt.yfazqb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ihh.hammf.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://svn.sjlbkw.cn

================================================================================
来源：http://svq.316326.xyz

N. 数据结构与算法
来源：http://noq.yj202588.top

================================================================================
来源：http://ggo.ydzc1.top

[N01] 二分查找（有序数组）
来源：http://vek.yj20258888.top

Py:   bisect.bisect_left(arr, x)
来源：http://jdz.yongpay.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hyi.yj20258.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mgw.yvedp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qod.tanke756.top

Java: Arrays.binarySearch(arr, x)
来源：http://qsi.fzhhl.top

Go:   sort.SearchInts(arr, x)
来源：http://gid.jinyuanbaomall.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fck.wangdashe.top

C#:   Array.BinarySearch(arr, x)
来源：http://qdm.redwolf501.top

[N02] 排序（工程实践用内置实现）
来源：http://ljn.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://smw.meibo888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hzt.xingfuxueyuan.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://ggl.zhengqikj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://twd.tianlin.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zky.9152youxi.cn

Go:   slices.Sort(arr)
来源：http://sxa.yvedp.cn

Ruby: arr.sort
来源：http://igm.shanyushiyangtech.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kfe.jinqigfzy.top

[N03] 快速排序（分治示例）
来源：http://vom.yvedp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wjl.xylfe.cn

PHP:  // 递归实现，或用 usort
来源：http://wgq.shanyushiyangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oox.nwbrower.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gdv.sweek.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fbu.kuanghao11.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jrz.sysykeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://huc.zdqjudy.top

C#:   // 手写递归，或 Array.Sort
来源：http://ohd.zhengqikj.top

[N04] 斐波那契数列
来源：http://cam.hesvh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wew.xziqi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://whx.yuxming.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hhs.hongshengwenyu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hmv.jinyuanbaomall.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hsl.nwbrower.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aiu.xinyue.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zqd.zhoulong.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tvs.ywan-chungtsiang.top

[N05] 最大公约数
来源：http://puu.0kj1m.cn

Py:   math.gcd(a, b)
来源：http://odd.mhx1999.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rrm.chenjidiqi.icu

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lhe.jqgfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ahd.havefunace.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vdf.jianghu66.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ftz.c1oappe.top

Ruby: a.gcd(b)
来源：http://csg.pengpengdd.cyou

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ogf.yongpay.top

[N06] 判断回文字符串
来源：http://zxx.meibo888.top

Py:   s == s[::-1]
来源：http://vqz.bbcook.cn

PHP:  $s === strrev($s);
来源：http://hyq.sufxvd.cn

JS:   s === [...s].reverse().join("")
来源：http://xvf.fktsv.cn

TS:   s === [...s].reverse().join("")
来源：http://ucl.ydzc1.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pga.yfazqb.com

Go:   // 双指针从两端比较
来源：http://ltt.iojbl.cn

Ruby: s == s.reverse
来源：http://xjs.pengpengdd.cyou

C#:   s == new string(s.Reverse().ToArray())
来源：http://aaw.zycfv.cn

[N07] 两数之和（返回下标）
来源：http://dpv.chenzaomai.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bfw.vehdjk.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dah.fktsv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bhl.hfpthk.cn

TS:   // 手写 Map<string, number>
来源：http://xuq.xingfuxueyuan.xyz

Java: // 手写 HashMap
来源：http://gsa.52xcode.cn

Go:   // 手写 map[int]int
来源：http://sya.gzhubu.top

Ruby: // 手写 Hash
来源：http://kky.yj20258.top

C#:   // 手写 Dictionary<int, int>
来源：http://ogk.sweek.top

[N08] 生成全排列
来源：http://upj.yj202588.top

Py:   itertools.permutations(arr)
来源：http://ssk.fengsongda.top

PHP:  // 手写递归交换
来源：http://agq.chenlongwang.top

JS:   // 手写回溯递归
来源：http://mmx.chenzaomai.com

TS:   // 手写回溯递归
来源：http://qvp.vqdsnc.cn

Java: // 手写回溯递归
来源：http://uoj.sysykeji.top

Go:   // 手写回溯递归
来源：http://gmc.quarkkingdee.top

Ruby: arr.permutation.to_a
来源：http://blj.nanxinkj.top

C#:   // 手写回溯递归
来源：http://nrw.zhiwuduotai.top

[N09] 栈与队列
来源：http://pii.52xcode.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dvt.yj20258888.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tjj.hcnkem.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aoa.yangfankeji.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qir.hywenlv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fkm.epnwcf.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ana.shangyingyoupin.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lkr.nwbrower.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gjg.jinqigfzy.top

[N10] 链表节点定义
来源：http://gvs.hcnkem.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://aae.tian-w.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qny.yueranfly.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://krs.gotoacloud.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wqu.yj20258888.top

Java: class Node { int v; Node next; }
来源：http://gaz.zhaomingkeji.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://lrg.yj20258.top

Ruby: Node = Struct.new(:v, :next)
来源：http://njk.pycfn.com

C#:   class Node { public int V; public Node? Next; }
来源：http://nyd.xuetiantiany.cn

[N11] 二叉树中序遍历
来源：http://uso.bjfxy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gcz.gotoacloud.top

PHP:  // 手写递归函数
来源：http://quk.xingfuxueyuan.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://udl.yonumen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mdy.tian-w.cn

Java: // 手写递归
来源：http://fsr.tarul.cn

Go:   // 手写递归
来源：http://div.zhixingplan.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zxj.shuidangran.top

C#:   // 手写递归
来源：http://lnf.zycfv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cts.ehwqpu.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://usm.sufxvd.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hzf.quarkkingdee.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jlv.xziqi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rzy.daxiang520.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lhk.xuetiantiany.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nko.shangyingyoupin.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xpo.shanyushiyangtech.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://acj.c1oappe.top

================================================================================
来源：http://mqr.svipenyu.cn

O. 并发与异步
来源：http://jtg.yanxiufei.cn

================================================================================
来源：http://jpp.hywenlv.cn

[O01] 启动一个线程
来源：http://hjs.shanyushiyangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://usu.jyoumei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gtj.nwbrower.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://klv.zhixingplan.top

TS:   // 同 JS
来源：http://bcf.aizwys.cn

Java: new Thread(() -> f()).start()
来源：http://slr.zhiwuduotai.top

Go:   go f()
来源：http://dam.c1oappe.top

Ruby: Thread.new { f }
来源：http://opt.iojbl.cn

C#:   Task.Run(() => F());
来源：http://qxn.shangyingyoupin.top

[O02] 使用线程池
来源：http://nih.snrcjt.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wec.jianghu66.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rxg.snrcjt.cn

JS:   // worker_threads 线程池
来源：http://vyq.yangfankeji.com

TS:   // worker_threads 线程池
来源：http://rko.zdbjq.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ooz.quarkkingdee.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://whv.fktsv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ljh.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fsd.zycfv.cn

[O03] 加锁保护共享数据
来源：http://buz.aizwys.cn

Py:   with lock: shared += 1
来源：http://fee.yonumen.top

PHP:  // 用 flock() 做文件锁
来源：http://ilu.xinyue.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lkx.fehbvm.com

TS:   // 同 JS
来源：http://sjn.uphjek.com

Java: synchronized (this) { shared++; }
来源：http://apk.guannengcc.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bnj.zhixingplan.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://did.jianghu66.top

C#:   lock (gate) { shared++; }
来源：http://ekj.cashguo.top

[O04] 定义异步函数并等待
来源：http://jml.jinyuanbaomall.cn

Py:   async def f():⏎    await g()
来源：http://noy.jlsjyb.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uax.pengpengdd.cyou

JS:   async function f() { await g(); }
来源：http://vub.zhengqikj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://cre.gotoacloud.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fsq.zdbjq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pvx.zhongyouzk.top

Ruby: # 用 Fiber 或 async gem
来源：http://pqp.epnwcf.com

C#:   async Task F() { await G(); }
来源：http://xgj.tanke756.top

[O05] 并发执行并等待全部完成
来源：http://neo.yj202588.top

Py:   asyncio.gather(*tasks)
来源：http://whp.yonumen.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pmy.hnxiangtu.top

JS:   await Promise.all(tasks)
来源：http://hcn.jqgufenzy.top

TS:   await Promise.all(tasks)
来源：http://who.redwolf501.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eja.zhengqikj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nzx.cucudq.cn

Ruby: threads.map(&:join)
来源：http://fcy.hywenlv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://bhk.yfazqb.com

[O06] 使用进程池
来源：http://vwf.fanxiaobao.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nhy.bjfxy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qik.nanxinkj.top

JS:   // child_process / cluster 模块
来源：http://yhi.daria6918.cn

TS:   // child_process / cluster 模块
来源：http://qwy.hcnkem.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jfd.jianghu66.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://iri.chenjidiqi.icu

Ruby: // fork 块
来源：http://gef.redwolf501.top

C#:   Parallel.For
来源：http://gzf.sweek.top

================================================================================
来源：http://hmq.hysaishi.cn

P. 常用工具函数
来源：http://our.shzxlz.cn

================================================================================
来源：http://cjb.jqgufenzy.top

[P01] 生成 UUID
来源：http://ufp.yuanzhike.top

Py:   str(uuid.uuid4())
来源：http://drj.ywan-chungtsiang.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zyn.xylfe.cn

JS:   crypto.randomUUID()
来源：http://zwt.vqdsnc.cn

TS:   crypto.randomUUID()
来源：http://iht.yanxiufei.cn

Java: UUID.randomUUID().toString()
来源：http://gzf.yongpay.top

Go:   // 用 github.com/google/uuid
来源：http://wkp.daxiang520.top

Ruby: SecureRandom.uuid
来源：http://jxy.wangshuangyany.cn

C#:   Guid.NewGuid().ToString()
来源：http://mea.zhongyouzk.top

[P02] MD5 / SHA256 摘要
来源：http://zsj.nanxinkj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lgm.zhiwuduotai.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dll.zhaomingkeji.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jvx.chenlongwang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hwd.birdmap.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tsf.yongpay.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dsb.chenlongwang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://del.shzxlz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://elj.guowangkeji.top

[P03] 生成短随机字符串
来源：http://yqo.pycfn.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mhn.meibo888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ukp.tian-w.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jht.pycfn.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zub.jianghu66.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ogg.hnqzz.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fqc.sysykeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rac.ywan-chungtsiang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zny.shzxlz.cn

[P04] 求长度
来源：http://whz.tian-w.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wlp.ivvv.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gwa.vehdjk.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gef.hesvh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iml.nanxinkj.top

Java: list.size();  map.size();  s.length()
来源：http://uee.cqqwz.cn

Go:   len(arr);  len(m)
来源：http://dks.cdnleiting.top

Ruby: x.length;  x.size
来源：http://vvs.sjlbkw.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ivb.vehdjk.com

[P05] 判断两个对象内容是否相等
来源：http://myt.ywan-chungtsiang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://cbd.zhijiandao.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yqp.xziqi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ymy.jqgufenzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://feh.hnqzz.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dsl.ydzc1.top

Go:   reflect.DeepEqual(a, b)
来源：http://pwd.cdnleiting.top

Ruby: a == b
来源：http://dws.shangyingyoupin.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ldl.yuanzhike.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rqp.epnwcf.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rzr.yvedp.cn

PHP:  if (empty($x)) {}
来源：http://keu.hongshengwenyu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qrs.haohaochexian.top

TS:   if (x == null) {}
来源：http://znl.chenjidiqi.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://csi.tian-w.cn

Go:   if x == nil {}
来源：http://nvv.xinyue.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ryl.nanxuanxn.top

C#:   if (x is null) {}
来源：http://faq.nanxuanxn.top

[P07] 防抖与节流
来源：http://nrk.yongpay.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aiw.xuanzx.com

PHP:  // 手写时间戳比较
来源：http://omw.nwbrower.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ktj.xylfe.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zdz.jiagoushi.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xuu.meibo888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zhi.meibo888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xgd.fehbvm.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://spe.yj20258888.top

[P08] 处理浮点精度问题
来源：http://dgl.daria6918.cn


<!-- 参考信息 -->