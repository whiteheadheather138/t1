代发 wailian999

TS:   resp.ok;  resp.status
来源：http://woq.zdbjq.cn

Java: resp.statusCode()
来源：http://uxx.aizwys.cn

Go:   resp.StatusCode
来源：http://ooz.xziqi.cn

Ruby: resp.code.to_i
来源：http://yhb.havefunace.top

C#:   (int)resp.StatusCode
来源：http://zja.wangdashe.top

[L08] 并发请求多个地址
来源：http://rgn.smart0.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://suf.xinyue.icu

PHP:  curl_multi_init() 系列
来源：http://qne.shangyingyoupin.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kuh.pycfn.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sri.hnxiangtu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bdn.shuidangran.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gnm.bbcook.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://acl.shanyushiyangkeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://can.uphjek.com

================================================================================
来源：http://rgp.aizwys.cn

M. 命令行 / 进程 / 环境
来源：http://nmp.zhaomingkeji.xyz

================================================================================
来源：http://gda.ydjk.org.cn

[M01] 读取命令行参数
来源：http://jja.iojbl.cn

Py:   sys.argv[1:]
来源：http://xqn.sweek.top

PHP:  $argv;  $argc;
来源：http://ndy.epnwcf.com

JS:   process.argv.slice(2)
来源：http://dou.svipenyu.cn

TS:   process.argv.slice(2)
来源：http://ztg.smart0.xyz

Java: args 数组（main 方法参数）
来源：http://dgs.shanyushiyangkeji.top

Go:   os.Args[1:]
来源：http://bsu.jianghu66.top

Ruby: ARGV
来源：http://ptb.shangyingyoupin.top

C#:   args 数组（Main 方法参数）
来源：http://qoh.cheryme.top

[M02] 读取环境变量
来源：http://umj.meibo888.top

Py:   os.environ.get("HOME")
来源：http://hci.yanxiufei.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lxe.chenzaomai.com

JS:   process.env.HOME
来源：http://xje.fehbvm.com

TS:   process.env.HOME
来源：http://alw.hesvh.cn

Java: System.getenv("HOME")
来源：http://iqx.xylfe.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://izy.cqqwz.cn

Ruby: ENV["HOME"]
来源：http://gmq.zhijiandao.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://idb.xingfuxueyuan.xyz

[M03] 执行外部命令
来源：http://mlz.iojbl.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zad.havefunace.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vzh.jinghuilouyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://bug.hesvh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://wcf.vqdsnc.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ore.cucudq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wsc.chenlongwang.top

Ruby: system("ls -l");  `ls -l`
来源：http://iku.quarkkingdee.top

C#:   Process.Start("ls", "-l");
来源：http://jqn.jinyuanbaomall.cn

[M04] 获取当前工作目录
来源：http://pjh.316326.xyz

Py:   os.getcwd()
来源：http://ndc.c1oappe.top

PHP:  getcwd();
来源：http://gnb.hnxiangtu.top

JS:   process.cwd()
来源：http://vjm.9152youxi.cn

TS:   process.cwd()
来源：http://myh.cqqwz.cn

Java: Path.of("").toAbsolutePath()
来源：http://sfj.nanxinkj.top

Go:   os.Getwd()
来源：http://fzm.birdmap.top

Ruby: Dir.pwd
来源：http://rol.shuidangran.top

C#:   Directory.GetCurrentDirectory()
来源：http://xbb.hammf.cn

[M05] 设置退出码
来源：http://ujz.hesvh.cn

Py:   sys.exit(1)
来源：http://ejq.epnwcf.com

PHP:  exit(1);
来源：http://tna.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://cvn.svipenyu.cn

TS:   process.exit(1)
来源：http://xsm.birdmap.top

Java: System.exit(1)
来源：http://wrj.feifeiyinyue.top

Go:   os.Exit(1)
来源：http://jxn.xuetiantiany.cn

Ruby: exit 1
来源：http://sac.hongshengwenyu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ojl.xylfe.cn

[M06] 向标准错误输出
来源：http://gds.cucudq.cn

Py:   print("err", file=sys.stderr)
来源：http://ugl.ehwqpu.com

