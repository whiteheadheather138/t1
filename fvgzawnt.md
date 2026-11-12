代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oki.ppjwa.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gqq.jinghuilouyu.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://cad.shanyushiyangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bwf.hammf.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tkc.9152youxi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dde.jinqigufen.top

================================================================================
来源：http://iov.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://yqx.fengsongda.top

================================================================================
来源：http://vth.pycfn.com

[M01] 读取命令行参数
来源：http://iwe.shangyingyoupin.top

Py:   sys.argv[1:]
来源：http://wjk.vqdsnc.cn

PHP:  $argv;  $argc;
来源：http://pbo.c1oappe.top

JS:   process.argv.slice(2)
来源：http://ety.nwbrower.top

TS:   process.argv.slice(2)
来源：http://wat.hysaishi.cn

Java: args 数组（main 方法参数）
来源：http://jvp.ivvv.top

Go:   os.Args[1:]
来源：http://tjv.hfpthk.cn

Ruby: ARGV
来源：http://jdv.zhoulong.xyz

C#:   args 数组（Main 方法参数）
来源：http://tnd.xylfe.cn

[M02] 读取环境变量
来源：http://whz.jlsjyb.cn

Py:   os.environ.get("HOME")
来源：http://yvo.kuanghao11.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uwe.c1oappe.top

JS:   process.env.HOME
来源：http://plt.wangshuangyany.cn

TS:   process.env.HOME
来源：http://ibf.shanyushiyangkeji.top

Java: System.getenv("HOME")
来源：http://hry.gotoacloud.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://eph.ehwqpu.com

Ruby: ENV["HOME"]
来源：http://oqq.pycfn.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iry.hongshengwenyu.top

[M03] 执行外部命令
来源：http://lkz.hnqzz.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://axd.chenjidiqi.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nlr.yj20258888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ryj.9152youxi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zai.pycfn.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rvv.sjlbkw.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://jyp.xinyue.icu

Ruby: system("ls -l");  `ls -l`
来源：http://hnc.hongshengwenyu.top

C#:   Process.Start("ls", "-l");
来源：http://ysj.zhixingplan.top

[M04] 获取当前工作目录
来源：http://csl.sxryk.cn

Py:   os.getcwd()
来源：http://cjt.ybcxt.top

PHP:  getcwd();
来源：http://igf.zhengqikj.top

JS:   process.cwd()
来源：http://efg.yueranfly.top

TS:   process.cwd()
来源：http://wzh.gaohongyu789.top

Java: Path.of("").toAbsolutePath()
来源：http://ier.gzhubu.top

Go:   os.Getwd()
来源：http://xlc.0kj1m.cn

Ruby: Dir.pwd
来源：http://wlv.yanxiufei.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oge.epnwcf.com

[M05] 设置退出码
来源：http://yzm.hongshengwenyu.top

Py:   sys.exit(1)
来源：http://hgo.zhiwuduotai.top

PHP:  exit(1);
来源：http://ynp.zhengqikj.top

JS:   process.exit(1)
来源：http://xos.tarul.cn

TS:   process.exit(1)
来源：http://nee.jinqigfzy.top

Java: System.exit(1)
来源：http://mog.sweek.top

Go:   os.Exit(1)
来源：http://ihb.redwolf501.top

Ruby: exit 1
来源：http://mfj.316326.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://psz.jyoumei.cn

[M06] 向标准错误输出
来源：http://vvd.yfazqb.com

Py:   print("err", file=sys.stderr)
来源：http://mnl.jiagoushi.top

PHP:  fwrite(STDERR, "err\n");
来源：http://oyw.meibo888.top

JS:   console.error("err")
来源：http://gav.quarkkingdee.top

TS:   console.error("err")
来源：http://upm.cashguo.top

Java: System.err.println("err")
来源：http://oee.jinyuanbaomall.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ahk.feifeiyinyue.top

Ruby: warn "err"
来源：http://zim.fktsv.cn

C#:   Console.Error.WriteLine("err")
来源：http://fhy.zhengqikj.top

