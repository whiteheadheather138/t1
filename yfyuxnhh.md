代发 wailian999

================================================================================
来源：http://hpy.ppjwa.cn

[M01] 读取命令行参数
来源：http://ihv.zdbjq.cn

Py:   sys.argv[1:]
来源：http://mcc.sufxvd.cn

PHP:  $argv;  $argc;
来源：http://wgx.mhx1999.top

JS:   process.argv.slice(2)
来源：http://npt.zhiwuduotai.top

TS:   process.argv.slice(2)
来源：http://ghr.hongshengwenyu.top

Java: args 数组（main 方法参数）
来源：http://fbc.jinqigufen.top

Go:   os.Args[1:]
来源：http://lbv.zhiwuduotai.top

Ruby: ARGV
来源：http://eyo.316326.xyz

C#:   args 数组（Main 方法参数）
来源：http://aym.bjfxy.top

[M02] 读取环境变量
来源：http://daw.ywan-chungtsiang.top

Py:   os.environ.get("HOME")
来源：http://epn.cdnleiting.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yqx.zhixingplan.top

JS:   process.env.HOME
来源：http://czs.aibaodan.cn

TS:   process.env.HOME
来源：http://dck.meibo888.top

Java: System.getenv("HOME")
来源：http://awi.smart0.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xrg.wangdashe.top

Ruby: ENV["HOME"]
来源：http://ukc.cucudq.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bts.xziqi.cn

[M03] 执行外部命令
来源：http://uon.sweek.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vap.dashuyun.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lpg.shuidangran.top

JS:   child_process.execSync("ls -l").toString()
来源：http://usn.cheryme.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zrn.ywan-chungtsiang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yhl.ehwqpu.com

Go:   exec.Command("ls", "-l").Output()
来源：http://wxu.gogol.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://kpn.smart0.xyz

C#:   Process.Start("ls", "-l");
来源：http://eoh.zhijiandao.cn

[M04] 获取当前工作目录
来源：http://eez.chenzaomai.com

Py:   os.getcwd()
来源：http://kly.zhengqikj.top

PHP:  getcwd();
来源：http://pou.havefunace.top

JS:   process.cwd()
来源：http://vup.xingfuxueyuan.xyz

TS:   process.cwd()
来源：http://xxn.xziqi.cn

Java: Path.of("").toAbsolutePath()
来源：http://htg.yuxming.cn

Go:   os.Getwd()
来源：http://gvq.bjfxy.top

Ruby: Dir.pwd
来源：http://uoz.tanke756.top

C#:   Directory.GetCurrentDirectory()
来源：http://dgk.meibo888.top

[M05] 设置退出码
来源：http://lwy.hesvh.cn

Py:   sys.exit(1)
来源：http://hcd.ppjwa.cn

PHP:  exit(1);
来源：http://asp.zdqjudy.top

JS:   process.exit(1)
来源：http://qgx.meibo888.top

TS:   process.exit(1)
来源：http://vvp.sxryk.cn

Java: System.exit(1)
来源：http://kjq.zhoulong.xyz

Go:   os.Exit(1)
来源：http://czy.sjlbkw.cn

Ruby: exit 1
来源：http://hkq.yonumen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mqt.havefunace.top

[M06] 向标准错误输出
来源：http://lic.wangdashe.top

Py:   print("err", file=sys.stderr)
来源：http://qbg.jinghuilouyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://pjs.gotoacloud.top

JS:   console.error("err")
来源：http://sly.shuidangran.top

TS:   console.error("err")
来源：http://sjc.quarkkingdee.top

Java: System.err.println("err")
来源：http://zkh.shuidangran.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qgt.nanxuanxn.top

Ruby: warn "err"
来源：http://zgx.hammf.cn

C#:   Console.Error.WriteLine("err")
来源：http://ygp.haohaochexian.top

[M07] 判断是否为主入口
来源：http://rqp.iojbl.cn

Py:   if __name__ == "__main__":
来源：http://vbe.yangfankeji.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nel.andypj.xyz

JS:   require.main === module
来源：http://wdg.sxryk.cn

TS:   require.main === module
来源：http://irr.svipenyu.cn

