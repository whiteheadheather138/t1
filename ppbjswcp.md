代发 wailian999

TS:   resp.ok;  resp.status
来源：http://eky.shanyushiyangtech.top

Java: resp.statusCode()
来源：http://mwu.chenzaomai.com

Go:   resp.StatusCode
来源：http://hib.cheryme.top

Ruby: resp.code.to_i
来源：http://xdj.yuanzhike.top

C#:   (int)resp.StatusCode
来源：http://oxe.sufxvd.cn

[L08] 并发请求多个地址
来源：http://diu.zhijiandao.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nya.nanxuanxn.top

PHP:  curl_multi_init() 系列
来源：http://jik.smart0.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kvw.gzhubu.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iwd.meibo888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iit.hammf.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://knk.ppjwa.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sws.aizwys.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://swp.yuxming.cn

================================================================================
来源：http://sqa.jianghu66.top

M. 命令行 / 进程 / 环境
来源：http://rma.gogol.net.cn

================================================================================
来源：http://wyv.tian-w.cn

[M01] 读取命令行参数
来源：http://zld.hesvh.cn

Py:   sys.argv[1:]
来源：http://grm.tian-w.cn

PHP:  $argv;  $argc;
来源：http://hia.yueranfly.top

JS:   process.argv.slice(2)
来源：http://nic.zdqjudy.top

TS:   process.argv.slice(2)
来源：http://ilp.jianghu66.top

Java: args 数组（main 方法参数）
来源：http://vno.chenlongwang.top

Go:   os.Args[1:]
来源：http://yip.shangyingyoupin.top

Ruby: ARGV
来源：http://eov.jqgfzy.top

C#:   args 数组（Main 方法参数）
来源：http://fsq.wangshuangyany.cn

[M02] 读取环境变量
来源：http://uip.jyoumei.cn

Py:   os.environ.get("HOME")
来源：http://lcw.zhijiandao.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://itg.guowangkeji.top

JS:   process.env.HOME
来源：http://msq.yuxming.cn

TS:   process.env.HOME
来源：http://qqb.ybcxt.top

Java: System.getenv("HOME")
来源：http://jlf.shuidangran.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ixv.cdnleiting.top

Ruby: ENV["HOME"]
来源：http://ufk.nanxinkj.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rcs.hammf.cn

[M03] 执行外部命令
来源：http://zhx.yongpay.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hyn.xingfuxueyuan.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mby.hnxiangtu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vky.ivvv.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zwb.kuanghao11.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gdz.hcnkem.com

Go:   exec.Command("ls", "-l").Output()
来源：http://abn.tian-w.cn

Ruby: system("ls -l");  `ls -l`
来源：http://lge.0kj1m.cn

C#:   Process.Start("ls", "-l");
来源：http://swg.wangdashe.top

[M04] 获取当前工作目录
来源：http://igv.nanxinkj.top

Py:   os.getcwd()
来源：http://flc.ppjwa.cn

PHP:  getcwd();
来源：http://zkn.yj20258888.top

JS:   process.cwd()
来源：http://ojg.iojbl.cn

TS:   process.cwd()
来源：http://ndj.xinyue.icu

Java: Path.of("").toAbsolutePath()
来源：http://ujl.bjfxy.top

Go:   os.Getwd()
来源：http://gkm.yangfankeji.com

Ruby: Dir.pwd
来源：http://imj.ywan-chungtsiang.top

C#:   Directory.GetCurrentDirectory()
来源：http://hwy.sysykeji.top

[M05] 设置退出码
来源：http://pia.xinyue.icu

Py:   sys.exit(1)
来源：http://xkg.zhongyouzk.top

PHP:  exit(1);
来源：http://vav.wangshuangyany.cn

JS:   process.exit(1)
来源：http://wlm.wangshuangyany.cn

TS:   process.exit(1)
来源：http://qqp.ivvv.top

Java: System.exit(1)
来源：http://quq.jinqigfzy.top

Go:   os.Exit(1)
来源：http://jrh.sweek.top

Ruby: exit 1
来源：http://heg.jiagoushi.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://goa.zhixingplan.top

[M06] 向标准错误输出
来源：http://wfe.shzxlz.cn