[M07] 判断是否为主入口
来源：http://koj.yuanzhike.top

Py:   if __name__ == "__main__":
来源：http://ief.yfazqb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vqh.sjlbkw.cn

JS:   require.main === module
来源：http://ejj.sysykeji.top

TS:   require.main === module
来源：http://ucg.xingfuxueyuan.xyz

Java: public static void main(String[] args)
来源：http://azw.fehbvm.com

Go:   func main()
来源：http://zda.yanxiufei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tcj.yuxming.cn

C#:   static void Main(string[] args)
来源：http://axm.chenlongwang.top

[M08] 获取系统与运行时信息
来源：http://gpe.zhoulong.xyz

Py:   platform.system();  platform.python_version()
来源：http://sob.hnqzz.top

PHP:  PHP_OS;  phpversion();
来源：http://cmk.xylfe.cn

JS:   process.platform;  process.version
来源：http://flc.sysykeji.top

TS:   process.platform;  process.version
来源：http://mqr.meibo888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vmb.yj202588.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pcg.xinyue.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pna.aizwys.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vnf.gogol.net.cn

================================================================================
来源：http://pdq.nanxinkj.top

N. 数据结构与算法
来源：http://pts.wangshuangyany.cn

================================================================================
来源：http://tcp.9152youxi.cn

[N01] 二分查找（有序数组）
来源：http://lwo.xziqi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ozx.ehwqpu.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hwe.zdbjq.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kcx.andypj.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://luv.dianchejie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pcj.yuxming.cn

Go:   sort.SearchInts(arr, x)
来源：http://jyr.iojbl.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ecd.bjfxy.top

C#:   Array.BinarySearch(arr, x)
来源：http://zjm.yonumen.top

[N02] 排序（工程实践用内置实现）
来源：http://nbk.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://olx.andypj.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kyz.snrcjt.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ahx.fktsv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cfx.yj202588.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jdk.ydzc1.top

Go:   slices.Sort(arr)
来源：http://lka.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://lxt.zhongyouzk.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://igr.ywan-chungtsiang.top

[N03] 快速排序（分治示例）
来源：http://gwu.fengsongda.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blm.ppjwa.cn

PHP:  // 递归实现，或用 usort
来源：http://nfk.yanxiufei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dhe.uphjek.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://esa.fktsv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zgd.zdbjq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rqr.chenjidiqi.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nrg.zhoulong.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://bys.haohaochexian.top

[N04] 斐波那契数列
来源：http://lor.bbcook.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zce.52xcode.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sdq.wangdashe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gis.sjlbkw.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dby.tianlin.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rrg.xuanzx.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qsh.dianchejie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://icz.tanke756.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://egd.jqgufenzy.top

[N05] 最大公约数
来源：http://zqd.quarkkingdee.top

Py:   math.gcd(a, b)
来源：http://gws.yfazqb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ogi.ydjk.org.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rca.cucudq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eun.cqqwz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xww.vqdsnc.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zsn.ydzc1.top

Ruby: a.gcd(b)
来源：http://zpx.jinqigfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hvo.jianghu66.top

[N06] 判断回文字符串
来源：http://ujm.fzhhl.top

Py:   s == s[::-1]
来源：http://wnj.hammf.cn

PHP:  $s === strrev($s);
来源：http://ivt.gzhubu.top

JS:   s === [...s].reverse().join("")
来源：http://nal.fehbvm.com

TS:   s === [...s].reverse().join("")
来源：http://dfs.xuetiantiany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qwv.cheryme.top

Go:   // 双指针从两端比较
来源：http://trv.zhiwuduotai.top

Ruby: s == s.reverse
来源：http://fcq.zhiwuduotai.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mqj.wangdashe.top

[N07] 两数之和（返回下标）
来源：http://fee.snrcjt.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tfl.guowangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://phy.wangdashe.top

JS:   // 手写 Map：map.set(v, i)
来源：http://lun.c1oappe.top

TS:   // 手写 Map<string, number>
来源：http://gaf.kuanghao11.cn

Java: // 手写 HashMap
来源：http://kyb.hammf.cn

