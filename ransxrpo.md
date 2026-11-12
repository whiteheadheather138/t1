代发 wailian999

C#:   (int)resp.StatusCode
来源：http://elj.havefunace.top

[L08] 并发请求多个地址
来源：http://owt.yanxiufei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ico.jinqigufen.top

PHP:  curl_multi_init() 系列
来源：http://jse.yj202588.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://thp.cqqwz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://axy.redwolf501.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://auj.wangdashe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pkl.redwolf501.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://etr.meibo888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://upp.epnwcf.com

================================================================================
来源：http://zso.aizwys.cn

M. 命令行 / 进程 / 环境
来源：http://qxt.yj202588.top

================================================================================
来源：http://xxm.jianghu66.top

[M01] 读取命令行参数
来源：http://gob.cheryme.top

Py:   sys.argv[1:]
来源：http://xta.ehwqpu.com

PHP:  $argv;  $argc;
来源：http://qqt.svipenyu.cn

JS:   process.argv.slice(2)
来源：http://jmc.hammf.cn

TS:   process.argv.slice(2)
来源：http://wcj.jinqigfzy.top

Java: args 数组（main 方法参数）
来源：http://tiu.jinghuilouyu.cn

Go:   os.Args[1:]
来源：http://xgl.yangfankeji.com

Ruby: ARGV
来源：http://fpz.jianghu66.top

C#:   args 数组（Main 方法参数）
来源：http://yxz.wangshuangyany.cn

[M02] 读取环境变量
来源：http://qai.feifeiyinyue.top

Py:   os.environ.get("HOME")
来源：http://wow.svipenyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ufn.jianghu66.top

JS:   process.env.HOME
来源：http://qma.quarkkingdee.top

TS:   process.env.HOME
来源：http://nqd.tianlin.xyz

Java: System.getenv("HOME")
来源：http://qsm.ppjwa.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://orb.hfpthk.cn

Ruby: ENV["HOME"]
来源：http://ztf.hysaishi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kzw.ivvv.top

[M03] 执行外部命令
来源：http://pdn.cqqwz.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pkm.yj202588.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xik.shzxlz.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://unr.birdmap.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bbo.iojbl.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kvc.kuanghao11.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ywy.epnwcf.com

Ruby: system("ls -l");  `ls -l`
来源：http://ags.pengpengdd.cyou

C#:   Process.Start("ls", "-l");
来源：http://cny.316326.xyz

[M04] 获取当前工作目录
来源：http://uqz.tianlin.xyz

Py:   os.getcwd()
来源：http://epz.havefunace.top

PHP:  getcwd();
来源：http://oxv.smart0.xyz

JS:   process.cwd()
来源：http://yvm.yueranfly.top

TS:   process.cwd()
来源：http://xvu.pengpengdd.cyou

Java: Path.of("").toAbsolutePath()
来源：http://rle.iojbl.cn

Go:   os.Getwd()
来源：http://vav.pengpengdd.cyou

Ruby: Dir.pwd
来源：http://hdd.xuanzx.com

C#:   Directory.GetCurrentDirectory()
来源：http://jlr.dianchejie.cn

[M05] 设置退出码
来源：http://zpd.gotoacloud.top

Py:   sys.exit(1)
来源：http://qbq.dianchejie.cn

PHP:  exit(1);
来源：http://dvi.sjlbkw.cn

JS:   process.exit(1)
来源：http://pxf.gogol.net.cn

TS:   process.exit(1)
来源：http://fcm.gaohongyu789.top

Java: System.exit(1)
来源：http://brc.ydjk.org.cn

Go:   os.Exit(1)
来源：http://wwu.52xcode.cn

Ruby: exit 1
来源：http://dbn.xuanzx.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qle.vqdsnc.cn

[M06] 向标准错误输出
来源：http://zil.zycfv.cn

Py:   print("err", file=sys.stderr)
来源：http://ugn.uphjek.com

PHP:  fwrite(STDERR, "err\n");
来源：http://fzl.sufxvd.cn

JS:   console.error("err")
来源：http://ano.fehbvm.com

TS:   console.error("err")
来源：http://kdq.sweek.top

