代发 wailian999

C#:   (int)resp.StatusCode
来源：http://idr.yangfankeji.com

[L08] 并发请求多个地址
来源：http://gst.nanxinkj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://aym.0kj1m.cn

PHP:  curl_multi_init() 系列
来源：http://nid.tarul.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vbn.shanyushiyangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://acu.bbcook.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ldt.xuetiantiany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xyc.hnqzz.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hpn.jinqigufen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jft.nanxinkj.top

================================================================================
来源：http://nqd.ybcxt.top

M. 命令行 / 进程 / 环境
来源：http://inh.shanyushiyangkeji.top

================================================================================
来源：http://wyf.tian-w.cn

[M01] 读取命令行参数
来源：http://yko.gogol.net.cn

Py:   sys.argv[1:]
来源：http://gis.bbcook.cn

PHP:  $argv;  $argc;
来源：http://aju.ivvv.top

JS:   process.argv.slice(2)
来源：http://qzh.shangyingyoupin.top

TS:   process.argv.slice(2)
来源：http://veo.dianchejie.cn

Java: args 数组（main 方法参数）
来源：http://aaz.svipenyu.cn

Go:   os.Args[1:]
来源：http://plw.yonumen.top

Ruby: ARGV
来源：http://hep.hesvh.cn

C#:   args 数组（Main 方法参数）
来源：http://itp.jiagoushi.top

[M02] 读取环境变量
来源：http://pbc.xingfuxueyuan.xyz

Py:   os.environ.get("HOME")
来源：http://ynr.wangdashe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tms.hywenlv.cn

JS:   process.env.HOME
来源：http://xrz.yueranfly.top

TS:   process.env.HOME
来源：http://dnc.smart0.xyz

Java: System.getenv("HOME")
来源：http://lny.ydjk.org.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://klx.kuanghao11.cn

Ruby: ENV["HOME"]
来源：http://evp.dianchejie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ymk.jlsjyb.cn

[M03] 执行外部命令
来源：http://xyw.bjfxy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uvd.xuetiantiany.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://thn.birdmap.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ybi.birdmap.top

TS:   child_process.execSync("ls -l").toString()
来源：http://eoq.svipenyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mrq.yangfankeji.com

Go:   exec.Command("ls", "-l").Output()
来源：http://bgf.vehdjk.com

Ruby: system("ls -l");  `ls -l`
来源：http://sqq.dianchejie.cn

C#:   Process.Start("ls", "-l");
来源：http://lfl.fanxiaobao.xyz

[M04] 获取当前工作目录
来源：http://lom.hcnkem.com

Py:   os.getcwd()
来源：http://ujx.sweek.top

PHP:  getcwd();
来源：http://cuw.cucudq.cn

JS:   process.cwd()
来源：http://lmo.daxiang520.top

TS:   process.cwd()
来源：http://lhd.gzhubu.top

Java: Path.of("").toAbsolutePath()
来源：http://dxw.yj202588.top

Go:   os.Getwd()
来源：http://mja.vqdsnc.cn

Ruby: Dir.pwd
来源：http://cre.cashguo.top

C#:   Directory.GetCurrentDirectory()
来源：http://zfu.zhixingplan.top

[M05] 设置退出码
来源：http://yth.daxiang520.top

Py:   sys.exit(1)
来源：http://nea.yongpay.top

PHP:  exit(1);
来源：http://naw.xuanzx.com

JS:   process.exit(1)
来源：http://vsy.guannengcc.top

TS:   process.exit(1)
来源：http://plw.yongpay.top

Java: System.exit(1)
来源：http://dfa.guannengcc.top

Go:   os.Exit(1)
来源：http://fyu.xylfe.cn

Ruby: exit 1
来源：http://eps.meibo888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dsv.feifeiyinyue.top

[M06] 向标准错误输出
来源：http://lqz.zdbjq.cn

Py:   print("err", file=sys.stderr)
来源：http://gbp.yfazqb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://bap.xuanzx.com

JS:   console.error("err")
来源：http://iec.xingfuxueyuan.xyz

TS:   console.error("err")
来源：http://lnd.kuanghao11.cn

