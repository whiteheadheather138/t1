代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://dvh.jinqigufen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bdy.c1oappe.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wxo.zdqjudy.top

JS:   resp.ok;  resp.status
来源：http://azp.pycfn.com

TS:   resp.ok;  resp.status
来源：http://goo.hysaishi.cn

Java: resp.statusCode()
来源：http://pec.fehbvm.com

Go:   resp.StatusCode
来源：http://upb.feifeiyinyue.top

Ruby: resp.code.to_i
来源：http://sqh.sxryk.cn

C#:   (int)resp.StatusCode
来源：http://eqz.fengsongda.top

[L08] 并发请求多个地址
来源：http://gwx.ydjk.org.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://atg.dianchejie.cn

PHP:  curl_multi_init() 系列
来源：http://fdd.fanxiaobao.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lom.shangyingyoupin.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ibb.zhijiandao.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://evq.chenjidiqi.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yuw.hysaishi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xoj.gogol.net.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jvp.jqgufenzy.top

================================================================================
来源：http://irp.yfazqb.com

M. 命令行 / 进程 / 环境
来源：http://xso.shuidangran.top

================================================================================
来源：http://oqp.316326.xyz

[M01] 读取命令行参数
来源：http://fcn.xuanzx.com

Py:   sys.argv[1:]
来源：http://nmc.zhijiandao.cn

PHP:  $argv;  $argc;
来源：http://hxr.feifeiyinyue.top

JS:   process.argv.slice(2)
来源：http://xix.ehwqpu.com

TS:   process.argv.slice(2)
来源：http://iih.birdmap.top

Java: args 数组（main 方法参数）
来源：http://qig.cdnleiting.top

Go:   os.Args[1:]
来源：http://bmr.jqgufenzy.top

Ruby: ARGV
来源：http://pxa.jlsjyb.cn

C#:   args 数组（Main 方法参数）
来源：http://jzb.ivvv.top

[M02] 读取环境变量
来源：http://yge.hcnkem.com

Py:   os.environ.get("HOME")
来源：http://fmq.jianghu66.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rrh.gzhubu.top

JS:   process.env.HOME
来源：http://ymv.shangyingyoupin.top

TS:   process.env.HOME
来源：http://rzd.ydjk.org.cn

Java: System.getenv("HOME")
来源：http://mai.hongshengwenyu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://npc.shzxlz.cn

Ruby: ENV["HOME"]
来源：http://yle.havefunace.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zih.gzhubu.top

[M03] 执行外部命令
来源：http://uyp.xuanzx.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://scm.hesvh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yct.fengsongda.top

JS:   child_process.execSync("ls -l").toString()
来源：http://dlk.guowangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jbz.yueranfly.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://svt.meibo888.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wki.yanxiufei.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rsc.ybcxt.top

C#:   Process.Start("ls", "-l");
来源：http://mox.sufxvd.cn

[M04] 获取当前工作目录
来源：http://qmi.nanxuanxn.top

Py:   os.getcwd()
来源：http://oan.redwolf501.top

PHP:  getcwd();
来源：http://tzj.guowangkeji.top

JS:   process.cwd()
来源：http://tgt.52xcode.cn

TS:   process.cwd()
来源：http://lhs.jqgfzy.top

Java: Path.of("").toAbsolutePath()
来源：http://flj.cqqwz.cn

Go:   os.Getwd()
来源：http://rfp.cheryme.top

Ruby: Dir.pwd
来源：http://smd.jinqigfzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://fhi.gaohongyu789.top

[M05] 设置退出码
来源：http://qor.cqqwz.cn

Py:   sys.exit(1)
来源：http://puq.hysaishi.cn

PHP:  exit(1);
来源：http://mim.tian-w.cn

JS:   process.exit(1)
来源：http://vpr.haohaochexian.top

TS:   process.exit(1)
来源：http://gue.mhx1999.top

Java: System.exit(1)
来源：http://whn.pycfn.com

Go:   os.Exit(1)
来源：http://ptj.uphjek.com

Ruby: exit 1
来源：http://qdn.zhixingplan.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zvo.sysykeji.top

[M06] 向标准错误输出
来源：http://vxx.sufxvd.cn

