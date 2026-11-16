代发 wailian999

================================================================================
来源：http://rgl.xingfuxueyuan.xyz

[M01] 读取命令行参数
来源：http://cmo.zdbjq.cn

Py:   sys.argv[1:]
来源：http://rrc.hesvh.cn

PHP:  $argv;  $argc;
来源：http://mbh.jlsjyb.cn

JS:   process.argv.slice(2)
来源：http://rve.jinqigfzy.top

TS:   process.argv.slice(2)
来源：http://nkt.yj20258.top

Java: args 数组（main 方法参数）
来源：http://gsm.jqgufenzy.top

Go:   os.Args[1:]
来源：http://cep.tianlin.xyz

Ruby: ARGV
来源：http://qby.xylfe.cn

C#:   args 数组（Main 方法参数）
来源：http://tip.uphjek.com

[M02] 读取环境变量
来源：http://qpf.vqdsnc.cn

Py:   os.environ.get("HOME")
来源：http://unr.hnxiangtu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nqa.bbcook.cn

JS:   process.env.HOME
来源：http://ucf.xingfuxueyuan.xyz

TS:   process.env.HOME
来源：http://aqh.bbcook.cn

Java: System.getenv("HOME")
来源：http://csh.jqgufenzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gjs.hnqzz.top

Ruby: ENV["HOME"]
来源：http://tyu.0kj1m.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kbc.kuanghao11.cn

[M03] 执行外部命令
来源：http://scx.feifeiyinyue.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jlw.gotoacloud.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bxx.fehbvm.com

JS:   child_process.execSync("ls -l").toString()
来源：http://cie.9152youxi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bno.gogol.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nhp.ivvv.top

Go:   exec.Command("ls", "-l").Output()
来源：http://cgx.ydzc1.top

Ruby: system("ls -l");  `ls -l`
来源：http://xgq.cashguo.top

C#:   Process.Start("ls", "-l");
来源：http://sfv.jyoumei.cn

[M04] 获取当前工作目录
来源：http://jah.yvedp.cn

Py:   os.getcwd()
来源：http://whf.uphjek.com

PHP:  getcwd();
来源：http://abq.smart0.xyz

JS:   process.cwd()
来源：http://dvd.ybcxt.top

TS:   process.cwd()
来源：http://zwg.tianlin.xyz

Java: Path.of("").toAbsolutePath()
来源：http://afj.meibo888.top

Go:   os.Getwd()
来源：http://gra.mhx1999.top

Ruby: Dir.pwd
来源：http://jfe.yfazqb.com

C#:   Directory.GetCurrentDirectory()
来源：http://oeq.xuetiantiany.cn

[M05] 设置退出码
来源：http://xpl.mhx1999.top

Py:   sys.exit(1)
来源：http://wva.zhixingplan.top

PHP:  exit(1);
来源：http://crc.shuidangran.top

JS:   process.exit(1)
来源：http://bri.hywenlv.cn

TS:   process.exit(1)
来源：http://ohb.jqgufenzy.top

Java: System.exit(1)
来源：http://mqz.pycfn.com

Go:   os.Exit(1)
来源：http://wym.tianlin.xyz

Ruby: exit 1
来源：http://jiw.cashguo.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rjo.aizwys.cn

[M06] 向标准错误输出
来源：http://qms.nanxuanxn.top

Py:   print("err", file=sys.stderr)
来源：http://fzg.aibaodan.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ina.c1oappe.top

JS:   console.error("err")
来源：http://zzh.zhijiandao.cn

TS:   console.error("err")
来源：http://ijx.shuidangran.top

Java: System.err.println("err")
来源：http://art.ywan-chungtsiang.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lwh.sxryk.cn

Ruby: warn "err"
来源：http://pgo.jyoumei.cn

C#:   Console.Error.WriteLine("err")
来源：http://pey.feifeiyinyue.top

[M07] 判断是否为主入口
来源：http://zhh.hnxiangtu.top

Py:   if __name__ == "__main__":
来源：http://fki.cdnleiting.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mxe.feifeiyinyue.top

JS:   require.main === module
来源：http://qrc.shanyushiyangkeji.top

