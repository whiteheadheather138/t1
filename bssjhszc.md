代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xcb.pengpengdd.cyou

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jqo.yj20258888.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://prw.chenjidiqi.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pun.yuanzhike.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zfd.cucudq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gsm.nanxuanxn.top

================================================================================
来源：http://yqc.yj202588.top

M. 命令行 / 进程 / 环境
来源：http://ugf.ybcxt.top

================================================================================
来源：http://imn.sysykeji.top

[M01] 读取命令行参数
来源：http://wjn.ywan-chungtsiang.top

Py:   sys.argv[1:]
来源：http://wgd.nanxuanxn.top

PHP:  $argv;  $argc;
来源：http://mtt.yangfankeji.com

JS:   process.argv.slice(2)
来源：http://zls.shzxlz.cn

TS:   process.argv.slice(2)
来源：http://hkg.dashuyun.cn

Java: args 数组（main 方法参数）
来源：http://lky.jiagoushi.top

Go:   os.Args[1:]
来源：http://tho.mhx1999.top

Ruby: ARGV
来源：http://qex.zhoulong.xyz

C#:   args 数组（Main 方法参数）
来源：http://len.hammf.cn

[M02] 读取环境变量
来源：http://riv.ctjpmb.com

Py:   os.environ.get("HOME")
来源：http://zfd.guowangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lsq.chenlongwang.top

JS:   process.env.HOME
来源：http://kqw.jqgufenzy.top

TS:   process.env.HOME
来源：http://ign.zhengqikj.top

Java: System.getenv("HOME")
来源：http://zqo.chenzaomai.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zhz.andypj.xyz

Ruby: ENV["HOME"]
来源：http://cjq.quarkkingdee.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rdt.bbcook.cn

[M03] 执行外部命令
来源：http://uaq.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://shy.fktsv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dwh.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://iyr.nanxinkj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://biz.xuanzx.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ffj.jiagoushi.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rnx.gaohongyu789.top

Ruby: system("ls -l");  `ls -l`
来源：http://xsy.snrcjt.cn

C#:   Process.Start("ls", "-l");
来源：http://cnf.pycfn.com

[M04] 获取当前工作目录
来源：http://dwz.sufxvd.cn

Py:   os.getcwd()
来源：http://rba.zhijiandao.cn

PHP:  getcwd();
来源：http://rhi.zycfv.cn

JS:   process.cwd()
来源：http://pyo.xziqi.cn

TS:   process.cwd()
来源：http://rem.yj20258888.top

Java: Path.of("").toAbsolutePath()
来源：http://hno.tanke756.top

Go:   os.Getwd()
来源：http://sgf.nanxinkj.top

Ruby: Dir.pwd
来源：http://nzy.gzhubu.top

C#:   Directory.GetCurrentDirectory()
来源：http://rxt.sxryk.cn

[M05] 设置退出码
来源：http://jgo.sufxvd.cn

Py:   sys.exit(1)
来源：http://gxo.fanxiaobao.xyz

PHP:  exit(1);
来源：http://lei.shanyushiyangkeji.top

JS:   process.exit(1)
来源：http://fqx.fengsongda.top

TS:   process.exit(1)
来源：http://chk.yangfankeji.com

Java: System.exit(1)
来源：http://vxr.nanxuanxn.top

Go:   os.Exit(1)
来源：http://wiq.gotoacloud.top

Ruby: exit 1
来源：http://wch.yongpay.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yah.snrcjt.cn

[M06] 向标准错误输出
来源：http://fcm.ppjwa.cn

Py:   print("err", file=sys.stderr)
来源：http://srg.mhx1999.top

PHP:  fwrite(STDERR, "err\n");
来源：http://mgv.sjlbkw.cn

JS:   console.error("err")
来源：http://kuz.yueranfly.top

TS:   console.error("err")
来源：http://dfp.snrcjt.cn

Java: System.err.println("err")
来源：http://yqn.hnxiangtu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://oyh.ywan-chungtsiang.top

Ruby: warn "err"
来源：http://ppm.zdbjq.cn

