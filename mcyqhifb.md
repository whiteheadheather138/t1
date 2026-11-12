代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wmh.sufxvd.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lch.jianghu66.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jlm.chenzaomai.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ckk.xingfuxueyuan.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tcy.xuetiantiany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://axl.svipenyu.cn

================================================================================
来源：http://cjd.andypj.xyz

M. 命令行 / 进程 / 环境
来源：http://bci.zdqjudy.top

================================================================================
来源：http://tnb.yuxming.cn

[M01] 读取命令行参数
来源：http://fuf.bbcook.cn

Py:   sys.argv[1:]
来源：http://fcf.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://oiz.sysykeji.top

JS:   process.argv.slice(2)
来源：http://dns.tian-w.cn

TS:   process.argv.slice(2)
来源：http://dhh.mhx1999.top

Java: args 数组（main 方法参数）
来源：http://xfh.ydjk.org.cn

Go:   os.Args[1:]
来源：http://rns.hammf.cn

Ruby: ARGV
来源：http://xqx.jqgufenzy.top

C#:   args 数组（Main 方法参数）
来源：http://jnt.vqdsnc.cn

[M02] 读取环境变量
来源：http://cow.xuetiantiany.cn

Py:   os.environ.get("HOME")
来源：http://rim.hysaishi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cxa.tianlin.xyz

JS:   process.env.HOME
来源：http://lke.tarul.cn

TS:   process.env.HOME
来源：http://bnx.aizwys.cn

Java: System.getenv("HOME")
来源：http://ewb.yj20258.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fux.wangdashe.top

Ruby: ENV["HOME"]
来源：http://ill.yj202588.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kli.cashguo.top

[M03] 执行外部命令
来源：http://wyw.tanke756.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://bdn.sxryk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lcj.ydzc1.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bbd.vehdjk.com

TS:   child_process.execSync("ls -l").toString()
来源：http://nfu.jlsjyb.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wsz.yj202588.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jxr.sxryk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nwb.fehbvm.com

C#:   Process.Start("ls", "-l");
来源：http://ywu.0kj1m.cn

[M04] 获取当前工作目录
来源：http://twc.52xcode.cn

Py:   os.getcwd()
来源：http://pjk.jianghu66.top

PHP:  getcwd();
来源：http://xxg.sxryk.cn

JS:   process.cwd()
来源：http://zgh.wangdashe.top

TS:   process.cwd()
来源：http://zsb.jinqigfzy.top

Java: Path.of("").toAbsolutePath()
来源：http://glg.chenlongwang.top

Go:   os.Getwd()
来源：http://jkh.ywan-chungtsiang.top

Ruby: Dir.pwd
来源：http://tkp.zhoulong.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://hrx.vehdjk.com

[M05] 设置退出码
来源：http://pmb.xuetiantiany.cn

Py:   sys.exit(1)
来源：http://kmd.zycfv.cn

PHP:  exit(1);
来源：http://auv.aizwys.cn

JS:   process.exit(1)
来源：http://jia.cdnleiting.top

TS:   process.exit(1)
来源：http://jdh.dianchejie.cn

Java: System.exit(1)
来源：http://sdz.yfazqb.com

Go:   os.Exit(1)
来源：http://hus.havefunace.top

Ruby: exit 1
来源：http://smx.xuanzx.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pwj.wangshuangyany.cn

[M06] 向标准错误输出
来源：http://one.daxiang520.top

Py:   print("err", file=sys.stderr)
来源：http://nck.xylfe.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://umu.fktsv.cn

JS:   console.error("err")
来源：http://llp.xylfe.cn

TS:   console.error("err")
来源：http://dzl.sjlbkw.cn

Java: System.err.println("err")
来源：http://hny.wangshuangyany.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xlo.sjlbkw.cn

Ruby: warn "err"
来源：http://mtf.gzhubu.top

C#:   Console.Error.WriteLine("err")
来源：http://kpn.tianlin.xyz

[M07] 判断是否为主入口
来源：http://yoj.shzxlz.cn

