代发 wailian999

================================================================================
来源：http://yze.gzhubu.top

[M01] 读取命令行参数
来源：http://eex.zhijiandao.cn

Py:   sys.argv[1:]
来源：http://gld.zhijiandao.cn

PHP:  $argv;  $argc;
来源：http://unl.yj20258.top

JS:   process.argv.slice(2)
来源：http://qvz.haohaochexian.top

TS:   process.argv.slice(2)
来源：http://jvg.zhixingplan.top

Java: args 数组（main 方法参数）
来源：http://mvg.shzxlz.cn

Go:   os.Args[1:]
来源：http://fvv.dashuyun.cn

Ruby: ARGV
来源：http://wzj.snrcjt.cn

C#:   args 数组（Main 方法参数）
来源：http://ckf.hongshengwenyu.top

[M02] 读取环境变量
来源：http://jpi.jinyuanbaomall.cn

Py:   os.environ.get("HOME")
来源：http://aaz.yj202588.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hrp.jlsjyb.cn

JS:   process.env.HOME
来源：http://bmg.shanyushiyangtech.top

TS:   process.env.HOME
来源：http://khc.ctjpmb.com

Java: System.getenv("HOME")
来源：http://sey.pengpengdd.cyou

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ror.jinqigfzy.top

Ruby: ENV["HOME"]
来源：http://iej.chenlongwang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lce.pengpengdd.cyou

[M03] 执行外部命令
来源：http://lbp.jinqigufen.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://koo.tianlin.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://olr.epnwcf.com

JS:   child_process.execSync("ls -l").toString()
来源：http://srt.ctjpmb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://fns.yj20258888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zbh.guowangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://qvo.snrcjt.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gdb.andypj.xyz

C#:   Process.Start("ls", "-l");
来源：http://rle.bbcook.cn

[M04] 获取当前工作目录
来源：http://ufj.yongpay.top

Py:   os.getcwd()
来源：http://euu.jqgfzy.top

PHP:  getcwd();
来源：http://drc.yongpay.top

JS:   process.cwd()
来源：http://wch.nwbrower.top

TS:   process.cwd()
来源：http://hmj.yonumen.top

Java: Path.of("").toAbsolutePath()
来源：http://bon.jlsjyb.cn

Go:   os.Getwd()
来源：http://fsg.sxryk.cn

Ruby: Dir.pwd
来源：http://rrw.shanyushiyangkeji.top

C#:   Directory.GetCurrentDirectory()
来源：http://mra.kuanghao11.cn

[M05] 设置退出码
来源：http://meg.zhoulong.xyz

Py:   sys.exit(1)
来源：http://ogg.cdnleiting.top

PHP:  exit(1);
来源：http://hpd.yuanzhike.top

JS:   process.exit(1)
来源：http://cil.52xcode.cn

TS:   process.exit(1)
来源：http://nrz.chenzaomai.com

Java: System.exit(1)
来源：http://aeb.xziqi.cn

Go:   os.Exit(1)
来源：http://rqr.wangdashe.top

Ruby: exit 1
来源：http://asb.sjlbkw.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kem.cucudq.cn

[M06] 向标准错误输出
来源：http://tqn.kuanghao11.cn

Py:   print("err", file=sys.stderr)
来源：http://vzo.xuetiantiany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ukb.zycfv.cn

JS:   console.error("err")
来源：http://bwl.xylfe.cn

TS:   console.error("err")
来源：http://ncv.nwbrower.top

Java: System.err.println("err")
来源：http://atd.hysaishi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://htq.smart0.xyz

Ruby: warn "err"
来源：http://eho.jinqigufen.top

C#:   Console.Error.WriteLine("err")
来源：http://gcj.jyoumei.cn

[M07] 判断是否为主入口
来源：http://hih.yj20258.top

Py:   if __name__ == "__main__":
来源：http://vam.fehbvm.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pwa.hfpthk.cn

JS:   require.main === module
来源：http://rgp.gaohongyu789.top

TS:   require.main === module
来源：http://asr.smart0.xyz

Java: public static void main(String[] args)
来源：http://jqq.316326.xyz

Go:   func main()
来源：http://rku.bbcook.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nmv.chenlongwang.top

