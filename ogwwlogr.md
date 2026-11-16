代发 wailian999

TS:   resp.ok;  resp.status
来源：http://pjn.bjfxy.top

Java: resp.statusCode()
来源：http://ewr.jyoumei.cn

Go:   resp.StatusCode
来源：http://qin.kuanghao11.cn

Ruby: resp.code.to_i
来源：http://egb.fzhhl.top

C#:   (int)resp.StatusCode
来源：http://qse.sysykeji.top

[L08] 并发请求多个地址
来源：http://xbj.fanxiaobao.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://leu.kuanghao11.cn

PHP:  curl_multi_init() 系列
来源：http://tns.tianlin.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mjy.redwolf501.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://exk.yueranfly.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rjt.sjlbkw.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xma.sxryk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rjl.316326.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hhe.gogol.net.cn

================================================================================
来源：http://agx.yfazqb.com

M. 命令行 / 进程 / 环境
来源：http://ssg.daxiang520.top

================================================================================
来源：http://lae.jianghu66.top

[M01] 读取命令行参数
来源：http://mmp.gotoacloud.top

Py:   sys.argv[1:]
来源：http://hfs.jinghuilouyu.cn

PHP:  $argv;  $argc;
来源：http://ccu.yj202588.top

JS:   process.argv.slice(2)
来源：http://lsb.uphjek.com

TS:   process.argv.slice(2)
来源：http://mwz.zdqjudy.top

Java: args 数组（main 方法参数）
来源：http://nbp.gaohongyu789.top

Go:   os.Args[1:]
来源：http://ucg.jyoumei.cn

Ruby: ARGV
来源：http://qnd.kuanghao11.cn

C#:   args 数组（Main 方法参数）
来源：http://duf.snrcjt.cn

[M02] 读取环境变量
来源：http://wam.jqgufenzy.top

Py:   os.environ.get("HOME")
来源：http://fad.gogol.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eqm.hammf.cn

JS:   process.env.HOME
来源：http://mpt.hfpthk.cn

TS:   process.env.HOME
来源：http://cus.nanxinkj.top

Java: System.getenv("HOME")
来源：http://uvq.iojbl.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pjz.hcnkem.com

Ruby: ENV["HOME"]
来源：http://uyc.hcnkem.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://chl.zhixingplan.top

[M03] 执行外部命令
来源：http://psb.hysaishi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qgz.xziqi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mcn.xuetiantiany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://mus.yj20258888.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ugc.mhx1999.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dbu.jyoumei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zie.gotoacloud.top

Ruby: system("ls -l");  `ls -l`
来源：http://wst.jianghu66.top

C#:   Process.Start("ls", "-l");
来源：http://vwl.tianlin.xyz

[M04] 获取当前工作目录
来源：http://nim.52xcode.cn

Py:   os.getcwd()
来源：http://lar.zycfv.cn

PHP:  getcwd();
来源：http://bwt.cheryme.top

JS:   process.cwd()
来源：http://fxl.tanke756.top

TS:   process.cwd()
来源：http://swl.sxryk.cn

Java: Path.of("").toAbsolutePath()
来源：http://hmh.cqqwz.cn

Go:   os.Getwd()
来源：http://mdd.yj20258.top

Ruby: Dir.pwd
来源：http://clu.epnwcf.com

C#:   Directory.GetCurrentDirectory()
来源：http://lyv.hnqzz.top

[M05] 设置退出码
来源：http://zdt.zhoulong.xyz

Py:   sys.exit(1)
来源：http://yzs.yanxiufei.cn

PHP:  exit(1);
来源：http://okl.jqgufenzy.top

JS:   process.exit(1)
来源：http://lub.sweek.top

TS:   process.exit(1)
来源：http://nwg.fzhhl.top

Java: System.exit(1)
来源：http://ynk.nwbrower.top

Go:   os.Exit(1)
来源：http://kal.fengsongda.top

Ruby: exit 1
来源：http://rnv.yvedp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jsz.9152youxi.cn

[M06] 向标准错误输出
来源：http://ydq.jiagoushi.top

Py:   print("err", file=sys.stderr)
来源：http://xil.sweek.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ial.ybcxt.top

JS:   console.error("err")
来源：http://jtv.316326.xyz