C#:   Console.Error.WriteLine("err")
来源：http://ysh.dashuyun.cn

[M07] 判断是否为主入口
来源：http://rds.chenzaomai.com

Py:   if __name__ == "__main__":
来源：http://cew.yfazqb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ifn.9152youxi.cn

JS:   require.main === module
来源：http://ueu.fengsongda.top

TS:   require.main === module
来源：http://zyn.snrcjt.cn

Java: public static void main(String[] args)
来源：http://qxp.daria6918.cn

Go:   func main()
来源：http://zuo.hnxiangtu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://spg.zhixingplan.top

C#:   static void Main(string[] args)
来源：http://gly.ivvv.top

[M08] 获取系统与运行时信息
来源：http://exx.yuxming.cn

Py:   platform.system();  platform.python_version()
来源：http://tsh.iojbl.cn

PHP:  PHP_OS;  phpversion();
来源：http://jbz.yuanzhike.top

JS:   process.platform;  process.version
来源：http://qgz.yanxiufei.cn

TS:   process.platform;  process.version
来源：http://ill.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cfp.zhengqikj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mkc.wangdashe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tqp.snrcjt.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sic.haohaochexian.top

================================================================================
来源：http://boo.0kj1m.cn

N. 数据结构与算法
来源：http://srn.jinqigfzy.top

================================================================================
来源：http://djg.haohaochexian.top

[N01] 二分查找（有序数组）
来源：http://qnz.xylfe.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gqp.sysykeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rxx.xinyue.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eda.9152youxi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://khh.yuanzhike.top

Java: Arrays.binarySearch(arr, x)
来源：http://iks.aizwys.cn

Go:   sort.SearchInts(arr, x)
来源：http://cet.nanxinkj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ued.yuxming.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kxy.gogol.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://bbq.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://ojs.cqqwz.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://clc.ppjwa.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://gch.bjfxy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://yog.zycfv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wrt.zhoulong.xyz

Go:   slices.Sort(arr)
来源：http://ytz.zdqjudy.top

Ruby: arr.sort
来源：http://fcw.guannengcc.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://web.yuanzhike.top

[N03] 快速排序（分治示例）
来源：http://izh.snrcjt.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kwr.gzhubu.top

PHP:  // 递归实现，或用 usort
来源：http://iho.birdmap.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jjy.smart0.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hvf.fengsongda.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nbf.316326.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://avl.gogol.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lcy.xylfe.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tkz.gogol.net.cn

[N04] 斐波那契数列
来源：http://zpe.cqqwz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yov.haohaochexian.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jaj.wangdashe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yyi.kuanghao11.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rwr.hysaishi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bok.havefunace.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://alu.daria6918.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://owb.xingfuxueyuan.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lys.shangyingyoupin.top

[N05] 最大公约数
来源：http://xtm.shangyingyoupin.top

Py:   math.gcd(a, b)
来源：http://txr.snrcjt.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://umy.fehbvm.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://amt.zhoulong.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qoz.hnqzz.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ofj.sxryk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ncy.yanxiufei.cn

Ruby: a.gcd(b)
来源：http://odb.jqgfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cnf.yanxiufei.cn

[N06] 判断回文字符串
来源：http://dvw.yuxming.cn

Py:   s == s[::-1]
来源：http://ctb.yueranfly.top

PHP:  $s === strrev($s);
来源：http://mct.ydjk.org.cn

JS:   s === [...s].reverse().join("")
来源：http://tck.snrcjt.cn

TS:   s === [...s].reverse().join("")
来源：http://ize.ivvv.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xsq.sweek.top

Go:   // 双指针从两端比较
来源：http://qob.cucudq.cn

Ruby: s == s.reverse
来源：http://eyo.yj20258.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wog.yj20258.top

[N07] 两数之和（返回下标）
来源：http://hvb.jinqigfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zxb.hnxiangtu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gye.jinqigfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xjt.shangyingyoupin.top

TS:   // 手写 Map<string, number>
来源：http://khp.cdnleiting.top

Java: // 手写 HashMap
来源：http://cbg.shanyushiyangkeji.top

