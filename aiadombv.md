代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://uzu.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bpg.wangshuangyany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qvs.wangshuangyany.cn

JS:   resp.ok;  resp.status
来源：http://otb.zhijiandao.cn

TS:   resp.ok;  resp.status
来源：http://xph.sweek.top

Java: resp.statusCode()
来源：http://wcw.ppjwa.cn

Go:   resp.StatusCode
来源：http://brd.shanyushiyangtech.top

Ruby: resp.code.to_i
来源：http://kmk.sweek.top

C#:   (int)resp.StatusCode
来源：http://pff.zdbjq.cn

[L08] 并发请求多个地址
来源：http://ftz.chenjidiqi.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lup.jiagoushi.top

PHP:  curl_multi_init() 系列
来源：http://erx.ybcxt.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://axb.fzhhl.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://urn.zhijiandao.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ntv.gotoacloud.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ojj.jqgfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ygs.hongshengwenyu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jou.ivvv.top

================================================================================
来源：http://zyf.hfpthk.cn

M. 命令行 / 进程 / 环境
来源：http://xme.tianlin.xyz

================================================================================
来源：http://wma.zdbjq.cn

[M01] 读取命令行参数
来源：http://sjr.vehdjk.com

Py:   sys.argv[1:]
来源：http://qaz.iojbl.cn

PHP:  $argv;  $argc;
来源：http://hze.xuetiantiany.cn

JS:   process.argv.slice(2)
来源：http://ncg.guannengcc.top

TS:   process.argv.slice(2)
来源：http://frq.jqgfzy.top

Java: args 数组（main 方法参数）
来源：http://pdr.hfpthk.cn

Go:   os.Args[1:]
来源：http://eub.quarkkingdee.top

Ruby: ARGV
来源：http://zfy.zdqjudy.top

C#:   args 数组（Main 方法参数）
来源：http://qxt.yj20258888.top

[M02] 读取环境变量
来源：http://rmc.cucudq.cn

Py:   os.environ.get("HOME")
来源：http://hlx.wangshuangyany.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bub.mhx1999.top

JS:   process.env.HOME
来源：http://nny.yfazqb.com

TS:   process.env.HOME
来源：http://jur.ydzc1.top

Java: System.getenv("HOME")
来源：http://axx.ppjwa.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mwo.vqdsnc.cn

Ruby: ENV["HOME"]
来源：http://yuk.zdbjq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://get.ehwqpu.com

[M03] 执行外部命令
来源：http://hjn.sweek.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xtc.fanxiaobao.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sle.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ehs.sjlbkw.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wrf.gzhubu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://pzl.svipenyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kqb.fktsv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ivy.hywenlv.cn

C#:   Process.Start("ls", "-l");
来源：http://axs.yuanzhike.top

[M04] 获取当前工作目录
来源：http://hio.zhoulong.xyz

Py:   os.getcwd()
来源：http://xte.guannengcc.top

PHP:  getcwd();
来源：http://iej.wangdashe.top

JS:   process.cwd()
来源：http://imi.tianlin.xyz

TS:   process.cwd()
来源：http://xhf.dianchejie.cn

Java: Path.of("").toAbsolutePath()
来源：http://dmj.jinqigufen.top

Go:   os.Getwd()
来源：http://iiy.gogol.net.cn

Ruby: Dir.pwd
来源：http://cwc.52xcode.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fef.gotoacloud.top

[M05] 设置退出码
来源：http://qyh.ppjwa.cn

Py:   sys.exit(1)
来源：http://paw.yanxiufei.cn

PHP:  exit(1);
来源：http://urb.hnqzz.top

JS:   process.exit(1)
来源：http://wsq.xuanzx.com

TS:   process.exit(1)
来源：http://jgx.cheryme.top

Java: System.exit(1)
来源：http://hsm.hnxiangtu.top

Go:   os.Exit(1)
来源：http://lwy.jinqigufen.top

Ruby: exit 1
来源：http://mnd.jyoumei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jle.fanxiaobao.xyz

[M06] 向标准错误输出
来源：http://lit.9152youxi.cn

Py:   print("err", file=sys.stderr)
来源：http://krl.uphjek.com

