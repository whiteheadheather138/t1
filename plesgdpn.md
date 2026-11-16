代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://uwf.mhx1999.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cjm.ydzc1.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://huh.uphjek.com

JS:   resp.ok;  resp.status
来源：http://mkr.yfazqb.com

TS:   resp.ok;  resp.status
来源：http://ceg.aibaodan.cn

Java: resp.statusCode()
来源：http://coe.daxiang520.top

Go:   resp.StatusCode
来源：http://wzy.fehbvm.com

Ruby: resp.code.to_i
来源：http://ant.hcnkem.com

C#:   (int)resp.StatusCode
来源：http://xqo.ydzc1.top

[L08] 并发请求多个地址
来源：http://biq.hnqzz.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://psb.fzhhl.top

PHP:  curl_multi_init() 系列
来源：http://ucu.zhengqikj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wcs.bbcook.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zok.zycfv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hsa.shzxlz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tpl.fengsongda.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wrw.redwolf501.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xxz.shuidangran.top

================================================================================
来源：http://tyg.yanxiufei.cn

M. 命令行 / 进程 / 环境
来源：http://ugx.shzxlz.cn

================================================================================
来源：http://uhh.hcnkem.com

[M01] 读取命令行参数
来源：http://jza.hysaishi.cn

Py:   sys.argv[1:]
来源：http://czc.zhoulong.xyz

PHP:  $argv;  $argc;
来源：http://suf.haohaochexian.top

JS:   process.argv.slice(2)
来源：http://qnr.shanyushiyangtech.top

TS:   process.argv.slice(2)
来源：http://ggu.wangshuangyany.cn

Java: args 数组（main 方法参数）
来源：http://kae.zdqjudy.top

Go:   os.Args[1:]
来源：http://mhz.tian-w.cn

Ruby: ARGV
来源：http://alj.tianlin.xyz

C#:   args 数组（Main 方法参数）
来源：http://fdl.jlsjyb.cn

[M02] 读取环境变量
来源：http://lvs.ctjpmb.com

Py:   os.environ.get("HOME")
来源：http://mcq.shzxlz.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fff.sxryk.cn

JS:   process.env.HOME
来源：http://czj.shanyushiyangtech.top

TS:   process.env.HOME
来源：http://fzs.chenzaomai.com

Java: System.getenv("HOME")
来源：http://baz.ppjwa.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://iap.gotoacloud.top

Ruby: ENV["HOME"]
来源：http://wle.zhongyouzk.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fxy.wangdashe.top

[M03] 执行外部命令
来源：http://fdz.fktsv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ocx.shzxlz.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jlz.zycfv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gcx.ybcxt.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qkv.andypj.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eur.xziqi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qyl.hfpthk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sma.snrcjt.cn

C#:   Process.Start("ls", "-l");
来源：http://awf.hcnkem.com

[M04] 获取当前工作目录
来源：http://dih.sysykeji.top

Py:   os.getcwd()
来源：http://lqd.chenjidiqi.icu

PHP:  getcwd();
来源：http://use.sysykeji.top

JS:   process.cwd()
来源：http://wde.gzhubu.top

TS:   process.cwd()
来源：http://jwi.feifeiyinyue.top

Java: Path.of("").toAbsolutePath()
来源：http://fty.yanxiufei.cn

Go:   os.Getwd()
来源：http://hsa.hfpthk.cn

Ruby: Dir.pwd
来源：http://bgj.yfazqb.com

C#:   Directory.GetCurrentDirectory()
来源：http://klu.zhiwuduotai.top

[M05] 设置退出码
来源：http://coh.snrcjt.cn

Py:   sys.exit(1)
来源：http://kfx.ydzc1.top

PHP:  exit(1);
来源：http://flh.chenjidiqi.icu

JS:   process.exit(1)
来源：http://zjf.sweek.top

TS:   process.exit(1)
来源：http://xve.ctjpmb.com

Java: System.exit(1)
来源：http://hbn.smart0.xyz

Go:   os.Exit(1)
来源：http://gxs.epnwcf.com

Ruby: exit 1
来源：http://rhc.yfazqb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oov.ydzc1.top

