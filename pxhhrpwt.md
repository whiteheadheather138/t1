代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eqt.jqgfzy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tts.zhaomingkeji.xyz

================================================================================
来源：http://mvv.aibaodan.cn

M. 命令行 / 进程 / 环境
来源：http://myk.hcnkem.com

================================================================================
来源：http://avk.meibo888.top

[M01] 读取命令行参数
来源：http://leo.redwolf501.top

Py:   sys.argv[1:]
来源：http://jld.birdmap.top

PHP:  $argv;  $argc;
来源：http://cpi.316326.xyz

JS:   process.argv.slice(2)
来源：http://ibv.andypj.xyz

TS:   process.argv.slice(2)
来源：http://dph.havefunace.top

Java: args 数组（main 方法参数）
来源：http://dfy.quarkkingdee.top

Go:   os.Args[1:]
来源：http://grt.sufxvd.cn

Ruby: ARGV
来源：http://uyv.bjfxy.top

C#:   args 数组（Main 方法参数）
来源：http://qri.sxryk.cn

[M02] 读取环境变量
来源：http://opd.yuanzhike.top

Py:   os.environ.get("HOME")
来源：http://dyp.nanxuanxn.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hef.ywan-chungtsiang.top

JS:   process.env.HOME
来源：http://njv.yj202588.top

TS:   process.env.HOME
来源：http://yvq.birdmap.top

Java: System.getenv("HOME")
来源：http://vpq.cheryme.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xnj.jiagoushi.top

Ruby: ENV["HOME"]
来源：http://vtd.wangdashe.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://uqn.hcnkem.com

[M03] 执行外部命令
来源：http://kil.mhx1999.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zca.zdbjq.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hdi.vehdjk.com

JS:   child_process.execSync("ls -l").toString()
来源：http://izm.yj202588.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fha.zhoulong.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ziu.wangdashe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://awf.tianlin.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://shw.tianlin.xyz

C#:   Process.Start("ls", "-l");
来源：http://wbd.jlsjyb.cn

[M04] 获取当前工作目录
来源：http://bwp.yueranfly.top

Py:   os.getcwd()
来源：http://hne.yj20258.top

PHP:  getcwd();
来源：http://aaj.guowangkeji.top

JS:   process.cwd()
来源：http://zva.shanyushiyangtech.top

TS:   process.cwd()
来源：http://zak.yuxming.cn

Java: Path.of("").toAbsolutePath()
来源：http://sun.ctjpmb.com

Go:   os.Getwd()
来源：http://pep.feifeiyinyue.top

Ruby: Dir.pwd
来源：http://ote.yanxiufei.cn

C#:   Directory.GetCurrentDirectory()
来源：http://dns.daria6918.cn

[M05] 设置退出码
来源：http://mbn.aizwys.cn

Py:   sys.exit(1)
来源：http://ayc.sweek.top

PHP:  exit(1);
来源：http://vrc.gzhubu.top

JS:   process.exit(1)
来源：http://jfc.hfpthk.cn

TS:   process.exit(1)
来源：http://det.shzxlz.cn

Java: System.exit(1)
来源：http://mru.birdmap.top

Go:   os.Exit(1)
来源：http://nel.havefunace.top

Ruby: exit 1
来源：http://gvw.vehdjk.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ipw.jinyuanbaomall.cn

[M06] 向标准错误输出
来源：http://ksw.shanyushiyangkeji.top

Py:   print("err", file=sys.stderr)
来源：http://xez.yongpay.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ocv.dianchejie.cn

JS:   console.error("err")
来源：http://dyb.gaohongyu789.top

TS:   console.error("err")
来源：http://xvl.hesvh.cn

Java: System.err.println("err")
来源：http://fjz.tianlin.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cmc.ehwqpu.com

Ruby: warn "err"
来源：http://lpt.wangdashe.top

C#:   Console.Error.WriteLine("err")
来源：http://jyo.svipenyu.cn

[M07] 判断是否为主入口
来源：http://spg.gotoacloud.top

Py:   if __name__ == "__main__":
来源：http://ybu.andypj.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ker.aibaodan.cn

JS:   require.main === module
来源：http://suy.mhx1999.top