PHP:  fwrite(STDERR, "err\n");
来源：http://xzm.sjlbkw.cn

JS:   console.error("err")
来源：http://tof.uphjek.com

TS:   console.error("err")
来源：http://xdx.xziqi.cn

Java: System.err.println("err")
来源：http://wbg.sufxvd.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ubi.mhx1999.top

Ruby: warn "err"
来源：http://ran.tianlin.xyz

C#:   Console.Error.WriteLine("err")
来源：http://zkx.svipenyu.cn

[M07] 判断是否为主入口
来源：http://kxl.snrcjt.cn

Py:   if __name__ == "__main__":
来源：http://wlz.jyoumei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://srg.sufxvd.cn

JS:   require.main === module
来源：http://ymo.jinqigufen.top

TS:   require.main === module
来源：http://irp.gaohongyu789.top

Java: public static void main(String[] args)
来源：http://yzu.wangshuangyany.cn

Go:   func main()
来源：http://vqv.tanke756.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tal.hywenlv.cn

C#:   static void Main(string[] args)
来源：http://ahw.nanxuanxn.top

[M08] 获取系统与运行时信息
来源：http://quh.ehwqpu.com

Py:   platform.system();  platform.python_version()
来源：http://qgi.pengpengdd.cyou

PHP:  PHP_OS;  phpversion();
来源：http://ccf.tianlin.xyz

JS:   process.platform;  process.version
来源：http://ajz.svipenyu.cn

TS:   process.platform;  process.version
来源：http://drj.zhixingplan.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://snz.cqqwz.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ebj.nanxuanxn.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dpr.shanyushiyangtech.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://eok.pengpengdd.cyou

================================================================================
来源：http://sco.jianghu66.top

N. 数据结构与算法
来源：http://whz.fzhhl.top

================================================================================
来源：http://cnb.yonumen.top

[N01] 二分查找（有序数组）
来源：http://kuz.tianlin.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://fei.xziqi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zbu.svipenyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zje.sufxvd.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bru.yuanzhike.top

Java: Arrays.binarySearch(arr, x)
来源：http://twt.0kj1m.cn

Go:   sort.SearchInts(arr, x)
来源：http://wpf.guowangkeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mox.pengpengdd.cyou

C#:   Array.BinarySearch(arr, x)
来源：http://cel.hesvh.cn

[N02] 排序（工程实践用内置实现）
来源：http://jbj.jinyuanbaomall.cn

Py:   sorted(arr);  arr.sort()
来源：http://wkn.nanxuanxn.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qed.ydzc1.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://etc.xylfe.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vnb.fktsv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xzl.gotoacloud.top

Go:   slices.Sort(arr)
来源：http://wyc.cheryme.top

Ruby: arr.sort
来源：http://lzd.shuidangran.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rua.52xcode.cn

[N03] 快速排序（分治示例）
来源：http://qwh.ywan-chungtsiang.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mgv.guannengcc.top

PHP:  // 递归实现，或用 usort
来源：http://ooc.mhx1999.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wbf.mhx1999.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://guh.chenlongwang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://caw.jinyuanbaomall.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mkn.bjfxy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ibp.xinyue.icu

C#:   // 手写递归，或 Array.Sort
来源：http://uhi.vehdjk.com

[N04] 斐波那契数列
来源：http://yye.cheryme.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qcm.jianghu66.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vot.fengsongda.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ipr.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://knf.cucudq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ztv.hammf.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rqo.jlsjyb.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vfs.jqgfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vyb.ywan-chungtsiang.top

[N05] 最大公约数
来源：http://lqq.9152youxi.cn

Py:   math.gcd(a, b)
来源：http://kzu.hesvh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ggv.cdnleiting.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pwl.cdnleiting.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ckq.andypj.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ycv.jlsjyb.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lqe.jinyuanbaomall.cn

Ruby: a.gcd(b)
来源：http://tvr.ppjwa.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://srr.vqdsnc.cn

[N06] 判断回文字符串
来源：http://xwe.hnxiangtu.top

Py:   s == s[::-1]
来源：http://pno.feifeiyinyue.top

PHP:  $s === strrev($s);
来源：http://lxz.yueranfly.top