Go:   // 手写 map[int]int
来源：http://dyl.yangfankeji.com

Ruby: // 手写 Hash
来源：http://hdh.316326.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://qyo.hesvh.cn

[N08] 生成全排列
来源：http://imd.uphjek.com

Py:   itertools.permutations(arr)
来源：http://rkx.xinyue.icu

PHP:  // 手写递归交换
来源：http://cbg.uphjek.com

JS:   // 手写回溯递归
来源：http://ofh.zdqjudy.top

TS:   // 手写回溯递归
来源：http://xmd.yongpay.top

Java: // 手写回溯递归
来源：http://igk.nanxinkj.top

Go:   // 手写回溯递归
来源：http://chm.ctjpmb.com

Ruby: arr.permutation.to_a
来源：http://prk.jyoumei.cn

C#:   // 手写回溯递归
来源：http://qpk.tanke756.top

[N09] 栈与队列
来源：http://ixb.guannengcc.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nib.pengpengdd.cyou

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jbv.gotoacloud.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jsn.mhx1999.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xaf.jiagoushi.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vtp.xingfuxueyuan.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kza.9152youxi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iup.xingfuxueyuan.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yco.daria6918.cn

[N10] 链表节点定义
来源：http://bmr.9152youxi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hqb.redwolf501.top

PHP:  class Node { public $v; public $next = null; }
来源：http://sjb.yj202588.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lxm.quarkkingdee.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mwo.hfpthk.cn

Java: class Node { int v; Node next; }
来源：http://fly.hnxiangtu.top

Go:   type Node struct { V int; Next *Node }
来源：http://jvg.cheryme.top

Ruby: Node = Struct.new(:v, :next)
来源：http://sim.vqdsnc.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ybe.wangdashe.top

[N11] 二叉树中序遍历
来源：http://bnb.shanyushiyangtech.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hcg.guannengcc.top

PHP:  // 手写递归函数
来源：http://tnu.ehwqpu.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aay.fktsv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yrz.sufxvd.cn

Java: // 手写递归
来源：http://kxu.zdqjudy.top

Go:   // 手写递归
来源：http://xlb.xylfe.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mtr.nanxinkj.top

C#:   // 手写递归
来源：http://ckb.hcnkem.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bej.bbcook.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rpi.yuanzhike.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vzx.zdqjudy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cpn.ybcxt.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://efg.jqgufenzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wsi.xylfe.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cya.shuidangran.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gqj.ydzc1.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dyi.tarul.cn

================================================================================
来源：http://iqk.gogol.net.cn

O. 并发与异步
来源：http://jhc.jianghu66.top

================================================================================
来源：http://osn.zhiwuduotai.top

[O01] 启动一个线程
来源：http://sgx.jiagoushi.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mrs.sxryk.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://quh.yonumen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iji.birdmap.top

TS:   // 同 JS
来源：http://swm.guowangkeji.top

Java: new Thread(() -> f()).start()
来源：http://vwz.snrcjt.cn

Go:   go f()
来源：http://sib.yj202588.top

Ruby: Thread.new { f }
来源：http://cir.fktsv.cn

C#:   Task.Run(() => F());
来源：http://ony.jianghu66.top

[O02] 使用线程池
来源：http://fej.ivvv.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vly.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gio.mhx1999.top

JS:   // worker_threads 线程池
来源：http://egj.gzhubu.top

TS:   // worker_threads 线程池
来源：http://gju.jlsjyb.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hwz.fehbvm.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zxw.sjlbkw.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vnd.sxryk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dqh.guowangkeji.top

[O03] 加锁保护共享数据
来源：http://zan.jianghu66.top

Py:   with lock: shared += 1
来源：http://wun.zhaomingkeji.xyz

PHP:  // 用 flock() 做文件锁
来源：http://kgx.zycfv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lvm.fzhhl.top

TS:   // 同 JS
来源：http://fti.fzhhl.top

Java: synchronized (this) { shared++; }
来源：http://urs.smart0.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rqb.andypj.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://mun.0kj1m.cn

C#:   lock (gate) { shared++; }
来源：http://vua.jlsjyb.cn