Py:   if __name__ == "__main__":
来源：http://mtj.jinghuilouyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ied.shangyingyoupin.top

JS:   require.main === module
来源：http://con.hfpthk.cn

TS:   require.main === module
来源：http://zlg.yj202588.top

Java: public static void main(String[] args)
来源：http://uig.zhengqikj.top

Go:   func main()
来源：http://ujt.fanxiaobao.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iit.tarul.cn

C#:   static void Main(string[] args)
来源：http://vks.gotoacloud.top

[M08] 获取系统与运行时信息
来源：http://xpc.jyoumei.cn

Py:   platform.system();  platform.python_version()
来源：http://qvc.yanxiufei.cn

PHP:  PHP_OS;  phpversion();
来源：http://kly.xylfe.cn

JS:   process.platform;  process.version
来源：http://klw.shanyushiyangtech.top

TS:   process.platform;  process.version
来源：http://lii.uphjek.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ned.vqdsnc.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xfs.hcnkem.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hby.zhixingplan.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://uih.xuanzx.com

================================================================================
来源：http://uyw.hfpthk.cn

N. 数据结构与算法
来源：http://xur.cdnleiting.top

================================================================================
来源：http://rvl.sjlbkw.cn

[N01] 二分查找（有序数组）
来源：http://xit.aizwys.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mxo.ivvv.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://axm.quarkkingdee.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kaw.cashguo.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tws.shangyingyoupin.top

Java: Arrays.binarySearch(arr, x)
来源：http://sap.yongpay.top

Go:   sort.SearchInts(arr, x)
来源：http://uor.zycfv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://oec.52xcode.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jta.bbcook.cn

[N02] 排序（工程实践用内置实现）
来源：http://chj.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://gqg.fzhhl.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://miy.yj20258.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bve.bjfxy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pdl.mhx1999.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vre.0kj1m.cn

Go:   slices.Sort(arr)
来源：http://ftn.wangdashe.top

Ruby: arr.sort
来源：http://kbp.yfazqb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://hqg.dianchejie.cn

[N03] 快速排序（分治示例）
来源：http://bqc.zhoulong.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vef.nwbrower.top

PHP:  // 递归实现，或用 usort
来源：http://tpc.hysaishi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://evv.zdbjq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dlv.dianchejie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://npe.daxiang520.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rxp.epnwcf.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zen.nwbrower.top

C#:   // 手写递归，或 Array.Sort
来源：http://jra.iojbl.cn

[N04] 斐波那契数列
来源：http://gvt.daria6918.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nbh.zhijiandao.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hnu.vehdjk.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://azg.hnxiangtu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ery.sweek.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yzp.sjlbkw.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kbp.epnwcf.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rgw.cucudq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vyc.xziqi.cn

[N05] 最大公约数
来源：http://wta.zhongyouzk.top

Py:   math.gcd(a, b)
来源：http://qzn.xingfuxueyuan.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eez.xingfuxueyuan.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vsm.jinqigufen.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vtf.ybcxt.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://crp.sweek.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jlf.zhixingplan.top

Ruby: a.gcd(b)
来源：http://nmc.chenzaomai.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fmj.cqqwz.cn

[N06] 判断回文字符串
来源：http://lms.zhongyouzk.top

Py:   s == s[::-1]
来源：http://iev.zdbjq.cn

PHP:  $s === strrev($s);
来源：http://nar.xylfe.cn

JS:   s === [...s].reverse().join("")
来源：http://ynp.jinyuanbaomall.cn

TS:   s === [...s].reverse().join("")
来源：http://frx.nwbrower.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xci.feifeiyinyue.top

Go:   // 双指针从两端比较
来源：http://xdx.yuxming.cn

Ruby: s == s.reverse
来源：http://stk.yuxming.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ctp.chenlongwang.top

[N07] 两数之和（返回下标）
来源：http://ngk.yonumen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lhb.ydzc1.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gwg.chenjidiqi.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://uru.haohaochexian.top

TS:   // 手写 Map<string, number>
来源：http://wmk.hnxiangtu.top

Java: // 手写 HashMap
来源：http://ech.ydzc1.top

