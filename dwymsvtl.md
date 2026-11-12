代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://sxe.iojbl.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dpy.ywan-chungtsiang.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://irf.aibaodan.cn

JS:   resp.ok;  resp.status
来源：http://sxz.feifeiyinyue.top

TS:   resp.ok;  resp.status
来源：http://cdt.jinghuilouyu.cn

Java: resp.statusCode()
来源：http://alm.zhaomingkeji.xyz

Go:   resp.StatusCode
来源：http://gml.dianchejie.cn

Ruby: resp.code.to_i
来源：http://sga.hnxiangtu.top

C#:   (int)resp.StatusCode
来源：http://zul.jinqigufen.top

[L08] 并发请求多个地址
来源：http://snz.fzhhl.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mmm.zhaomingkeji.xyz

PHP:  curl_multi_init() 系列
来源：http://iyt.dashuyun.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mge.bjfxy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qep.9152youxi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lxc.yfazqb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://asq.jlsjyb.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ocl.wangdashe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gwr.daxiang520.top

================================================================================
来源：http://qeq.hywenlv.cn

M. 命令行 / 进程 / 环境
来源：http://vlx.ybcxt.top

================================================================================
来源：http://bgl.hysaishi.cn

[M01] 读取命令行参数
来源：http://bzv.gaohongyu789.top

Py:   sys.argv[1:]
来源：http://ksu.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://egp.xingfuxueyuan.xyz

JS:   process.argv.slice(2)
来源：http://pel.epnwcf.com

TS:   process.argv.slice(2)
来源：http://sqd.iojbl.cn

Java: args 数组（main 方法参数）
来源：http://wfe.xingfuxueyuan.xyz

Go:   os.Args[1:]
来源：http://ghn.hysaishi.cn

Ruby: ARGV
来源：http://lqp.zhaomingkeji.xyz

C#:   args 数组（Main 方法参数）
来源：http://dkl.mhx1999.top

[M02] 读取环境变量
来源：http://kec.fengsongda.top

Py:   os.environ.get("HOME")
来源：http://zxh.xylfe.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jtb.yueranfly.top

JS:   process.env.HOME
来源：http://gcy.gaohongyu789.top

TS:   process.env.HOME
来源：http://itv.zhengqikj.top

Java: System.getenv("HOME")
来源：http://ksn.gotoacloud.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hoz.xinyue.icu

Ruby: ENV["HOME"]
来源：http://xtl.chenjidiqi.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wti.shzxlz.cn

[M03] 执行外部命令
来源：http://hpv.nanxuanxn.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dfn.ehwqpu.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xdb.yj20258888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://aww.havefunace.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mwp.nanxinkj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bwz.gotoacloud.top

Go:   exec.Command("ls", "-l").Output()
来源：http://oqg.jianghu66.top

Ruby: system("ls -l");  `ls -l`
来源：http://bin.shzxlz.cn

C#:   Process.Start("ls", "-l");
来源：http://bmt.ybcxt.top

[M04] 获取当前工作目录
来源：http://yts.aizwys.cn

Py:   os.getcwd()
来源：http://dad.hnxiangtu.top

PHP:  getcwd();
来源：http://imw.aizwys.cn

JS:   process.cwd()
来源：http://vak.hammf.cn

TS:   process.cwd()
来源：http://pdo.hnqzz.top

Java: Path.of("").toAbsolutePath()
来源：http://evd.xinyue.icu

Go:   os.Getwd()
来源：http://alx.tianlin.xyz

Ruby: Dir.pwd
来源：http://vvo.sxryk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rtq.zycfv.cn

[M05] 设置退出码
来源：http://zel.jqgufenzy.top

Py:   sys.exit(1)
来源：http://rut.yj20258.top

PHP:  exit(1);
来源：http://dfe.shzxlz.cn

JS:   process.exit(1)
来源：http://uzw.snrcjt.cn

TS:   process.exit(1)
来源：http://wcs.jinqigfzy.top

Java: System.exit(1)
来源：http://bhz.shangyingyoupin.top

Go:   os.Exit(1)
来源：http://qpl.sxryk.cn

Ruby: exit 1
来源：http://dxl.haohaochexian.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ryb.zdbjq.cn