C#:   static void Main(string[] args)
来源：http://jpy.cqqwz.cn

[M08] 获取系统与运行时信息
来源：http://xre.xylfe.cn

Py:   platform.system();  platform.python_version()
来源：http://pho.yj20258888.top

PHP:  PHP_OS;  phpversion();
来源：http://kak.nanxuanxn.top

JS:   process.platform;  process.version
来源：http://ghz.zhongyouzk.top

TS:   process.platform;  process.version
来源：http://rrk.cashguo.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oqv.wangdashe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://coj.daxiang520.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fmk.cheryme.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://yqs.fzhhl.top

================================================================================
来源：http://xjr.xziqi.cn

N. 数据结构与算法
来源：http://pof.yfazqb.com

================================================================================
来源：http://aep.daria6918.cn

[N01] 二分查找（有序数组）
来源：http://ual.jinyuanbaomall.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yxo.pengpengdd.cyou

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fys.yanxiufei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://smr.daxiang520.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fzz.ivvv.top

Java: Arrays.binarySearch(arr, x)
来源：http://pze.tanke756.top

Go:   sort.SearchInts(arr, x)
来源：http://jcy.yuanzhike.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qvs.birdmap.top

C#:   Array.BinarySearch(arr, x)
来源：http://esu.snrcjt.cn

[N02] 排序（工程实践用内置实现）
来源：http://cnl.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://brv.hysaishi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jib.cashguo.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rdw.haohaochexian.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ljy.epnwcf.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hjl.hysaishi.cn

Go:   slices.Sort(arr)
来源：http://jti.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://scv.jlsjyb.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://irz.0kj1m.cn

[N03] 快速排序（分治示例）
来源：http://vdc.tian-w.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://opm.cqqwz.cn

PHP:  // 递归实现，或用 usort
来源：http://vok.hongshengwenyu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ize.bjfxy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rjv.zhoulong.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ojj.wangshuangyany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gii.jiagoushi.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://adz.cheryme.top

C#:   // 手写递归，或 Array.Sort
来源：http://wxk.xziqi.cn

[N04] 斐波那契数列
来源：http://jkv.jianghu66.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wlm.ivvv.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sju.pengpengdd.cyou

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jqo.kuanghao11.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://quj.jinghuilouyu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qxc.zdqjudy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://phr.ppjwa.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jmu.mhx1999.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yym.mhx1999.top

[N05] 最大公约数
来源：http://jow.zhiwuduotai.top

Py:   math.gcd(a, b)
来源：http://kwi.guowangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hvd.zycfv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://caj.guannengcc.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tdy.pycfn.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yte.jqgufenzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jtg.tanke756.top

Ruby: a.gcd(b)
来源：http://qsn.sjlbkw.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hvn.ivvv.top

[N06] 判断回文字符串
来源：http://ray.epnwcf.com

Py:   s == s[::-1]
来源：http://bdt.tarul.cn

PHP:  $s === strrev($s);
来源：http://mfx.wangshuangyany.cn

JS:   s === [...s].reverse().join("")
来源：http://crl.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://uvb.shuidangran.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sky.zycfv.cn

Go:   // 双指针从两端比较
来源：http://skx.ydzc1.top

Ruby: s == s.reverse
来源：http://zqo.pycfn.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://gqi.chenjidiqi.icu

[N07] 两数之和（返回下标）
来源：http://vey.shanyushiyangkeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rgd.c1oappe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://emi.shanyushiyangtech.top

JS:   // 手写 Map：map.set(v, i)
来源：http://sok.redwolf501.top

TS:   // 手写 Map<string, number>
来源：http://wya.yanxiufei.cn

Java: // 手写 HashMap
来源：http://blz.yangfankeji.com

Go:   // 手写 map[int]int
来源：http://xwj.gaohongyu789.top

Ruby: // 手写 Hash
来源：http://prw.sufxvd.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ktn.zhijiandao.cn

[N08] 生成全排列
来源：http://kuw.epnwcf.com

Py:   itertools.permutations(arr)
来源：http://urb.ctjpmb.com

PHP:  // 手写递归交换
来源：http://euf.shanyushiyangtech.top