Java: public static void main(String[] args)
来源：http://zta.nanxinkj.top

Go:   func main()
来源：http://mhx.nanxinkj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mqy.xinyue.icu

C#:   static void Main(string[] args)
来源：http://wdc.smart0.xyz

[M08] 获取系统与运行时信息
来源：http://qqk.gogol.net.cn

Py:   platform.system();  platform.python_version()
来源：http://iyv.xingfuxueyuan.xyz

PHP:  PHP_OS;  phpversion();
来源：http://uyi.vehdjk.com

JS:   process.platform;  process.version
来源：http://jtv.ctjpmb.com

TS:   process.platform;  process.version
来源：http://iou.ehwqpu.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jnf.yfazqb.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://wje.tianlin.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://siz.zdqjudy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ane.gzhubu.top

================================================================================
来源：http://qav.ybcxt.top

N. 数据结构与算法
来源：http://rsr.chenzaomai.com

================================================================================
来源：http://nev.zhongyouzk.top

[N01] 二分查找（有序数组）
来源：http://vyl.fktsv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qxa.sxryk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wof.cheryme.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://foq.chenjidiqi.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nwr.uphjek.com

Java: Arrays.binarySearch(arr, x)
来源：http://vgx.zdqjudy.top

Go:   sort.SearchInts(arr, x)
来源：http://fsj.mhx1999.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ikp.yuanzhike.top

C#:   Array.BinarySearch(arr, x)
来源：http://nwk.jyoumei.cn

[N02] 排序（工程实践用内置实现）
来源：http://dvj.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://wgz.shzxlz.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://she.kuanghao11.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ukc.yanxiufei.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ega.cucudq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uss.zycfv.cn

Go:   slices.Sort(arr)
来源：http://hlf.yueranfly.top

Ruby: arr.sort
来源：http://cur.daria6918.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lcw.zhaomingkeji.xyz

[N03] 快速排序（分治示例）
来源：http://jkh.zycfv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gam.snrcjt.cn

PHP:  // 递归实现，或用 usort
来源：http://haf.yangfankeji.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mxt.yanxiufei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ruc.jqgufenzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://off.xuetiantiany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qqr.svipenyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jyf.ehwqpu.com

C#:   // 手写递归，或 Array.Sort
来源：http://zee.hywenlv.cn

[N04] 斐波那契数列
来源：http://tnu.cqqwz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xzi.cheryme.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://njk.haohaochexian.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://slf.smart0.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pgc.yanxiufei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://txo.andypj.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vtb.sufxvd.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rpl.nanxinkj.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lnu.yvedp.cn

[N05] 最大公约数
来源：http://rbo.redwolf501.top

Py:   math.gcd(a, b)
来源：http://ome.jqgufenzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fcn.hammf.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zyc.wangdashe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tix.yonumen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ptc.mhx1999.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oqi.yangfankeji.com

Ruby: a.gcd(b)
来源：http://gfz.xuanzx.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://usa.dashuyun.cn

[N06] 判断回文字符串
来源：http://mms.wangshuangyany.cn

Py:   s == s[::-1]
来源：http://zmi.xinyue.icu

PHP:  $s === strrev($s);
来源：http://acb.zhengqikj.top

JS:   s === [...s].reverse().join("")
来源：http://fja.gaohongyu789.top

TS:   s === [...s].reverse().join("")
来源：http://txq.chenlongwang.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dzt.havefunace.top

Go:   // 双指针从两端比较
来源：http://lyv.aizwys.cn

Ruby: s == s.reverse
来源：http://qdj.cucudq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jdp.yangfankeji.com

[N07] 两数之和（返回下标）
来源：http://zji.jinqigfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zjt.quarkkingdee.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qcf.hammf.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fae.xziqi.cn

TS:   // 手写 Map<string, number>
来源：http://jyg.sweek.top

Java: // 手写 HashMap
来源：http://ixe.yuanzhike.top

Go:   // 手写 map[int]int
来源：http://dnr.zhaomingkeji.xyz

Ruby: // 手写 Hash
来源：http://aym.snrcjt.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mrc.yanxiufei.cn

[N08] 生成全排列
来源：http://ays.hysaishi.cn