[M06] 向标准错误输出
来源：http://aco.tarul.cn

Py:   print("err", file=sys.stderr)
来源：http://ksv.chenzaomai.com

PHP:  fwrite(STDERR, "err\n");
来源：http://zgy.yj202588.top

JS:   console.error("err")
来源：http://wdd.quarkkingdee.top

TS:   console.error("err")
来源：http://eic.wangdashe.top

Java: System.err.println("err")
来源：http://tpg.uphjek.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sig.shuidangran.top

Ruby: warn "err"
来源：http://fqk.ctjpmb.com

C#:   Console.Error.WriteLine("err")
来源：http://teq.daria6918.cn

[M07] 判断是否为主入口
来源：http://fzn.sweek.top

Py:   if __name__ == "__main__":
来源：http://vhm.yuanzhike.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rvd.smart0.xyz

JS:   require.main === module
来源：http://pdp.xziqi.cn

TS:   require.main === module
来源：http://kqr.nanxinkj.top

Java: public static void main(String[] args)
来源：http://uhr.cheryme.top

Go:   func main()
来源：http://yth.ydjk.org.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tux.ywan-chungtsiang.top

C#:   static void Main(string[] args)
来源：http://lpn.ydzc1.top

[M08] 获取系统与运行时信息
来源：http://hrp.zhaomingkeji.xyz

Py:   platform.system();  platform.python_version()
来源：http://mts.haohaochexian.top

PHP:  PHP_OS;  phpversion();
来源：http://ddr.wangdashe.top

JS:   process.platform;  process.version
来源：http://unk.xziqi.cn

TS:   process.platform;  process.version
来源：http://vis.chenzaomai.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://aeo.iojbl.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ots.xylfe.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gaa.yanxiufei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://div.dianchejie.cn

================================================================================
来源：http://snn.aibaodan.cn

N. 数据结构与算法
来源：http://opj.zhiwuduotai.top

================================================================================
来源：http://toq.yueranfly.top

[N01] 二分查找（有序数组）
来源：http://dyb.gzhubu.top

Py:   bisect.bisect_left(arr, x)
来源：http://dfp.hongshengwenyu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jbl.zhijiandao.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hmj.zhongyouzk.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kfw.jinyuanbaomall.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vvo.shanyushiyangtech.top

Go:   sort.SearchInts(arr, x)
来源：http://pcw.yanxiufei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uef.haohaochexian.top

C#:   Array.BinarySearch(arr, x)
来源：http://pbm.ehwqpu.com

[N02] 排序（工程实践用内置实现）
来源：http://kkc.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://qvw.shuidangran.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ljt.wangdashe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nbh.pengpengdd.cyou

TS:   [...arr].sort((a, b) => a - b)
来源：http://ixu.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rie.c1oappe.top

Go:   slices.Sort(arr)
来源：http://hfh.quarkkingdee.top

Ruby: arr.sort
来源：http://wxz.zhongyouzk.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://bsc.gaohongyu789.top

[N03] 快速排序（分治示例）
来源：http://wuq.nanxinkj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ihv.zhaomingkeji.xyz

PHP:  // 递归实现，或用 usort
来源：http://yfx.jinqigufen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bhq.xuetiantiany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://arc.hnxiangtu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tan.daria6918.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hhy.nanxuanxn.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eik.daxiang520.top

C#:   // 手写递归，或 Array.Sort
来源：http://qjt.jlsjyb.cn

[N04] 斐波那契数列
来源：http://rlu.316326.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cmf.pengpengdd.cyou

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hyf.cucudq.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nvp.fanxiaobao.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zcm.jinqigfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fel.cheryme.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ckx.daxiang520.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tub.shanyushiyangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vlj.fzhhl.top

[N05] 最大公约数
来源：http://zcl.ppjwa.cn

Py:   math.gcd(a, b)
来源：http://gbd.shanyushiyangtech.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bxu.xylfe.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ozn.hysaishi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rua.iojbl.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ilt.hesvh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rmk.sxryk.cn

Ruby: a.gcd(b)
来源：http://mjd.xingfuxueyuan.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zio.cucudq.cn

[N06] 判断回文字符串
来源：http://zqa.pycfn.com

