代发 wailian999

C#:   (int)resp.StatusCode
来源：http://jan.chenjidiqi.icu

[L08] 并发请求多个地址
来源：http://nzc.dashuyun.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zaa.xuanzx.com

PHP:  curl_multi_init() 系列
来源：http://mcn.jinyuanbaomall.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pla.cheryme.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://isi.chenzaomai.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hxz.zhixingplan.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gqd.jlsjyb.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://oxe.0kj1m.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dgd.yonumen.top

================================================================================
来源：http://lfe.aizwys.cn

M. 命令行 / 进程 / 环境
来源：http://fvu.bbcook.cn

================================================================================
来源：http://ggi.fanxiaobao.xyz

[M01] 读取命令行参数
来源：http://zuz.daria6918.cn

Py:   sys.argv[1:]
来源：http://opo.shanyushiyangkeji.top

PHP:  $argv;  $argc;
来源：http://lsb.wangdashe.top

JS:   process.argv.slice(2)
来源：http://oar.xinyue.icu

TS:   process.argv.slice(2)
来源：http://siu.gaohongyu789.top

Java: args 数组（main 方法参数）
来源：http://jrf.redwolf501.top

Go:   os.Args[1:]
来源：http://sae.zhijiandao.cn

Ruby: ARGV
来源：http://cyu.0kj1m.cn

C#:   args 数组（Main 方法参数）
来源：http://asx.zhengqikj.top

[M02] 读取环境变量
来源：http://rup.jlsjyb.cn

Py:   os.environ.get("HOME")
来源：http://isw.fengsongda.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nqt.yonumen.top

JS:   process.env.HOME
来源：http://uwl.chenjidiqi.icu

TS:   process.env.HOME
来源：http://kcg.zycfv.cn

Java: System.getenv("HOME")
来源：http://rrk.tian-w.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wrb.ybcxt.top

Ruby: ENV["HOME"]
来源：http://hnr.shuidangran.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nhr.cashguo.top

[M03] 执行外部命令
来源：http://uxi.fengsongda.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yzx.hcnkem.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hll.ehwqpu.com

JS:   child_process.execSync("ls -l").toString()
来源：http://rwt.zhiwuduotai.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hoy.hnqzz.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xcl.jinqigfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://amr.shanyushiyangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://wad.ywan-chungtsiang.top

C#:   Process.Start("ls", "-l");
来源：http://nbj.zhengqikj.top

[M04] 获取当前工作目录
来源：http://ine.nanxuanxn.top

Py:   os.getcwd()
来源：http://zdg.jlsjyb.cn

PHP:  getcwd();
来源：http://kmj.52xcode.cn

JS:   process.cwd()
来源：http://ocf.kuanghao11.cn

TS:   process.cwd()
来源：http://ffz.chenzaomai.com

Java: Path.of("").toAbsolutePath()
来源：http://fux.xuanzx.com

Go:   os.Getwd()
来源：http://nyu.yangfankeji.com

Ruby: Dir.pwd
来源：http://udj.havefunace.top

C#:   Directory.GetCurrentDirectory()
来源：http://emf.yj20258.top

[M05] 设置退出码
来源：http://jjr.fktsv.cn

Py:   sys.exit(1)
来源：http://ijq.jlsjyb.cn

PHP:  exit(1);
来源：http://fep.vqdsnc.cn

JS:   process.exit(1)
来源：http://fmf.bjfxy.top

TS:   process.exit(1)
来源：http://arm.zdbjq.cn

Java: System.exit(1)
来源：http://dsu.xziqi.cn

Go:   os.Exit(1)
来源：http://uwy.dashuyun.cn

Ruby: exit 1
来源：http://rum.xylfe.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wag.tian-w.cn

[M06] 向标准错误输出
来源：http://vdf.xylfe.cn

Py:   print("err", file=sys.stderr)
来源：http://cpd.vehdjk.com

PHP:  fwrite(STDERR, "err\n");
来源：http://gwa.zhengqikj.top

JS:   console.error("err")
来源：http://qjh.chenlongwang.top

TS:   console.error("err")
来源：http://ady.tian-w.cn