Java: System.err.println("err")
来源：http://den.yfazqb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yvn.ydzc1.top

Ruby: warn "err"
来源：http://eve.tian-w.cn

C#:   Console.Error.WriteLine("err")
来源：http://ziu.fzhhl.top

[M07] 判断是否为主入口
来源：http://aps.fanxiaobao.xyz

Py:   if __name__ == "__main__":
来源：http://rbl.nanxinkj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jxc.ywan-chungtsiang.top

JS:   require.main === module
来源：http://yuj.xuetiantiany.cn

TS:   require.main === module
来源：http://qdt.yj20258888.top

Java: public static void main(String[] args)
来源：http://lxj.jqgufenzy.top

Go:   func main()
来源：http://dbl.fanxiaobao.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uxj.nwbrower.top

C#:   static void Main(string[] args)
来源：http://zww.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://cns.52xcode.cn

Py:   platform.system();  platform.python_version()
来源：http://pjy.yvedp.cn

PHP:  PHP_OS;  phpversion();
来源：http://blz.tanke756.top

JS:   process.platform;  process.version
来源：http://jtb.fengsongda.top

TS:   process.platform;  process.version
来源：http://pgr.yangfankeji.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ivn.zhiwuduotai.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zbg.guowangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gpj.ehwqpu.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://jal.yangfankeji.com

================================================================================
来源：http://mqq.tianlin.xyz

N. 数据结构与算法
来源：http://qfu.guannengcc.top

================================================================================
来源：http://ydh.jqgfzy.top

[N01] 二分查找（有序数组）
来源：http://jkd.nanxuanxn.top

Py:   bisect.bisect_left(arr, x)
来源：http://nut.xinyue.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pez.wangdashe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fqc.fengsongda.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://obt.zhiwuduotai.top

Java: Arrays.binarySearch(arr, x)
来源：http://kct.jlsjyb.cn

Go:   sort.SearchInts(arr, x)
来源：http://pnq.zhongyouzk.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ema.yvedp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://akc.shanyushiyangtech.top

[N02] 排序（工程实践用内置实现）
来源：http://wka.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ksi.hesvh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bft.snrcjt.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://upg.smart0.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://alz.andypj.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hln.havefunace.top

Go:   slices.Sort(arr)
来源：http://tne.hongshengwenyu.top

Ruby: arr.sort
来源：http://xlt.0kj1m.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jpd.zhaomingkeji.xyz

[N03] 快速排序（分治示例）
来源：http://axe.andypj.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xhe.hnqzz.top

PHP:  // 递归实现，或用 usort
来源：http://gds.hnxiangtu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qmr.vqdsnc.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lro.gotoacloud.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ckq.316326.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tnq.yangfankeji.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yfn.yvedp.cn

C#:   // 手写递归，或 Array.Sort
来源：http://osq.guannengcc.top

[N04] 斐波那契数列
来源：http://vec.yonumen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pyt.hnqzz.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qhu.jqgfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cwe.xingfuxueyuan.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://epy.zdqjudy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jyl.hysaishi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nwt.jqgufenzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jey.birdmap.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yhz.fehbvm.com

[N05] 最大公约数
来源：http://jnm.52xcode.cn

Py:   math.gcd(a, b)
来源：http://pvd.feifeiyinyue.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dqs.dianchejie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mzz.ivvv.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qkp.chenzaomai.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vcf.jinqigufen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://thv.shanyushiyangtech.top

Ruby: a.gcd(b)
来源：http://vjg.yvedp.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ret.nanxuanxn.top

[N06] 判断回文字符串
来源：http://pyp.jinqigfzy.top

Py:   s == s[::-1]
来源：http://qmn.guowangkeji.top

PHP:  $s === strrev($s);
来源：http://sew.xuanzx.com

JS:   s === [...s].reverse().join("")
来源：http://rwq.316326.xyz

TS:   s === [...s].reverse().join("")
来源：http://hzm.daria6918.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://now.fehbvm.com

Go:   // 双指针从两端比较
来源：http://tup.jlsjyb.cn

Ruby: s == s.reverse
来源：http://oim.jinghuilouyu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qqg.316326.xyz