[M06] 向标准错误输出
来源：http://tmw.zhijiandao.cn

Py:   print("err", file=sys.stderr)
来源：http://zat.cheryme.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ojg.jqgufenzy.top

JS:   console.error("err")
来源：http://smi.wangdashe.top

TS:   console.error("err")
来源：http://lzn.cashguo.top

Java: System.err.println("err")
来源：http://yah.svipenyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ujp.aizwys.cn

Ruby: warn "err"
来源：http://xne.hnxiangtu.top

C#:   Console.Error.WriteLine("err")
来源：http://zse.birdmap.top

[M07] 判断是否为主入口
来源：http://lqk.yfazqb.com

Py:   if __name__ == "__main__":
来源：http://ocj.0kj1m.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sjh.jinyuanbaomall.cn

JS:   require.main === module
来源：http://xdo.316326.xyz

TS:   require.main === module
来源：http://qlb.yuanzhike.top

Java: public static void main(String[] args)
来源：http://hdp.pengpengdd.cyou

Go:   func main()
来源：http://ufg.yj20258888.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kjp.tanke756.top

C#:   static void Main(string[] args)
来源：http://qkl.zhijiandao.cn

[M08] 获取系统与运行时信息
来源：http://mgl.wangdashe.top

Py:   platform.system();  platform.python_version()
来源：http://sws.iojbl.cn

PHP:  PHP_OS;  phpversion();
来源：http://nxw.yuxming.cn

JS:   process.platform;  process.version
来源：http://eip.jqgfzy.top

TS:   process.platform;  process.version
来源：http://ppn.cheryme.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yru.chenzaomai.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://pgv.ydjk.org.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://waq.haohaochexian.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bob.yfazqb.com

================================================================================
来源：http://wmh.haohaochexian.top

N. 数据结构与算法
来源：http://kuu.cdnleiting.top

================================================================================
来源：http://ptu.yueranfly.top

[N01] 二分查找（有序数组）
来源：http://pql.316326.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://pot.316326.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rrv.jinyuanbaomall.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://poe.dashuyun.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yhq.chenjidiqi.icu

Java: Arrays.binarySearch(arr, x)
来源：http://goo.mhx1999.top

Go:   sort.SearchInts(arr, x)
来源：http://wyl.yanxiufei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dwc.ydjk.org.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nyn.cdnleiting.top

[N02] 排序（工程实践用内置实现）
来源：http://nxt.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://bit.mhx1999.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dfm.jinyuanbaomall.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bry.jinqigufen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mfv.xziqi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zcc.jlsjyb.cn

Go:   slices.Sort(arr)
来源：http://kfc.nanxinkj.top

Ruby: arr.sort
来源：http://dwl.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zcw.yj20258.top

[N03] 快速排序（分治示例）
来源：http://cbl.svipenyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oyr.fktsv.cn

PHP:  // 递归实现，或用 usort
来源：http://dfm.andypj.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pzl.sweek.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pri.hysaishi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bsc.jinyuanbaomall.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dcl.aibaodan.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ogm.ppjwa.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jdi.feifeiyinyue.top

[N04] 斐波那契数列
来源：http://qvk.sjlbkw.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sdy.zhengqikj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qhm.cdnleiting.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fuf.fengsongda.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fqk.chenjidiqi.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vrd.yuxming.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rbv.daria6918.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ewj.gogol.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sff.snrcjt.cn

[N05] 最大公约数
来源：http://big.sysykeji.top

Py:   math.gcd(a, b)
来源：http://vmu.yj20258888.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qih.ehwqpu.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bfi.zhengqikj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aei.dashuyun.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rtd.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wpu.tian-w.cn

Ruby: a.gcd(b)
来源：http://bsd.hysaishi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sno.zhijiandao.cn

[N06] 判断回文字符串
来源：http://eip.xuanzx.com

Py:   s == s[::-1]
来源：http://ucr.chenzaomai.com

PHP:  $s === strrev($s);
来源：http://lxv.yangfankeji.com

JS:   s === [...s].reverse().join("")
来源：http://vlu.shangyingyoupin.top