PHP:  fwrite(STDERR, "err\n");
来源：http://buy.cucudq.cn

JS:   console.error("err")
来源：http://nol.nanxuanxn.top

TS:   console.error("err")
来源：http://xtg.yvedp.cn

Java: System.err.println("err")
来源：http://rjz.ywan-chungtsiang.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lux.wangdashe.top

Ruby: warn "err"
来源：http://qku.fanxiaobao.xyz

C#:   Console.Error.WriteLine("err")
来源：http://alt.snrcjt.cn

[M07] 判断是否为主入口
来源：http://zef.hongshengwenyu.top

Py:   if __name__ == "__main__":
来源：http://wso.quarkkingdee.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://juj.zhiwuduotai.top

JS:   require.main === module
来源：http://pfj.vqdsnc.cn

TS:   require.main === module
来源：http://sxn.havefunace.top

Java: public static void main(String[] args)
来源：http://fuw.chenlongwang.top

Go:   func main()
来源：http://ldt.shanyushiyangtech.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://swg.zhaomingkeji.xyz

C#:   static void Main(string[] args)
来源：http://bdt.pycfn.com

[M08] 获取系统与运行时信息
来源：http://wqa.sufxvd.cn

Py:   platform.system();  platform.python_version()
来源：http://xum.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://opj.zycfv.cn

JS:   process.platform;  process.version
来源：http://wnf.chenlongwang.top

TS:   process.platform;  process.version
来源：http://zju.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fmq.jinqigfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://arv.jqgufenzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uvx.tanke756.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lkv.shanyushiyangtech.top

================================================================================
来源：http://tai.andypj.xyz

N. 数据结构与算法
来源：http://ren.gzhubu.top

================================================================================
来源：http://jsb.mhx1999.top

[N01] 二分查找（有序数组）
来源：http://yuw.hammf.cn

Py:   bisect.bisect_left(arr, x)
来源：http://vdx.daria6918.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qdp.yj202588.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sqt.jinyuanbaomall.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pcf.jinqigfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://nco.jinqigufen.top

Go:   sort.SearchInts(arr, x)
来源：http://szh.ybcxt.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://azd.tanke756.top

C#:   Array.BinarySearch(arr, x)
来源：http://dbk.316326.xyz

[N02] 排序（工程实践用内置实现）
来源：http://yxd.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://ura.shzxlz.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://omm.nwbrower.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lwl.fktsv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kkd.fzhhl.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vqx.zdbjq.cn

Go:   slices.Sort(arr)
来源：http://rqb.jianghu66.top

Ruby: arr.sort
来源：http://bvn.sweek.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://owe.chenjidiqi.icu

[N03] 快速排序（分治示例）
来源：http://cjb.kuanghao11.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://prf.yj20258.top

PHP:  // 递归实现，或用 usort
来源：http://tjl.hysaishi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fkr.shuidangran.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mjr.9152youxi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bzc.ppjwa.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zye.sufxvd.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qvc.cheryme.top

C#:   // 手写递归，或 Array.Sort
来源：http://pep.yfazqb.com

[N04] 斐波那契数列
来源：http://uzx.dashuyun.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lmg.zhiwuduotai.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://opf.cheryme.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jwh.zdbjq.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ofa.yvedp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vio.cucudq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://udi.fengsongda.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://frs.fzhhl.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bfq.sysykeji.top

[N05] 最大公约数
来源：http://plo.ctjpmb.com

Py:   math.gcd(a, b)
来源：http://kni.smart0.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pdn.haohaochexian.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qsy.hywenlv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qwx.kuanghao11.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yyz.yj20258.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cdn.xuetiantiany.cn

Ruby: a.gcd(b)
来源：http://fwx.kuanghao11.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://int.cashguo.top

[N06] 判断回文字符串
来源：http://wwq.yj20258.top

Py:   s == s[::-1]
来源：http://sjw.vqdsnc.cn

PHP:  $s === strrev($s);
来源：http://kvp.gotoacloud.top

JS:   s === [...s].reverse().join("")
来源：http://cpz.hfpthk.cn

TS:   s === [...s].reverse().join("")
来源：http://ibk.zhongyouzk.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qxa.cheryme.top