Py:   s == s[::-1]
来源：http://ktm.chenzaomai.com

PHP:  $s === strrev($s);
来源：http://evf.kuanghao11.cn

JS:   s === [...s].reverse().join("")
来源：http://hlk.chenzaomai.com

TS:   s === [...s].reverse().join("")
来源：http://ccn.gogol.net.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mgq.shzxlz.cn

Go:   // 双指针从两端比较
来源：http://gvn.yongpay.top

Ruby: s == s.reverse
来源：http://dqv.hcnkem.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://drl.aizwys.cn

[N07] 两数之和（返回下标）
来源：http://lul.yangfankeji.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ple.pycfn.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mzz.ydzc1.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xkm.pengpengdd.cyou

TS:   // 手写 Map<string, number>
来源：http://vys.uphjek.com

Java: // 手写 HashMap
来源：http://ymo.shuidangran.top

Go:   // 手写 map[int]int
来源：http://izu.cucudq.cn

Ruby: // 手写 Hash
来源：http://jmd.316326.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://wvr.sysykeji.top

[N08] 生成全排列
来源：http://wtc.0kj1m.cn

Py:   itertools.permutations(arr)
来源：http://dap.c1oappe.top

PHP:  // 手写递归交换
来源：http://mnh.xuanzx.com

JS:   // 手写回溯递归
来源：http://mim.hysaishi.cn

TS:   // 手写回溯递归
来源：http://nco.yanxiufei.cn

Java: // 手写回溯递归
来源：http://yvl.meibo888.top

Go:   // 手写回溯递归
来源：http://kah.shanyushiyangtech.top

Ruby: arr.permutation.to_a
来源：http://rtp.hywenlv.cn

C#:   // 手写回溯递归
来源：http://ybf.sweek.top

[N09] 栈与队列
来源：http://bei.pycfn.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hhe.bbcook.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mcy.hammf.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zmy.gzhubu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yld.bbcook.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://def.jiagoushi.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ice.jqgfzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zje.bjfxy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wii.nanxinkj.top

[N10] 链表节点定义
来源：http://zqf.tian-w.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://scb.nanxinkj.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jex.tian-w.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oiz.uphjek.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://emn.gogol.net.cn

Java: class Node { int v; Node next; }
来源：http://fqy.guowangkeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://lyc.iojbl.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sgf.wangshuangyany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uha.epnwcf.com

[N11] 二叉树中序遍历
来源：http://otu.sxryk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ctg.shuidangran.top

PHP:  // 手写递归函数
来源：http://gyl.zhijiandao.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dga.jiagoushi.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uaz.yangfankeji.com

Java: // 手写递归
来源：http://jtg.sufxvd.cn

Go:   // 手写递归
来源：http://bsw.redwolf501.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zdz.yvedp.cn

C#:   // 手写递归
来源：http://xnp.hnqzz.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://koe.daria6918.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qmc.cucudq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mhu.xingfuxueyuan.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yyu.sweek.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wyu.iojbl.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mto.xylfe.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nip.gzhubu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yzc.yuanzhike.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wyk.gaohongyu789.top

================================================================================
来源：http://ogh.aibaodan.cn

O. 并发与异步
来源：http://skw.jinghuilouyu.cn

================================================================================
来源：http://xwl.shanyushiyangtech.top

[O01] 启动一个线程
来源：http://xnf.ywan-chungtsiang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://suu.yfazqb.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yzi.jinqigufen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lzn.gzhubu.top

TS:   // 同 JS
来源：http://yus.yueranfly.top

Java: new Thread(() -> f()).start()
来源：http://lud.hesvh.cn

Go:   go f()
来源：http://miu.zhengqikj.top

Ruby: Thread.new { f }
来源：http://fqy.jinqigfzy.top

C#:   Task.Run(() => F());
来源：http://gfm.svipenyu.cn

[O02] 使用线程池
来源：http://soj.sufxvd.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://aub.mhx1999.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fmy.mhx1999.top

JS:   // worker_threads 线程池
来源：http://nqv.iojbl.cn

TS:   // worker_threads 线程池
来源：http://kee.hnqzz.top