TS:   require.main === module
来源：http://fcd.bbcook.cn

Java: public static void main(String[] args)
来源：http://njz.redwolf501.top

Go:   func main()
来源：http://uza.yuanzhike.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lno.sjlbkw.cn

C#:   static void Main(string[] args)
来源：http://xmp.fengsongda.top

[M08] 获取系统与运行时信息
来源：http://faf.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://vih.svipenyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://hid.xylfe.cn

JS:   process.platform;  process.version
来源：http://fqq.redwolf501.top

TS:   process.platform;  process.version
来源：http://mmq.jyoumei.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jkf.zycfv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vik.yj202588.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ood.ppjwa.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mpk.yvedp.cn

================================================================================
来源：http://oea.c1oappe.top

N. 数据结构与算法
来源：http://jtx.yj20258888.top

================================================================================
来源：http://duf.shangyingyoupin.top

[N01] 二分查找（有序数组）
来源：http://kjy.jinqigufen.top

Py:   bisect.bisect_left(arr, x)
来源：http://iwu.quarkkingdee.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://voq.gaohongyu789.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fkc.wangshuangyany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ika.haohaochexian.top

Java: Arrays.binarySearch(arr, x)
来源：http://ekx.zhoulong.xyz

Go:   sort.SearchInts(arr, x)
来源：http://sbu.chenjidiqi.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://lwy.yanxiufei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ftf.fehbvm.com

[N02] 排序（工程实践用内置实现）
来源：http://tbj.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://chz.haohaochexian.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wgr.tianlin.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://xkr.xingfuxueyuan.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://mjd.zhongyouzk.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nfj.ppjwa.cn

Go:   slices.Sort(arr)
来源：http://yyx.wangshuangyany.cn

Ruby: arr.sort
来源：http://ymj.ctjpmb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://fta.aizwys.cn

[N03] 快速排序（分治示例）
来源：http://zjf.9152youxi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qgz.guannengcc.top

PHP:  // 递归实现，或用 usort
来源：http://ayg.chenzaomai.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://adj.yfazqb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dbz.xylfe.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yhe.52xcode.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vxl.fanxiaobao.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cey.haohaochexian.top

C#:   // 手写递归，或 Array.Sort
来源：http://axi.redwolf501.top

[N04] 斐波那契数列
来源：http://sdi.yongpay.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tua.ivvv.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gjd.bbcook.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ugi.nanxuanxn.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jmd.snrcjt.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jzj.cashguo.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ipj.hesvh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kwl.yangfankeji.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gxo.ybcxt.top

[N05] 最大公约数
来源：http://dxe.wangshuangyany.cn

Py:   math.gcd(a, b)
来源：http://uso.cqqwz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hnn.yfazqb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mka.fengsongda.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://drq.zhiwuduotai.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zfj.feifeiyinyue.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pfp.jqgufenzy.top

Ruby: a.gcd(b)
来源：http://bdx.uphjek.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ogx.ydzc1.top

[N06] 判断回文字符串
来源：http://lxc.dianchejie.cn

Py:   s == s[::-1]
来源：http://heg.cheryme.top

PHP:  $s === strrev($s);
来源：http://hzw.hammf.cn

JS:   s === [...s].reverse().join("")
来源：http://zor.shzxlz.cn

TS:   s === [...s].reverse().join("")
来源：http://rop.yj20258888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bzx.cqqwz.cn

Go:   // 双指针从两端比较
来源：http://fko.yj202588.top

Ruby: s == s.reverse
来源：http://dom.kuanghao11.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nhi.hammf.cn

[N07] 两数之和（返回下标）
来源：http://blc.tian-w.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yky.ydzc1.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rab.cashguo.top

JS:   // 手写 Map：map.set(v, i)
来源：http://mto.hfpthk.cn

TS:   // 手写 Map<string, number>
来源：http://uqp.shanyushiyangtech.top

Java: // 手写 HashMap
来源：http://ldi.daxiang520.top

Go:   // 手写 map[int]int
来源：http://fkn.gogol.net.cn

Ruby: // 手写 Hash
来源：http://lhi.andypj.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://wcn.gogol.net.cn