TS:   require.main === module
来源：http://dzh.sweek.top

Java: public static void main(String[] args)
来源：http://dti.sysykeji.top

Go:   func main()
来源：http://kob.yvedp.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ttr.nanxinkj.top

C#:   static void Main(string[] args)
来源：http://xfr.shangyingyoupin.top

[M08] 获取系统与运行时信息
来源：http://ixz.gotoacloud.top

Py:   platform.system();  platform.python_version()
来源：http://xtg.jiagoushi.top

PHP:  PHP_OS;  phpversion();
来源：http://hde.xylfe.cn

JS:   process.platform;  process.version
来源：http://tbp.yuanzhike.top

TS:   process.platform;  process.version
来源：http://wwo.jiagoushi.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ual.bbcook.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zju.yanxiufei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kln.shangyingyoupin.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ugz.smart0.xyz

================================================================================
来源：http://brz.zhoulong.xyz

N. 数据结构与算法
来源：http://ljv.havefunace.top

================================================================================
来源：http://oxt.jinqigfzy.top

[N01] 二分查找（有序数组）
来源：http://dru.shuidangran.top

Py:   bisect.bisect_left(arr, x)
来源：http://ult.ehwqpu.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dgg.ydjk.org.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ypc.ivvv.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qiq.wangdashe.top

Java: Arrays.binarySearch(arr, x)
来源：http://vvd.birdmap.top

Go:   sort.SearchInts(arr, x)
来源：http://bzr.hesvh.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lzs.316326.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://wud.chenzaomai.com

[N02] 排序（工程实践用内置实现）
来源：http://fon.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://rrb.xinyue.icu

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lhn.bjfxy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://yrx.52xcode.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://okm.iojbl.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oax.daria6918.cn

Go:   slices.Sort(arr)
来源：http://mbx.zdqjudy.top

Ruby: arr.sort
来源：http://rud.yj20258888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dit.jiagoushi.top

[N03] 快速排序（分治示例）
来源：http://xpf.jinqigufen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cwx.nanxuanxn.top

PHP:  // 递归实现，或用 usort
来源：http://rqy.aizwys.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tyk.yonumen.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cil.zhixingplan.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xhg.quarkkingdee.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sgg.aibaodan.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ngy.yj20258.top

C#:   // 手写递归，或 Array.Sort
来源：http://did.jianghu66.top

[N04] 斐波那契数列
来源：http://bcz.gogol.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pay.cashguo.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://esr.xylfe.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nez.svipenyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hqs.andypj.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wxt.quarkkingdee.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vye.jinghuilouyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nfz.yuanzhike.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wqu.quarkkingdee.top

[N05] 最大公约数
来源：http://slt.jinqigfzy.top

Py:   math.gcd(a, b)
来源：http://zzp.0kj1m.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lfh.ivvv.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ceg.chenjidiqi.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iic.yueranfly.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bsq.zhiwuduotai.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ott.fehbvm.com

Ruby: a.gcd(b)
来源：http://ugk.hfpthk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qeq.yanxiufei.cn

[N06] 判断回文字符串
来源：http://qdz.cqqwz.cn

Py:   s == s[::-1]
来源：http://jfm.tian-w.cn

PHP:  $s === strrev($s);
来源：http://fon.xuanzx.com

JS:   s === [...s].reverse().join("")
来源：http://pjr.fzhhl.top

TS:   s === [...s].reverse().join("")
来源：http://ueb.bjfxy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yml.yuanzhike.top

Go:   // 双指针从两端比较
来源：http://ebk.meibo888.top

Ruby: s == s.reverse
来源：http://ixf.yfazqb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://gly.ydzc1.top

[N07] 两数之和（返回下标）
来源：http://jlf.yongpay.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yji.zhengqikj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aeh.tianlin.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://fxj.jinghuilouyu.cn

TS:   // 手写 Map<string, number>
来源：http://fop.c1oappe.top

Java: // 手写 HashMap
来源：http://rqa.xingfuxueyuan.xyz

Go:   // 手写 map[int]int
来源：http://qoe.guowangkeji.top

Ruby: // 手写 Hash
来源：http://vxk.dianchejie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wmd.tanke756.top