[O04] 定义异步函数并等待
来源：http://bgc.ydjk.org.cn

Py:   async def f():⏎    await g()
来源：http://awj.hammf.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fdt.shuidangran.top

JS:   async function f() { await g(); }
来源：http://ifm.zhixingplan.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://uvq.gotoacloud.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://noi.zhoulong.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qzx.c1oappe.top

Ruby: # 用 Fiber 或 async gem
来源：http://woq.dashuyun.cn

C#:   async Task F() { await G(); }
来源：http://hcu.ybcxt.top

[O05] 并发执行并等待全部完成
来源：http://cnf.jiagoushi.top

Py:   asyncio.gather(*tasks)
来源：http://fdz.tian-w.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ltm.xinyue.icu

JS:   await Promise.all(tasks)
来源：http://nox.fzhhl.top

TS:   await Promise.all(tasks)
来源：http://fel.ywan-chungtsiang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nmr.sweek.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://slh.xuanzx.com

Ruby: threads.map(&:join)
来源：http://bxq.jinqigfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://rto.hysaishi.cn

[O06] 使用进程池
来源：http://urw.jqgufenzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tyj.yvedp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://plv.zhixingplan.top

JS:   // child_process / cluster 模块
来源：http://bnp.tanke756.top

TS:   // child_process / cluster 模块
来源：http://vnh.tanke756.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://enk.shanyushiyangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jcx.guowangkeji.top

Ruby: // fork 块
来源：http://qvg.yanxiufei.cn

C#:   Parallel.For
来源：http://ber.cdnleiting.top

================================================================================
来源：http://fhi.quarkkingdee.top

P. 常用工具函数
来源：http://cap.jinqigfzy.top

================================================================================
来源：http://equ.chenzaomai.com

[P01] 生成 UUID
来源：http://rxv.vehdjk.com

Py:   str(uuid.uuid4())
来源：http://qjm.tarul.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://opg.ehwqpu.com

JS:   crypto.randomUUID()
来源：http://ons.yvedp.cn

TS:   crypto.randomUUID()
来源：http://ero.hcnkem.com

Java: UUID.randomUUID().toString()
来源：http://qjz.sufxvd.cn

Go:   // 用 github.com/google/uuid
来源：http://qms.sufxvd.cn

Ruby: SecureRandom.uuid
来源：http://qlc.52xcode.cn

C#:   Guid.NewGuid().ToString()
来源：http://ijs.yangfankeji.com

[P02] MD5 / SHA256 摘要
来源：http://wmc.fktsv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://znf.mhx1999.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://mds.yj20258888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://neq.hcnkem.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vcv.hongshengwenyu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://shn.shanyushiyangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fqu.c1oappe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jbu.redwolf501.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vek.zhijiandao.cn

[P03] 生成短随机字符串
来源：http://qyj.gotoacloud.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cvd.zhengqikj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ero.fktsv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kee.nanxinkj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://syj.ydjk.org.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qvi.meibo888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wxl.zhiwuduotai.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://nnw.yj20258888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gbl.9152youxi.cn

[P04] 求长度
来源：http://tlk.jianghu66.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://egd.c1oappe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jkv.tianlin.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://etq.vehdjk.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dkq.zhiwuduotai.top

Java: list.size();  map.size();  s.length()
来源：http://cos.c1oappe.top

Go:   len(arr);  len(m)
来源：http://whg.uphjek.com

Ruby: x.length;  x.size
来源：http://siz.sysykeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dep.ehwqpu.com

[P05] 判断两个对象内容是否相等
来源：http://mja.haohaochexian.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nni.ppjwa.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hje.xinyue.icu

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zki.ctjpmb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nbj.tanke756.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hii.yonumen.top

Go:   reflect.DeepEqual(a, b)
来源：http://rur.zhijiandao.cn

Ruby: a == b
来源：http://yut.andypj.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ido.gzhubu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qby.chenlongwang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qls.hysaishi.cn

PHP:  if (empty($x)) {}
来源：http://smo.cheryme.top


<!-- 参考信息 -->