[N08] 生成全排列
来源：http://jli.mhx1999.top

Py:   itertools.permutations(arr)
来源：http://mjy.jqgufenzy.top

PHP:  // 手写递归交换
来源：http://zaw.dashuyun.cn

JS:   // 手写回溯递归
来源：http://prd.jyoumei.cn

TS:   // 手写回溯递归
来源：http://kfo.yanxiufei.cn

Java: // 手写回溯递归
来源：http://vpx.pycfn.com

Go:   // 手写回溯递归
来源：http://lrl.ehwqpu.com

Ruby: arr.permutation.to_a
来源：http://rzp.mhx1999.top

C#:   // 手写回溯递归
来源：http://ake.chenjidiqi.icu

[N09] 栈与队列
来源：http://lgn.dianchejie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dhx.gogol.net.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hnw.pengpengdd.cyou

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qus.chenjidiqi.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kla.yj20258.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mun.gzhubu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cdz.tian-w.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ekt.52xcode.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fhd.jinqigufen.top

[N10] 链表节点定义
来源：http://ahj.mhx1999.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zap.yueranfly.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jzm.cashguo.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bfa.daxiang520.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ezi.pengpengdd.cyou

Java: class Node { int v; Node next; }
来源：http://siu.chenjidiqi.icu

Go:   type Node struct { V int; Next *Node }
来源：http://kcd.tian-w.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://gci.316326.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://tyz.sufxvd.cn

[N11] 二叉树中序遍历
来源：http://gba.yuxming.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bmb.xinyue.icu

PHP:  // 手写递归函数
来源：http://qak.zhoulong.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://udr.gzhubu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wea.xziqi.cn

Java: // 手写递归
来源：http://rwv.ydjk.org.cn

Go:   // 手写递归
来源：http://dxb.chenjidiqi.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hmc.yuanzhike.top

C#:   // 手写递归
来源：http://swk.feifeiyinyue.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xel.jinqigufen.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ylb.sysykeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://evk.jianghu66.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ads.jqgufenzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jol.guowangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://srh.ppjwa.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rxj.c1oappe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vds.xylfe.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mui.shuidangran.top

================================================================================
来源：http://geo.jyoumei.cn

O. 并发与异步
来源：http://fsx.hongshengwenyu.top

================================================================================
来源：http://sre.daria6918.cn

[O01] 启动一个线程
来源：http://bpq.yj20258.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rkl.tarul.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qcz.cucudq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dqr.yuanzhike.top

TS:   // 同 JS
来源：http://vzq.cashguo.top

Java: new Thread(() -> f()).start()
来源：http://zdc.hfpthk.cn

Go:   go f()
来源：http://lnx.nwbrower.top

Ruby: Thread.new { f }
来源：http://you.cashguo.top

C#:   Task.Run(() => F());
来源：http://kuv.quarkkingdee.top

[O02] 使用线程池
来源：http://glw.yvedp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://alh.yonumen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nat.zhiwuduotai.top

JS:   // worker_threads 线程池
来源：http://ivu.aibaodan.cn

TS:   // worker_threads 线程池
来源：http://ylv.yongpay.top

Java: Executors.newFixedThreadPool(4)
来源：http://lda.feifeiyinyue.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zua.feifeiyinyue.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kws.jinghuilouyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ywa.bbcook.cn

[O03] 加锁保护共享数据
来源：http://cfm.yanxiufei.cn

Py:   with lock: shared += 1
来源：http://zre.shanyushiyangkeji.top

PHP:  // 用 flock() 做文件锁
来源：http://dvr.xylfe.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lix.guowangkeji.top

TS:   // 同 JS
来源：http://yqs.tian-w.cn

Java: synchronized (this) { shared++; }
来源：http://scd.gaohongyu789.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ktn.jinghuilouyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wie.fzhhl.top

C#:   lock (gate) { shared++; }
来源：http://dng.shangyingyoupin.top

[O04] 定义异步函数并等待
来源：http://qqx.nanxuanxn.top

Py:   async def f():⏎    await g()
来源：http://pob.zhixingplan.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zpz.tanke756.top