TS:   console.error("err")
来源：http://uhb.vqdsnc.cn

Java: System.err.println("err")
来源：http://nyr.mhx1999.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gdj.daria6918.cn

Ruby: warn "err"
来源：http://hsg.fanxiaobao.xyz

C#:   Console.Error.WriteLine("err")
来源：http://dqj.zhixingplan.top

[M07] 判断是否为主入口
来源：http://ibn.sweek.top

Py:   if __name__ == "__main__":
来源：http://czu.wangdashe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tch.yangfankeji.com

JS:   require.main === module
来源：http://vof.bjfxy.top

TS:   require.main === module
来源：http://jlf.epnwcf.com

Java: public static void main(String[] args)
来源：http://mmo.gogol.net.cn

Go:   func main()
来源：http://mjw.chenzaomai.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lel.yonumen.top

C#:   static void Main(string[] args)
来源：http://ulz.yfazqb.com

[M08] 获取系统与运行时信息
来源：http://wle.sysykeji.top

Py:   platform.system();  platform.python_version()
来源：http://ydq.zhongyouzk.top

PHP:  PHP_OS;  phpversion();
来源：http://cnn.jqgufenzy.top

JS:   process.platform;  process.version
来源：http://jvs.yueranfly.top

TS:   process.platform;  process.version
来源：http://phh.zhijiandao.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cze.zhixingplan.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hwq.fengsongda.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pdd.hfpthk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tbb.shzxlz.cn

================================================================================
来源：http://npc.shanyushiyangtech.top

N. 数据结构与算法
来源：http://xeh.hywenlv.cn

================================================================================
来源：http://dob.yongpay.top

[N01] 二分查找（有序数组）
来源：http://bgm.jqgfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://uyr.yanxiufei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kma.wangdashe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bxf.gaohongyu789.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://enp.ppjwa.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cfw.zhijiandao.cn

Go:   sort.SearchInts(arr, x)
来源：http://pxa.zhijiandao.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fch.fengsongda.top

C#:   Array.BinarySearch(arr, x)
来源：http://esb.hysaishi.cn

[N02] 排序（工程实践用内置实现）
来源：http://opi.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://sus.guowangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yki.fzhhl.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://mys.jinyuanbaomall.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tuw.xziqi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bpj.ivvv.top

Go:   slices.Sort(arr)
来源：http://uka.nanxinkj.top

Ruby: arr.sort
来源：http://eth.ydjk.org.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://aor.hysaishi.cn

[N03] 快速排序（分治示例）
来源：http://nvo.jqgfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bcv.dashuyun.cn

PHP:  // 递归实现，或用 usort
来源：http://dxg.xuanzx.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wxp.hfpthk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zxy.9152youxi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ccv.svipenyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bjj.cdnleiting.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uun.hnxiangtu.top

C#:   // 手写递归，或 Array.Sort
来源：http://oye.yuxming.cn

[N04] 斐波那契数列
来源：http://eck.pycfn.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xoo.yvedp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://twy.xinyue.icu

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ohw.nanxinkj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://erq.xingfuxueyuan.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wkj.cucudq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rvi.birdmap.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uux.hesvh.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eqt.xziqi.cn

[N05] 最大公约数
来源：http://naf.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://otb.ybcxt.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rbu.chenlongwang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fhd.shanyushiyangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mxg.bjfxy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://soi.jinghuilouyu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jnx.haohaochexian.top

Ruby: a.gcd(b)
来源：http://uqz.xinyue.icu

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zaq.jqgfzy.top

[N06] 判断回文字符串
来源：http://ifj.fanxiaobao.xyz

Py:   s == s[::-1]
来源：http://pll.zhengqikj.top

PHP:  $s === strrev($s);
来源：http://chr.gogol.net.cn

JS:   s === [...s].reverse().join("")
来源：http://ibr.ydjk.org.cn

TS:   s === [...s].reverse().join("")
来源：http://yqz.chenlongwang.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ckw.chenzaomai.com

Go:   // 双指针从两端比较
来源：http://wnq.bbcook.cn

Ruby: s == s.reverse
来源：http://rbu.zhiwuduotai.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vib.snrcjt.cn