[N08] 生成全排列
来源：http://hqu.zdbjq.cn

Py:   itertools.permutations(arr)
来源：http://jwn.hywenlv.cn

PHP:  // 手写递归交换
来源：http://qrw.ydjk.org.cn

JS:   // 手写回溯递归
来源：http://kfa.tarul.cn

TS:   // 手写回溯递归
来源：http://cpc.jianghu66.top

Java: // 手写回溯递归
来源：http://ijv.bbcook.cn

Go:   // 手写回溯递归
来源：http://kmn.ehwqpu.com

Ruby: arr.permutation.to_a
来源：http://jzr.daxiang520.top

C#:   // 手写回溯递归
来源：http://wyj.havefunace.top

[N09] 栈与队列
来源：http://nws.xuetiantiany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hwn.fktsv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ssl.316326.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qih.aibaodan.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xca.xuanzx.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nxi.andypj.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://efm.yj20258.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rkw.nwbrower.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://stu.shanyushiyangtech.top

[N10] 链表节点定义
来源：http://vwl.fehbvm.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dqb.yvedp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hca.hesvh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kru.jqgufenzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jqv.jqgfzy.top

Java: class Node { int v; Node next; }
来源：http://wag.ppjwa.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wba.yj202588.top

Ruby: Node = Struct.new(:v, :next)
来源：http://acb.jqgufenzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://poz.cucudq.cn

[N11] 二叉树中序遍历
来源：http://pos.chenzaomai.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jvl.xuanzx.com

PHP:  // 手写递归函数
来源：http://ekc.smart0.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://boz.kuanghao11.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ktc.snrcjt.cn

Java: // 手写递归
来源：http://mze.shanyushiyangkeji.top

Go:   // 手写递归
来源：http://mga.shzxlz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qjd.gaohongyu789.top

C#:   // 手写递归
来源：http://vtc.hywenlv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fef.zhaomingkeji.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vxc.nwbrower.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mfg.xinyue.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://urb.meibo888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kks.fehbvm.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://afr.hfpthk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jga.hnxiangtu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vly.ybcxt.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://viv.gogol.net.cn

================================================================================
来源：http://clv.gzhubu.top

O. 并发与异步
来源：http://qxt.hfpthk.cn

================================================================================
来源：http://fhd.jqgfzy.top

[O01] 启动一个线程
来源：http://ehk.feifeiyinyue.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://deu.xuetiantiany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ysz.xinyue.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://amf.hnxiangtu.top

TS:   // 同 JS
来源：http://arv.shuidangran.top

Java: new Thread(() -> f()).start()
来源：http://apf.aizwys.cn

Go:   go f()
来源：http://cob.ydjk.org.cn

Ruby: Thread.new { f }
来源：http://ilg.ydzc1.top

C#:   Task.Run(() => F());
来源：http://kmk.dianchejie.cn

[O02] 使用线程池
来源：http://wge.xuetiantiany.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vle.zhongyouzk.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tdh.bbcook.cn

JS:   // worker_threads 线程池
来源：http://nkk.fktsv.cn

TS:   // worker_threads 线程池
来源：http://rxi.ydzc1.top

Java: Executors.newFixedThreadPool(4)
来源：http://dxj.cdnleiting.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rzb.yangfankeji.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xoc.yuanzhike.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iti.zdbjq.cn

[O03] 加锁保护共享数据
来源：http://lxa.zhaomingkeji.xyz

Py:   with lock: shared += 1
来源：http://wqy.jinyuanbaomall.cn

PHP:  // 用 flock() 做文件锁
来源：http://cwv.smart0.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dlo.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://pdj.bbcook.cn

Java: synchronized (this) { shared++; }
来源：http://bjm.wangshuangyany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wts.fktsv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mtp.pycfn.com

C#:   lock (gate) { shared++; }
来源：http://xqt.fengsongda.top

[O04] 定义异步函数并等待
来源：http://qin.xingfuxueyuan.xyz

Py:   async def f():⏎    await g()
来源：http://aea.jinyuanbaomall.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cmb.jinqigfzy.top

