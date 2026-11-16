代发 wailian999

TS:   resp.ok;  resp.status
来源：http://rfe.hysaishi.cn

Java: resp.statusCode()
来源：http://scd.shanyushiyangkeji.top

Go:   resp.StatusCode
来源：http://fhc.jianghu66.top

Ruby: resp.code.to_i
来源：http://jdr.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://xhs.sweek.top

[L08] 并发请求多个地址
来源：http://akp.cashguo.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cav.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://fws.guannengcc.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lxh.fehbvm.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fdg.xuetiantiany.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wuu.wangdashe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://osc.zycfv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pxx.zhoulong.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ayf.pycfn.com

================================================================================
来源：http://vys.ybcxt.top

M. 命令行 / 进程 / 环境
来源：http://ayl.sweek.top

================================================================================
来源：http://ysa.sufxvd.cn

[M01] 读取命令行参数
来源：http://gqg.jqgfzy.top

Py:   sys.argv[1:]
来源：http://srd.9152youxi.cn

PHP:  $argv;  $argc;
来源：http://gsa.zhoulong.xyz

JS:   process.argv.slice(2)
来源：http://cyn.xuanzx.com

TS:   process.argv.slice(2)
来源：http://ezv.guowangkeji.top

Java: args 数组（main 方法参数）
来源：http://izi.nanxinkj.top

Go:   os.Args[1:]
来源：http://jou.pengpengdd.cyou

Ruby: ARGV
来源：http://khq.yvedp.cn

C#:   args 数组（Main 方法参数）
来源：http://rca.hammf.cn

[M02] 读取环境变量
来源：http://pvy.tian-w.cn

Py:   os.environ.get("HOME")
来源：http://mjm.tianlin.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bpr.yj202588.top

JS:   process.env.HOME
来源：http://ghd.shanyushiyangtech.top

TS:   process.env.HOME
来源：http://ghq.jinqigfzy.top

Java: System.getenv("HOME")
来源：http://vil.hesvh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cpg.shzxlz.cn

Ruby: ENV["HOME"]
来源：http://jdg.tanke756.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fib.sufxvd.cn

[M03] 执行外部命令
来源：http://bms.xuanzx.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://knf.ywan-chungtsiang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jbg.cashguo.top

JS:   child_process.execSync("ls -l").toString()
来源：http://huo.316326.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://yzw.smart0.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yan.jinyuanbaomall.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://rpo.andypj.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://kng.jqgfzy.top

C#:   Process.Start("ls", "-l");
来源：http://dnd.zhiwuduotai.top

[M04] 获取当前工作目录
来源：http://hnb.52xcode.cn

Py:   os.getcwd()
来源：http://jlg.mhx1999.top

PHP:  getcwd();
来源：http://vvj.yfazqb.com

JS:   process.cwd()
来源：http://dnw.quarkkingdee.top

TS:   process.cwd()
来源：http://czr.mhx1999.top

Java: Path.of("").toAbsolutePath()
来源：http://zcy.9152youxi.cn

Go:   os.Getwd()
来源：http://hzz.52xcode.cn

Ruby: Dir.pwd
来源：http://ilf.daxiang520.top

C#:   Directory.GetCurrentDirectory()
来源：http://uys.jinghuilouyu.cn

[M05] 设置退出码
来源：http://wxu.guowangkeji.top

Py:   sys.exit(1)
来源：http://oqx.cashguo.top

PHP:  exit(1);
来源：http://oaq.ywan-chungtsiang.top

JS:   process.exit(1)
来源：http://vvk.xingfuxueyuan.xyz

TS:   process.exit(1)
来源：http://tuk.ctjpmb.com

Java: System.exit(1)
来源：http://zcu.xylfe.cn

Go:   os.Exit(1)
来源：http://szn.ivvv.top

Ruby: exit 1
来源：http://acs.yueranfly.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xfc.epnwcf.com

[M06] 向标准错误输出
来源：http://lda.jyoumei.cn

Py:   print("err", file=sys.stderr)
来源：http://jbj.nanxuanxn.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lyi.316326.xyz

JS:   console.error("err")
来源：http://wja.fzhhl.top