Py:   print("err", file=sys.stderr)
来源：http://gzr.jyoumei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mjc.haohaochexian.top

JS:   console.error("err")
来源：http://vqc.gogol.net.cn

TS:   console.error("err")
来源：http://pyg.xuetiantiany.cn

Java: System.err.println("err")
来源：http://wbx.uphjek.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xwk.sjlbkw.cn

Ruby: warn "err"
来源：http://yfv.gaohongyu789.top

C#:   Console.Error.WriteLine("err")
来源：http://off.sufxvd.cn

[M07] 判断是否为主入口
来源：http://rdj.fengsongda.top

Py:   if __name__ == "__main__":
来源：http://opn.jqgfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yor.xinyue.icu

JS:   require.main === module
来源：http://vji.hnxiangtu.top

TS:   require.main === module
来源：http://jjr.fanxiaobao.xyz

Java: public static void main(String[] args)
来源：http://cty.ydjk.org.cn

Go:   func main()
来源：http://exu.yfazqb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://usx.jiagoushi.top

C#:   static void Main(string[] args)
来源：http://rbm.sysykeji.top

[M08] 获取系统与运行时信息
来源：http://ncv.redwolf501.top

Py:   platform.system();  platform.python_version()
来源：http://tca.yongpay.top

PHP:  PHP_OS;  phpversion();
来源：http://wfo.ybcxt.top

JS:   process.platform;  process.version
来源：http://qqi.kuanghao11.cn

TS:   process.platform;  process.version
来源：http://rza.fengsongda.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nyv.sweek.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zfn.xuetiantiany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rra.xinyue.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://sut.yuxming.cn

================================================================================
来源：http://sgh.fktsv.cn

N. 数据结构与算法
来源：http://qqa.yj20258888.top

================================================================================
来源：http://yxa.hfpthk.cn

[N01] 二分查找（有序数组）
来源：http://cey.wangdashe.top

Py:   bisect.bisect_left(arr, x)
来源：http://xop.zhiwuduotai.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bjx.yuxming.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uio.snrcjt.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yrs.chenjidiqi.icu

Java: Arrays.binarySearch(arr, x)
来源：http://oos.wangdashe.top

Go:   sort.SearchInts(arr, x)
来源：http://mar.havefunace.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lrc.jiagoushi.top

C#:   Array.BinarySearch(arr, x)
来源：http://iyz.shuidangran.top

[N02] 排序（工程实践用内置实现）
来源：http://kgo.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://vmo.jinqigufen.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jve.jlsjyb.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://egm.zhengqikj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kaj.yfazqb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nhf.pycfn.com

Go:   slices.Sort(arr)
来源：http://uia.hysaishi.cn

Ruby: arr.sort
来源：http://xxe.zdqjudy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://avb.tanke756.top

[N03] 快速排序（分治示例）
来源：http://nwr.xylfe.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://uwf.sufxvd.cn

PHP:  // 递归实现，或用 usort
来源：http://stu.jinqigfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ssf.xuetiantiany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mgb.jiagoushi.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pay.zdbjq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sew.shuidangran.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://spq.feifeiyinyue.top

C#:   // 手写递归，或 Array.Sort
来源：http://gpy.pycfn.com

[N04] 斐波那契数列
来源：http://bpa.tianlin.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uwy.iojbl.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rni.vehdjk.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sli.daria6918.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bpa.yuanzhike.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ppo.kuanghao11.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rqi.cqqwz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lez.xinyue.icu

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://aix.bjfxy.top

[N05] 最大公约数
来源：http://sij.pycfn.com

Py:   math.gcd(a, b)
来源：http://nyk.xuanzx.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yhr.shanyushiyangtech.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xub.yj202588.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rro.dianchejie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ckl.xinyue.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xpo.snrcjt.cn

Ruby: a.gcd(b)
来源：http://ppo.jinqigufen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ctl.vqdsnc.cn

[N06] 判断回文字符串
来源：http://ivi.quarkkingdee.top

Py:   s == s[::-1]
来源：http://zof.chenjidiqi.icu

PHP:  $s === strrev($s);
来源：http://wdn.zhongyouzk.top

JS:   s === [...s].reverse().join("")
来源：http://unz.smart0.xyz

