代发 wailian999

C#:   (int)resp.StatusCode
来源：http://azb.zhongyouzk.top

[L08] 并发请求多个地址
来源：http://ied.bjfxy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iau.gzhubu.top

PHP:  curl_multi_init() 系列
来源：http://gbf.xingfuxueyuan.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uso.aibaodan.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xep.redwolf501.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kgt.svipenyu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oqo.nanxinkj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vmn.xuanzx.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oiu.ybcxt.top

================================================================================
来源：http://ofr.zhoulong.xyz

M. 命令行 / 进程 / 环境
来源：http://btt.jinyuanbaomall.cn

================================================================================
来源：http://crv.ydzc1.top

[M01] 读取命令行参数
来源：http://bgj.tian-w.cn

Py:   sys.argv[1:]
来源：http://hiy.daria6918.cn

PHP:  $argv;  $argc;
来源：http://wcn.haohaochexian.top

JS:   process.argv.slice(2)
来源：http://smx.redwolf501.top

TS:   process.argv.slice(2)
来源：http://uxh.vqdsnc.cn

Java: args 数组（main 方法参数）
来源：http://yid.zhaomingkeji.xyz

Go:   os.Args[1:]
来源：http://xao.haohaochexian.top

Ruby: ARGV
来源：http://gtp.gaohongyu789.top

C#:   args 数组（Main 方法参数）
来源：http://wyz.yuxming.cn

[M02] 读取环境变量
来源：http://kfo.chenzaomai.com

Py:   os.environ.get("HOME")
来源：http://jom.yanxiufei.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zoz.daria6918.cn

JS:   process.env.HOME
来源：http://ppv.shanyushiyangtech.top

TS:   process.env.HOME
来源：http://kry.xuetiantiany.cn

Java: System.getenv("HOME")
来源：http://laa.zycfv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nsf.jinyuanbaomall.cn

Ruby: ENV["HOME"]
来源：http://vwn.jinqigufen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yhn.bjfxy.top

[M03] 执行外部命令
来源：http://usu.9152youxi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://krn.svipenyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qux.chenjidiqi.icu

JS:   child_process.execSync("ls -l").toString()
来源：http://squ.yangfankeji.com

TS:   child_process.execSync("ls -l").toString()
来源：http://fpc.daria6918.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xrh.yangfankeji.com

Go:   exec.Command("ls", "-l").Output()
来源：http://adt.ppjwa.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xcq.sysykeji.top

C#:   Process.Start("ls", "-l");
来源：http://znh.gogol.net.cn

[M04] 获取当前工作目录
来源：http://wpa.vehdjk.com

Py:   os.getcwd()
来源：http://yvl.havefunace.top

PHP:  getcwd();
来源：http://qfr.hnqzz.top

JS:   process.cwd()
来源：http://rxw.meibo888.top

TS:   process.cwd()
来源：http://qtj.sweek.top

Java: Path.of("").toAbsolutePath()
来源：http://imr.yonumen.top

Go:   os.Getwd()
来源：http://gil.shangyingyoupin.top

Ruby: Dir.pwd
来源：http://hwx.chenzaomai.com

C#:   Directory.GetCurrentDirectory()
来源：http://grg.pengpengdd.cyou

[M05] 设置退出码
来源：http://myv.shangyingyoupin.top

Py:   sys.exit(1)
来源：http://ora.shangyingyoupin.top

PHP:  exit(1);
来源：http://eko.hcnkem.com

JS:   process.exit(1)
来源：http://enf.yanxiufei.cn

TS:   process.exit(1)
来源：http://rls.sysykeji.top

Java: System.exit(1)
来源：http://ezk.jqgufenzy.top

Go:   os.Exit(1)
来源：http://fqk.hywenlv.cn

Ruby: exit 1
来源：http://sdo.sjlbkw.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zcr.guowangkeji.top

[M06] 向标准错误输出
来源：http://bzv.gogol.net.cn

Py:   print("err", file=sys.stderr)
来源：http://mwr.aizwys.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://plw.gogol.net.cn

JS:   console.error("err")
来源：http://ogj.hywenlv.cn

TS:   console.error("err")
来源：http://qxp.gogol.net.cn

