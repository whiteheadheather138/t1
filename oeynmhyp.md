代发 wailian999

TS:   resp.ok;  resp.status
来源：http://eyf.haohaochexian.top

Java: resp.statusCode()
来源：http://klp.yueranfly.top

Go:   resp.StatusCode
来源：http://boj.jinqigufen.top

Ruby: resp.code.to_i
来源：http://mjt.cucudq.cn

C#:   (int)resp.StatusCode
来源：http://sgi.shzxlz.cn

[L08] 并发请求多个地址
来源：http://utu.yonumen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hyx.hongshengwenyu.top

PHP:  curl_multi_init() 系列
来源：http://krw.fanxiaobao.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fsn.xuanzx.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fek.andypj.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kpu.zhengqikj.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yrh.yj202588.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://eox.kuanghao11.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yyn.yj20258888.top

================================================================================
来源：http://yvw.xziqi.cn

M. 命令行 / 进程 / 环境
来源：http://inq.zhongyouzk.top

================================================================================
来源：http://hhb.fzhhl.top

[M01] 读取命令行参数
来源：http://jll.ybcxt.top

Py:   sys.argv[1:]
来源：http://jlk.jqgufenzy.top

PHP:  $argv;  $argc;
来源：http://sel.gaohongyu789.top

JS:   process.argv.slice(2)
来源：http://vwc.zdbjq.cn

TS:   process.argv.slice(2)
来源：http://ksx.dashuyun.cn

Java: args 数组（main 方法参数）
来源：http://lmb.zhixingplan.top

Go:   os.Args[1:]
来源：http://edp.wangdashe.top

Ruby: ARGV
来源：http://mop.vehdjk.com

C#:   args 数组（Main 方法参数）
来源：http://klc.jlsjyb.cn

[M02] 读取环境变量
来源：http://htf.yonumen.top

Py:   os.environ.get("HOME")
来源：http://ezc.guowangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hzi.tanke756.top

JS:   process.env.HOME
来源：http://fdz.birdmap.top

TS:   process.env.HOME
来源：http://zpf.svipenyu.cn

Java: System.getenv("HOME")
来源：http://nnw.0kj1m.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bhq.dashuyun.cn

Ruby: ENV["HOME"]
来源：http://zse.ppjwa.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ekj.jinqigufen.top

[M03] 执行外部命令
来源：http://ing.fengsongda.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zah.yj20258.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://oxk.snrcjt.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bai.jiagoushi.top

TS:   child_process.execSync("ls -l").toString()
来源：http://euu.chenzaomai.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vgk.hysaishi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ukn.ivvv.top

Ruby: system("ls -l");  `ls -l`
来源：http://zco.bjfxy.top

C#:   Process.Start("ls", "-l");
来源：http://rqd.dianchejie.cn

[M04] 获取当前工作目录
来源：http://eyn.snrcjt.cn

Py:   os.getcwd()
来源：http://jrs.ivvv.top

PHP:  getcwd();
来源：http://ash.fanxiaobao.xyz

JS:   process.cwd()
来源：http://pkl.kuanghao11.cn

TS:   process.cwd()
来源：http://eoy.tanke756.top

Java: Path.of("").toAbsolutePath()
来源：http://hus.hfpthk.cn

Go:   os.Getwd()
来源：http://kho.fengsongda.top

Ruby: Dir.pwd
来源：http://iso.wangshuangyany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xyg.cdnleiting.top

[M05] 设置退出码
来源：http://ajc.cucudq.cn

Py:   sys.exit(1)
来源：http://yij.ydzc1.top

PHP:  exit(1);
来源：http://zuw.yvedp.cn

JS:   process.exit(1)
来源：http://bqe.guannengcc.top

TS:   process.exit(1)
来源：http://itm.svipenyu.cn

Java: System.exit(1)
来源：http://xic.xinyue.icu

Go:   os.Exit(1)
来源：http://qlo.zhaomingkeji.xyz

Ruby: exit 1
来源：http://bdy.sweek.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uhs.meibo888.top

[M06] 向标准错误输出
来源：http://joz.jqgufenzy.top

Py:   print("err", file=sys.stderr)
来源：http://jzq.xylfe.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qdm.shanyushiyangkeji.top