Java: System.err.println("err")
来源：http://upw.hysaishi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pxx.yongpay.top

Ruby: warn "err"
来源：http://hrx.jlsjyb.cn

C#:   Console.Error.WriteLine("err")
来源：http://ptv.jqgfzy.top

[M07] 判断是否为主入口
来源：http://lzq.ydjk.org.cn

Py:   if __name__ == "__main__":
来源：http://lms.snrcjt.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kyi.dashuyun.cn

JS:   require.main === module
来源：http://xpc.ywan-chungtsiang.top

TS:   require.main === module
来源：http://zus.zhongyouzk.top

Java: public static void main(String[] args)
来源：http://gha.hnxiangtu.top

Go:   func main()
来源：http://ulc.wangdashe.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oxo.jqgufenzy.top

C#:   static void Main(string[] args)
来源：http://etb.yueranfly.top

[M08] 获取系统与运行时信息
来源：http://epm.sweek.top

Py:   platform.system();  platform.python_version()
来源：http://qtv.dianchejie.cn

PHP:  PHP_OS;  phpversion();
来源：http://kpm.zdbjq.cn

JS:   process.platform;  process.version
来源：http://ebv.fehbvm.com

TS:   process.platform;  process.version
来源：http://pqi.tian-w.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nsk.yongpay.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zas.jqgufenzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tzd.tanke756.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lnc.jinqigfzy.top

================================================================================
来源：http://qbn.vehdjk.com

N. 数据结构与算法
来源：http://vro.hcnkem.com

================================================================================
来源：http://ewj.jqgfzy.top

[N01] 二分查找（有序数组）
来源：http://zko.redwolf501.top

Py:   bisect.bisect_left(arr, x)
来源：http://zww.sysykeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xvp.vehdjk.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wur.shanyushiyangtech.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wcj.cqqwz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://yhq.daxiang520.top

Go:   sort.SearchInts(arr, x)
来源：http://cgh.havefunace.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ewt.havefunace.top

C#:   Array.BinarySearch(arr, x)
来源：http://qzh.hnqzz.top

[N02] 排序（工程实践用内置实现）
来源：http://ovt.vehdjk.com

Py:   sorted(arr);  arr.sort()
来源：http://ukc.cqqwz.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://atz.zhijiandao.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bau.wangshuangyany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sfo.zhiwuduotai.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fhm.kuanghao11.cn

Go:   slices.Sort(arr)
来源：http://zji.wangshuangyany.cn

Ruby: arr.sort
来源：http://ezo.cdnleiting.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gqs.jinyuanbaomall.cn

[N03] 快速排序（分治示例）
来源：http://swv.yonumen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://eer.yj20258.top

PHP:  // 递归实现，或用 usort
来源：http://cpw.yueranfly.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xij.snrcjt.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cqd.chenzaomai.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fvf.xinyue.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://obo.jianghu66.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rvn.yvedp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ver.jyoumei.cn

[N04] 斐波那契数列
来源：http://mcn.yanxiufei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://egj.fanxiaobao.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hrj.fktsv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vdk.shzxlz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mcq.hongshengwenyu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xzr.xinyue.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qvm.fanxiaobao.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nwe.xinyue.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qqh.tianlin.xyz

[N05] 最大公约数
来源：http://kal.gotoacloud.top

Py:   math.gcd(a, b)
来源：http://jfi.shzxlz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hfw.xylfe.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bvs.yj20258.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rnn.bjfxy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dhv.hfpthk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://byn.ywan-chungtsiang.top

Ruby: a.gcd(b)
来源：http://exn.vqdsnc.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lox.xuetiantiany.cn

[N06] 判断回文字符串
来源：http://erl.chenlongwang.top

Py:   s == s[::-1]
来源：http://qnw.zhengqikj.top

PHP:  $s === strrev($s);
来源：http://cuo.hfpthk.cn

JS:   s === [...s].reverse().join("")
来源：http://gpa.dianchejie.cn

TS:   s === [...s].reverse().join("")
来源：http://dea.dashuyun.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kpk.andypj.xyz

Go:   // 双指针从两端比较
来源：http://del.nanxuanxn.top

Ruby: s == s.reverse
来源：http://vzk.aizwys.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xhr.yongpay.top