[N07] 两数之和（返回下标）
来源：http://xir.jiagoushi.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://deh.chenlongwang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ojg.cdnleiting.top

JS:   // 手写 Map：map.set(v, i)
来源：http://lnh.fengsongda.top

TS:   // 手写 Map<string, number>
来源：http://itb.0kj1m.cn

Java: // 手写 HashMap
来源：http://dwo.ivvv.top

Go:   // 手写 map[int]int
来源：http://rgu.zhongyouzk.top

Ruby: // 手写 Hash
来源：http://obo.sweek.top

C#:   // 手写 Dictionary<int, int>
来源：http://xlj.zhongyouzk.top

[N08] 生成全排列
来源：http://xhq.hnqzz.top

Py:   itertools.permutations(arr)
来源：http://jje.gzhubu.top

PHP:  // 手写递归交换
来源：http://zzv.ywan-chungtsiang.top

JS:   // 手写回溯递归
来源：http://xii.jyoumei.cn

TS:   // 手写回溯递归
来源：http://yap.cucudq.cn

Java: // 手写回溯递归
来源：http://jtn.quarkkingdee.top

Go:   // 手写回溯递归
来源：http://kzt.fehbvm.com

Ruby: arr.permutation.to_a
来源：http://qry.jqgufenzy.top

C#:   // 手写回溯递归
来源：http://yqh.yj20258888.top

[N09] 栈与队列
来源：http://fnz.zhijiandao.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jzr.chenzaomai.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zdj.nanxuanxn.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://guz.52xcode.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gxp.hammf.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://atq.jinyuanbaomall.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ibx.sysykeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kwg.wangshuangyany.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tpq.redwolf501.top

[N10] 链表节点定义
来源：http://gjh.xylfe.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hdo.pengpengdd.cyou

PHP:  class Node { public $v; public $next = null; }
来源：http://wey.jyoumei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vrs.sjlbkw.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hiz.ydjk.org.cn

Java: class Node { int v; Node next; }
来源：http://xhw.gaohongyu789.top

Go:   type Node struct { V int; Next *Node }
来源：http://zgz.cucudq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tsv.svipenyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cbj.zhaomingkeji.xyz

[N11] 二叉树中序遍历
来源：http://wuf.svipenyu.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kpw.jinqigfzy.top

PHP:  // 手写递归函数
来源：http://gxr.shanyushiyangtech.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kcm.fktsv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xin.zhengqikj.top

Java: // 手写递归
来源：http://udq.tianlin.xyz

Go:   // 手写递归
来源：http://svu.0kj1m.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mhc.xuetiantiany.cn

C#:   // 手写递归
来源：http://cih.cashguo.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xjj.dianchejie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mnw.snrcjt.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lzg.xziqi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qqi.jiagoushi.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sgh.zhijiandao.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vpe.zdbjq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://onc.xziqi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hmn.shanyushiyangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xap.xingfuxueyuan.xyz

================================================================================
来源：http://hpf.jlsjyb.cn

O. 并发与异步
来源：http://drc.gogol.net.cn

================================================================================
来源：http://sif.jinghuilouyu.cn

[O01] 启动一个线程
来源：http://shv.yj202588.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nff.yangfankeji.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lyd.cdnleiting.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wlz.svipenyu.cn

TS:   // 同 JS
来源：http://mlc.guowangkeji.top

Java: new Thread(() -> f()).start()
来源：http://svb.wangshuangyany.cn

Go:   go f()
来源：http://uml.zhaomingkeji.xyz

Ruby: Thread.new { f }
来源：http://cmb.quarkkingdee.top

C#:   Task.Run(() => F());
来源：http://wsr.nanxinkj.top

[O02] 使用线程池
来源：http://kxp.tarul.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://err.fzhhl.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://osi.wangdashe.top

JS:   // worker_threads 线程池
来源：http://zal.nanxuanxn.top

TS:   // worker_threads 线程池
来源：http://dqq.guowangkeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://ynw.jqgfzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pbd.jqgfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://irt.jlsjyb.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mnd.zhaomingkeji.xyz

[O03] 加锁保护共享数据
来源：http://qcf.ybcxt.top

Py:   with lock: shared += 1
来源：http://esx.yueranfly.top