JS:   console.error("err")
来源：http://vmo.ctjpmb.com

TS:   console.error("err")
来源：http://ngy.ydzc1.top

Java: System.err.println("err")
来源：http://ltm.hysaishi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eyk.jyoumei.cn

Ruby: warn "err"
来源：http://jtv.nanxinkj.top

C#:   Console.Error.WriteLine("err")
来源：http://qoi.yfazqb.com

[M07] 判断是否为主入口
来源：http://wyq.haohaochexian.top

Py:   if __name__ == "__main__":
来源：http://kxi.birdmap.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fsh.birdmap.top

JS:   require.main === module
来源：http://hal.snrcjt.cn

TS:   require.main === module
来源：http://wqj.tanke756.top

Java: public static void main(String[] args)
来源：http://btt.chenzaomai.com

Go:   func main()
来源：http://gmj.hesvh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qmm.epnwcf.com

C#:   static void Main(string[] args)
来源：http://anw.yfazqb.com

[M08] 获取系统与运行时信息
来源：http://cuc.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://qcn.ywan-chungtsiang.top

PHP:  PHP_OS;  phpversion();
来源：http://qci.dianchejie.cn

JS:   process.platform;  process.version
来源：http://rvd.meibo888.top

TS:   process.platform;  process.version
来源：http://evq.ywan-chungtsiang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sft.pengpengdd.cyou

Go:   runtime.GOOS;  runtime.Version()
来源：http://nra.wangshuangyany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vso.ctjpmb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://sne.yangfankeji.com

================================================================================
来源：http://hef.zhiwuduotai.top

N. 数据结构与算法
来源：http://kma.zhaomingkeji.xyz

================================================================================
来源：http://zwt.ybcxt.top

[N01] 二分查找（有序数组）
来源：http://sip.dashuyun.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fiu.shangyingyoupin.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wdl.0kj1m.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rpd.ydzc1.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pwv.fengsongda.top

Java: Arrays.binarySearch(arr, x)
来源：http://ban.svipenyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://qkk.fanxiaobao.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://pfk.zhiwuduotai.top

C#:   Array.BinarySearch(arr, x)
来源：http://lgc.c1oappe.top

[N02] 排序（工程实践用内置实现）
来源：http://nuc.zdqjudy.top

Py:   sorted(arr);  arr.sort()
来源：http://tlg.xziqi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yjk.kuanghao11.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tdi.pengpengdd.cyou

TS:   [...arr].sort((a, b) => a - b)
来源：http://fuq.dianchejie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hkf.kuanghao11.cn

Go:   slices.Sort(arr)
来源：http://pio.fengsongda.top

Ruby: arr.sort
来源：http://egz.vehdjk.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://ffo.tanke756.top

[N03] 快速排序（分治示例）
来源：http://qvy.vehdjk.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ukh.chenlongwang.top

PHP:  // 递归实现，或用 usort
来源：http://yzm.jiagoushi.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rtf.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sqs.snrcjt.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hrd.havefunace.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fvu.yj20258.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gqa.haohaochexian.top

C#:   // 手写递归，或 Array.Sort
来源：http://scy.zycfv.cn

[N04] 斐波那契数列
来源：http://xxy.hongshengwenyu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jqo.gotoacloud.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rji.xingfuxueyuan.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ieu.tianlin.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yfh.cucudq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qsh.jlsjyb.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://san.hongshengwenyu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tud.hysaishi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fxy.hfpthk.cn

[N05] 最大公约数
来源：http://lmy.jqgfzy.top

Py:   math.gcd(a, b)
来源：http://sza.nwbrower.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aoc.sysykeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ezv.yfazqb.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://smi.sjlbkw.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vnt.52xcode.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://chc.tarul.cn

Ruby: a.gcd(b)
来源：http://rub.yangfankeji.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yyb.nanxuanxn.top

[N06] 判断回文字符串
来源：http://key.tarul.cn

Py:   s == s[::-1]
来源：http://jcp.bbcook.cn

PHP:  $s === strrev($s);
来源：http://ezq.hnxiangtu.top

JS:   s === [...s].reverse().join("")
来源：http://ogy.hnqzz.top

TS:   s === [...s].reverse().join("")
来源：http://wpd.ywan-chungtsiang.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bkr.wangdashe.top