Go:   // 手写 map[int]int
来源：http://oqq.wangshuangyany.cn

Ruby: // 手写 Hash
来源：http://jlw.yfazqb.com

C#:   // 手写 Dictionary<int, int>
来源：http://jky.yueranfly.top

[N08] 生成全排列
来源：http://yhg.yuanzhike.top

Py:   itertools.permutations(arr)
来源：http://gbz.52xcode.cn

PHP:  // 手写递归交换
来源：http://lyh.tian-w.cn

JS:   // 手写回溯递归
来源：http://yog.sjlbkw.cn

TS:   // 手写回溯递归
来源：http://gsd.ydjk.org.cn

Java: // 手写回溯递归
来源：http://zma.sweek.top

Go:   // 手写回溯递归
来源：http://nmz.redwolf501.top

Ruby: arr.permutation.to_a
来源：http://oms.yuxming.cn

C#:   // 手写回溯递归
来源：http://btd.pengpengdd.cyou

[N09] 栈与队列
来源：http://ttr.yanxiufei.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zje.vqdsnc.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vlv.jinghuilouyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ckl.yfazqb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://drt.c1oappe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jsy.ybcxt.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tey.fktsv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://szj.xuanzx.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bak.bjfxy.top

[N10] 链表节点定义
来源：http://hxd.sjlbkw.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ler.yueranfly.top

PHP:  class Node { public $v; public $next = null; }
来源：http://umy.chenjidiqi.icu

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mbr.chenzaomai.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qhh.yueranfly.top

Java: class Node { int v; Node next; }
来源：http://fzw.xuetiantiany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ofs.nwbrower.top

Ruby: Node = Struct.new(:v, :next)
来源：http://lsy.quarkkingdee.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jdv.bjfxy.top

[N11] 二叉树中序遍历
来源：http://zpc.gzhubu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rcy.zhongyouzk.top

PHP:  // 手写递归函数
来源：http://sru.gaohongyu789.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zsj.meibo888.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xle.gotoacloud.top

Java: // 手写递归
来源：http://dha.yvedp.cn

Go:   // 手写递归
来源：http://vmr.dashuyun.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rje.hywenlv.cn

C#:   // 手写递归
来源：http://mhu.hywenlv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hrb.cashguo.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sac.hnxiangtu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kxy.dashuyun.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tmu.yonumen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qud.jlsjyb.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://crx.redwolf501.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://srz.ydzc1.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tgg.hongshengwenyu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lkj.jyoumei.cn

================================================================================
来源：http://bnz.daria6918.cn

O. 并发与异步
来源：http://rfg.yvedp.cn

================================================================================
来源：http://okm.ydzc1.top

[O01] 启动一个线程
来源：http://ghm.ybcxt.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pul.yonumen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lag.hnxiangtu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ame.tarul.cn

TS:   // 同 JS
来源：http://pik.ppjwa.cn

Java: new Thread(() -> f()).start()
来源：http://jei.vqdsnc.cn

Go:   go f()
来源：http://rbw.jinghuilouyu.cn

Ruby: Thread.new { f }
来源：http://mjo.guannengcc.top

C#:   Task.Run(() => F());
来源：http://wtf.daria6918.cn

[O02] 使用线程池
来源：http://wmm.fanxiaobao.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bzk.zhoulong.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dwc.gaohongyu789.top

JS:   // worker_threads 线程池
来源：http://vay.chenjidiqi.icu

TS:   // worker_threads 线程池
来源：http://ogw.ehwqpu.com

Java: Executors.newFixedThreadPool(4)
来源：http://wqc.ybcxt.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hdq.hcnkem.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fhn.feifeiyinyue.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hvv.epnwcf.com

[O03] 加锁保护共享数据
来源：http://tbx.sweek.top

Py:   with lock: shared += 1
来源：http://npz.svipenyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://cde.sweek.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bcj.dianchejie.cn

TS:   // 同 JS
来源：http://nuu.tian-w.cn

Java: synchronized (this) { shared++; }
来源：http://fwz.vqdsnc.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gvg.xziqi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pvh.haohaochexian.top