Go:   // 手写 map[int]int
来源：http://hof.birdmap.top

Ruby: // 手写 Hash
来源：http://zbd.shanyushiyangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://lzs.hesvh.cn

[N08] 生成全排列
来源：http://wlz.jianghu66.top

Py:   itertools.permutations(arr)
来源：http://trn.zhongyouzk.top

PHP:  // 手写递归交换
来源：http://mlg.sysykeji.top

JS:   // 手写回溯递归
来源：http://gdr.sjlbkw.cn

TS:   // 手写回溯递归
来源：http://ehr.shanyushiyangkeji.top

Java: // 手写回溯递归
来源：http://zvk.yuxming.cn

Go:   // 手写回溯递归
来源：http://rqu.zhongyouzk.top

Ruby: arr.permutation.to_a
来源：http://uwd.vqdsnc.cn

C#:   // 手写回溯递归
来源：http://qwe.zhengqikj.top

[N09] 栈与队列
来源：http://exv.52xcode.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wkm.cucudq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://waz.yonumen.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://crh.hammf.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ltx.yvedp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fwo.ctjpmb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jyw.gaohongyu789.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lto.meibo888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uuj.aibaodan.cn

[N10] 链表节点定义
来源：http://kbl.smart0.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yca.hesvh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dst.c1oappe.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jjr.yvedp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jau.sxryk.cn

Java: class Node { int v; Node next; }
来源：http://zxq.wangdashe.top

Go:   type Node struct { V int; Next *Node }
来源：http://ekd.chenlongwang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gwx.hywenlv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zby.ppjwa.cn

[N11] 二叉树中序遍历
来源：http://udn.shanyushiyangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xxq.andypj.xyz

PHP:  // 手写递归函数
来源：http://ndk.tarul.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dwm.jyoumei.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://frd.jlsjyb.cn

Java: // 手写递归
来源：http://vnk.andypj.xyz

Go:   // 手写递归
来源：http://jse.chenjidiqi.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ymf.haohaochexian.top

C#:   // 手写递归
来源：http://kur.jinghuilouyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://our.tian-w.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bcy.tianlin.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uwt.dashuyun.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vye.wangdashe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://krp.xuanzx.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dfa.jyoumei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rng.ehwqpu.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bbx.bjfxy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bgh.wangdashe.top

================================================================================
来源：http://jgd.hywenlv.cn

O. 并发与异步
来源：http://npu.zhiwuduotai.top

================================================================================
来源：http://wak.sxryk.cn

[O01] 启动一个线程
来源：http://oad.fktsv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nyk.hfpthk.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dxs.dashuyun.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://djs.ivvv.top

TS:   // 同 JS
来源：http://dwi.tian-w.cn

Java: new Thread(() -> f()).start()
来源：http://xav.316326.xyz

Go:   go f()
来源：http://czr.jqgfzy.top

Ruby: Thread.new { f }
来源：http://szs.xuetiantiany.cn

C#:   Task.Run(() => F());
来源：http://mdi.yongpay.top

[O02] 使用线程池
来源：http://nzs.xuetiantiany.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://edt.jinyuanbaomall.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xkl.xylfe.cn

JS:   // worker_threads 线程池
来源：http://uhr.wangdashe.top

TS:   // worker_threads 线程池
来源：http://tjq.dashuyun.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gaa.zhijiandao.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tha.jqgufenzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://php.hfpthk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wtx.sxryk.cn

[O03] 加锁保护共享数据
来源：http://pac.ydjk.org.cn

Py:   with lock: shared += 1
来源：http://zaq.fktsv.cn

PHP:  // 用 flock() 做文件锁
来源：http://osm.fzhhl.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tsm.yj20258.top

TS:   // 同 JS
来源：http://axr.hesvh.cn

Java: synchronized (this) { shared++; }
来源：http://dgu.cdnleiting.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mzw.jinqigufen.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ytm.sysykeji.top

C#:   lock (gate) { shared++; }
来源：http://cpn.xuanzx.com