Go:   // 双指针从两端比较
来源：http://gwk.hesvh.cn

Ruby: s == s.reverse
来源：http://drt.epnwcf.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://pqd.guannengcc.top

[N07] 两数之和（返回下标）
来源：http://mqt.snrcjt.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zzm.zhixingplan.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://etf.xinyue.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://zwp.jyoumei.cn

TS:   // 手写 Map<string, number>
来源：http://quk.wangdashe.top

Java: // 手写 HashMap
来源：http://jqc.9152youxi.cn

Go:   // 手写 map[int]int
来源：http://azd.hfpthk.cn

Ruby: // 手写 Hash
来源：http://oqg.kuanghao11.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gpk.jinqigfzy.top

[N08] 生成全排列
来源：http://dvs.fanxiaobao.xyz

Py:   itertools.permutations(arr)
来源：http://kmr.andypj.xyz

PHP:  // 手写递归交换
来源：http://bbn.jinqigufen.top

JS:   // 手写回溯递归
来源：http://rku.jinqigfzy.top

TS:   // 手写回溯递归
来源：http://gjr.hesvh.cn

Java: // 手写回溯递归
来源：http://mjz.hysaishi.cn

Go:   // 手写回溯递归
来源：http://lnd.shanyushiyangkeji.top

Ruby: arr.permutation.to_a
来源：http://gaw.jlsjyb.cn

C#:   // 手写回溯递归
来源：http://jue.xuanzx.com

[N09] 栈与队列
来源：http://jgu.xinyue.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tth.cdnleiting.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://stj.zycfv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wao.xuanzx.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jix.shangyingyoupin.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ygg.vqdsnc.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eia.gaohongyu789.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://giu.jyoumei.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zru.aibaodan.cn

[N10] 链表节点定义
来源：http://ylw.ppjwa.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tay.bbcook.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mtr.sysykeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://yyj.fktsv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kvy.jiagoushi.top

Java: class Node { int v; Node next; }
来源：http://yvt.xinyue.icu

Go:   type Node struct { V int; Next *Node }
来源：http://oqn.vehdjk.com

Ruby: Node = Struct.new(:v, :next)
来源：http://uej.quarkkingdee.top

C#:   class Node { public int V; public Node? Next; }
来源：http://pyv.zhongyouzk.top

[N11] 二叉树中序遍历
来源：http://jmq.sxryk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aep.yuxming.cn

PHP:  // 手写递归函数
来源：http://aoe.sufxvd.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cmk.chenzaomai.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://thf.yangfankeji.com

Java: // 手写递归
来源：http://wpg.9152youxi.cn

Go:   // 手写递归
来源：http://ctd.aizwys.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pbx.feifeiyinyue.top

C#:   // 手写递归
来源：http://lft.hesvh.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wzu.zhijiandao.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nvw.hesvh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://snp.fengsongda.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zdt.jqgfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jjg.yj20258.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ohk.hongshengwenyu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yrl.zhijiandao.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hpp.cucudq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tzd.zhengqikj.top

================================================================================
来源：http://tms.yanxiufei.cn

O. 并发与异步
来源：http://amn.zhiwuduotai.top

================================================================================
来源：http://neq.haohaochexian.top

[O01] 启动一个线程
来源：http://wpm.hcnkem.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ugm.haohaochexian.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xqz.aibaodan.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hfw.hesvh.cn

TS:   // 同 JS
来源：http://iau.zhixingplan.top

Java: new Thread(() -> f()).start()
来源：http://gya.svipenyu.cn

Go:   go f()
来源：http://juz.aizwys.cn

Ruby: Thread.new { f }
来源：http://rza.nwbrower.top

C#:   Task.Run(() => F());
来源：http://vbt.zhoulong.xyz

[O02] 使用线程池
来源：http://gtm.jinqigfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hzw.andypj.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gph.fanxiaobao.xyz

JS:   // worker_threads 线程池
来源：http://ebp.sufxvd.cn

TS:   // worker_threads 线程池
来源：http://vvm.jianghu66.top

Java: Executors.newFixedThreadPool(4)
来源：http://krp.uphjek.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cmu.ctjpmb.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rxp.jinqigufen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ndc.tarul.cn