Py:   itertools.permutations(arr)
来源：http://cpk.zdqjudy.top

PHP:  // 手写递归交换
来源：http://rtn.pycfn.com

JS:   // 手写回溯递归
来源：http://iim.hesvh.cn

TS:   // 手写回溯递归
来源：http://xbe.epnwcf.com

Java: // 手写回溯递归
来源：http://rhg.yfazqb.com

Go:   // 手写回溯递归
来源：http://szj.zdqjudy.top

Ruby: arr.permutation.to_a
来源：http://evz.nwbrower.top

C#:   // 手写回溯递归
来源：http://hka.sysykeji.top

[N09] 栈与队列
来源：http://vff.cdnleiting.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jpx.gzhubu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://shm.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://osl.dianchejie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dxc.feifeiyinyue.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xnu.zycfv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fcp.xuetiantiany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wzc.52xcode.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lcl.birdmap.top

[N10] 链表节点定义
来源：http://mcy.andypj.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dad.haohaochexian.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qyp.yuanzhike.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bes.yanxiufei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://nmw.ybcxt.top

Java: class Node { int v; Node next; }
来源：http://ewf.yj20258888.top

Go:   type Node struct { V int; Next *Node }
来源：http://ptw.shangyingyoupin.top

Ruby: Node = Struct.new(:v, :next)
来源：http://vzd.chenjidiqi.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://qbm.jinghuilouyu.cn

[N11] 二叉树中序遍历
来源：http://zwy.chenjidiqi.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pmt.hywenlv.cn

PHP:  // 手写递归函数
来源：http://tik.andypj.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gfj.yonumen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://imb.kuanghao11.cn

Java: // 手写递归
来源：http://tye.yfazqb.com

Go:   // 手写递归
来源：http://uql.meibo888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lfc.snrcjt.cn

C#:   // 手写递归
来源：http://ojr.aizwys.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ytv.tianlin.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lox.shanyushiyangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ijs.ywan-chungtsiang.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oqe.kuanghao11.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vfe.sxryk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vqt.shzxlz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wef.sxryk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wwk.hywenlv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://seg.yvedp.cn

================================================================================
来源：http://onk.bjfxy.top

O. 并发与异步
来源：http://pbx.xylfe.cn

================================================================================
来源：http://ago.dashuyun.cn

[O01] 启动一个线程
来源：http://xpf.shanyushiyangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vey.havefunace.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nbt.cashguo.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rjm.wangdashe.top

TS:   // 同 JS
来源：http://ixo.xinyue.icu

Java: new Thread(() -> f()).start()
来源：http://uvi.ctjpmb.com

Go:   go f()
来源：http://ruw.sweek.top

Ruby: Thread.new { f }
来源：http://iua.zdqjudy.top

C#:   Task.Run(() => F());
来源：http://kgl.fengsongda.top

[O02] 使用线程池
来源：http://puk.cqqwz.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tar.fengsongda.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nis.epnwcf.com

JS:   // worker_threads 线程池
来源：http://xay.iojbl.cn

TS:   // worker_threads 线程池
来源：http://rhe.kuanghao11.cn

Java: Executors.newFixedThreadPool(4)
来源：http://oll.fktsv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hsl.fanxiaobao.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zsd.zhijiandao.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ixz.xziqi.cn

[O03] 加锁保护共享数据
来源：http://iod.aibaodan.cn

Py:   with lock: shared += 1
来源：http://ttz.ywan-chungtsiang.top

PHP:  // 用 flock() 做文件锁
来源：http://fhq.shanyushiyangtech.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ltz.hcnkem.com

TS:   // 同 JS
来源：http://san.epnwcf.com

Java: synchronized (this) { shared++; }
来源：http://skh.ybcxt.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://van.ctjpmb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://vcl.bbcook.cn

C#:   lock (gate) { shared++; }
来源：http://jho.dashuyun.cn

[O04] 定义异步函数并等待
来源：http://nvk.wangdashe.top

Py:   async def f():⏎    await g()
来源：http://evx.ehwqpu.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qvb.hongshengwenyu.top

JS:   async function f() { await g(); }
来源：http://btv.yanxiufei.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kpf.zhengqikj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zbf.316326.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ugq.xuanzx.com