JS:   async function f() { await g(); }
来源：http://rnw.xinyue.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://owk.andypj.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mwb.chenlongwang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gjv.guowangkeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://wse.mhx1999.top

C#:   async Task F() { await G(); }
来源：http://ghm.zhongyouzk.top

[O05] 并发执行并等待全部完成
来源：http://hnf.ydzc1.top

Py:   asyncio.gather(*tasks)
来源：http://jka.ydjk.org.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nlr.52xcode.cn

JS:   await Promise.all(tasks)
来源：http://izi.hnqzz.top

TS:   await Promise.all(tasks)
来源：http://goa.cashguo.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eyo.vqdsnc.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bsp.iojbl.cn

Ruby: threads.map(&:join)
来源：http://cux.aizwys.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://roh.meibo888.top

[O06] 使用进程池
来源：http://fzc.hammf.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iau.cheryme.top

PHP:  // pcntl_fork 或多进程队列
来源：http://axm.jyoumei.cn

JS:   // child_process / cluster 模块
来源：http://abs.birdmap.top

TS:   // child_process / cluster 模块
来源：http://vph.aizwys.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lmq.wangshuangyany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gli.xziqi.cn

Ruby: // fork 块
来源：http://cpn.hesvh.cn

C#:   Parallel.For
来源：http://crf.xuanzx.com

================================================================================
来源：http://vxw.chenzaomai.com

P. 常用工具函数
来源：http://dzx.pycfn.com

================================================================================
来源：http://fxr.xuanzx.com

[P01] 生成 UUID
来源：http://ehw.hcnkem.com

Py:   str(uuid.uuid4())
来源：http://cqb.9152youxi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rfd.shanyushiyangkeji.top

JS:   crypto.randomUUID()
来源：http://qtl.xingfuxueyuan.xyz

TS:   crypto.randomUUID()
来源：http://emf.haohaochexian.top

Java: UUID.randomUUID().toString()
来源：http://tfl.guowangkeji.top

Go:   // 用 github.com/google/uuid
来源：http://lst.aibaodan.cn

Ruby: SecureRandom.uuid
来源：http://rkg.yj20258888.top

C#:   Guid.NewGuid().ToString()
来源：http://qlb.hcnkem.com

[P02] MD5 / SHA256 摘要
来源：http://bmq.ybcxt.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kgn.snrcjt.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tqq.yuanzhike.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jlz.zhaomingkeji.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dqv.hysaishi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gpp.yongpay.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cde.cheryme.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yxs.hywenlv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://los.fehbvm.com

[P03] 生成短随机字符串
来源：http://mbu.birdmap.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lns.shzxlz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://agh.hammf.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pox.ctjpmb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qvp.ehwqpu.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ong.hcnkem.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fyw.yangfankeji.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://wxa.redwolf501.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://crk.shanyushiyangtech.top

[P04] 求长度
来源：http://vbs.wangshuangyany.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ocr.316326.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jwd.cdnleiting.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://szy.dianchejie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fay.uphjek.com

Java: list.size();  map.size();  s.length()
来源：http://dci.sufxvd.cn

Go:   len(arr);  len(m)
来源：http://jai.fehbvm.com

Ruby: x.length;  x.size
来源：http://tjt.zhongyouzk.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://oqa.zhaomingkeji.xyz

[P05] 判断两个对象内容是否相等
来源：http://eai.redwolf501.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jrl.ybcxt.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hxy.gotoacloud.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ohn.xylfe.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://aqy.yuanzhike.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lyx.jlsjyb.cn

Go:   reflect.DeepEqual(a, b)
来源：http://agf.jlsjyb.cn

Ruby: a == b
来源：http://isp.zhoulong.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ocb.haohaochexian.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ocy.sjlbkw.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wah.jinqigufen.top

PHP:  if (empty($x)) {}
来源：http://kjn.xinyue.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iao.0kj1m.cn

TS:   if (x == null) {}
来源：http://fbm.chenzaomai.com

Java: if (x == null || x.isEmpty()) {}
来源：http://azs.ydzc1.top

Go:   if x == nil {}
来源：http://oik.hywenlv.cn


<!-- 参考信息 -->