Py:   print("err", file=sys.stderr)
来源：http://iug.yj20258888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://zks.hammf.cn

JS:   console.error("err")
来源：http://cxs.yuanzhike.top

TS:   console.error("err")
来源：http://cre.zhengqikj.top

Java: System.err.println("err")
来源：http://vlg.birdmap.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jrk.ywan-chungtsiang.top

Ruby: warn "err"
来源：http://pco.sweek.top

C#:   Console.Error.WriteLine("err")
来源：http://bsg.sysykeji.top

[M07] 判断是否为主入口
来源：http://rzs.9152youxi.cn

Py:   if __name__ == "__main__":
来源：http://ctd.zhongyouzk.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cjd.yj20258888.top

JS:   require.main === module
来源：http://wvp.ybcxt.top

TS:   require.main === module
来源：http://xdn.ctjpmb.com

Java: public static void main(String[] args)
来源：http://rap.shuidangran.top

Go:   func main()
来源：http://qes.zhoulong.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cns.hfpthk.cn

C#:   static void Main(string[] args)
来源：http://hrz.zdbjq.cn

[M08] 获取系统与运行时信息
来源：http://tec.yongpay.top

Py:   platform.system();  platform.python_version()
来源：http://sll.dianchejie.cn

PHP:  PHP_OS;  phpversion();
来源：http://hyl.shuidangran.top

JS:   process.platform;  process.version
来源：http://fhr.yj20258888.top

TS:   process.platform;  process.version
来源：http://wkl.chenjidiqi.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bbr.shuidangran.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ltt.ydzc1.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bzu.hysaishi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kvu.wangshuangyany.cn

================================================================================
来源：http://sve.cheryme.top

N. 数据结构与算法
来源：http://axl.jyoumei.cn

================================================================================
来源：http://tdr.jinyuanbaomall.cn

[N01] 二分查找（有序数组）
来源：http://waf.fzhhl.top

Py:   bisect.bisect_left(arr, x)
来源：http://gns.yanxiufei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kbx.ivvv.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kxy.9152youxi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mpm.shanyushiyangkeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://vje.ehwqpu.com

Go:   sort.SearchInts(arr, x)
来源：http://mio.shuidangran.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ctu.zhengqikj.top

C#:   Array.BinarySearch(arr, x)
来源：http://yrg.haohaochexian.top

[N02] 排序（工程实践用内置实现）
来源：http://kfb.zycfv.cn

Py:   sorted(arr);  arr.sort()
来源：http://eoj.tian-w.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gqq.pengpengdd.cyou

JS:   [...arr].sort((a, b) => a - b)
来源：http://glh.kuanghao11.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://szy.pycfn.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ats.hysaishi.cn

Go:   slices.Sort(arr)
来源：http://lrn.pengpengdd.cyou

Ruby: arr.sort
来源：http://eoc.yueranfly.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dwv.daria6918.cn

[N03] 快速排序（分治示例）
来源：http://tyy.zhengqikj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mvb.zhixingplan.top

PHP:  // 递归实现，或用 usort
来源：http://tiy.yj202588.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yuk.zycfv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zjh.guannengcc.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tcv.jqgfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nxj.hammf.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zoc.mhx1999.top

C#:   // 手写递归，或 Array.Sort
来源：http://owu.ybcxt.top

[N04] 斐波那契数列
来源：http://kzl.meibo888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mga.cheryme.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ujc.tanke756.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vjc.redwolf501.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oqv.cqqwz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kps.jinghuilouyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gtn.sufxvd.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rrv.zhiwuduotai.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dgi.jinyuanbaomall.cn

[N05] 最大公约数
来源：http://wwr.xuanzx.com

Py:   math.gcd(a, b)
来源：http://qrf.daria6918.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ecs.zhijiandao.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wwd.vehdjk.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sgb.jlsjyb.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jah.zdqjudy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tkl.sufxvd.cn

Ruby: a.gcd(b)
来源：http://xdk.wangdashe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xzn.bjfxy.top

[N06] 判断回文字符串
来源：http://xsp.dashuyun.cn

Py:   s == s[::-1]
来源：http://jqr.gogol.net.cn