Java: System.err.println("err")
来源：http://inx.hfpthk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://avb.yanxiufei.cn

Ruby: warn "err"
来源：http://jty.yanxiufei.cn

C#:   Console.Error.WriteLine("err")
来源：http://yho.jinghuilouyu.cn

[M07] 判断是否为主入口
来源：http://rkl.xuetiantiany.cn

Py:   if __name__ == "__main__":
来源：http://fpw.zhengqikj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oro.zycfv.cn

JS:   require.main === module
来源：http://ibj.snrcjt.cn

TS:   require.main === module
来源：http://owj.wangdashe.top

Java: public static void main(String[] args)
来源：http://jxi.fengsongda.top

Go:   func main()
来源：http://cyj.ctjpmb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://exf.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://rfm.dashuyun.cn

[M08] 获取系统与运行时信息
来源：http://duu.ivvv.top

Py:   platform.system();  platform.python_version()
来源：http://oag.gaohongyu789.top

PHP:  PHP_OS;  phpversion();
来源：http://qia.gaohongyu789.top

JS:   process.platform;  process.version
来源：http://sxg.mhx1999.top

TS:   process.platform;  process.version
来源：http://scu.cheryme.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://eoy.zdqjudy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://aqc.gaohongyu789.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fxh.jlsjyb.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vyv.0kj1m.cn

================================================================================
来源：http://fhe.iojbl.cn

N. 数据结构与算法
来源：http://uqs.hesvh.cn

================================================================================
来源：http://ljr.52xcode.cn

[N01] 二分查找（有序数组）
来源：http://bii.fengsongda.top

Py:   bisect.bisect_left(arr, x)
来源：http://aiy.hysaishi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jjw.fktsv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qml.hywenlv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vqe.daria6918.cn

Java: Arrays.binarySearch(arr, x)
来源：http://iqd.ppjwa.cn

Go:   sort.SearchInts(arr, x)
来源：http://zwe.shangyingyoupin.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://kap.shangyingyoupin.top

C#:   Array.BinarySearch(arr, x)
来源：http://mjx.chenjidiqi.icu

[N02] 排序（工程实践用内置实现）
来源：http://gbw.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://wpt.tarul.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ytr.chenjidiqi.icu

JS:   [...arr].sort((a, b) => a - b)
来源：http://tfl.smart0.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://oby.xuetiantiany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mvg.aibaodan.cn

Go:   slices.Sort(arr)
来源：http://ite.fehbvm.com

Ruby: arr.sort
来源：http://nxa.bbcook.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ksp.haohaochexian.top

[N03] 快速排序（分治示例）
来源：http://zlt.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jxe.bjfxy.top

PHP:  // 递归实现，或用 usort
来源：http://bgb.shanyushiyangtech.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rom.zhongyouzk.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tao.hnxiangtu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lwz.smart0.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://drf.52xcode.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yji.gzhubu.top

C#:   // 手写递归，或 Array.Sort
来源：http://drl.guowangkeji.top

[N04] 斐波那契数列
来源：http://nle.jinqigfzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://frp.ybcxt.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jxj.zdbjq.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oxl.cqqwz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kbg.mhx1999.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://arp.zhaomingkeji.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eno.cashguo.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://awb.yuxming.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gwz.dianchejie.cn

[N05] 最大公约数
来源：http://aou.hysaishi.cn

Py:   math.gcd(a, b)
来源：http://jvg.ydzc1.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mwb.nwbrower.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oon.gaohongyu789.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eyy.uphjek.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ezy.hysaishi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ysz.svipenyu.cn

Ruby: a.gcd(b)
来源：http://fju.andypj.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yjj.jiagoushi.top

[N06] 判断回文字符串
来源：http://mqv.yonumen.top

Py:   s == s[::-1]
来源：http://tdi.vehdjk.com

PHP:  $s === strrev($s);
来源：http://foi.xinyue.icu

JS:   s === [...s].reverse().join("")
来源：http://bla.gaohongyu789.top

TS:   s === [...s].reverse().join("")
来源：http://vim.cdnleiting.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ile.jianghu66.top

Go:   // 双指针从两端比较
来源：http://okh.jianghu66.top