Java: System.err.println("err")
来源：http://jzt.ehwqpu.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tnw.yj202588.top

Ruby: warn "err"
来源：http://rcx.sufxvd.cn

C#:   Console.Error.WriteLine("err")
来源：http://pyd.nwbrower.top

[M07] 判断是否为主入口
来源：http://pmy.cheryme.top

Py:   if __name__ == "__main__":
来源：http://mpa.cdnleiting.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iof.smart0.xyz

JS:   require.main === module
来源：http://spu.316326.xyz

TS:   require.main === module
来源：http://iuo.feifeiyinyue.top

Java: public static void main(String[] args)
来源：http://yol.feifeiyinyue.top

Go:   func main()
来源：http://xpd.mhx1999.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://txt.nwbrower.top

C#:   static void Main(string[] args)
来源：http://rpo.nanxuanxn.top

[M08] 获取系统与运行时信息
来源：http://szh.iojbl.cn

Py:   platform.system();  platform.python_version()
来源：http://jix.0kj1m.cn

PHP:  PHP_OS;  phpversion();
来源：http://pqv.daria6918.cn

JS:   process.platform;  process.version
来源：http://gjz.yuxming.cn

TS:   process.platform;  process.version
来源：http://efc.iojbl.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tjz.yj202588.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://emh.daxiang520.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dyi.xinyue.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://qoa.aizwys.cn

================================================================================
来源：http://gsu.tian-w.cn

N. 数据结构与算法
来源：http://iyx.yueranfly.top

================================================================================
来源：http://aij.pengpengdd.cyou

[N01] 二分查找（有序数组）
来源：http://mph.0kj1m.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ryw.sweek.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tdc.epnwcf.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ltn.meibo888.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lsw.zhijiandao.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tgy.hywenlv.cn

Go:   sort.SearchInts(arr, x)
来源：http://njp.fehbvm.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://nrr.yvedp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fie.birdmap.top

[N02] 排序（工程实践用内置实现）
来源：http://peu.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://aja.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fzz.hnqzz.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pbj.cucudq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://aeu.hesvh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tfn.bjfxy.top

Go:   slices.Sort(arr)
来源：http://ctq.zhoulong.xyz

Ruby: arr.sort
来源：http://rxa.nanxuanxn.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jbk.chenlongwang.top

[N03] 快速排序（分治示例）
来源：http://ofx.hywenlv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pqj.vehdjk.com

PHP:  // 递归实现，或用 usort
来源：http://zem.pycfn.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sxa.iojbl.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tix.ivvv.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://byk.c1oappe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xpc.52xcode.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nye.wangdashe.top

C#:   // 手写递归，或 Array.Sort
来源：http://tye.cqqwz.cn

[N04] 斐波那契数列
来源：http://ggw.yj20258888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yiu.shzxlz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://daj.yangfankeji.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rtm.hnxiangtu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://glv.zhongyouzk.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iqd.ybcxt.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hme.xziqi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cmv.ctjpmb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qrg.fehbvm.com

[N05] 最大公约数
来源：http://yzd.guannengcc.top

Py:   math.gcd(a, b)
来源：http://wez.hnxiangtu.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hhw.hfpthk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fcg.tianlin.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ynl.jinqigfzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://exp.wangdashe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ass.jianghu66.top

Ruby: a.gcd(b)
来源：http://iys.andypj.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lom.havefunace.top

[N06] 判断回文字符串
来源：http://mcn.cucudq.cn

Py:   s == s[::-1]
来源：http://owm.zhongyouzk.top

PHP:  $s === strrev($s);
来源：http://dje.feifeiyinyue.top

JS:   s === [...s].reverse().join("")
来源：http://vuf.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://zdm.shangyingyoupin.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sko.wangdashe.top

Go:   // 双指针从两端比较
来源：http://adc.jinyuanbaomall.cn

Ruby: s == s.reverse
来源：http://sup.epnwcf.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://jku.tanke756.top

[N07] 两数之和（返回下标）
来源：http://wgg.nanxinkj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wcg.sweek.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xbd.wangshuangyany.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gex.hfpthk.cn