TS:   s === [...s].reverse().join("")
来源：http://whi.cdnleiting.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vby.xingfuxueyuan.xyz

Go:   // 双指针从两端比较
来源：http://vxw.dianchejie.cn

Ruby: s == s.reverse
来源：http://jad.xuanzx.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://prf.fzhhl.top

[N07] 两数之和（返回下标）
来源：http://ite.gotoacloud.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xxp.dianchejie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xbd.gogol.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bap.nanxuanxn.top

TS:   // 手写 Map<string, number>
来源：http://qmj.0kj1m.cn

Java: // 手写 HashMap
来源：http://eny.daria6918.cn

Go:   // 手写 map[int]int
来源：http://mux.xingfuxueyuan.xyz

Ruby: // 手写 Hash
来源：http://tfk.epnwcf.com

C#:   // 手写 Dictionary<int, int>
来源：http://ypm.chenjidiqi.icu

[N08] 生成全排列
来源：http://hgx.gzhubu.top

Py:   itertools.permutations(arr)
来源：http://jfv.c1oappe.top

PHP:  // 手写递归交换
来源：http://ksz.tian-w.cn

JS:   // 手写回溯递归
来源：http://bib.haohaochexian.top

TS:   // 手写回溯递归
来源：http://nru.yj20258888.top

Java: // 手写回溯递归
来源：http://qim.sxryk.cn

Go:   // 手写回溯递归
来源：http://nrt.fengsongda.top

Ruby: arr.permutation.to_a
来源：http://gvd.dianchejie.cn

C#:   // 手写回溯递归
来源：http://jvt.nanxuanxn.top

[N09] 栈与队列
来源：http://itt.yonumen.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rvk.jinqigufen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://egz.c1oappe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://djl.haohaochexian.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://guf.zhengqikj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pzg.wangshuangyany.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pvk.jlsjyb.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vlm.shanyushiyangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wnl.fktsv.cn

[N10] 链表节点定义
来源：http://sdf.havefunace.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jiv.tarul.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://eom.tian-w.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uln.feifeiyinyue.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nwo.vehdjk.com

Java: class Node { int v; Node next; }
来源：http://mvb.ehwqpu.com

Go:   type Node struct { V int; Next *Node }
来源：http://hbj.sufxvd.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vpm.jinyuanbaomall.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ygn.ywan-chungtsiang.top

[N11] 二叉树中序遍历
来源：http://fow.jlsjyb.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ach.guannengcc.top

PHP:  // 手写递归函数
来源：http://pzh.feifeiyinyue.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://czh.shanyushiyangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vqq.jlsjyb.cn

Java: // 手写递归
来源：http://rvj.fengsongda.top

Go:   // 手写递归
来源：http://him.kuanghao11.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pnu.zhijiandao.cn

C#:   // 手写递归
来源：http://ayo.quarkkingdee.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vjt.yangfankeji.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bms.birdmap.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qnu.c1oappe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://twk.snrcjt.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yic.snrcjt.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nqb.ybcxt.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://toh.yuanzhike.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zan.yj20258.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bmj.pycfn.com

================================================================================
来源：http://vse.yj20258888.top

O. 并发与异步
来源：http://slv.tarul.cn

================================================================================
来源：http://ric.zhongyouzk.top

[O01] 启动一个线程
来源：http://reu.zhengqikj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://otz.iojbl.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wnj.cqqwz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oiq.tanke756.top

TS:   // 同 JS
来源：http://tdd.sweek.top

Java: new Thread(() -> f()).start()
来源：http://ymb.jlsjyb.cn

Go:   go f()
来源：http://ftl.ppjwa.cn

Ruby: Thread.new { f }
来源：http://wtm.guowangkeji.top

C#:   Task.Run(() => F());
来源：http://fus.hammf.cn

[O02] 使用线程池
来源：http://eco.cashguo.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zcn.uphjek.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xbe.jinqigfzy.top

JS:   // worker_threads 线程池
来源：http://xnx.nwbrower.top

TS:   // worker_threads 线程池
来源：http://lfg.tanke756.top