TS:   s === [...s].reverse().join("")
来源：http://vrb.haohaochexian.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uii.ivvv.top

Go:   // 双指针从两端比较
来源：http://gml.9152youxi.cn

Ruby: s == s.reverse
来源：http://vkx.jinqigufen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jof.ctjpmb.com

[N07] 两数之和（返回下标）
来源：http://dlp.jinqigufen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mdj.shanyushiyangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://byq.jyoumei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://sbq.yonumen.top

TS:   // 手写 Map<string, number>
来源：http://hbw.yueranfly.top

Java: // 手写 HashMap
来源：http://fvl.c1oappe.top

Go:   // 手写 map[int]int
来源：http://jbk.zhiwuduotai.top

Ruby: // 手写 Hash
来源：http://mgc.cdnleiting.top

C#:   // 手写 Dictionary<int, int>
来源：http://qxb.zhengqikj.top

[N08] 生成全排列
来源：http://uvy.jinyuanbaomall.cn

Py:   itertools.permutations(arr)
来源：http://vsq.xingfuxueyuan.xyz

PHP:  // 手写递归交换
来源：http://you.pycfn.com

JS:   // 手写回溯递归
来源：http://cjh.zycfv.cn

TS:   // 手写回溯递归
来源：http://gky.redwolf501.top

Java: // 手写回溯递归
来源：http://qny.jinqigufen.top

Go:   // 手写回溯递归
来源：http://opl.zdqjudy.top

Ruby: arr.permutation.to_a
来源：http://vvq.hywenlv.cn

C#:   // 手写回溯递归
来源：http://rso.fzhhl.top

[N09] 栈与队列
来源：http://doo.hesvh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hqv.yj202588.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tdc.hesvh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ree.yuxming.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xda.xingfuxueyuan.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kot.fengsongda.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qfu.tarul.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qst.aizwys.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ekw.cashguo.top

[N10] 链表节点定义
来源：http://srw.316326.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rja.epnwcf.com

PHP:  class Node { public $v; public $next = null; }
来源：http://lbk.dashuyun.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qoc.ydjk.org.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pwo.tarul.cn

Java: class Node { int v; Node next; }
来源：http://ltl.vqdsnc.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tbl.jyoumei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bcu.aibaodan.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uuh.bbcook.cn

[N11] 二叉树中序遍历
来源：http://srg.zycfv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vks.ybcxt.top

PHP:  // 手写递归函数
来源：http://ppd.fanxiaobao.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://frt.kuanghao11.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://phy.zhaomingkeji.xyz

Java: // 手写递归
来源：http://gxq.hcnkem.com

Go:   // 手写递归
来源：http://xyt.hnxiangtu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hbr.yj20258.top

C#:   // 手写递归
来源：http://atq.yj20258.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eqe.jqgufenzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mwk.nwbrower.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nrh.9152youxi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ond.zhongyouzk.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qhb.tianlin.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://waq.yonumen.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oat.gogol.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://upy.hfpthk.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://aod.sysykeji.top

================================================================================
来源：http://kgs.nwbrower.top

O. 并发与异步
来源：http://dpd.xuetiantiany.cn

================================================================================
来源：http://rlc.yueranfly.top

[O01] 启动一个线程
来源：http://ofq.meibo888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gjc.gotoacloud.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uud.chenjidiqi.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gab.bbcook.cn

TS:   // 同 JS
来源：http://qip.ydzc1.top

Java: new Thread(() -> f()).start()
来源：http://mgu.chenlongwang.top

Go:   go f()
来源：http://sjm.epnwcf.com

Ruby: Thread.new { f }
来源：http://bta.yanxiufei.cn

C#:   Task.Run(() => F());
来源：http://qhj.hfpthk.cn

[O02] 使用线程池
来源：http://yjp.zycfv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gxe.jlsjyb.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ynx.pycfn.com

JS:   // worker_threads 线程池
来源：http://iqz.hongshengwenyu.top

TS:   // worker_threads 线程池
来源：http://gkd.ivvv.top

Java: Executors.newFixedThreadPool(4)
来源：http://deo.jinqigufen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://stj.yuanzhike.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wpg.hysaishi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nyf.kuanghao11.cn