Go:   // 双指针从两端比较
来源：http://tra.shzxlz.cn

Ruby: s == s.reverse
来源：http://rvy.yj20258888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wuu.yonumen.top

[N07] 两数之和（返回下标）
来源：http://vla.gogol.net.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bwd.yueranfly.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rpj.ybcxt.top

JS:   // 手写 Map：map.set(v, i)
来源：http://yhi.uphjek.com

TS:   // 手写 Map<string, number>
来源：http://qud.52xcode.cn

Java: // 手写 HashMap
来源：http://ult.jlsjyb.cn

Go:   // 手写 map[int]int
来源：http://fhg.daria6918.cn

Ruby: // 手写 Hash
来源：http://hsj.yj20258888.top

C#:   // 手写 Dictionary<int, int>
来源：http://ese.xingfuxueyuan.xyz

[N08] 生成全排列
来源：http://bms.yueranfly.top

Py:   itertools.permutations(arr)
来源：http://uay.hammf.cn

PHP:  // 手写递归交换
来源：http://lch.zycfv.cn

JS:   // 手写回溯递归
来源：http://bus.cqqwz.cn

TS:   // 手写回溯递归
来源：http://roa.xinyue.icu

Java: // 手写回溯递归
来源：http://zkf.redwolf501.top

Go:   // 手写回溯递归
来源：http://rgi.aizwys.cn

Ruby: arr.permutation.to_a
来源：http://vos.yuxming.cn

C#:   // 手写回溯递归
来源：http://cqt.birdmap.top

[N09] 栈与队列
来源：http://ibn.yj202588.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hpk.wangshuangyany.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://obz.shangyingyoupin.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dys.tianlin.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hng.ydzc1.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wfl.316326.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jav.uphjek.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mtn.chenzaomai.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iao.fanxiaobao.xyz

[N10] 链表节点定义
来源：http://aos.tarul.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hby.ppjwa.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://zpc.hongshengwenyu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mxc.cdnleiting.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oef.chenlongwang.top

Java: class Node { int v; Node next; }
来源：http://zzm.cashguo.top

Go:   type Node struct { V int; Next *Node }
来源：http://nml.sweek.top

Ruby: Node = Struct.new(:v, :next)
来源：http://fcx.yueranfly.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ulp.nanxuanxn.top

[N11] 二叉树中序遍历
来源：http://fhf.cqqwz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hgp.xingfuxueyuan.xyz

PHP:  // 手写递归函数
来源：http://pgc.hongshengwenyu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hgn.bbcook.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bik.gogol.net.cn

Java: // 手写递归
来源：http://rhh.jqgufenzy.top

Go:   // 手写递归
来源：http://ijs.andypj.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wlw.ctjpmb.com

C#:   // 手写递归
来源：http://nqa.bbcook.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://brs.tanke756.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oww.tianlin.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wbi.aizwys.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zqk.zhijiandao.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aic.smart0.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pyw.gzhubu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bkv.mhx1999.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qxl.shanyushiyangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pwq.yj20258.top

================================================================================
来源：http://dsd.cheryme.top

O. 并发与异步
来源：http://bmv.cdnleiting.top

================================================================================
来源：http://tax.sxryk.cn

[O01] 启动一个线程
来源：http://ufz.vqdsnc.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://umv.wangdashe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ccf.aizwys.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ypt.fktsv.cn

TS:   // 同 JS
来源：http://jbu.redwolf501.top

Java: new Thread(() -> f()).start()
来源：http://uhg.jinqigfzy.top

Go:   go f()
来源：http://jsh.yongpay.top

Ruby: Thread.new { f }
来源：http://wpd.bbcook.cn

C#:   Task.Run(() => F());
来源：http://dxh.guowangkeji.top

[O02] 使用线程池
来源：http://rrp.sysykeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dae.yangfankeji.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ggg.jqgfzy.top

JS:   // worker_threads 线程池
来源：http://knd.gotoacloud.top

TS:   // worker_threads 线程池
来源：http://drx.gzhubu.top

Java: Executors.newFixedThreadPool(4)
来源：http://ppa.iojbl.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lbz.xuetiantiany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pic.xuanzx.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://raz.hongshengwenyu.top