Ruby: # 用 Fiber 或 async gem
来源：http://qnn.jinyuanbaomall.cn

C#:   async Task F() { await G(); }
来源：http://jrp.gotoacloud.top

[O05] 并发执行并等待全部完成
来源：http://lpg.gogol.net.cn

Py:   asyncio.gather(*tasks)
来源：http://fjq.iojbl.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nzz.yj20258.top

JS:   await Promise.all(tasks)
来源：http://kvv.chenjidiqi.icu

TS:   await Promise.all(tasks)
来源：http://ujr.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://apf.zhoulong.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dck.52xcode.cn

Ruby: threads.map(&:join)
来源：http://ysa.hesvh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://aae.zycfv.cn

[O06] 使用进程池
来源：http://ddw.xziqi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zhc.aizwys.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vod.jinghuilouyu.cn

JS:   // child_process / cluster 模块
来源：http://ztd.wangdashe.top

TS:   // child_process / cluster 模块
来源：http://zbm.yuanzhike.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lua.pengpengdd.cyou

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yhm.ppjwa.cn

Ruby: // fork 块
来源：http://dfs.yanxiufei.cn

C#:   Parallel.For
来源：http://thg.zhaomingkeji.xyz

================================================================================
来源：http://ire.jianghu66.top

P. 常用工具函数
来源：http://uxw.yueranfly.top

================================================================================
来源：http://tmf.aibaodan.cn

[P01] 生成 UUID
来源：http://vie.jlsjyb.cn

Py:   str(uuid.uuid4())
来源：http://snt.hesvh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dlz.zhoulong.xyz

JS:   crypto.randomUUID()
来源：http://psz.shzxlz.cn

TS:   crypto.randomUUID()
来源：http://lzu.jqgfzy.top

Java: UUID.randomUUID().toString()
来源：http://rai.smart0.xyz

Go:   // 用 github.com/google/uuid
来源：http://kix.jqgufenzy.top

Ruby: SecureRandom.uuid
来源：http://igs.birdmap.top

C#:   Guid.NewGuid().ToString()
来源：http://xyi.fktsv.cn

[P02] MD5 / SHA256 摘要
来源：http://ahs.guannengcc.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kql.tarul.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vwy.aizwys.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ifc.uphjek.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tpy.xingfuxueyuan.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://agd.tarul.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wka.jinqigufen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lbm.shangyingyoupin.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qgp.sysykeji.top

[P03] 生成短随机字符串
来源：http://oov.ctjpmb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pgz.ybcxt.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lub.kuanghao11.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qrt.cqqwz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zqt.iojbl.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qgv.feifeiyinyue.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iyb.meibo888.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://olp.guannengcc.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eev.chenlongwang.top

[P04] 求长度
来源：http://oyu.mhx1999.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ozi.shzxlz.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rao.jqgfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://usj.tian-w.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://veq.hnxiangtu.top

Java: list.size();  map.size();  s.length()
来源：http://xav.daria6918.cn

Go:   len(arr);  len(m)
来源：http://ifh.svipenyu.cn

Ruby: x.length;  x.size
来源：http://nri.ctjpmb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://qxt.jinghuilouyu.cn

[P05] 判断两个对象内容是否相等
来源：http://suo.xziqi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zwy.hongshengwenyu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tfn.zhengqikj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ziz.zhiwuduotai.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uve.zhaomingkeji.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tyr.316326.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://yhp.yvedp.cn

Ruby: a == b
来源：http://cyu.yj20258888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://aix.c1oappe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xxw.mhx1999.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wfj.ppjwa.cn

PHP:  if (empty($x)) {}
来源：http://hno.chenjidiqi.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rjr.fzhhl.top

TS:   if (x == null) {}
来源：http://tqo.hnqzz.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ivg.pycfn.com

Go:   if x == nil {}
来源：http://gjo.shuidangran.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eab.aizwys.cn

C#:   if (x is null) {}
来源：http://rsb.guowangkeji.top

[P07] 防抖与节流
来源：http://wsu.dianchejie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dxt.0kj1m.cn


<!-- 参考信息 -->