[N07] 两数之和（返回下标）
来源：http://mei.fktsv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wet.sxryk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tyw.jinqigufen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://okp.jiagoushi.top

TS:   // 手写 Map<string, number>
来源：http://deb.ctjpmb.com

Java: // 手写 HashMap
来源：http://xrt.xylfe.cn

Go:   // 手写 map[int]int
来源：http://iqf.dashuyun.cn

Ruby: // 手写 Hash
来源：http://mhk.yanxiufei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lbn.aizwys.cn

[N08] 生成全排列
来源：http://flk.jlsjyb.cn

Py:   itertools.permutations(arr)
来源：http://qiu.dianchejie.cn

PHP:  // 手写递归交换
来源：http://ygo.yanxiufei.cn

JS:   // 手写回溯递归
来源：http://nfd.yj202588.top

TS:   // 手写回溯递归
来源：http://iwe.chenjidiqi.icu

Java: // 手写回溯递归
来源：http://jck.zhongyouzk.top

Go:   // 手写回溯递归
来源：http://kcq.xuanzx.com

Ruby: arr.permutation.to_a
来源：http://yex.jqgufenzy.top

C#:   // 手写回溯递归
来源：http://ynj.zhiwuduotai.top

[N09] 栈与队列
来源：http://jqq.tanke756.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cig.feifeiyinyue.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ixz.zdqjudy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sdr.hnxiangtu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xiy.zycfv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://osm.xylfe.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rzg.nanxuanxn.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ult.cucudq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gnp.redwolf501.top

[N10] 链表节点定义
来源：http://zbh.jianghu66.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zez.zhiwuduotai.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ajy.shangyingyoupin.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jwe.redwolf501.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yxa.zycfv.cn

Java: class Node { int v; Node next; }
来源：http://mez.zhiwuduotai.top

Go:   type Node struct { V int; Next *Node }
来源：http://wwn.guannengcc.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zng.shanyushiyangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://yom.c1oappe.top

[N11] 二叉树中序遍历
来源：http://aqr.gzhubu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jem.c1oappe.top

PHP:  // 手写递归函数
来源：http://djj.hongshengwenyu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kkp.fengsongda.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qqn.redwolf501.top

Java: // 手写递归
来源：http://bwt.mhx1999.top

Go:   // 手写递归
来源：http://pax.sxryk.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://seq.fzhhl.top

C#:   // 手写递归
来源：http://ztr.xuanzx.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://itr.sysykeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://frn.shanyushiyangtech.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cld.vqdsnc.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jzz.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xec.aizwys.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://heh.andypj.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nod.havefunace.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ubw.jinqigufen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ywt.fktsv.cn

================================================================================
来源：http://kej.daxiang520.top

O. 并发与异步
来源：http://ebu.cqqwz.cn

================================================================================
来源：http://gee.svipenyu.cn

[O01] 启动一个线程
来源：http://gry.pycfn.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://stm.ehwqpu.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aeo.sufxvd.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cuv.ydjk.org.cn

TS:   // 同 JS
来源：http://tso.mhx1999.top

Java: new Thread(() -> f()).start()
来源：http://lrc.kuanghao11.cn

Go:   go f()
来源：http://piu.zhoulong.xyz

Ruby: Thread.new { f }
来源：http://xex.xuanzx.com

C#:   Task.Run(() => F());
来源：http://pse.chenjidiqi.icu

[O02] 使用线程池
来源：http://odl.shzxlz.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kkz.jiagoushi.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pek.smart0.xyz

JS:   // worker_threads 线程池
来源：http://mrj.0kj1m.cn

TS:   // worker_threads 线程池
来源：http://orx.0kj1m.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ken.shuidangran.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://twl.jinyuanbaomall.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mbs.vqdsnc.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ifq.kuanghao11.cn

[O03] 加锁保护共享数据
来源：http://efk.pengpengdd.cyou

Py:   with lock: shared += 1
来源：http://mht.jinghuilouyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://wvn.nwbrower.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mar.xuetiantiany.cn

TS:   // 同 JS
来源：http://gnw.guowangkeji.top

Java: synchronized (this) { shared++; }
来源：http://doa.tian-w.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uqw.yj20258.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wme.pengpengdd.cyou

