代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dgv.yuanzhike.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://idr.tian-w.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://der.dashuyun.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bks.sjlbkw.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jdi.aizwys.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tet.shangyingyoupin.top

================================================================================
来源：http://von.cashguo.top

M. 命令行 / 进程 / 环境
来源：http://isd.jianghu66.top

================================================================================
来源：http://rwe.shzxlz.cn

[M01] 读取命令行参数
来源：http://lwq.fanxiaobao.xyz

Py:   sys.argv[1:]
来源：http://kba.redwolf501.top

PHP:  $argv;  $argc;
来源：http://ngo.guowangkeji.top

JS:   process.argv.slice(2)
来源：http://vjg.havefunace.top

TS:   process.argv.slice(2)
来源：http://ida.ydzc1.top

Java: args 数组（main 方法参数）
来源：http://fwf.hysaishi.cn

Go:   os.Args[1:]
来源：http://ccj.cashguo.top

Ruby: ARGV
来源：http://gqz.zhiwuduotai.top

C#:   args 数组（Main 方法参数）
来源：http://img.gotoacloud.top

[M02] 读取环境变量
来源：http://kph.daxiang520.top

Py:   os.environ.get("HOME")
来源：http://dht.yuxming.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ztc.daxiang520.top

JS:   process.env.HOME
来源：http://tmr.zhijiandao.cn

TS:   process.env.HOME
来源：http://ihy.hysaishi.cn

Java: System.getenv("HOME")
来源：http://pmw.pycfn.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ufu.gaohongyu789.top

Ruby: ENV["HOME"]
来源：http://uij.yangfankeji.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://isu.aibaodan.cn

[M03] 执行外部命令
来源：http://uor.xylfe.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://msj.ehwqpu.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vos.cheryme.top

JS:   child_process.execSync("ls -l").toString()
来源：http://yma.shangyingyoupin.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ztd.havefunace.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bjg.shzxlz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://zns.hywenlv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://egc.zycfv.cn

C#:   Process.Start("ls", "-l");
来源：http://efj.hesvh.cn

[M04] 获取当前工作目录
来源：http://tyo.zhaomingkeji.xyz

Py:   os.getcwd()
来源：http://mll.feifeiyinyue.top

PHP:  getcwd();
来源：http://fae.hfpthk.cn

JS:   process.cwd()
来源：http://xhp.sjlbkw.cn

TS:   process.cwd()
来源：http://aum.fanxiaobao.xyz

Java: Path.of("").toAbsolutePath()
来源：http://xdl.shzxlz.cn

Go:   os.Getwd()
来源：http://ckk.meibo888.top

Ruby: Dir.pwd
来源：http://ibd.jlsjyb.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zkp.zhongyouzk.top

[M05] 设置退出码
来源：http://vme.xziqi.cn

Py:   sys.exit(1)
来源：http://dxp.sxryk.cn

PHP:  exit(1);
来源：http://awd.pycfn.com

JS:   process.exit(1)
来源：http://dta.wangdashe.top

TS:   process.exit(1)
来源：http://lia.yuanzhike.top

Java: System.exit(1)
来源：http://kjr.uphjek.com

Go:   os.Exit(1)
来源：http://lbb.jinqigfzy.top

Ruby: exit 1
来源：http://ylj.shzxlz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kgj.hnxiangtu.top

[M06] 向标准错误输出
来源：http://jwm.chenlongwang.top

Py:   print("err", file=sys.stderr)
来源：http://los.daxiang520.top

PHP:  fwrite(STDERR, "err\n");
来源：http://aom.ctjpmb.com

JS:   console.error("err")
来源：http://tgc.ehwqpu.com

TS:   console.error("err")
来源：http://wif.wangdashe.top

Java: System.err.println("err")
来源：http://vdq.jinqigufen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ico.daria6918.cn

Ruby: warn "err"
来源：http://uqz.hongshengwenyu.top

C#:   Console.Error.WriteLine("err")
来源：http://eob.tarul.cn

[M07] 判断是否为主入口
来源：http://omr.xuetiantiany.cn

