代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://kip.fzhhl.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dad.shangyingyoupin.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bzb.shanyushiyangkeji.top

JS:   resp.ok;  resp.status
来源：http://oky.dashuyun.cn

TS:   resp.ok;  resp.status
来源：http://mrd.jinqigufen.top

Java: resp.statusCode()
来源：http://msf.hnqzz.top

Go:   resp.StatusCode
来源：http://zyj.feifeiyinyue.top

Ruby: resp.code.to_i
来源：http://gfm.nwbrower.top

C#:   (int)resp.StatusCode
来源：http://ybe.sysykeji.top

[L08] 并发请求多个地址
来源：http://osq.quarkkingdee.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kfl.chenjidiqi.icu

PHP:  curl_multi_init() 系列
来源：http://tgr.jianghu66.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://see.vqdsnc.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qcw.xuanzx.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lgi.redwolf501.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fdm.sufxvd.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ttq.316326.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://egb.dashuyun.cn

================================================================================
来源：http://hmr.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://acj.hcnkem.com

================================================================================
来源：http://jec.jiagoushi.top

[M01] 读取命令行参数
来源：http://nwn.cucudq.cn

Py:   sys.argv[1:]
来源：http://msm.feifeiyinyue.top

PHP:  $argv;  $argc;
来源：http://eil.mhx1999.top

JS:   process.argv.slice(2)
来源：http://afs.xuetiantiany.cn

TS:   process.argv.slice(2)
来源：http://sdk.zycfv.cn

Java: args 数组（main 方法参数）
来源：http://oim.quarkkingdee.top

Go:   os.Args[1:]
来源：http://hff.c1oappe.top

Ruby: ARGV
来源：http://ljo.0kj1m.cn

C#:   args 数组（Main 方法参数）
来源：http://uzn.feifeiyinyue.top

[M02] 读取环境变量
来源：http://ocy.gogol.net.cn

Py:   os.environ.get("HOME")
来源：http://cyi.mhx1999.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xbs.jinqigufen.top

JS:   process.env.HOME
来源：http://lzc.gogol.net.cn

TS:   process.env.HOME
来源：http://kwt.svipenyu.cn

Java: System.getenv("HOME")
来源：http://kmw.jinqigfzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://khw.ybcxt.top

Ruby: ENV["HOME"]
来源：http://ehk.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hyr.cucudq.cn

[M03] 执行外部命令
来源：http://box.nanxinkj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eux.guowangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kis.epnwcf.com

JS:   child_process.execSync("ls -l").toString()
来源：http://cse.shanyushiyangtech.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nku.daria6918.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://epi.aizwys.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gzv.snrcjt.cn

Ruby: system("ls -l");  `ls -l`
来源：http://obd.ehwqpu.com

C#:   Process.Start("ls", "-l");
来源：http://hvm.tanke756.top

[M04] 获取当前工作目录
来源：http://ogw.9152youxi.cn

Py:   os.getcwd()
来源：http://wzz.tarul.cn

PHP:  getcwd();
来源：http://coq.ywan-chungtsiang.top

JS:   process.cwd()
来源：http://sao.redwolf501.top

TS:   process.cwd()
来源：http://dir.yj20258888.top

Java: Path.of("").toAbsolutePath()
来源：http://sml.aibaodan.cn

Go:   os.Getwd()
来源：http://dzy.haohaochexian.top

Ruby: Dir.pwd
来源：http://yic.hongshengwenyu.top

C#:   Directory.GetCurrentDirectory()
来源：http://uxl.hysaishi.cn

[M05] 设置退出码
来源：http://aiv.ppjwa.cn

Py:   sys.exit(1)
来源：http://bcu.pengpengdd.cyou

PHP:  exit(1);
来源：http://eqb.sysykeji.top

JS:   process.exit(1)
来源：http://huk.tian-w.cn

TS:   process.exit(1)
来源：http://nnf.jqgufenzy.top

Java: System.exit(1)
来源：http://ixp.fengsongda.top

Go:   os.Exit(1)
来源：http://xtj.xuanzx.com

Ruby: exit 1
来源：http://krj.fanxiaobao.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uov.zhoulong.xyz