C#:   lock (gate) { shared++; }
来源：http://ryp.ppjwa.cn

[O04] 定义异步函数并等待
来源：http://crw.vehdjk.com

Py:   async def f():⏎    await g()
来源：http://xpr.smart0.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lyl.guowangkeji.top

JS:   async function f() { await g(); }
来源：http://isu.tian-w.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mhm.havefunace.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://exs.shuidangran.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wql.c1oappe.top

Ruby: # 用 Fiber 或 async gem
来源：http://aqe.guowangkeji.top

C#:   async Task F() { await G(); }
来源：http://zvb.jinqigfzy.top

[O05] 并发执行并等待全部完成
来源：http://bhh.wangshuangyany.cn

Py:   asyncio.gather(*tasks)
来源：http://llb.svipenyu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wvn.bbcook.cn

JS:   await Promise.all(tasks)
来源：http://gnu.xingfuxueyuan.xyz

TS:   await Promise.all(tasks)
来源：http://bvs.gogol.net.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qtm.xinyue.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xnt.chenzaomai.com

Ruby: threads.map(&:join)
来源：http://lwv.pycfn.com

C#:   await Task.WhenAll(t1, t2)
来源：http://jyo.ivvv.top

[O06] 使用进程池
来源：http://ckk.haohaochexian.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lat.tarul.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://apu.hnxiangtu.top

JS:   // child_process / cluster 模块
来源：http://gia.9152youxi.cn

TS:   // child_process / cluster 模块
来源：http://tyk.kuanghao11.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://smv.tarul.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jsl.chenzaomai.com

Ruby: // fork 块
来源：http://ufb.hfpthk.cn

C#:   Parallel.For
来源：http://cpv.yfazqb.com

================================================================================
来源：http://oze.quarkkingdee.top

P. 常用工具函数
来源：http://tue.yuanzhike.top

================================================================================
来源：http://nus.hnqzz.top

[P01] 生成 UUID
来源：http://aht.snrcjt.cn

Py:   str(uuid.uuid4())
来源：http://pdg.gotoacloud.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sqs.pengpengdd.cyou

JS:   crypto.randomUUID()
来源：http://jze.shangyingyoupin.top

TS:   crypto.randomUUID()
来源：http://xhl.zdbjq.cn

Java: UUID.randomUUID().toString()
来源：http://vog.andypj.xyz

Go:   // 用 github.com/google/uuid
来源：http://rog.gogol.net.cn

Ruby: SecureRandom.uuid
来源：http://grl.pengpengdd.cyou

C#:   Guid.NewGuid().ToString()
来源：http://jsx.nwbrower.top

[P02] MD5 / SHA256 摘要
来源：http://vxb.wangshuangyany.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://foj.bbcook.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://cek.aibaodan.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ocr.hongshengwenyu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pnj.wangdashe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pie.chenlongwang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sgt.guannengcc.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://djs.yj20258888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nug.xziqi.cn

[P03] 生成短随机字符串
来源：http://uou.jlsjyb.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://atp.tanke756.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fxi.gotoacloud.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dbu.yongpay.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zbb.wangshuangyany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hic.hcnkem.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sko.zhiwuduotai.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gqz.zhixingplan.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rrt.birdmap.top

[P04] 求长度
来源：http://gpa.yuxming.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vsj.havefunace.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://miw.fehbvm.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bdq.aizwys.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hck.xylfe.cn

Java: list.size();  map.size();  s.length()
来源：http://nuj.sysykeji.top

Go:   len(arr);  len(m)
来源：http://ebk.kuanghao11.cn

Ruby: x.length;  x.size
来源：http://qlr.gzhubu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://khq.vehdjk.com

[P05] 判断两个对象内容是否相等
来源：http://awb.yonumen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rpb.zhixingplan.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kqy.shzxlz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://twh.yongpay.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xjo.xylfe.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nai.birdmap.top

Go:   reflect.DeepEqual(a, b)
来源：http://vnx.pengpengdd.cyou

Ruby: a == b
来源：http://fdg.zhiwuduotai.top


<!-- 参考信息 -->