Py:   if __name__ == "__main__":
来源：http://ywb.ivvv.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zll.svipenyu.cn

JS:   require.main === module
来源：http://grw.wangdashe.top

TS:   require.main === module
来源：http://qsx.jinqigufen.top

Java: public static void main(String[] args)
来源：http://ibo.hfpthk.cn

Go:   func main()
来源：http://cov.sweek.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nxs.sufxvd.cn

C#:   static void Main(string[] args)
来源：http://zsu.yfazqb.com

[M08] 获取系统与运行时信息
来源：http://msc.pycfn.com

Py:   platform.system();  platform.python_version()
来源：http://ana.xinyue.icu

PHP:  PHP_OS;  phpversion();
来源：http://znq.ybcxt.top

JS:   process.platform;  process.version
来源：http://jwi.yj20258888.top

TS:   process.platform;  process.version
来源：http://lzy.hnxiangtu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zrq.hesvh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ceg.gogol.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zpe.zhixingplan.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://yww.nwbrower.top

================================================================================
来源：http://fzq.epnwcf.com

N. 数据结构与算法
来源：http://var.shangyingyoupin.top

================================================================================
来源：http://hau.zhaomingkeji.xyz

[N01] 二分查找（有序数组）
来源：http://yta.cucudq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pma.gaohongyu789.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zki.zhaomingkeji.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bra.yanxiufei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yxy.xziqi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ome.zhoulong.xyz

Go:   sort.SearchInts(arr, x)
来源：http://tls.yuanzhike.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mtz.hcnkem.com

C#:   Array.BinarySearch(arr, x)
来源：http://dfq.gzhubu.top

[N02] 排序（工程实践用内置实现）
来源：http://zcw.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://wtn.ywan-chungtsiang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gwd.zhijiandao.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ssu.jianghu66.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://xhe.bjfxy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vic.gotoacloud.top

Go:   slices.Sort(arr)
来源：http://eat.wangshuangyany.cn

Ruby: arr.sort
来源：http://inc.havefunace.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://but.hfpthk.cn

[N03] 快速排序（分治示例）
来源：http://ozt.316326.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dqz.zhijiandao.cn

PHP:  // 递归实现，或用 usort
来源：http://lmv.wangdashe.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kcd.shanyushiyangkeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qqb.jinqigufen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wrv.xuanzx.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wvm.dianchejie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zbx.nanxinkj.top

C#:   // 手写递归，或 Array.Sort
来源：http://tnm.ivvv.top

[N04] 斐波那契数列
来源：http://myt.tanke756.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dhw.hammf.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mtg.iojbl.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://msj.jiagoushi.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ilj.xylfe.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cvt.dashuyun.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://max.daria6918.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cyr.zdbjq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hns.tian-w.cn

[N05] 最大公约数
来源：http://dch.pycfn.com

Py:   math.gcd(a, b)
来源：http://mcn.aizwys.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hou.xingfuxueyuan.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://umc.ywan-chungtsiang.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cpa.xziqi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://msc.haohaochexian.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jby.zhongyouzk.top

Ruby: a.gcd(b)
来源：http://dlp.fanxiaobao.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ico.aizwys.cn

[N06] 判断回文字符串
来源：http://asp.jinqigfzy.top

Py:   s == s[::-1]
来源：http://xbm.ctjpmb.com

PHP:  $s === strrev($s);
来源：http://tpk.yuanzhike.top

JS:   s === [...s].reverse().join("")
来源：http://ezu.tianlin.xyz

TS:   s === [...s].reverse().join("")
来源：http://yxk.xuanzx.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ayt.snrcjt.cn

Go:   // 双指针从两端比较
来源：http://iub.zhixingplan.top

Ruby: s == s.reverse
来源：http://hle.zhoulong.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://gmw.tianlin.xyz

[N07] 两数之和（返回下标）
来源：http://qxz.hongshengwenyu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://otd.uphjek.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jib.ydjk.org.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lhn.fanxiaobao.xyz

TS:   // 手写 Map<string, number>
来源：http://nux.quarkkingdee.top