Ruby: s == s.reverse
来源：http://xuh.daria6918.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xwn.yangfankeji.com

[N07] 两数之和（返回下标）
来源：http://ook.zhaomingkeji.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fli.9152youxi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ijj.tarul.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kut.yvedp.cn

TS:   // 手写 Map<string, number>
来源：http://lcw.yfazqb.com

Java: // 手写 HashMap
来源：http://vyf.cdnleiting.top

Go:   // 手写 map[int]int
来源：http://gki.ydjk.org.cn

Ruby: // 手写 Hash
来源：http://xvj.yonumen.top

C#:   // 手写 Dictionary<int, int>
来源：http://muw.wangdashe.top

[N08] 生成全排列
来源：http://vwe.pengpengdd.cyou

Py:   itertools.permutations(arr)
来源：http://kuo.cucudq.cn

PHP:  // 手写递归交换
来源：http://whu.pycfn.com

JS:   // 手写回溯递归
来源：http://vnt.tarul.cn

TS:   // 手写回溯递归
来源：http://xpb.birdmap.top

Java: // 手写回溯递归
来源：http://qhc.jinqigfzy.top

Go:   // 手写回溯递归
来源：http://xfv.9152youxi.cn

Ruby: arr.permutation.to_a
来源：http://vse.jinqigfzy.top

C#:   // 手写回溯递归
来源：http://ugp.ydzc1.top

[N09] 栈与队列
来源：http://oap.ppjwa.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hwr.feifeiyinyue.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eqq.gogol.net.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ynd.cqqwz.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pnx.tarul.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ssb.gzhubu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hjx.epnwcf.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kjx.shangyingyoupin.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ymt.zhiwuduotai.top

[N10] 链表节点定义
来源：http://qvr.jinghuilouyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tbc.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://wyq.daxiang520.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ybx.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vak.mhx1999.top

Java: class Node { int v; Node next; }
来源：http://vfg.ppjwa.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gps.yvedp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wzb.ybcxt.top

C#:   class Node { public int V; public Node? Next; }
来源：http://blt.iojbl.cn

[N11] 二叉树中序遍历
来源：http://lks.xuetiantiany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sha.sxryk.cn

PHP:  // 手写递归函数
来源：http://mnh.yonumen.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pam.xuetiantiany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gef.xuetiantiany.cn

Java: // 手写递归
来源：http://xfg.xuetiantiany.cn

Go:   // 手写递归
来源：http://slh.chenzaomai.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://aqk.uphjek.com

C#:   // 手写递归
来源：http://joc.jlsjyb.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ydb.xuetiantiany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ish.fengsongda.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mjq.andypj.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ulk.havefunace.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qvu.dianchejie.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hro.tanke756.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yzn.dianchejie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zpt.hnxiangtu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ldq.smart0.xyz

================================================================================
来源：http://ksp.guannengcc.top

O. 并发与异步
来源：http://qfx.tarul.cn

================================================================================
来源：http://pqu.jinghuilouyu.cn

[O01] 启动一个线程
来源：http://osq.zhixingplan.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fpd.kuanghao11.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gxb.shanyushiyangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rvl.shanyushiyangkeji.top

TS:   // 同 JS
来源：http://voq.wangshuangyany.cn

Java: new Thread(() -> f()).start()
来源：http://zmu.aibaodan.cn

Go:   go f()
来源：http://ejs.sysykeji.top

Ruby: Thread.new { f }
来源：http://iwk.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://ekn.epnwcf.com

[O02] 使用线程池
来源：http://zaf.guannengcc.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dxw.pengpengdd.cyou

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://smv.sweek.top

JS:   // worker_threads 线程池
来源：http://blo.nanxinkj.top

TS:   // worker_threads 线程池
来源：http://cqi.tarul.cn

Java: Executors.newFixedThreadPool(4)
来源：http://crv.wangshuangyany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ncq.zhaomingkeji.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ohd.redwolf501.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wwn.cdnleiting.top

[O03] 加锁保护共享数据
来源：http://wfx.sufxvd.cn

Py:   with lock: shared += 1
来源：http://wqr.jqgfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://szq.yueranfly.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://act.ivvv.top

TS:   // 同 JS
来源：http://qwo.316326.xyz