TS:   console.error("err")
来源：http://eqy.wangshuangyany.cn

Java: System.err.println("err")
来源：http://iem.jqgfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xfa.dianchejie.cn

Ruby: warn "err"
来源：http://qfc.xylfe.cn

C#:   Console.Error.WriteLine("err")
来源：http://mxj.daria6918.cn

[M07] 判断是否为主入口
来源：http://wtd.zhijiandao.cn

Py:   if __name__ == "__main__":
来源：http://loq.ehwqpu.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://olj.nanxuanxn.top

JS:   require.main === module
来源：http://qvw.aizwys.cn

TS:   require.main === module
来源：http://uex.smart0.xyz

Java: public static void main(String[] args)
来源：http://ryu.nanxuanxn.top

Go:   func main()
来源：http://loi.cdnleiting.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://imr.haohaochexian.top

C#:   static void Main(string[] args)
来源：http://jjz.shzxlz.cn

[M08] 获取系统与运行时信息
来源：http://akb.hysaishi.cn

Py:   platform.system();  platform.python_version()
来源：http://dmr.zhengqikj.top

PHP:  PHP_OS;  phpversion();
来源：http://akz.iojbl.cn

JS:   process.platform;  process.version
来源：http://atu.ivvv.top

TS:   process.platform;  process.version
来源：http://znn.jinyuanbaomall.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nwy.xylfe.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zzg.jinqigfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://riv.chenjidiqi.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://crj.pengpengdd.cyou

================================================================================
来源：http://dvk.tarul.cn

N. 数据结构与算法
来源：http://kbm.jinghuilouyu.cn

================================================================================
来源：http://gym.jyoumei.cn

[N01] 二分查找（有序数组）
来源：http://nfd.jinqigfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://iql.fengsongda.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://irs.jinyuanbaomall.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dyq.mhx1999.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dun.yj20258888.top

Java: Arrays.binarySearch(arr, x)
来源：http://xec.ehwqpu.com

Go:   sort.SearchInts(arr, x)
来源：http://vof.sufxvd.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qma.ivvv.top

C#:   Array.BinarySearch(arr, x)
来源：http://krb.vqdsnc.cn

[N02] 排序（工程实践用内置实现）
来源：http://yms.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://vai.gaohongyu789.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wav.cqqwz.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wzf.zhaomingkeji.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://bza.smart0.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rcm.yuxming.cn

Go:   slices.Sort(arr)
来源：http://nhz.hammf.cn

Ruby: arr.sort
来源：http://coa.aibaodan.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ufl.kuanghao11.cn

[N03] 快速排序（分治示例）
来源：http://fsu.jlsjyb.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gfq.bjfxy.top

PHP:  // 递归实现，或用 usort
来源：http://ogz.zhixingplan.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kjs.aibaodan.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wnv.dashuyun.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ffe.cdnleiting.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jbg.9152youxi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hqm.tarul.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hhv.yueranfly.top

[N04] 斐波那契数列
来源：http://atg.yj20258888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://evc.sxryk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qhk.haohaochexian.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jtu.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hdu.cdnleiting.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eqg.shanyushiyangtech.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sqo.zhiwuduotai.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://scq.daria6918.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://usg.hesvh.cn

[N05] 最大公约数
来源：http://dyb.yangfankeji.com

Py:   math.gcd(a, b)
来源：http://tzl.9152youxi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bab.yvedp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lbs.gzhubu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bbg.jianghu66.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://obk.jqgfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gaf.epnwcf.com

Ruby: a.gcd(b)
来源：http://gpt.aizwys.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qtu.chenzaomai.com

[N06] 判断回文字符串
来源：http://clj.hongshengwenyu.top

Py:   s == s[::-1]
来源：http://bhd.jqgufenzy.top

PHP:  $s === strrev($s);
来源：http://mab.yfazqb.com

JS:   s === [...s].reverse().join("")
来源：http://rct.sjlbkw.cn

TS:   s === [...s].reverse().join("")
来源：http://cvd.guannengcc.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xvd.hnxiangtu.top

Go:   // 双指针从两端比较
来源：http://zro.ppjwa.cn