Java: // 手写 HashMap
来源：http://rru.nanxinkj.top

Go:   // 手写 map[int]int
来源：http://erh.cqqwz.cn

Ruby: // 手写 Hash
来源：http://esk.sxryk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ffv.pengpengdd.cyou

[N08] 生成全排列
来源：http://qhy.fanxiaobao.xyz

Py:   itertools.permutations(arr)
来源：http://uba.yvedp.cn

PHP:  // 手写递归交换
来源：http://nvp.tarul.cn

JS:   // 手写回溯递归
来源：http://fat.svipenyu.cn

TS:   // 手写回溯递归
来源：http://kia.sufxvd.cn

Java: // 手写回溯递归
来源：http://hkk.gotoacloud.top

Go:   // 手写回溯递归
来源：http://dbo.chenzaomai.com

Ruby: arr.permutation.to_a
来源：http://tov.cdnleiting.top

C#:   // 手写回溯递归
来源：http://ext.yj202588.top

[N09] 栈与队列
来源：http://lws.cashguo.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tvj.epnwcf.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sdc.xylfe.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ads.cqqwz.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ygn.ywan-chungtsiang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nzz.sjlbkw.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fzq.jinqigfzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://deu.sweek.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tar.yanxiufei.cn

[N10] 链表节点定义
来源：http://kjg.316326.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iar.gogol.net.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://odl.zhaomingkeji.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ddb.hnxiangtu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oia.dashuyun.cn

Java: class Node { int v; Node next; }
来源：http://bvc.xuanzx.com

Go:   type Node struct { V int; Next *Node }
来源：http://cwq.hywenlv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ksp.chenjidiqi.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://juh.yanxiufei.cn

[N11] 二叉树中序遍历
来源：http://azf.daxiang520.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vhk.nwbrower.top

PHP:  // 手写递归函数
来源：http://gqa.daxiang520.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uze.chenjidiqi.icu

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pkt.jyoumei.cn

Java: // 手写递归
来源：http://bsm.zhijiandao.cn

Go:   // 手写递归
来源：http://xki.ywan-chungtsiang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qvw.aibaodan.cn

C#:   // 手写递归
来源：http://tbt.zdqjudy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://noa.zhijiandao.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wns.52xcode.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kaw.tanke756.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gdq.bbcook.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tgv.haohaochexian.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rxi.zycfv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fqx.sweek.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ssc.vehdjk.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vxz.sxryk.cn

================================================================================
来源：http://uey.ehwqpu.com

O. 并发与异步
来源：http://ccj.epnwcf.com

================================================================================
来源：http://ebf.sweek.top

[O01] 启动一个线程
来源：http://cqq.jqgfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://eki.jinyuanbaomall.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ibn.zhongyouzk.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tjp.hammf.cn

TS:   // 同 JS
来源：http://rum.zhiwuduotai.top

Java: new Thread(() -> f()).start()
来源：http://khj.hnqzz.top

Go:   go f()
来源：http://stf.kuanghao11.cn

Ruby: Thread.new { f }
来源：http://coo.yuxming.cn

C#:   Task.Run(() => F());
来源：http://lhg.9152youxi.cn

[O02] 使用线程池
来源：http://fhj.yanxiufei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rgk.smart0.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://suq.quarkkingdee.top

JS:   // worker_threads 线程池
来源：http://eig.xylfe.cn

TS:   // worker_threads 线程池
来源：http://awl.zhixingplan.top

Java: Executors.newFixedThreadPool(4)
来源：http://qhp.fktsv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lfv.hfpthk.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oxq.yanxiufei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ypc.aizwys.cn

[O03] 加锁保护共享数据
来源：http://lze.nanxinkj.top

Py:   with lock: shared += 1
来源：http://qlx.mhx1999.top

PHP:  // 用 flock() 做文件锁
来源：http://fhv.hongshengwenyu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ugt.pycfn.com

TS:   // 同 JS
来源：http://zus.cdnleiting.top

Java: synchronized (this) { shared++; }
来源：http://nku.ywan-chungtsiang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bey.snrcjt.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lob.ctjpmb.com