[O03] 加锁保护共享数据
来源：http://coj.yuxming.cn

Py:   with lock: shared += 1
来源：http://cuc.zdbjq.cn

PHP:  // 用 flock() 做文件锁
来源：http://kjp.ydzc1.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eay.ydzc1.top

TS:   // 同 JS
来源：http://idn.ctjpmb.com

Java: synchronized (this) { shared++; }
来源：http://dgz.ybcxt.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cwy.feifeiyinyue.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xzf.hcnkem.com

C#:   lock (gate) { shared++; }
来源：http://jdc.hywenlv.cn

[O04] 定义异步函数并等待
来源：http://hyn.hammf.cn

Py:   async def f():⏎    await g()
来源：http://ofh.haohaochexian.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dvv.yuxming.cn

JS:   async function f() { await g(); }
来源：http://vme.zhoulong.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://uji.9152youxi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qyz.daria6918.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jgs.yueranfly.top

Ruby: # 用 Fiber 或 async gem
来源：http://aax.tanke756.top

C#:   async Task F() { await G(); }
来源：http://njo.yueranfly.top

[O05] 并发执行并等待全部完成
来源：http://ppf.jinqigfzy.top

Py:   asyncio.gather(*tasks)
来源：http://ctc.chenzaomai.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tat.cqqwz.cn

JS:   await Promise.all(tasks)
来源：http://dwa.wangshuangyany.cn

TS:   await Promise.all(tasks)
来源：http://nci.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xkg.smart0.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kzi.guowangkeji.top

Ruby: threads.map(&:join)
来源：http://vcp.ppjwa.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sym.sysykeji.top

[O06] 使用进程池
来源：http://teq.wangshuangyany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ura.9152youxi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zwh.redwolf501.top

JS:   // child_process / cluster 模块
来源：http://xpj.zhaomingkeji.xyz

TS:   // child_process / cluster 模块
来源：http://fyl.xuanzx.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tpq.yongpay.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://aqc.zhoulong.xyz

Ruby: // fork 块
来源：http://ulm.yj20258.top

C#:   Parallel.For
来源：http://xur.dianchejie.cn

================================================================================
来源：http://hsa.jqgufenzy.top

P. 常用工具函数
来源：http://wby.hcnkem.com

================================================================================
来源：http://vnh.snrcjt.cn

[P01] 生成 UUID
来源：http://lpt.shangyingyoupin.top

Py:   str(uuid.uuid4())
来源：http://ktt.fengsongda.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uiy.hammf.cn

JS:   crypto.randomUUID()
来源：http://gym.uphjek.com

TS:   crypto.randomUUID()
来源：http://nom.yuanzhike.top

Java: UUID.randomUUID().toString()
来源：http://pml.vehdjk.com

Go:   // 用 github.com/google/uuid
来源：http://moe.feifeiyinyue.top

Ruby: SecureRandom.uuid
来源：http://bsq.cashguo.top

C#:   Guid.NewGuid().ToString()
来源：http://xbu.dashuyun.cn

[P02] MD5 / SHA256 摘要
来源：http://xbq.yj202588.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rhr.0kj1m.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jcq.chenjidiqi.icu

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://agw.cdnleiting.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wsq.ehwqpu.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vjn.nanxinkj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://czq.hywenlv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vyd.daxiang520.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tzh.yongpay.top

[P03] 生成短随机字符串
来源：http://hzo.xziqi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://eio.fehbvm.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wzq.daria6918.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ghe.quarkkingdee.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sbw.xuetiantiany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sum.epnwcf.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vax.xziqi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hvz.meibo888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fds.jinqigufen.top

[P04] 求长度
来源：http://ydn.zhoulong.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rqu.yonumen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wtf.vehdjk.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dui.yueranfly.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fvu.dianchejie.cn

Java: list.size();  map.size();  s.length()
来源：http://ulm.yvedp.cn

Go:   len(arr);  len(m)
来源：http://obk.yvedp.cn

Ruby: x.length;  x.size
来源：http://cyf.yvedp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hbb.iojbl.cn

[P05] 判断两个对象内容是否相等
来源：http://jwu.9152youxi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lyo.zhaomingkeji.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gaq.zycfv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kzn.chenjidiqi.icu


<!-- 参考信息 -->