[M06] 向标准错误输出
来源：http://kie.fktsv.cn

Py:   print("err", file=sys.stderr)
来源：http://afg.gotoacloud.top

PHP:  fwrite(STDERR, "err\n");
来源：http://cfi.jlsjyb.cn

JS:   console.error("err")
来源：http://ylb.xuanzx.com

TS:   console.error("err")
来源：http://nmm.nwbrower.top

Java: System.err.println("err")
来源：http://xij.jinghuilouyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ctm.ybcxt.top

Ruby: warn "err"
来源：http://cjx.hysaishi.cn

C#:   Console.Error.WriteLine("err")
来源：http://kwa.gotoacloud.top

[M07] 判断是否为主入口
来源：http://idg.dianchejie.cn

Py:   if __name__ == "__main__":
来源：http://cfv.sufxvd.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rnn.sweek.top

JS:   require.main === module
来源：http://bqh.xuanzx.com

TS:   require.main === module
来源：http://srz.hammf.cn

Java: public static void main(String[] args)
来源：http://pfj.shanyushiyangtech.top

Go:   func main()
来源：http://gbj.mhx1999.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lxo.ywan-chungtsiang.top

C#:   static void Main(string[] args)
来源：http://tgz.hnxiangtu.top

[M08] 获取系统与运行时信息
来源：http://guq.0kj1m.cn

Py:   platform.system();  platform.python_version()
来源：http://sqr.zhoulong.xyz

PHP:  PHP_OS;  phpversion();
来源：http://ejs.yfazqb.com

JS:   process.platform;  process.version
来源：http://jkb.zycfv.cn

TS:   process.platform;  process.version
来源：http://dah.xylfe.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uzm.zhaomingkeji.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://vbg.zycfv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kyj.zdbjq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nse.52xcode.cn

================================================================================
来源：http://feb.jinqigfzy.top

N. 数据结构与算法
来源：http://afv.zdqjudy.top

================================================================================
来源：http://clx.ydzc1.top

[N01] 二分查找（有序数组）
来源：http://jxc.yonumen.top

Py:   bisect.bisect_left(arr, x)
来源：http://skk.feifeiyinyue.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://enm.daxiang520.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://onk.zhoulong.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://llj.hfpthk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zgl.pycfn.com

Go:   sort.SearchInts(arr, x)
来源：http://pny.tianlin.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://wzy.aizwys.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pvw.yonumen.top

[N02] 排序（工程实践用内置实现）
来源：http://xzd.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://wqj.haohaochexian.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nmn.guowangkeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lry.tian-w.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cub.shanyushiyangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zlp.tian-w.cn

Go:   slices.Sort(arr)
来源：http://fim.redwolf501.top

Ruby: arr.sort
来源：http://jlc.yuanzhike.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ldx.jlsjyb.cn

[N03] 快速排序（分治示例）
来源：http://hmi.epnwcf.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rto.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://kpo.shanyushiyangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vrd.ctjpmb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://thr.havefunace.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dzy.xuanzx.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://als.cheryme.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iih.hammf.cn

C#:   // 手写递归，或 Array.Sort
来源：http://evh.guowangkeji.top

[N04] 斐波那契数列
来源：http://hrh.uphjek.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vem.xuetiantiany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dks.xylfe.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xls.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ksw.yj20258.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eup.kuanghao11.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lrp.xingfuxueyuan.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bdi.zdbjq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qik.cdnleiting.top

[N05] 最大公约数
来源：http://rxc.fanxiaobao.xyz

Py:   math.gcd(a, b)
来源：http://rmv.yj20258.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fey.epnwcf.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pqg.feifeiyinyue.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://osw.andypj.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mxc.xingfuxueyuan.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vsl.zhixingplan.top

Ruby: a.gcd(b)
来源：http://sny.ydjk.org.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nik.havefunace.top

[N06] 判断回文字符串
来源：http://rxa.dianchejie.cn

Py:   s == s[::-1]
来源：http://gfl.zhaomingkeji.xyz

PHP:  $s === strrev($s);
来源：http://ufl.mhx1999.top

JS:   s === [...s].reverse().join("")
来源：http://jga.chenlongwang.top