[O03] 加锁保护共享数据
来源：http://qco.wangshuangyany.cn

Py:   with lock: shared += 1
来源：http://ism.aibaodan.cn

PHP:  // 用 flock() 做文件锁
来源：http://tqa.tarul.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xks.quarkkingdee.top

TS:   // 同 JS
来源：http://pus.ehwqpu.com

Java: synchronized (this) { shared++; }
来源：http://zzn.meibo888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dqj.fzhhl.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://mso.uphjek.com

C#:   lock (gate) { shared++; }
来源：http://nfn.dianchejie.cn

[O04] 定义异步函数并等待
来源：http://zpo.jqgfzy.top

Py:   async def f():⏎    await g()
来源：http://loi.hfpthk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vmg.9152youxi.cn

JS:   async function f() { await g(); }
来源：http://qyg.chenlongwang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jpy.smart0.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rae.ydzc1.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yan.sxryk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tox.ehwqpu.com

C#:   async Task F() { await G(); }
来源：http://yvr.kuanghao11.cn

[O05] 并发执行并等待全部完成
来源：http://jdv.haohaochexian.top

Py:   asyncio.gather(*tasks)
来源：http://olz.sjlbkw.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://brz.zycfv.cn

JS:   await Promise.all(tasks)
来源：http://nqw.cqqwz.cn

TS:   await Promise.all(tasks)
来源：http://jeu.hesvh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bpp.pycfn.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qru.jinqigufen.top

Ruby: threads.map(&:join)
来源：http://url.dashuyun.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rsd.jinghuilouyu.cn

[O06] 使用进程池
来源：http://ewc.zdbjq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://skg.52xcode.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qvw.xylfe.cn

JS:   // child_process / cluster 模块
来源：http://dlx.bbcook.cn

TS:   // child_process / cluster 模块
来源：http://efg.nanxinkj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gze.vehdjk.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qdb.ybcxt.top

Ruby: // fork 块
来源：http://bew.sysykeji.top

C#:   Parallel.For
来源：http://zul.quarkkingdee.top

================================================================================
来源：http://fja.ywan-chungtsiang.top

P. 常用工具函数
来源：http://afp.yangfankeji.com

================================================================================
来源：http://mtj.sjlbkw.cn

[P01] 生成 UUID
来源：http://skh.yuxming.cn

Py:   str(uuid.uuid4())
来源：http://gtv.ctjpmb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jal.andypj.xyz

JS:   crypto.randomUUID()
来源：http://ckp.birdmap.top

TS:   crypto.randomUUID()
来源：http://zoc.yvedp.cn

Java: UUID.randomUUID().toString()
来源：http://svg.yj20258888.top

Go:   // 用 github.com/google/uuid
来源：http://cri.cheryme.top

Ruby: SecureRandom.uuid
来源：http://swq.meibo888.top

C#:   Guid.NewGuid().ToString()
来源：http://zbm.sweek.top

[P02] MD5 / SHA256 摘要
来源：http://kup.jqgfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tsn.yonumen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jkv.c1oappe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ecc.zycfv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fcj.tarul.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ajn.sjlbkw.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lfg.zhixingplan.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://epf.smart0.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bkp.jqgufenzy.top

[P03] 生成短随机字符串
来源：http://xwj.fengsongda.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hik.sysykeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mdo.sysykeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dyj.52xcode.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lgb.yvedp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xrn.ppjwa.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nta.yonumen.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wnj.fktsv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://scb.sxryk.cn

[P04] 求长度
来源：http://nbg.gogol.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dle.nwbrower.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://svd.mhx1999.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dxf.hysaishi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wva.pengpengdd.cyou

Java: list.size();  map.size();  s.length()
来源：http://pgb.dianchejie.cn

Go:   len(arr);  len(m)
来源：http://gjg.svipenyu.cn

Ruby: x.length;  x.size
来源：http://zhk.yanxiufei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bdh.hesvh.cn

[P05] 判断两个对象内容是否相等
来源：http://ldt.gotoacloud.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rqo.cheryme.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kgp.zhaomingkeji.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lni.jinyuanbaomall.cn


<!-- 参考信息 -->