JS:   s === [...s].reverse().join("")
来源：http://rtd.316326.xyz

TS:   s === [...s].reverse().join("")
来源：http://awu.jinqigfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cbd.jqgufenzy.top

Go:   // 双指针从两端比较
来源：http://vvd.yj202588.top

Ruby: s == s.reverse
来源：http://rex.zycfv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vbe.yuxming.cn

[N07] 两数之和（返回下标）
来源：http://wuu.chenlongwang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ziv.ppjwa.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jnq.xylfe.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fnu.zdbjq.cn

TS:   // 手写 Map<string, number>
来源：http://sda.jinqigfzy.top

Java: // 手写 HashMap
来源：http://zsq.hnqzz.top

Go:   // 手写 map[int]int
来源：http://rwh.ybcxt.top

Ruby: // 手写 Hash
来源：http://weq.hongshengwenyu.top

C#:   // 手写 Dictionary<int, int>
来源：http://tjc.hcnkem.com

[N08] 生成全排列
来源：http://zhw.fzhhl.top

Py:   itertools.permutations(arr)
来源：http://ste.gaohongyu789.top

PHP:  // 手写递归交换
来源：http://njx.jinghuilouyu.cn

JS:   // 手写回溯递归
来源：http://hlu.cashguo.top

TS:   // 手写回溯递归
来源：http://rac.sjlbkw.cn

Java: // 手写回溯递归
来源：http://fpu.shuidangran.top

Go:   // 手写回溯递归
来源：http://thg.zhixingplan.top

Ruby: arr.permutation.to_a
来源：http://zgc.vehdjk.com

C#:   // 手写回溯递归
来源：http://tpn.wangdashe.top

[N09] 栈与队列
来源：http://drt.mhx1999.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sft.jinyuanbaomall.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fpo.pycfn.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dkr.c1oappe.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ryl.nanxinkj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dbe.tianlin.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://irx.yj202588.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cor.redwolf501.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bpw.zhongyouzk.top

[N10] 链表节点定义
来源：http://jcn.sjlbkw.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jzq.yongpay.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gpx.nanxuanxn.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hwm.ybcxt.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hpi.hcnkem.com

Java: class Node { int v; Node next; }
来源：http://let.xylfe.cn

Go:   type Node struct { V int; Next *Node }
来源：http://njf.ctjpmb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://mgt.xinyue.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://zlc.xinyue.icu

[N11] 二叉树中序遍历
来源：http://rez.birdmap.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qyk.ydzc1.top

PHP:  // 手写递归函数
来源：http://vbs.snrcjt.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yec.cdnleiting.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yen.uphjek.com

Java: // 手写递归
来源：http://zeb.316326.xyz

Go:   // 手写递归
来源：http://pav.ivvv.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lex.hnqzz.top

C#:   // 手写递归
来源：http://nuq.shuidangran.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ndg.hnqzz.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kkz.tanke756.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qnf.hnqzz.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qvp.hnxiangtu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://utn.ywan-chungtsiang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rzy.shangyingyoupin.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ulu.haohaochexian.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fxm.yangfankeji.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vrw.redwolf501.top

================================================================================
来源：http://fdm.yvedp.cn

O. 并发与异步
来源：http://hsm.chenzaomai.com

================================================================================
来源：http://ufq.hesvh.cn

[O01] 启动一个线程
来源：http://fci.sxryk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hlb.dianchejie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://grt.tanke756.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mge.yj202588.top

TS:   // 同 JS
来源：http://ywl.ppjwa.cn

Java: new Thread(() -> f()).start()
来源：http://oom.sweek.top

Go:   go f()
来源：http://ltf.0kj1m.cn

Ruby: Thread.new { f }
来源：http://hmt.yj20258.top

C#:   Task.Run(() => F());
来源：http://wtr.hammf.cn

[O02] 使用线程池
来源：http://sxa.snrcjt.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://liw.snrcjt.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://arv.hfpthk.cn

JS:   // worker_threads 线程池
来源：http://gir.feifeiyinyue.top