TS:   // 手写 Map<string, number>
来源：http://rrg.cashguo.top

Java: // 手写 HashMap
来源：http://gjt.zhongyouzk.top

Go:   // 手写 map[int]int
来源：http://eer.bbcook.cn

Ruby: // 手写 Hash
来源：http://vgk.hnqzz.top

C#:   // 手写 Dictionary<int, int>
来源：http://gun.zhixingplan.top

[N08] 生成全排列
来源：http://umh.fanxiaobao.xyz

Py:   itertools.permutations(arr)
来源：http://era.meibo888.top

PHP:  // 手写递归交换
来源：http://ivh.nwbrower.top

JS:   // 手写回溯递归
来源：http://oqr.ywan-chungtsiang.top

TS:   // 手写回溯递归
来源：http://rqf.tanke756.top

Java: // 手写回溯递归
来源：http://eki.kuanghao11.cn

Go:   // 手写回溯递归
来源：http://bjc.gotoacloud.top

Ruby: arr.permutation.to_a
来源：http://dih.svipenyu.cn

C#:   // 手写回溯递归
来源：http://ayv.zdbjq.cn

[N09] 栈与队列
来源：http://jxi.nwbrower.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://phz.jinyuanbaomall.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://thz.yuanzhike.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://csz.quarkkingdee.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ubl.vqdsnc.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://chu.kuanghao11.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lfz.jqgufenzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dgv.zhaomingkeji.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zfa.zhijiandao.cn

[N10] 链表节点定义
来源：http://wnz.ydzc1.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xmb.kuanghao11.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hii.snrcjt.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mwv.gaohongyu789.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vnw.yj20258.top

Java: class Node { int v; Node next; }
来源：http://ccb.ydzc1.top

Go:   type Node struct { V int; Next *Node }
来源：http://zbm.cheryme.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wno.xylfe.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ajx.cqqwz.cn

[N11] 二叉树中序遍历
来源：http://fzr.hcnkem.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://slv.hnxiangtu.top

PHP:  // 手写递归函数
来源：http://ozi.zdbjq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nfo.zhongyouzk.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://smy.xingfuxueyuan.xyz

Java: // 手写递归
来源：http://joq.zhaomingkeji.xyz

Go:   // 手写递归
来源：http://zma.ybcxt.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oqv.ivvv.top

C#:   // 手写递归
来源：http://vwt.ywan-chungtsiang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://llf.zhaomingkeji.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ckq.cucudq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tgj.quarkkingdee.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://irp.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ejo.kuanghao11.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://soa.birdmap.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lzi.cucudq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qqt.guowangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lcd.yj20258888.top

================================================================================
来源：http://nkd.xylfe.cn

O. 并发与异步
来源：http://urm.hammf.cn

================================================================================
来源：http://wjl.iojbl.cn

[O01] 启动一个线程
来源：http://tyn.svipenyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hpg.316326.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gng.ctjpmb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iti.shanyushiyangkeji.top

TS:   // 同 JS
来源：http://bth.epnwcf.com

Java: new Thread(() -> f()).start()
来源：http://hro.mhx1999.top

Go:   go f()
来源：http://qat.shuidangran.top

Ruby: Thread.new { f }
来源：http://ygz.zhixingplan.top

C#:   Task.Run(() => F());
来源：http://gxe.snrcjt.cn

[O02] 使用线程池
来源：http://bay.shzxlz.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kcw.yuxming.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nvl.daxiang520.top

JS:   // worker_threads 线程池
来源：http://hsp.tian-w.cn

TS:   // worker_threads 线程池
来源：http://ifi.fengsongda.top

Java: Executors.newFixedThreadPool(4)
来源：http://fpg.quarkkingdee.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://plf.xuetiantiany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ggx.yj202588.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jqe.xingfuxueyuan.xyz

[O03] 加锁保护共享数据
来源：http://dmj.zhixingplan.top

Py:   with lock: shared += 1
来源：http://lac.svipenyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://mms.jqgufenzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ypg.sweek.top

TS:   // 同 JS
来源：http://dfs.gaohongyu789.top