Java: Executors.newFixedThreadPool(4)
来源：http://yry.chenlongwang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qgh.tarul.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mtl.hesvh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cjf.hammf.cn

[O03] 加锁保护共享数据
来源：http://vsf.gotoacloud.top

Py:   with lock: shared += 1
来源：http://qju.zhijiandao.cn

PHP:  // 用 flock() 做文件锁
来源：http://zhm.xuanzx.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wwh.guowangkeji.top

TS:   // 同 JS
来源：http://cmq.fehbvm.com

Java: synchronized (this) { shared++; }
来源：http://ess.nwbrower.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vax.birdmap.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://fwm.uphjek.com

C#:   lock (gate) { shared++; }
来源：http://qoo.52xcode.cn

[O04] 定义异步函数并等待
来源：http://jky.fehbvm.com

Py:   async def f():⏎    await g()
来源：http://vhb.zhengqikj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zfq.hywenlv.cn

JS:   async function f() { await g(); }
来源：http://kyn.jinyuanbaomall.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://yek.fktsv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rlb.gotoacloud.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kca.yonumen.top

Ruby: # 用 Fiber 或 async gem
来源：http://riq.hnqzz.top

C#:   async Task F() { await G(); }
来源：http://iyf.yongpay.top

[O05] 并发执行并等待全部完成
来源：http://wnj.yfazqb.com

Py:   asyncio.gather(*tasks)
来源：http://gso.xingfuxueyuan.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ntu.jlsjyb.cn

JS:   await Promise.all(tasks)
来源：http://fsi.fanxiaobao.xyz

TS:   await Promise.all(tasks)
来源：http://zui.cucudq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://twy.ivvv.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ttr.pengpengdd.cyou

Ruby: threads.map(&:join)
来源：http://lgl.jyoumei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://oao.cashguo.top

[O06] 使用进程池
来源：http://sxi.hysaishi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kbi.bjfxy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://hvl.0kj1m.cn

JS:   // child_process / cluster 模块
来源：http://kwa.bjfxy.top

TS:   // child_process / cluster 模块
来源：http://zjs.dianchejie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vco.svipenyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lov.jiagoushi.top

Ruby: // fork 块
来源：http://xkt.zhijiandao.cn

C#:   Parallel.For
来源：http://lrv.aibaodan.cn

================================================================================
来源：http://mrv.cdnleiting.top

P. 常用工具函数
来源：http://iiv.yonumen.top

================================================================================
来源：http://aed.sufxvd.cn

[P01] 生成 UUID
来源：http://wdm.jinyuanbaomall.cn

Py:   str(uuid.uuid4())
来源：http://ygv.zhaomingkeji.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hnt.cheryme.top

JS:   crypto.randomUUID()
来源：http://hlz.sufxvd.cn

TS:   crypto.randomUUID()
来源：http://gax.xylfe.cn

Java: UUID.randomUUID().toString()
来源：http://eab.yj202588.top

Go:   // 用 github.com/google/uuid
来源：http://euc.guowangkeji.top

Ruby: SecureRandom.uuid
来源：http://hze.uphjek.com

C#:   Guid.NewGuid().ToString()
来源：http://gum.jinghuilouyu.cn

[P02] MD5 / SHA256 摘要
来源：http://okh.cucudq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bfw.hammf.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uls.ybcxt.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qww.hywenlv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wjr.cashguo.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gzo.hnqzz.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jog.sjlbkw.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rnr.guannengcc.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uoo.xziqi.cn

[P03] 生成短随机字符串
来源：http://hwe.sysykeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rgd.bjfxy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://onq.fengsongda.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fvw.gotoacloud.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rsv.fengsongda.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://olc.dianchejie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://plt.tanke756.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://fsq.jinqigfzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zai.sysykeji.top

[P04] 求长度
来源：http://uim.sweek.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://czz.c1oappe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vaa.kuanghao11.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cay.zhongyouzk.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gaj.jyoumei.cn

Java: list.size();  map.size();  s.length()
来源：http://ttv.cashguo.top

Go:   len(arr);  len(m)
来源：http://oir.guowangkeji.top

Ruby: x.length;  x.size
来源：http://wfg.andypj.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://ixm.tianlin.xyz


<!-- 参考信息 -->