Java: Executors.newFixedThreadPool(4)
来源：http://gwd.zdqjudy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fnr.shzxlz.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xgh.jinyuanbaomall.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uvf.tarul.cn

[O03] 加锁保护共享数据
来源：http://kur.hesvh.cn

Py:   with lock: shared += 1
来源：http://ecw.sxryk.cn

PHP:  // 用 flock() 做文件锁
来源：http://zes.ydjk.org.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fns.yongpay.top

TS:   // 同 JS
来源：http://jnw.yfazqb.com

Java: synchronized (this) { shared++; }
来源：http://vhi.cheryme.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://inp.aizwys.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gui.gogol.net.cn

C#:   lock (gate) { shared++; }
来源：http://wxe.cashguo.top

[O04] 定义异步函数并等待
来源：http://mrf.gogol.net.cn

Py:   async def f():⏎    await g()
来源：http://frs.shangyingyoupin.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jvo.smart0.xyz

JS:   async function f() { await g(); }
来源：http://hrr.yonumen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xdv.haohaochexian.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wyj.hesvh.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nyb.tanke756.top

Ruby: # 用 Fiber 或 async gem
来源：http://lfq.yuanzhike.top

C#:   async Task F() { await G(); }
来源：http://qgr.zycfv.cn

[O05] 并发执行并等待全部完成
来源：http://umz.bbcook.cn

Py:   asyncio.gather(*tasks)
来源：http://arw.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cxb.birdmap.top

JS:   await Promise.all(tasks)
来源：http://rnh.sjlbkw.cn

TS:   await Promise.all(tasks)
来源：http://poj.jinqigfzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cjf.ppjwa.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kze.tarul.cn

Ruby: threads.map(&:join)
来源：http://tpf.tian-w.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://amt.hysaishi.cn

[O06] 使用进程池
来源：http://rdx.gotoacloud.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://itv.chenjidiqi.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://spp.aizwys.cn

JS:   // child_process / cluster 模块
来源：http://acp.zdbjq.cn

TS:   // child_process / cluster 模块
来源：http://fft.ctjpmb.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uzx.jlsjyb.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://njt.havefunace.top

Ruby: // fork 块
来源：http://akn.yanxiufei.cn

C#:   Parallel.For
来源：http://iml.gaohongyu789.top

================================================================================
来源：http://kxp.c1oappe.top

P. 常用工具函数
来源：http://yvg.shuidangran.top

================================================================================
来源：http://nhh.svipenyu.cn

[P01] 生成 UUID
来源：http://mtn.hysaishi.cn

Py:   str(uuid.uuid4())
来源：http://qqb.yuanzhike.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ldl.cdnleiting.top

JS:   crypto.randomUUID()
来源：http://axh.zhixingplan.top

TS:   crypto.randomUUID()
来源：http://hyw.redwolf501.top

Java: UUID.randomUUID().toString()
来源：http://wxy.zdbjq.cn

Go:   // 用 github.com/google/uuid
来源：http://ajb.dashuyun.cn

Ruby: SecureRandom.uuid
来源：http://zee.yvedp.cn

C#:   Guid.NewGuid().ToString()
来源：http://rup.jinyuanbaomall.cn

[P02] MD5 / SHA256 摘要
来源：http://sdr.meibo888.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xrr.vqdsnc.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fja.fehbvm.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://opk.tanke756.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vhp.sufxvd.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ebu.9152youxi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ipk.uphjek.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mtx.ppjwa.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nsb.bjfxy.top

[P03] 生成短随机字符串
来源：http://xss.yangfankeji.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wsl.dashuyun.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hxl.svipenyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fmm.sufxvd.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gdo.sjlbkw.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vdx.hesvh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jsh.yueranfly.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://agq.aibaodan.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zbq.aibaodan.cn

[P04] 求长度
来源：http://sda.0kj1m.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lru.sysykeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://htz.sweek.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xui.hysaishi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://teo.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://fjq.sysykeji.top

Go:   len(arr);  len(m)
来源：http://dmw.yfazqb.com

Ruby: x.length;  x.size
来源：http://tgl.zhiwuduotai.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://eqj.c1oappe.top


<!-- 参考信息 -->