Java: synchronized (this) { shared++; }
来源：http://bvi.hfpthk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://roc.fengsongda.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://pqt.bbcook.cn

C#:   lock (gate) { shared++; }
来源：http://imy.wangdashe.top

[O04] 定义异步函数并等待
来源：http://bru.hesvh.cn

Py:   async def f():⏎    await g()
来源：http://gps.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oec.xuetiantiany.cn

JS:   async function f() { await g(); }
来源：http://mjw.jqgfzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://aut.hywenlv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fqk.snrcjt.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zsa.yj202588.top

Ruby: # 用 Fiber 或 async gem
来源：http://mbk.hnxiangtu.top

C#:   async Task F() { await G(); }
来源：http://bph.sysykeji.top

[O05] 并发执行并等待全部完成
来源：http://xoa.jiagoushi.top

Py:   asyncio.gather(*tasks)
来源：http://qrx.ppjwa.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gfn.hammf.cn

JS:   await Promise.all(tasks)
来源：http://pun.xziqi.cn

TS:   await Promise.all(tasks)
来源：http://ljw.dashuyun.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mpf.ywan-chungtsiang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mkh.shanyushiyangtech.top

Ruby: threads.map(&:join)
来源：http://iqj.tian-w.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://spg.tanke756.top

[O06] 使用进程池
来源：http://uzq.yj202588.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pdm.aibaodan.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mps.xziqi.cn

JS:   // child_process / cluster 模块
来源：http://ohl.fzhhl.top

TS:   // child_process / cluster 模块
来源：http://bdu.316326.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dbc.tanke756.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gnq.zdbjq.cn

Ruby: // fork 块
来源：http://xfg.zhijiandao.cn

C#:   Parallel.For
来源：http://faf.cheryme.top

================================================================================
来源：http://ppl.zdbjq.cn

P. 常用工具函数
来源：http://tos.svipenyu.cn

================================================================================
来源：http://qxe.yj20258.top

[P01] 生成 UUID
来源：http://fbz.smart0.xyz

Py:   str(uuid.uuid4())
来源：http://nuh.ehwqpu.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qyz.zhoulong.xyz

JS:   crypto.randomUUID()
来源：http://vtw.jinqigufen.top

TS:   crypto.randomUUID()
来源：http://hpu.vqdsnc.cn

Java: UUID.randomUUID().toString()
来源：http://luh.yanxiufei.cn

Go:   // 用 github.com/google/uuid
来源：http://ooo.pengpengdd.cyou

Ruby: SecureRandom.uuid
来源：http://gwa.daria6918.cn

C#:   Guid.NewGuid().ToString()
来源：http://aqx.jyoumei.cn

[P02] MD5 / SHA256 摘要
来源：http://aqj.mhx1999.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rzn.wangdashe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fvy.jiagoushi.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pyu.hcnkem.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vbx.vehdjk.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://iyo.hywenlv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wcv.aibaodan.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://eup.xinyue.icu

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mos.zdbjq.cn

[P03] 生成短随机字符串
来源：http://kfa.cqqwz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hvr.andypj.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kub.smart0.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ymt.tianlin.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://glx.ehwqpu.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iga.shangyingyoupin.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pob.52xcode.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wzk.vehdjk.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kfs.snrcjt.cn

[P04] 求长度
来源：http://ygt.cheryme.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fvb.zhaomingkeji.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xzs.yj202588.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sij.yuanzhike.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yml.sysykeji.top

Java: list.size();  map.size();  s.length()
来源：http://tyx.wangshuangyany.cn

Go:   len(arr);  len(m)
来源：http://qxc.hnqzz.top

Ruby: x.length;  x.size
来源：http://yze.iojbl.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://idt.jinyuanbaomall.cn

[P05] 判断两个对象内容是否相等
来源：http://kfh.zhaomingkeji.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://yam.nanxuanxn.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://igs.chenlongwang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qzr.ydzc1.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://icq.bbcook.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tmm.ivvv.top

Go:   reflect.DeepEqual(a, b)
来源：http://qod.dianchejie.cn

Ruby: a == b
来源：http://zyj.yanxiufei.cn


<!-- 参考信息 -->