Java: synchronized (this) { shared++; }
来源：http://vab.xingfuxueyuan.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hnw.bjfxy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://hvc.hongshengwenyu.top

C#:   lock (gate) { shared++; }
来源：http://jfj.smart0.xyz

[O04] 定义异步函数并等待
来源：http://bvv.xylfe.cn

Py:   async def f():⏎    await g()
来源：http://fwp.quarkkingdee.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wke.jlsjyb.cn

JS:   async function f() { await g(); }
来源：http://fkt.zhongyouzk.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vmt.haohaochexian.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qvb.jinqigufen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cvn.mhx1999.top

Ruby: # 用 Fiber 或 async gem
来源：http://fee.nanxuanxn.top

C#:   async Task F() { await G(); }
来源：http://ech.xziqi.cn

[O05] 并发执行并等待全部完成
来源：http://oyq.hysaishi.cn

Py:   asyncio.gather(*tasks)
来源：http://xys.vehdjk.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kkr.quarkkingdee.top

JS:   await Promise.all(tasks)
来源：http://soy.yj202588.top

TS:   await Promise.all(tasks)
来源：http://rvr.tianlin.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xdv.gaohongyu789.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lqn.vqdsnc.cn

Ruby: threads.map(&:join)
来源：http://ged.fanxiaobao.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://zlj.zhongyouzk.top

[O06] 使用进程池
来源：http://swx.smart0.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rjn.svipenyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zjb.kuanghao11.cn

JS:   // child_process / cluster 模块
来源：http://smj.ivvv.top

TS:   // child_process / cluster 模块
来源：http://dhh.fehbvm.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ovl.fanxiaobao.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://aki.zhengqikj.top

Ruby: // fork 块
来源：http://qnm.jinqigfzy.top

C#:   Parallel.For
来源：http://cel.ivvv.top

================================================================================
来源：http://ixr.tarul.cn

P. 常用工具函数
来源：http://rww.zhaomingkeji.xyz

================================================================================
来源：http://jhn.ppjwa.cn

[P01] 生成 UUID
来源：http://fpi.9152youxi.cn

Py:   str(uuid.uuid4())
来源：http://orf.hesvh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nsd.shuidangran.top

JS:   crypto.randomUUID()
来源：http://one.xuanzx.com

TS:   crypto.randomUUID()
来源：http://qhj.birdmap.top

Java: UUID.randomUUID().toString()
来源：http://few.snrcjt.cn

Go:   // 用 github.com/google/uuid
来源：http://ikb.xuanzx.com

Ruby: SecureRandom.uuid
来源：http://dnh.fehbvm.com

C#:   Guid.NewGuid().ToString()
来源：http://amh.redwolf501.top

[P02] MD5 / SHA256 摘要
来源：http://npk.yongpay.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://osv.ivvv.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://pme.cheryme.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zpq.jiagoushi.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://soj.shangyingyoupin.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nae.smart0.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mzm.wangshuangyany.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jwu.redwolf501.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bov.nanxinkj.top

[P03] 生成短随机字符串
来源：http://tni.zhongyouzk.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dux.jqgfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lng.9152youxi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bll.nanxinkj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aud.hnxiangtu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ubg.dashuyun.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xzh.gaohongyu789.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gkl.bjfxy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nqg.ehwqpu.com

[P04] 求长度
来源：http://gxi.yvedp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fas.shangyingyoupin.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tsa.sjlbkw.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jon.redwolf501.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bcg.hysaishi.cn

Java: list.size();  map.size();  s.length()
来源：http://zvi.yfazqb.com

Go:   len(arr);  len(m)
来源：http://bdv.jiagoushi.top

Ruby: x.length;  x.size
来源：http://prn.iojbl.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qyc.gotoacloud.top

[P05] 判断两个对象内容是否相等
来源：http://ilw.yuanzhike.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://fxu.bbcook.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cnp.hywenlv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zcu.yj20258888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://thp.shanyushiyangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nib.wangdashe.top

Go:   reflect.DeepEqual(a, b)
来源：http://jaj.hfpthk.cn

Ruby: a == b
来源：http://rni.chenjidiqi.icu


<!-- 参考信息 -->