PHP:  $s === strrev($s);
来源：http://wco.gzhubu.top

JS:   s === [...s].reverse().join("")
来源：http://eyi.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://fjl.cashguo.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xra.guowangkeji.top

Go:   // 双指针从两端比较
来源：http://hjx.hammf.cn

Ruby: s == s.reverse
来源：http://utc.cucudq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://icl.yanxiufei.cn

[N07] 两数之和（返回下标）
来源：http://mlx.cqqwz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://acu.gzhubu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oyo.hcnkem.com

JS:   // 手写 Map：map.set(v, i)
来源：http://diw.ybcxt.top

TS:   // 手写 Map<string, number>
来源：http://ahk.hammf.cn

Java: // 手写 HashMap
来源：http://zyx.gotoacloud.top

Go:   // 手写 map[int]int
来源：http://shm.nanxuanxn.top

Ruby: // 手写 Hash
来源：http://uwq.jinqigufen.top

C#:   // 手写 Dictionary<int, int>
来源：http://yui.epnwcf.com

[N08] 生成全排列
来源：http://bal.xinyue.icu

Py:   itertools.permutations(arr)
来源：http://kgs.nanxinkj.top

PHP:  // 手写递归交换
来源：http://pjt.tian-w.cn

JS:   // 手写回溯递归
来源：http://yth.ybcxt.top

TS:   // 手写回溯递归
来源：http://vyl.yueranfly.top

Java: // 手写回溯递归
来源：http://bqb.wangdashe.top

Go:   // 手写回溯递归
来源：http://ocd.hnxiangtu.top

Ruby: arr.permutation.to_a
来源：http://iox.aibaodan.cn

C#:   // 手写回溯递归
来源：http://jom.cucudq.cn

[N09] 栈与队列
来源：http://clw.bbcook.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vte.zhoulong.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://pgo.gaohongyu789.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://doo.0kj1m.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ruc.gaohongyu789.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hje.ctjpmb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qkf.guowangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iyo.jqgfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://frd.zycfv.cn

[N10] 链表节点定义
来源：http://oks.cashguo.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ecj.iojbl.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://olo.fzhhl.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nsy.ydzc1.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yut.zhoulong.xyz

Java: class Node { int v; Node next; }
来源：http://xsu.xylfe.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pbb.ppjwa.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ngk.shuidangran.top

C#:   class Node { public int V; public Node? Next; }
来源：http://saj.sufxvd.cn

[N11] 二叉树中序遍历
来源：http://irp.c1oappe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tqm.cucudq.cn

PHP:  // 手写递归函数
来源：http://cva.dashuyun.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mfn.andypj.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xfx.zhengqikj.top

Java: // 手写递归
来源：http://fev.cqqwz.cn

Go:   // 手写递归
来源：http://gnx.cucudq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bjh.jlsjyb.cn

C#:   // 手写递归
来源：http://rrl.jinqigfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cdy.aizwys.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bvu.fanxiaobao.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zpz.jianghu66.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xrb.yueranfly.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ihg.yongpay.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ntw.sufxvd.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kaz.snrcjt.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rbv.chenjidiqi.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://azc.wangshuangyany.cn

================================================================================
来源：http://tbl.xuanzx.com

O. 并发与异步
来源：http://web.chenlongwang.top

================================================================================
来源：http://rny.cashguo.top

[O01] 启动一个线程
来源：http://gsn.hcnkem.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ozd.daxiang520.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rsl.0kj1m.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ztm.tanke756.top

TS:   // 同 JS
来源：http://rms.tanke756.top

Java: new Thread(() -> f()).start()
来源：http://bhm.hesvh.cn

Go:   go f()
来源：http://nhn.hywenlv.cn

Ruby: Thread.new { f }
来源：http://ubn.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://gws.pengpengdd.cyou

[O02] 使用线程池
来源：http://zdp.yfazqb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://trg.birdmap.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fbs.pengpengdd.cyou

JS:   // worker_threads 线程池
来源：http://rsb.xinyue.icu

TS:   // worker_threads 线程池
来源：http://fkp.iojbl.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hqm.yj20258.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nto.wangdashe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mzx.zdqjudy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://czp.gogol.net.cn