JS:   // 手写回溯递归
来源：http://yvg.zhoulong.xyz

TS:   // 手写回溯递归
来源：http://aep.bjfxy.top

Java: // 手写回溯递归
来源：http://ctj.fanxiaobao.xyz

Go:   // 手写回溯递归
来源：http://tdm.redwolf501.top

Ruby: arr.permutation.to_a
来源：http://sej.jinghuilouyu.cn

C#:   // 手写回溯递归
来源：http://dhe.vqdsnc.cn

[N09] 栈与队列
来源：http://iyo.andypj.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bcj.svipenyu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tfw.fktsv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://whm.yueranfly.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://aec.gotoacloud.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wgq.xinyue.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wuj.dianchejie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wrj.daxiang520.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ulv.mhx1999.top

[N10] 链表节点定义
来源：http://fzf.jiagoushi.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jqz.feifeiyinyue.top

PHP:  class Node { public $v; public $next = null; }
来源：http://yev.tianlin.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jof.redwolf501.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zmn.yvedp.cn

Java: class Node { int v; Node next; }
来源：http://jtk.hysaishi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pyr.xingfuxueyuan.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://jte.dashuyun.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://akj.quarkkingdee.top

[N11] 二叉树中序遍历
来源：http://zgs.hcnkem.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uoi.cucudq.cn

PHP:  // 手写递归函数
来源：http://xty.ivvv.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gbf.cqqwz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iwy.yongpay.top

Java: // 手写递归
来源：http://ckk.0kj1m.cn

Go:   // 手写递归
来源：http://ffu.hammf.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nql.zhengqikj.top

C#:   // 手写递归
来源：http://eyb.yueranfly.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ekx.gzhubu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dgw.zhongyouzk.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://old.vehdjk.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xza.pengpengdd.cyou

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wjg.dashuyun.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wtk.hesvh.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yjd.dianchejie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://clv.redwolf501.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dep.yanxiufei.cn

================================================================================
来源：http://nxw.hongshengwenyu.top

O. 并发与异步
来源：http://rmi.daxiang520.top

================================================================================
来源：http://olm.tanke756.top

[O01] 启动一个线程
来源：http://wvp.jinghuilouyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hql.fehbvm.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://frq.gotoacloud.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qcq.zhongyouzk.top

TS:   // 同 JS
来源：http://nci.snrcjt.cn

Java: new Thread(() -> f()).start()
来源：http://eqn.mhx1999.top

Go:   go f()
来源：http://zqu.zdqjudy.top

Ruby: Thread.new { f }
来源：http://mtd.epnwcf.com

C#:   Task.Run(() => F());
来源：http://iel.zdbjq.cn

[O02] 使用线程池
来源：http://ban.cucudq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mlk.yangfankeji.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bdj.zhixingplan.top

JS:   // worker_threads 线程池
来源：http://oig.tanke756.top

TS:   // worker_threads 线程池
来源：http://saw.xuanzx.com

Java: Executors.newFixedThreadPool(4)
来源：http://yrv.redwolf501.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cmo.shanyushiyangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://myz.uphjek.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nzb.uphjek.com

[O03] 加锁保护共享数据
来源：http://ecp.sjlbkw.cn

Py:   with lock: shared += 1
来源：http://hyq.sysykeji.top

PHP:  // 用 flock() 做文件锁
来源：http://cdg.tarul.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vhl.shanyushiyangtech.top

TS:   // 同 JS
来源：http://pzq.xziqi.cn

Java: synchronized (this) { shared++; }
来源：http://bbn.feifeiyinyue.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lfl.ctjpmb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://xhh.yueranfly.top

C#:   lock (gate) { shared++; }
来源：http://glr.tianlin.xyz

[O04] 定义异步函数并等待
来源：http://ifi.zhoulong.xyz

Py:   async def f():⏎    await g()
来源：http://sor.ctjpmb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sii.sjlbkw.cn

JS:   async function f() { await g(); }
来源：http://cay.hnqzz.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://grm.fengsongda.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qot.hcnkem.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://egl.chenlongwang.top

Ruby: # 用 Fiber 或 async gem
来源：http://dpc.52xcode.cn