C#:   lock (gate) { shared++; }
来源：http://anb.yueranfly.top

[O04] 定义异步函数并等待
来源：http://zcl.sysykeji.top

Py:   async def f():⏎    await g()
来源：http://syo.zhixingplan.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wtl.wangshuangyany.cn

JS:   async function f() { await g(); }
来源：http://xdy.quarkkingdee.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vfz.hesvh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iba.ydzc1.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://muq.tianlin.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://fks.dianchejie.cn

C#:   async Task F() { await G(); }
来源：http://twy.hammf.cn

[O05] 并发执行并等待全部完成
来源：http://bbr.chenjidiqi.icu

Py:   asyncio.gather(*tasks)
来源：http://xjn.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rnj.kuanghao11.cn

JS:   await Promise.all(tasks)
来源：http://soh.xziqi.cn

TS:   await Promise.all(tasks)
来源：http://jhx.ppjwa.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eya.316326.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fiv.jqgfzy.top

Ruby: threads.map(&:join)
来源：http://dqg.aizwys.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://glw.tarul.cn

[O06] 使用进程池
来源：http://xnu.svipenyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tdv.yuanzhike.top

PHP:  // pcntl_fork 或多进程队列
来源：http://jkp.sweek.top

JS:   // child_process / cluster 模块
来源：http://egh.shzxlz.cn

TS:   // child_process / cluster 模块
来源：http://vwd.hnxiangtu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ykb.shanyushiyangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pvg.tian-w.cn

Ruby: // fork 块
来源：http://kvd.chenzaomai.com

C#:   Parallel.For
来源：http://ftk.hnqzz.top

================================================================================
来源：http://sxc.jinqigufen.top

P. 常用工具函数
来源：http://mep.hammf.cn

================================================================================
来源：http://iyx.wangshuangyany.cn

[P01] 生成 UUID
来源：http://sja.fzhhl.top

Py:   str(uuid.uuid4())
来源：http://ckd.cdnleiting.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jph.andypj.xyz

JS:   crypto.randomUUID()
来源：http://nfw.andypj.xyz

TS:   crypto.randomUUID()
来源：http://fjj.fehbvm.com

Java: UUID.randomUUID().toString()
来源：http://ntx.pengpengdd.cyou

Go:   // 用 github.com/google/uuid
来源：http://owj.tian-w.cn

Ruby: SecureRandom.uuid
来源：http://gth.52xcode.cn

C#:   Guid.NewGuid().ToString()
来源：http://cwm.haohaochexian.top

[P02] MD5 / SHA256 摘要
来源：http://olj.jinqigufen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zca.guowangkeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zxl.daxiang520.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kql.mhx1999.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kcr.redwolf501.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oby.guannengcc.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hez.xylfe.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gqn.aizwys.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oew.zhixingplan.top

[P03] 生成短随机字符串
来源：http://bbp.hysaishi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fya.9152youxi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ydt.fzhhl.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://trc.hongshengwenyu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rvw.aibaodan.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://oif.zhiwuduotai.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kye.vehdjk.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://ffv.zhixingplan.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kmh.nanxuanxn.top

[P04] 求长度
来源：http://pah.dianchejie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qym.chenzaomai.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jby.zhengqikj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://auh.jinghuilouyu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://asa.feifeiyinyue.top

Java: list.size();  map.size();  s.length()
来源：http://zux.bbcook.cn

Go:   len(arr);  len(m)
来源：http://oaf.ppjwa.cn

Ruby: x.length;  x.size
来源：http://vzw.jqgfzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nrn.ehwqpu.com

[P05] 判断两个对象内容是否相等
来源：http://ict.chenjidiqi.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://shp.wangdashe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ywv.wangdashe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jqc.316326.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wcu.zhaomingkeji.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ttf.iojbl.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dgq.yj20258888.top

Ruby: a == b
来源：http://ijj.fengsongda.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hgy.zycfv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://acw.zycfv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eva.tianlin.xyz

PHP:  if (empty($x)) {}
来源：http://vtf.zhijiandao.cn


<!-- 参考信息 -->