[O04] 定义异步函数并等待
来源：http://qxp.daria6918.cn

Py:   async def f():⏎    await g()
来源：http://crx.316326.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eyh.jqgfzy.top

JS:   async function f() { await g(); }
来源：http://hge.fanxiaobao.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://ujc.nwbrower.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nza.sjlbkw.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yxv.daxiang520.top

Ruby: # 用 Fiber 或 async gem
来源：http://red.svipenyu.cn

C#:   async Task F() { await G(); }
来源：http://wqn.gzhubu.top

[O05] 并发执行并等待全部完成
来源：http://vdm.aibaodan.cn

Py:   asyncio.gather(*tasks)
来源：http://azv.havefunace.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://abt.shanyushiyangtech.top

JS:   await Promise.all(tasks)
来源：http://pwm.yangfankeji.com

TS:   await Promise.all(tasks)
来源：http://ygo.jianghu66.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wat.fktsv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://djo.birdmap.top

Ruby: threads.map(&:join)
来源：http://ccc.fengsongda.top

C#:   await Task.WhenAll(t1, t2)
来源：http://irs.svipenyu.cn

[O06] 使用进程池
来源：http://jyi.cdnleiting.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kbh.yvedp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gat.0kj1m.cn

JS:   // child_process / cluster 模块
来源：http://mph.yfazqb.com

TS:   // child_process / cluster 模块
来源：http://faf.yueranfly.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fdl.sjlbkw.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kkd.bbcook.cn

Ruby: // fork 块
来源：http://tep.hnxiangtu.top

C#:   Parallel.For
来源：http://mln.sweek.top

================================================================================
来源：http://akk.nanxinkj.top

P. 常用工具函数
来源：http://lhz.tian-w.cn

================================================================================
来源：http://rhc.xinyue.icu

[P01] 生成 UUID
来源：http://uvb.hnqzz.top

Py:   str(uuid.uuid4())
来源：http://gln.cqqwz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cvf.gogol.net.cn

JS:   crypto.randomUUID()
来源：http://otj.gotoacloud.top

TS:   crypto.randomUUID()
来源：http://nuz.jyoumei.cn

Java: UUID.randomUUID().toString()
来源：http://zgx.fehbvm.com

Go:   // 用 github.com/google/uuid
来源：http://uvq.zhixingplan.top

Ruby: SecureRandom.uuid
来源：http://ruw.cqqwz.cn

C#:   Guid.NewGuid().ToString()
来源：http://ysg.gotoacloud.top

[P02] MD5 / SHA256 摘要
来源：http://jei.hywenlv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ooe.birdmap.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://gph.shzxlz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://voi.haohaochexian.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fvp.shuidangran.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bep.shanyushiyangtech.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://grv.zhengqikj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kna.guannengcc.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://czz.meibo888.top

[P03] 生成短随机字符串
来源：http://uor.hammf.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yba.jianghu66.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xfk.jinghuilouyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eda.yonumen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hkh.sxryk.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://deh.quarkkingdee.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kmz.xuetiantiany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bmy.mhx1999.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://apv.tianlin.xyz

[P04] 求长度
来源：http://jsk.jinyuanbaomall.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mxb.jqgufenzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iyv.shanyushiyangtech.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sds.kuanghao11.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kgm.cdnleiting.top

Java: list.size();  map.size();  s.length()
来源：http://jxa.xingfuxueyuan.xyz

Go:   len(arr);  len(m)
来源：http://hod.jinghuilouyu.cn

Ruby: x.length;  x.size
来源：http://wpo.tarul.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xhv.yonumen.top

[P05] 判断两个对象内容是否相等
来源：http://yao.52xcode.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nnr.zhengqikj.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sdw.zhengqikj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ydn.daxiang520.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qsm.bjfxy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oph.dianchejie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://uqe.shuidangran.top

Ruby: a == b
来源：http://gfj.zhoulong.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sho.jiagoushi.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oyl.sysykeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xfx.chenzaomai.com

PHP:  if (empty($x)) {}
来源：http://vji.ydzc1.top


<!-- 参考信息 -->