Ruby: s == s.reverse
来源：http://glr.zhiwuduotai.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://gln.wangshuangyany.cn

[N07] 两数之和（返回下标）
来源：http://fxx.tarul.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kra.uphjek.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ayg.ivvv.top

JS:   // 手写 Map：map.set(v, i)
来源：http://efn.aibaodan.cn

TS:   // 手写 Map<string, number>
来源：http://orw.cashguo.top

Java: // 手写 HashMap
来源：http://ryk.zhixingplan.top

Go:   // 手写 map[int]int
来源：http://sfm.ybcxt.top

Ruby: // 手写 Hash
来源：http://xux.shanyushiyangtech.top

C#:   // 手写 Dictionary<int, int>
来源：http://gdx.epnwcf.com

[N08] 生成全排列
来源：http://ezn.zhongyouzk.top

Py:   itertools.permutations(arr)
来源：http://iwt.hywenlv.cn

PHP:  // 手写递归交换
来源：http://sru.hcnkem.com

JS:   // 手写回溯递归
来源：http://uci.iojbl.cn

TS:   // 手写回溯递归
来源：http://axy.yuxming.cn

Java: // 手写回溯递归
来源：http://kcp.hammf.cn

Go:   // 手写回溯递归
来源：http://anw.ehwqpu.com

Ruby: arr.permutation.to_a
来源：http://cru.aizwys.cn

C#:   // 手写回溯递归
来源：http://qqj.vehdjk.com

[N09] 栈与队列
来源：http://ihe.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ysu.mhx1999.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hcf.zhiwuduotai.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zdw.gotoacloud.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vxq.tanke756.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gmx.bjfxy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mdj.fehbvm.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pwu.gogol.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lee.sjlbkw.cn

[N10] 链表节点定义
来源：http://hqv.guannengcc.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jtt.feifeiyinyue.top

PHP:  class Node { public $v; public $next = null; }
来源：http://pjz.fengsongda.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wrw.bjfxy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://beb.fehbvm.com

Java: class Node { int v; Node next; }
来源：http://own.cucudq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tpq.fanxiaobao.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://jsl.zhengqikj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://kcy.nwbrower.top

[N11] 二叉树中序遍历
来源：http://rre.snrcjt.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zpm.gotoacloud.top

PHP:  // 手写递归函数
来源：http://slm.yfazqb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qis.shanyushiyangtech.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uit.shzxlz.cn

Java: // 手写递归
来源：http://pdk.shzxlz.cn

Go:   // 手写递归
来源：http://kur.bbcook.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nep.mhx1999.top

C#:   // 手写递归
来源：http://zhl.shanyushiyangtech.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xob.c1oappe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zdr.svipenyu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ntd.vqdsnc.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://shw.52xcode.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ref.fktsv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zho.uphjek.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://miv.sufxvd.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rnp.fktsv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ysz.xuetiantiany.cn

================================================================================
来源：http://ttn.vehdjk.com

O. 并发与异步
来源：http://epu.gzhubu.top

================================================================================
来源：http://gfw.uphjek.com

[O01] 启动一个线程
来源：http://awg.chenzaomai.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://udk.shanyushiyangtech.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://via.316326.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://siw.zhijiandao.cn

TS:   // 同 JS
来源：http://ymn.meibo888.top

Java: new Thread(() -> f()).start()
来源：http://rpm.andypj.xyz

Go:   go f()
来源：http://pvf.jinqigfzy.top

Ruby: Thread.new { f }
来源：http://psb.kuanghao11.cn

C#:   Task.Run(() => F());
来源：http://spl.bbcook.cn

[O02] 使用线程池
来源：http://cvn.hammf.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eyt.sweek.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xax.iojbl.cn

JS:   // worker_threads 线程池
来源：http://ruj.52xcode.cn

TS:   // worker_threads 线程池
来源：http://xks.9152youxi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tsn.shzxlz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ira.wangdashe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://erp.c1oappe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oph.zdbjq.cn

[O03] 加锁保护共享数据
来源：http://zuw.snrcjt.cn

Py:   with lock: shared += 1
来源：http://hah.zhiwuduotai.top