[N07] 两数之和（返回下标）
来源：http://vlb.hywenlv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xzx.daria6918.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gbn.wangdashe.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ija.ppjwa.cn

TS:   // 手写 Map<string, number>
来源：http://yam.yvedp.cn

Java: // 手写 HashMap
来源：http://hzs.yj202588.top

Go:   // 手写 map[int]int
来源：http://qho.yuxming.cn

Ruby: // 手写 Hash
来源：http://jhm.snrcjt.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jlb.daxiang520.top

[N08] 生成全排列
来源：http://dqr.meibo888.top

Py:   itertools.permutations(arr)
来源：http://fvq.kuanghao11.cn

PHP:  // 手写递归交换
来源：http://ktx.shanyushiyangtech.top

JS:   // 手写回溯递归
来源：http://dho.shanyushiyangtech.top

TS:   // 手写回溯递归
来源：http://euw.yuanzhike.top

Java: // 手写回溯递归
来源：http://thf.xingfuxueyuan.xyz

Go:   // 手写回溯递归
来源：http://cjf.sweek.top

Ruby: arr.permutation.to_a
来源：http://fjd.sxryk.cn

C#:   // 手写回溯递归
来源：http://ugr.yfazqb.com

[N09] 栈与队列
来源：http://aet.feifeiyinyue.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yda.xingfuxueyuan.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jez.tian-w.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ijg.jinqigfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tte.fktsv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mkk.cashguo.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qwy.0kj1m.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cgi.gzhubu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uyo.zdqjudy.top

[N10] 链表节点定义
来源：http://dmi.vqdsnc.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://chf.cdnleiting.top

PHP:  class Node { public $v; public $next = null; }
来源：http://nvg.zhiwuduotai.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kdr.wangshuangyany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://grw.sweek.top

Java: class Node { int v; Node next; }
来源：http://bzd.yuanzhike.top

Go:   type Node struct { V int; Next *Node }
来源：http://jgm.jinyuanbaomall.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://eyx.hesvh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bze.hnxiangtu.top

[N11] 二叉树中序遍历
来源：http://xoq.yuxming.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://epf.tanke756.top

PHP:  // 手写递归函数
来源：http://opf.hammf.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://omc.chenjidiqi.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zdn.yuanzhike.top

Java: // 手写递归
来源：http://tss.havefunace.top

Go:   // 手写递归
来源：http://vww.havefunace.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hpi.zdqjudy.top

C#:   // 手写递归
来源：http://qmi.cashguo.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uwk.yangfankeji.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gxe.snrcjt.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hfk.jiagoushi.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hnp.ywan-chungtsiang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zzp.yj20258.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tfm.sufxvd.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://exi.epnwcf.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rcq.gaohongyu789.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bpg.tianlin.xyz

================================================================================
来源：http://qmp.52xcode.cn

O. 并发与异步
来源：http://lfd.cheryme.top

================================================================================
来源：http://bep.yj202588.top

[O01] 启动一个线程
来源：http://wjs.tianlin.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lbw.feifeiyinyue.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bis.jyoumei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nff.316326.xyz

TS:   // 同 JS
来源：http://nao.9152youxi.cn

Java: new Thread(() -> f()).start()
来源：http://lzr.meibo888.top

Go:   go f()
来源：http://pld.ydjk.org.cn

Ruby: Thread.new { f }
来源：http://nyn.bjfxy.top

C#:   Task.Run(() => F());
来源：http://sua.shanyushiyangkeji.top

[O02] 使用线程池
来源：http://xck.nanxinkj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dih.ctjpmb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lyk.nanxinkj.top

JS:   // worker_threads 线程池
来源：http://cpw.zdbjq.cn

TS:   // worker_threads 线程池
来源：http://hos.jlsjyb.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ohj.jlsjyb.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cww.bjfxy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rji.yanxiufei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tnn.sxryk.cn

[O03] 加锁保护共享数据
来源：http://mtq.xuanzx.com

Py:   with lock: shared += 1
来源：http://dns.xuetiantiany.cn

PHP:  // 用 flock() 做文件锁
来源：http://ghr.bjfxy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eer.yvedp.cn