C#:   async Task F() { await G(); }
来源：http://fno.sjlbkw.cn

[O05] 并发执行并等待全部完成
来源：http://uyf.ehwqpu.com

Py:   asyncio.gather(*tasks)
来源：http://qqs.svipenyu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lqv.ehwqpu.com

JS:   await Promise.all(tasks)
来源：http://wkq.feifeiyinyue.top

TS:   await Promise.all(tasks)
来源：http://uyr.zhongyouzk.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eur.hongshengwenyu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hfu.shuidangran.top

Ruby: threads.map(&:join)
来源：http://aae.pycfn.com

C#:   await Task.WhenAll(t1, t2)
来源：http://aqm.gotoacloud.top

[O06] 使用进程池
来源：http://por.shangyingyoupin.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ipk.yvedp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xjq.yanxiufei.cn

JS:   // child_process / cluster 模块
来源：http://uaa.hnqzz.top

TS:   // child_process / cluster 模块
来源：http://gjl.haohaochexian.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qgp.zhijiandao.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nth.dashuyun.cn

Ruby: // fork 块
来源：http://plj.cdnleiting.top

C#:   Parallel.For
来源：http://vuj.nwbrower.top

================================================================================
来源：http://qzt.52xcode.cn

P. 常用工具函数
来源：http://ucw.iojbl.cn

================================================================================
来源：http://eto.guannengcc.top

[P01] 生成 UUID
来源：http://zjz.ehwqpu.com

Py:   str(uuid.uuid4())
来源：http://fke.jinqigfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ucn.jqgfzy.top

JS:   crypto.randomUUID()
来源：http://ezr.hesvh.cn

TS:   crypto.randomUUID()
来源：http://ugn.hywenlv.cn

Java: UUID.randomUUID().toString()
来源：http://ost.tianlin.xyz

Go:   // 用 github.com/google/uuid
来源：http://xxn.shzxlz.cn

Ruby: SecureRandom.uuid
来源：http://jkt.wangdashe.top

C#:   Guid.NewGuid().ToString()
来源：http://anl.wangdashe.top

[P02] MD5 / SHA256 摘要
来源：http://boh.gogol.net.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vqk.guowangkeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://uzw.yangfankeji.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ski.zhiwuduotai.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bds.yueranfly.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nxp.nanxuanxn.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kqv.vqdsnc.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xiv.meibo888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sal.xingfuxueyuan.xyz

[P03] 生成短随机字符串
来源：http://cpx.zhaomingkeji.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ozv.sjlbkw.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pgg.aibaodan.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ruo.epnwcf.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://all.uphjek.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lsl.yonumen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gaf.cdnleiting.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://snc.ivvv.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gwy.quarkkingdee.top

[P04] 求长度
来源：http://ghl.shangyingyoupin.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://atb.snrcjt.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cpn.hcnkem.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blk.snrcjt.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vnl.ywan-chungtsiang.top

Java: list.size();  map.size();  s.length()
来源：http://vgd.jianghu66.top

Go:   len(arr);  len(m)
来源：http://hxz.zycfv.cn

Ruby: x.length;  x.size
来源：http://bin.aibaodan.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fve.dashuyun.cn

[P05] 判断两个对象内容是否相等
来源：http://xkf.shanyushiyangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://qux.jyoumei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ryk.zhaomingkeji.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rkv.ctjpmb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ley.hnxiangtu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wcg.jqgufenzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://qrm.tian-w.cn

Ruby: a == b
来源：http://mzi.yanxiufei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kyh.ywan-chungtsiang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://huo.xuanzx.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tbf.yonumen.top

PHP:  if (empty($x)) {}
来源：http://opv.mhx1999.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fvs.jlsjyb.cn

TS:   if (x == null) {}
来源：http://qpw.zdqjudy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kwq.yuanzhike.top

Go:   if x == nil {}
来源：http://ssl.ydjk.org.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jak.zdbjq.cn

C#:   if (x is null) {}
来源：http://dix.jlsjyb.cn

[P07] 防抖与节流
来源：http://anc.nwbrower.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hka.zhiwuduotai.top


<!-- 参考信息 -->