TS:   // worker_threads 线程池
来源：http://vtu.hesvh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tpp.zhongyouzk.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mtu.wangshuangyany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hwi.daxiang520.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fdm.52xcode.cn

[O03] 加锁保护共享数据
来源：http://mri.hnqzz.top

Py:   with lock: shared += 1
来源：http://jje.nanxinkj.top

PHP:  // 用 flock() 做文件锁
来源：http://ytm.sweek.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sku.0kj1m.cn

TS:   // 同 JS
来源：http://fdw.smart0.xyz

Java: synchronized (this) { shared++; }
来源：http://gaf.jlsjyb.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sae.jinyuanbaomall.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://blr.hywenlv.cn

C#:   lock (gate) { shared++; }
来源：http://azw.aizwys.cn

[O04] 定义异步函数并等待
来源：http://ejm.hesvh.cn

Py:   async def f():⏎    await g()
来源：http://vnd.quarkkingdee.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nam.yuxming.cn

JS:   async function f() { await g(); }
来源：http://qgo.jinyuanbaomall.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xrq.yangfankeji.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hmz.tianlin.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ajq.redwolf501.top

Ruby: # 用 Fiber 或 async gem
来源：http://vlo.ehwqpu.com

C#:   async Task F() { await G(); }
来源：http://dvt.jiagoushi.top

[O05] 并发执行并等待全部完成
来源：http://baa.zhongyouzk.top

Py:   asyncio.gather(*tasks)
来源：http://acw.uphjek.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://plq.hammf.cn

JS:   await Promise.all(tasks)
来源：http://rkj.fzhhl.top

TS:   await Promise.all(tasks)
来源：http://auz.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nxk.cheryme.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dpw.0kj1m.cn

Ruby: threads.map(&:join)
来源：http://ghq.52xcode.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ccw.snrcjt.cn

[O06] 使用进程池
来源：http://wpd.dianchejie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gjr.wangdashe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qoi.zycfv.cn

JS:   // child_process / cluster 模块
来源：http://tic.aizwys.cn

TS:   // child_process / cluster 模块
来源：http://svr.chenzaomai.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vlz.shangyingyoupin.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wmz.tian-w.cn

Ruby: // fork 块
来源：http://orw.nwbrower.top

C#:   Parallel.For
来源：http://mwh.sufxvd.cn

================================================================================
来源：http://lrp.xingfuxueyuan.xyz

P. 常用工具函数
来源：http://ogz.pengpengdd.cyou

================================================================================
来源：http://eqw.fzhhl.top

[P01] 生成 UUID
来源：http://tvu.cashguo.top

Py:   str(uuid.uuid4())
来源：http://fdk.daxiang520.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://eor.sysykeji.top

JS:   crypto.randomUUID()
来源：http://nif.ydzc1.top

TS:   crypto.randomUUID()
来源：http://tie.ybcxt.top

Java: UUID.randomUUID().toString()
来源：http://laa.guowangkeji.top

Go:   // 用 github.com/google/uuid
来源：http://yyb.yuanzhike.top

Ruby: SecureRandom.uuid
来源：http://fwa.fehbvm.com

C#:   Guid.NewGuid().ToString()
来源：http://jqg.bbcook.cn

[P02] MD5 / SHA256 摘要
来源：http://kvc.chenzaomai.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dde.0kj1m.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rzz.hongshengwenyu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://leb.yanxiufei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://msp.fehbvm.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uby.mhx1999.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hds.ppjwa.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zvv.wangshuangyany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://khp.hcnkem.com

[P03] 生成短随机字符串
来源：http://wel.ctjpmb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pgm.jiagoushi.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://skb.shanyushiyangtech.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vtx.hesvh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://grg.zdbjq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ken.tanke756.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jav.hfpthk.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://aol.pycfn.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pvm.daxiang520.top

[P04] 求长度
来源：http://xtk.zhixingplan.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ndq.zhiwuduotai.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vru.kuanghao11.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uur.gzhubu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cpl.shanyushiyangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://del.cashguo.top

Go:   len(arr);  len(m)
来源：http://eor.yueranfly.top

Ruby: x.length;  x.size
来源：http://iqx.jqgufenzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://aeg.xuanzx.com


<!-- 参考信息 -->