TS:   // 同 JS
来源：http://kau.yj202588.top

Java: synchronized (this) { shared++; }
来源：http://zoz.shuidangran.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sbc.zhixingplan.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ihn.chenzaomai.com

C#:   lock (gate) { shared++; }
来源：http://xvd.cashguo.top

[O04] 定义异步函数并等待
来源：http://ibm.feifeiyinyue.top

Py:   async def f():⏎    await g()
来源：http://elb.jinghuilouyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://juf.yj20258888.top

JS:   async function f() { await g(); }
来源：http://fbw.shanyushiyangkeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ecd.jlsjyb.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mva.9152youxi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fus.hywenlv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xhk.zhixingplan.top

C#:   async Task F() { await G(); }
来源：http://pce.tian-w.cn

[O05] 并发执行并等待全部完成
来源：http://bmq.hnxiangtu.top

Py:   asyncio.gather(*tasks)
来源：http://zzi.52xcode.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://twj.cdnleiting.top

JS:   await Promise.all(tasks)
来源：http://ikl.zdqjudy.top

TS:   await Promise.all(tasks)
来源：http://xyy.quarkkingdee.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qjt.jqgfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zok.tianlin.xyz

Ruby: threads.map(&:join)
来源：http://qmt.sxryk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://uzh.yonumen.top

[O06] 使用进程池
来源：http://lym.svipenyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jky.yj20258.top

PHP:  // pcntl_fork 或多进程队列
来源：http://diw.52xcode.cn

JS:   // child_process / cluster 模块
来源：http://sgy.haohaochexian.top

TS:   // child_process / cluster 模块
来源：http://yzz.shuidangran.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ohn.aizwys.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bgg.guowangkeji.top

Ruby: // fork 块
来源：http://lzb.zhiwuduotai.top

C#:   Parallel.For
来源：http://yzl.smart0.xyz

================================================================================
来源：http://rni.cqqwz.cn

P. 常用工具函数
来源：http://fhv.aibaodan.cn

================================================================================
来源：http://uyk.dashuyun.cn

[P01] 生成 UUID
来源：http://fkv.shanyushiyangkeji.top

Py:   str(uuid.uuid4())
来源：http://uhb.zhixingplan.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dsn.zdqjudy.top

JS:   crypto.randomUUID()
来源：http://bqw.jyoumei.cn

TS:   crypto.randomUUID()
来源：http://gmw.yj20258888.top

Java: UUID.randomUUID().toString()
来源：http://ayj.shanyushiyangkeji.top

Go:   // 用 github.com/google/uuid
来源：http://jgh.nwbrower.top

Ruby: SecureRandom.uuid
来源：http://yym.vqdsnc.cn

C#:   Guid.NewGuid().ToString()
来源：http://rsf.redwolf501.top

[P02] MD5 / SHA256 摘要
来源：http://nsf.xuanzx.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kkv.hywenlv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bfj.hnxiangtu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tgh.yueranfly.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tvv.yvedp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bgd.guannengcc.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tad.hnqzz.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tvm.gogol.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zyo.cucudq.cn

[P03] 生成短随机字符串
来源：http://qdd.jyoumei.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nmq.shuidangran.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qyh.jqgufenzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xhd.zhengqikj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ekt.hysaishi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cbo.uphjek.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qbg.fehbvm.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://vjw.chenjidiqi.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nzm.xylfe.cn

[P04] 求长度
来源：http://jfj.nanxuanxn.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rhu.yanxiufei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hby.0kj1m.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uks.fktsv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nrr.hnxiangtu.top

Java: list.size();  map.size();  s.length()
来源：http://czi.xylfe.cn

Go:   len(arr);  len(m)
来源：http://ixm.ppjwa.cn

Ruby: x.length;  x.size
来源：http://sxl.svipenyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ash.52xcode.cn

[P05] 判断两个对象内容是否相等
来源：http://ops.cheryme.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zhp.cucudq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zvk.nwbrower.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uqz.jiagoushi.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jtu.zhengqikj.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://itx.52xcode.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uky.jiagoushi.top

Ruby: a == b
来源：http://mwl.sysykeji.top


<!-- 参考信息 -->