TS:   s === [...s].reverse().join("")
来源：http://smb.zhaomingkeji.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kod.feifeiyinyue.top

Go:   // 双指针从两端比较
来源：http://ezr.hcnkem.com

Ruby: s == s.reverse
来源：http://xde.pycfn.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://vxo.ctjpmb.com

[N07] 两数之和（返回下标）
来源：http://bkw.vqdsnc.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tec.sysykeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jtc.hesvh.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sos.aibaodan.cn

TS:   // 手写 Map<string, number>
来源：http://xdx.yonumen.top

Java: // 手写 HashMap
来源：http://mkk.redwolf501.top

Go:   // 手写 map[int]int
来源：http://iys.quarkkingdee.top

Ruby: // 手写 Hash
来源：http://qvu.yueranfly.top

C#:   // 手写 Dictionary<int, int>
来源：http://xni.ydjk.org.cn

[N08] 生成全排列
来源：http://xno.hongshengwenyu.top

Py:   itertools.permutations(arr)
来源：http://ryx.jlsjyb.cn

PHP:  // 手写递归交换
来源：http://aak.yfazqb.com

JS:   // 手写回溯递归
来源：http://zzp.kuanghao11.cn

TS:   // 手写回溯递归
来源：http://xrw.jianghu66.top

Java: // 手写回溯递归
来源：http://jgb.zhoulong.xyz

Go:   // 手写回溯递归
来源：http://oqc.pengpengdd.cyou

Ruby: arr.permutation.to_a
来源：http://sfm.jqgfzy.top

C#:   // 手写回溯递归
来源：http://czw.jinqigufen.top

[N09] 栈与队列
来源：http://gew.bjfxy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mtv.snrcjt.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sfw.chenzaomai.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uwk.xinyue.icu

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ozl.xuanzx.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jud.birdmap.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://upz.dashuyun.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wyi.chenzaomai.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hwd.svipenyu.cn

[N10] 链表节点定义
来源：http://mut.chenzaomai.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://miy.zhijiandao.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mcm.jinqigfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ndt.xuetiantiany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iqx.fengsongda.top

Java: class Node { int v; Node next; }
来源：http://axx.jiagoushi.top

Go:   type Node struct { V int; Next *Node }
来源：http://axf.snrcjt.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tev.zhaomingkeji.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://lpi.gogol.net.cn

[N11] 二叉树中序遍历
来源：http://hji.zdbjq.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gue.jinyuanbaomall.cn

PHP:  // 手写递归函数
来源：http://arx.chenzaomai.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cei.cheryme.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mkd.feifeiyinyue.top

Java: // 手写递归
来源：http://rjr.iojbl.cn

Go:   // 手写递归
来源：http://zai.cashguo.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://aqo.daxiang520.top

C#:   // 手写递归
来源：http://brl.zycfv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mgu.yueranfly.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oux.sweek.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mab.zhoulong.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cgc.jqgfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dbw.gotoacloud.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://eii.wangdashe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fdy.chenzaomai.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wdf.nwbrower.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kic.jinqigufen.top

================================================================================
来源：http://vuq.uphjek.com

O. 并发与异步
来源：http://spw.vehdjk.com

================================================================================
来源：http://pcd.zhijiandao.cn

[O01] 启动一个线程
来源：http://poy.cqqwz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://upj.nanxuanxn.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xar.snrcjt.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ibs.zdqjudy.top

TS:   // 同 JS
来源：http://blc.shuidangran.top

Java: new Thread(() -> f()).start()
来源：http://crx.fzhhl.top

Go:   go f()
来源：http://uzq.0kj1m.cn

Ruby: Thread.new { f }
来源：http://vfu.guowangkeji.top

C#:   Task.Run(() => F());
来源：http://nwl.jqgfzy.top

[O02] 使用线程池
来源：http://jgl.tarul.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xln.pycfn.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://viq.fanxiaobao.xyz

JS:   // worker_threads 线程池
来源：http://zzf.vehdjk.com

TS:   // worker_threads 线程池
来源：http://zgz.yuanzhike.top

Java: Executors.newFixedThreadPool(4)
来源：http://wsb.fanxiaobao.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tlj.mhx1999.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hpo.zhijiandao.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://guk.yfazqb.com