PHP:  // 用 flock() 做文件锁
来源：http://jom.yfazqb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bfr.jyoumei.cn

TS:   // 同 JS
来源：http://xxb.yj20258888.top

Java: synchronized (this) { shared++; }
来源：http://yjo.zhengqikj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dlo.zhengqikj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://uij.xuetiantiany.cn

C#:   lock (gate) { shared++; }
来源：http://bvc.yj20258888.top

[O04] 定义异步函数并等待
来源：http://stl.zhongyouzk.top

Py:   async def f():⏎    await g()
来源：http://uns.tarul.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cqb.jqgfzy.top

JS:   async function f() { await g(); }
来源：http://oxy.zhoulong.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://dof.hongshengwenyu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nxz.zhijiandao.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eaw.cashguo.top

Ruby: # 用 Fiber 或 async gem
来源：http://har.bbcook.cn

C#:   async Task F() { await G(); }
来源：http://azp.ydjk.org.cn

[O05] 并发执行并等待全部完成
来源：http://xce.snrcjt.cn

Py:   asyncio.gather(*tasks)
来源：http://cko.redwolf501.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pcj.xuanzx.com

JS:   await Promise.all(tasks)
来源：http://bwu.cdnleiting.top

TS:   await Promise.all(tasks)
来源：http://npi.haohaochexian.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://spn.fktsv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uiw.zdqjudy.top

Ruby: threads.map(&:join)
来源：http://nmz.feifeiyinyue.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lpc.chenlongwang.top

[O06] 使用进程池
来源：http://wej.hysaishi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ytw.yj202588.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xid.ehwqpu.com

JS:   // child_process / cluster 模块
来源：http://qcn.svipenyu.cn

TS:   // child_process / cluster 模块
来源：http://uvi.zdqjudy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mwh.sxryk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ufd.haohaochexian.top

Ruby: // fork 块
来源：http://nyo.vqdsnc.cn

C#:   Parallel.For
来源：http://gpi.fanxiaobao.xyz

================================================================================
来源：http://jyh.mhx1999.top

P. 常用工具函数
来源：http://uyp.gzhubu.top

================================================================================
来源：http://lrn.hesvh.cn

[P01] 生成 UUID
来源：http://dtl.xuetiantiany.cn

Py:   str(uuid.uuid4())
来源：http://twv.zhixingplan.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rke.hnxiangtu.top

JS:   crypto.randomUUID()
来源：http://xpp.ctjpmb.com

TS:   crypto.randomUUID()
来源：http://dci.fanxiaobao.xyz

Java: UUID.randomUUID().toString()
来源：http://aar.quarkkingdee.top

Go:   // 用 github.com/google/uuid
来源：http://nrv.0kj1m.cn

Ruby: SecureRandom.uuid
来源：http://rtk.andypj.xyz

C#:   Guid.NewGuid().ToString()
来源：http://epq.zhengqikj.top

[P02] MD5 / SHA256 摘要
来源：http://uro.dianchejie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ixj.yueranfly.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://uqk.316326.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mmm.uphjek.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dzz.hammf.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qib.hywenlv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kue.chenjidiqi.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cor.gzhubu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://esg.quarkkingdee.top

[P03] 生成短随机字符串
来源：http://vky.jinqigufen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ion.gogol.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mbo.tianlin.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mjp.epnwcf.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bnw.nanxinkj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uuk.gotoacloud.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kzd.zhiwuduotai.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xak.ydzc1.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gsc.wangshuangyany.cn

[P04] 求长度
来源：http://ipl.zhoulong.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tca.yongpay.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jhq.cashguo.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yjl.jinqigufen.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vrt.chenlongwang.top

Java: list.size();  map.size();  s.length()
来源：http://pcr.xuanzx.com

Go:   len(arr);  len(m)
来源：http://tyq.xinyue.icu

Ruby: x.length;  x.size
来源：http://qjv.zhengqikj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pms.iojbl.cn

[P05] 判断两个对象内容是否相等
来源：http://xvp.yj202588.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://xua.zycfv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fde.bjfxy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://adf.sweek.top


<!-- 参考信息 -->