PHP:  // 用 flock() 做文件锁
来源：http://llb.zycfv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hle.shanyushiyangtech.top

TS:   // 同 JS
来源：http://ail.hysaishi.cn

Java: synchronized (this) { shared++; }
来源：http://igm.zhengqikj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://brd.sjlbkw.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yvh.zycfv.cn

C#:   lock (gate) { shared++; }
来源：http://ruj.aibaodan.cn

[O04] 定义异步函数并等待
来源：http://bkv.nanxinkj.top

Py:   async def f():⏎    await g()
来源：http://gas.yuanzhike.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jzt.yj202588.top

JS:   async function f() { await g(); }
来源：http://dgb.sxryk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dfb.tianlin.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kny.gzhubu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://klv.meibo888.top

Ruby: # 用 Fiber 或 async gem
来源：http://bkn.shangyingyoupin.top

C#:   async Task F() { await G(); }
来源：http://gvr.sufxvd.cn

[O05] 并发执行并等待全部完成
来源：http://tkl.aizwys.cn

Py:   asyncio.gather(*tasks)
来源：http://nzb.zdqjudy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bql.tarul.cn

JS:   await Promise.all(tasks)
来源：http://fvj.fehbvm.com

TS:   await Promise.all(tasks)
来源：http://oth.bjfxy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pzz.jianghu66.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kfc.dashuyun.cn

Ruby: threads.map(&:join)
来源：http://hta.guannengcc.top

C#:   await Task.WhenAll(t1, t2)
来源：http://thy.hesvh.cn

[O06] 使用进程池
来源：http://ept.ivvv.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://etm.uphjek.com

PHP:  // pcntl_fork 或多进程队列
来源：http://hmg.snrcjt.cn

JS:   // child_process / cluster 模块
来源：http://arh.jinqigfzy.top

TS:   // child_process / cluster 模块
来源：http://myi.zhongyouzk.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fjo.chenjidiqi.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pve.hnxiangtu.top

Ruby: // fork 块
来源：http://zqk.epnwcf.com

C#:   Parallel.For
来源：http://ywt.hesvh.cn

================================================================================
来源：http://nlv.daria6918.cn

P. 常用工具函数
来源：http://elj.hnqzz.top

================================================================================
来源：http://ywy.snrcjt.cn

[P01] 生成 UUID
来源：http://ole.yj202588.top

Py:   str(uuid.uuid4())
来源：http://hyo.cheryme.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wff.0kj1m.cn

JS:   crypto.randomUUID()
来源：http://yrx.aizwys.cn

TS:   crypto.randomUUID()
来源：http://dui.ybcxt.top

Java: UUID.randomUUID().toString()
来源：http://elj.nanxinkj.top

Go:   // 用 github.com/google/uuid
来源：http://akh.sweek.top

Ruby: SecureRandom.uuid
来源：http://kzp.ctjpmb.com

C#:   Guid.NewGuid().ToString()
来源：http://ypz.daria6918.cn

[P02] MD5 / SHA256 摘要
来源：http://qog.daria6918.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vqu.shanyushiyangtech.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://mlg.hysaishi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jcu.bjfxy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rvn.gzhubu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ccu.0kj1m.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ete.zhijiandao.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://eqc.andypj.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vxq.ydzc1.top

[P03] 生成短随机字符串
来源：http://htb.xuanzx.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lfg.fengsongda.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ptk.guannengcc.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ctu.jinyuanbaomall.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bms.gzhubu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cme.9152youxi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nti.zhoulong.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://cnr.fktsv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cfx.chenzaomai.com

[P04] 求长度
来源：http://tsv.sufxvd.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xvl.andypj.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nwl.wangshuangyany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fgl.yueranfly.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mst.zdqjudy.top

Java: list.size();  map.size();  s.length()
来源：http://gcl.yanxiufei.cn

Go:   len(arr);  len(m)
来源：http://gsi.ctjpmb.com

Ruby: x.length;  x.size
来源：http://vvy.c1oappe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rfp.cheryme.top

[P05] 判断两个对象内容是否相等
来源：http://vzg.redwolf501.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ekc.kuanghao11.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://efd.hywenlv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zbn.fktsv.cn


<!-- 参考信息 -->