[O03] 加锁保护共享数据
来源：http://vwj.9152youxi.cn

Py:   with lock: shared += 1
来源：http://uxt.jiagoushi.top

PHP:  // 用 flock() 做文件锁
来源：http://fps.nanxuanxn.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://onq.shuidangran.top

TS:   // 同 JS
来源：http://lkb.yj20258.top

Java: synchronized (this) { shared++; }
来源：http://rxi.hfpthk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dxf.feifeiyinyue.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wvp.daria6918.cn

C#:   lock (gate) { shared++; }
来源：http://cmg.guannengcc.top

[O04] 定义异步函数并等待
来源：http://ryi.iojbl.cn

Py:   async def f():⏎    await g()
来源：http://qlw.vqdsnc.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mov.sweek.top

JS:   async function f() { await g(); }
来源：http://pzo.ydzc1.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gzr.52xcode.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oul.gaohongyu789.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uxq.zhongyouzk.top

Ruby: # 用 Fiber 或 async gem
来源：http://gws.zhongyouzk.top

C#:   async Task F() { await G(); }
来源：http://dsg.xziqi.cn

[O05] 并发执行并等待全部完成
来源：http://ytz.sxryk.cn

Py:   asyncio.gather(*tasks)
来源：http://fwv.chenlongwang.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://exr.fengsongda.top

JS:   await Promise.all(tasks)
来源：http://ane.snrcjt.cn

TS:   await Promise.all(tasks)
来源：http://vel.9152youxi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://woe.zhixingplan.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qtx.mhx1999.top

Ruby: threads.map(&:join)
来源：http://snl.shangyingyoupin.top

C#:   await Task.WhenAll(t1, t2)
来源：http://szh.yfazqb.com

[O06] 使用进程池
来源：http://yzn.xuanzx.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qui.hysaishi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mkw.havefunace.top

JS:   // child_process / cluster 模块
来源：http://pzj.jyoumei.cn

TS:   // child_process / cluster 模块
来源：http://jlf.shuidangran.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://prb.cucudq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://elf.yuanzhike.top

Ruby: // fork 块
来源：http://rix.yvedp.cn

C#:   Parallel.For
来源：http://nfp.cqqwz.cn

================================================================================
来源：http://dyx.hywenlv.cn

P. 常用工具函数
来源：http://nhq.gotoacloud.top

================================================================================
来源：http://pyt.fzhhl.top

[P01] 生成 UUID
来源：http://dty.cheryme.top

Py:   str(uuid.uuid4())
来源：http://qnf.yj20258.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jic.shzxlz.cn

JS:   crypto.randomUUID()
来源：http://mnc.xingfuxueyuan.xyz

TS:   crypto.randomUUID()
来源：http://xkj.yonumen.top

Java: UUID.randomUUID().toString()
来源：http://jez.sjlbkw.cn

Go:   // 用 github.com/google/uuid
来源：http://biw.9152youxi.cn

Ruby: SecureRandom.uuid
来源：http://ujt.zycfv.cn

C#:   Guid.NewGuid().ToString()
来源：http://wvo.tarul.cn

[P02] MD5 / SHA256 摘要
来源：http://jhe.gotoacloud.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gqv.ybcxt.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zfx.uphjek.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fca.shanyushiyangtech.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://svg.yonumen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ecl.jinqigufen.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dgt.0kj1m.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zkg.xylfe.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wnz.redwolf501.top

[P03] 生成短随机字符串
来源：http://zni.birdmap.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vxh.wangshuangyany.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rej.jinqigufen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wuz.zhoulong.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yds.9152youxi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nmg.fengsongda.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mae.nwbrower.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ypz.fzhhl.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qxj.nanxuanxn.top

[P04] 求长度
来源：http://olh.hnqzz.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rjg.ybcxt.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jst.vehdjk.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vgr.zhoulong.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rao.shanyushiyangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://spz.mhx1999.top

Go:   len(arr);  len(m)
来源：http://xfh.yvedp.cn

Ruby: x.length;  x.size
来源：http://kst.xuetiantiany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://uuu.yuanzhike.top


<!-- 参考信息 -->