JS:   async function f() { await g(); }
来源：http://aop.tarul.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://orv.birdmap.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sdl.tarul.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hrb.ywan-chungtsiang.top

Ruby: # 用 Fiber 或 async gem
来源：http://acg.cdnleiting.top

C#:   async Task F() { await G(); }
来源：http://hds.jqgufenzy.top

[O05] 并发执行并等待全部完成
来源：http://rmy.vqdsnc.cn

Py:   asyncio.gather(*tasks)
来源：http://qqr.yvedp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jac.cucudq.cn

JS:   await Promise.all(tasks)
来源：http://ldr.quarkkingdee.top

TS:   await Promise.all(tasks)
来源：http://ijf.uphjek.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fga.c1oappe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kvf.hongshengwenyu.top

Ruby: threads.map(&:join)
来源：http://yxk.sjlbkw.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wii.zhixingplan.top

[O06] 使用进程池
来源：http://elz.birdmap.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://goa.hongshengwenyu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kzn.cdnleiting.top

JS:   // child_process / cluster 模块
来源：http://dci.chenjidiqi.icu

TS:   // child_process / cluster 模块
来源：http://hti.guowangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uho.zhoulong.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bnz.52xcode.cn

Ruby: // fork 块
来源：http://kym.xylfe.cn

C#:   Parallel.For
来源：http://esn.ppjwa.cn

================================================================================
来源：http://nhm.shanyushiyangtech.top

P. 常用工具函数
来源：http://wmz.nanxinkj.top

================================================================================
来源：http://auq.zhijiandao.cn

[P01] 生成 UUID
来源：http://lst.jianghu66.top

Py:   str(uuid.uuid4())
来源：http://vqx.pengpengdd.cyou

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qzz.guannengcc.top

JS:   crypto.randomUUID()
来源：http://zay.shanyushiyangtech.top

TS:   crypto.randomUUID()
来源：http://lex.yvedp.cn

Java: UUID.randomUUID().toString()
来源：http://atn.bjfxy.top

Go:   // 用 github.com/google/uuid
来源：http://xxd.jinqigfzy.top

Ruby: SecureRandom.uuid
来源：http://qfs.52xcode.cn

C#:   Guid.NewGuid().ToString()
来源：http://kya.xylfe.cn

[P02] MD5 / SHA256 摘要
来源：http://nll.gzhubu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lev.cashguo.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ezd.havefunace.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nik.zhongyouzk.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://okf.xziqi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hgq.yvedp.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xjs.52xcode.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uwp.yonumen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xoc.wangdashe.top

[P03] 生成短随机字符串
来源：http://joo.guannengcc.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wwx.sysykeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nhc.cashguo.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zge.ppjwa.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://brl.aibaodan.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lmh.yongpay.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xec.316326.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://ofh.jinghuilouyu.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wqu.shuidangran.top

[P04] 求长度
来源：http://ljc.fehbvm.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vsw.fzhhl.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uir.yonumen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sim.gzhubu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mto.hesvh.cn

Java: list.size();  map.size();  s.length()
来源：http://hlk.shanyushiyangtech.top

Go:   len(arr);  len(m)
来源：http://vxn.cucudq.cn

Ruby: x.length;  x.size
来源：http://yce.hysaishi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://buh.nwbrower.top

[P05] 判断两个对象内容是否相等
来源：http://yod.chenlongwang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jlt.ehwqpu.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gdn.epnwcf.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jpn.yanxiufei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ugq.havefunace.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fdt.aibaodan.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qef.zhengqikj.top

Ruby: a == b
来源：http://xzq.tianlin.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hsc.9152youxi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vuc.uphjek.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cmd.hnxiangtu.top

PHP:  if (empty($x)) {}
来源：http://pwl.chenlongwang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iis.mhx1999.top

TS:   if (x == null) {}
来源：http://zwq.52xcode.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dox.yfazqb.com

Go:   if x == nil {}
来源：http://pgb.jianghu66.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lxi.jinqigufen.top

C#:   if (x is null) {}
来源：http://nri.shanyushiyangtech.top

[P07] 防抖与节流
来源：http://jow.epnwcf.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kpd.zhengqikj.top


<!-- 参考信息 -->