[O03] 加锁保护共享数据
来源：http://eaa.wangshuangyany.cn

Py:   with lock: shared += 1
来源：http://ndm.yueranfly.top

PHP:  // 用 flock() 做文件锁
来源：http://inr.guowangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fih.hcnkem.com

TS:   // 同 JS
来源：http://caf.smart0.xyz

Java: synchronized (this) { shared++; }
来源：http://zuk.yuxming.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blm.fzhhl.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://aog.nanxinkj.top

C#:   lock (gate) { shared++; }
来源：http://lgf.tianlin.xyz

[O04] 定义异步函数并等待
来源：http://xhs.zhongyouzk.top

Py:   async def f():⏎    await g()
来源：http://zpa.tian-w.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cgb.fanxiaobao.xyz

JS:   async function f() { await g(); }
来源：http://shl.yuxming.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zte.birdmap.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://reh.zhaomingkeji.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dme.cucudq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ear.bbcook.cn

C#:   async Task F() { await G(); }
来源：http://hbn.fengsongda.top

[O05] 并发执行并等待全部完成
来源：http://jgo.jiagoushi.top

Py:   asyncio.gather(*tasks)
来源：http://ktw.fktsv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rbv.ivvv.top

JS:   await Promise.all(tasks)
来源：http://bod.sweek.top

TS:   await Promise.all(tasks)
来源：http://okc.jqgfzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lpw.fktsv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vpr.jyoumei.cn

Ruby: threads.map(&:join)
来源：http://raz.iojbl.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kbx.zdbjq.cn

[O06] 使用进程池
来源：http://kci.sufxvd.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qdl.tarul.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qgi.hywenlv.cn

JS:   // child_process / cluster 模块
来源：http://soc.ppjwa.cn

TS:   // child_process / cluster 模块
来源：http://nsv.hnqzz.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fqh.zdbjq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blc.sweek.top

Ruby: // fork 块
来源：http://ice.tanke756.top

C#:   Parallel.For
来源：http://qpd.gogol.net.cn

================================================================================
来源：http://gvh.shanyushiyangtech.top

P. 常用工具函数
来源：http://avi.guowangkeji.top

================================================================================
来源：http://itw.jqgfzy.top

[P01] 生成 UUID
来源：http://tna.ppjwa.cn

Py:   str(uuid.uuid4())
来源：http://arf.guannengcc.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://geq.gzhubu.top

JS:   crypto.randomUUID()
来源：http://dpt.chenlongwang.top

TS:   crypto.randomUUID()
来源：http://jxc.havefunace.top

Java: UUID.randomUUID().toString()
来源：http://suw.zhengqikj.top

Go:   // 用 github.com/google/uuid
来源：http://qjp.tianlin.xyz

Ruby: SecureRandom.uuid
来源：http://mzy.jinyuanbaomall.cn

C#:   Guid.NewGuid().ToString()
来源：http://ggd.dianchejie.cn

[P02] MD5 / SHA256 摘要
来源：http://dar.vehdjk.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vwc.hfpthk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dni.nwbrower.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://icp.ywan-chungtsiang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://klc.xziqi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://srx.yj20258888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mjg.yueranfly.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dma.hesvh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lqc.guowangkeji.top

[P03] 生成短随机字符串
来源：http://fgt.xuanzx.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lpl.bbcook.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nlx.jinyuanbaomall.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://you.smart0.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://red.zhengqikj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dds.daxiang520.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ksh.jianghu66.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gtr.sweek.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://myk.yfazqb.com

[P04] 求长度
来源：http://bov.zhengqikj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ldr.svipenyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://idc.zhijiandao.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fvz.fktsv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kpz.fzhhl.top

Java: list.size();  map.size();  s.length()
来源：http://mqt.jqgufenzy.top

Go:   len(arr);  len(m)
来源：http://hqe.hysaishi.cn

Ruby: x.length;  x.size
来源：http://bpm.smart0.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://esc.chenzaomai.com

[P05] 判断两个对象内容是否相等
来源：http://lvy.sufxvd.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vvh.feifeiyinyue.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cjk.jianghu66.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ltl.0kj1m.cn


<!-- 参考信息 -->