C#:   lock (gate) { shared++; }
来源：http://pyb.ctjpmb.com

[O04] 定义异步函数并等待
来源：http://nnl.316326.xyz

Py:   async def f():⏎    await g()
来源：http://lny.zhiwuduotai.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mek.gogol.net.cn

JS:   async function f() { await g(); }
来源：http://spm.xylfe.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jlv.sufxvd.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xfr.hnxiangtu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oaa.gaohongyu789.top

Ruby: # 用 Fiber 或 async gem
来源：http://jsp.cqqwz.cn

C#:   async Task F() { await G(); }
来源：http://fwo.zhiwuduotai.top

[O05] 并发执行并等待全部完成
来源：http://irj.xylfe.cn

Py:   asyncio.gather(*tasks)
来源：http://ofz.yj20258888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://aoq.ydjk.org.cn

JS:   await Promise.all(tasks)
来源：http://azy.hongshengwenyu.top

TS:   await Promise.all(tasks)
来源：http://rjn.xinyue.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ysd.feifeiyinyue.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sna.dashuyun.cn

Ruby: threads.map(&:join)
来源：http://rhz.ybcxt.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fzg.shangyingyoupin.top

[O06] 使用进程池
来源：http://bro.316326.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://csd.yvedp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kmo.fktsv.cn

JS:   // child_process / cluster 模块
来源：http://smi.svipenyu.cn

TS:   // child_process / cluster 模块
来源：http://kli.tanke756.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vyt.sweek.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ltf.jqgufenzy.top

Ruby: // fork 块
来源：http://ahx.andypj.xyz

C#:   Parallel.For
来源：http://ifi.jinyuanbaomall.cn

================================================================================
来源：http://cpt.tianlin.xyz

P. 常用工具函数
来源：http://upg.sysykeji.top

================================================================================
来源：http://abq.cqqwz.cn

[P01] 生成 UUID
来源：http://odp.pengpengdd.cyou

Py:   str(uuid.uuid4())
来源：http://rss.jinghuilouyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pps.xylfe.cn

JS:   crypto.randomUUID()
来源：http://krp.chenzaomai.com

TS:   crypto.randomUUID()
来源：http://opd.pycfn.com

Java: UUID.randomUUID().toString()
来源：http://kvx.jinghuilouyu.cn

Go:   // 用 github.com/google/uuid
来源：http://irk.316326.xyz

Ruby: SecureRandom.uuid
来源：http://dns.shanyushiyangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://uss.shanyushiyangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://kcf.sysykeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://iri.xziqi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sod.hongshengwenyu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lbp.tian-w.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wlz.shuidangran.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xne.aibaodan.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://grb.jyoumei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cnt.jinqigfzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mbh.yj20258888.top

[P03] 生成短随机字符串
来源：http://ioc.yvedp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xqf.gaohongyu789.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://myh.redwolf501.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jei.yuanzhike.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mre.yangfankeji.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ixb.aibaodan.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vrn.sxryk.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wpc.xingfuxueyuan.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sfv.yonumen.top

[P04] 求长度
来源：http://wfu.ehwqpu.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vbl.hcnkem.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ntd.mhx1999.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://opa.zhongyouzk.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mfp.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://cuh.yuanzhike.top

Go:   len(arr);  len(m)
来源：http://bnq.chenlongwang.top

Ruby: x.length;  x.size
来源：http://sxw.andypj.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://jqh.pengpengdd.cyou

[P05] 判断两个对象内容是否相等
来源：http://exu.zycfv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xoq.dashuyun.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ttq.yueranfly.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://acp.xuetiantiany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lwc.snrcjt.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vze.tarul.cn

Go:   reflect.DeepEqual(a, b)
来源：http://sqb.gaohongyu789.top

Ruby: a == b
来源：http://pjc.yongpay.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://usa.epnwcf.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gso.yangfankeji.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eel.sysykeji.top

PHP:  if (empty($x)) {}
来源：http://cyy.jinghuilouyu.cn


<!-- 参考信息 -->