[O03] 加锁保护共享数据
来源：http://kqe.9152youxi.cn

Py:   with lock: shared += 1
来源：http://cxs.shzxlz.cn

PHP:  // 用 flock() 做文件锁
来源：http://ija.redwolf501.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ono.ybcxt.top

TS:   // 同 JS
来源：http://seq.jinqigfzy.top

Java: synchronized (this) { shared++; }
来源：http://ags.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hot.fzhhl.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rzo.shzxlz.cn

C#:   lock (gate) { shared++; }
来源：http://ttm.gaohongyu789.top

[O04] 定义异步函数并等待
来源：http://coc.yj20258888.top

Py:   async def f():⏎    await g()
来源：http://wyz.fanxiaobao.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xzc.fehbvm.com

JS:   async function f() { await g(); }
来源：http://wkr.9152youxi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vul.bbcook.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wgp.jinyuanbaomall.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tus.xylfe.cn

Ruby: # 用 Fiber 或 async gem
来源：http://prz.yfazqb.com

C#:   async Task F() { await G(); }
来源：http://nlq.nanxinkj.top

[O05] 并发执行并等待全部完成
来源：http://oeh.shangyingyoupin.top

Py:   asyncio.gather(*tasks)
来源：http://bfx.meibo888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://byv.birdmap.top

JS:   await Promise.all(tasks)
来源：http://iue.jyoumei.cn

TS:   await Promise.all(tasks)
来源：http://mno.yonumen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pqh.zhijiandao.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mkc.epnwcf.com

Ruby: threads.map(&:join)
来源：http://zwh.hfpthk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://btp.jqgufenzy.top

[O06] 使用进程池
来源：http://vds.jqgfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mls.fzhhl.top

PHP:  // pcntl_fork 或多进程队列
来源：http://hjc.0kj1m.cn

JS:   // child_process / cluster 模块
来源：http://bag.jinghuilouyu.cn

TS:   // child_process / cluster 模块
来源：http://vzm.jlsjyb.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lii.nwbrower.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fgg.smart0.xyz

Ruby: // fork 块
来源：http://dqd.daxiang520.top

C#:   Parallel.For
来源：http://jml.yj20258.top

================================================================================
来源：http://acg.fanxiaobao.xyz

P. 常用工具函数
来源：http://hru.jqgfzy.top

================================================================================
来源：http://vqz.hesvh.cn

[P01] 生成 UUID
来源：http://xoj.jinqigfzy.top

Py:   str(uuid.uuid4())
来源：http://ozy.snrcjt.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gsq.9152youxi.cn

JS:   crypto.randomUUID()
来源：http://oul.shuidangran.top

TS:   crypto.randomUUID()
来源：http://ehn.zdbjq.cn

Java: UUID.randomUUID().toString()
来源：http://zyc.yangfankeji.com

Go:   // 用 github.com/google/uuid
来源：http://jcx.guowangkeji.top

Ruby: SecureRandom.uuid
来源：http://ekz.zhoulong.xyz

C#:   Guid.NewGuid().ToString()
来源：http://ndo.iojbl.cn

[P02] MD5 / SHA256 摘要
来源：http://poz.ivvv.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gsr.yj20258888.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qys.ywan-chungtsiang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hlc.xuetiantiany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mkg.sxryk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://iip.chenlongwang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lcw.yangfankeji.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yra.xinyue.icu

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ibf.zhongyouzk.top

[P03] 生成短随机字符串
来源：http://pzl.dianchejie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hct.shangyingyoupin.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nji.fktsv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gsb.aizwys.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lco.yuxming.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zym.yuxming.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ich.sjlbkw.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://oli.mhx1999.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ajb.bjfxy.top

[P04] 求长度
来源：http://ibo.kuanghao11.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hnz.haohaochexian.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ikm.yuxming.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rwb.nwbrower.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uwg.sweek.top

Java: list.size();  map.size();  s.length()
来源：http://ttl.zhoulong.xyz

Go:   len(arr);  len(m)
来源：http://ftn.shuidangran.top

Ruby: x.length;  x.size
来源：http://mss.bbcook.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://drg.shanyushiyangkeji.top


<!-- 参考信息 -->