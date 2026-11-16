代发 wailian999

TS:   resp.ok;  resp.status
来源：http://swq.yanxiufei.cn

Java: resp.statusCode()
来源：http://cdm.jinqigufen.top

Go:   resp.StatusCode
来源：http://gyb.hammf.cn

Ruby: resp.code.to_i
来源：http://wia.gaohongyu789.top

C#:   (int)resp.StatusCode
来源：http://ncz.zhoulong.xyz

[L08] 并发请求多个地址
来源：http://eqs.hnxiangtu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://asg.cdnleiting.top

PHP:  curl_multi_init() 系列
来源：http://wbr.hcnkem.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xqb.yueranfly.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cde.fehbvm.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zbn.ctjpmb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lnj.jqgfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sow.chenjidiqi.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eqk.yongpay.top

================================================================================
来源：http://sxm.birdmap.top

M. 命令行 / 进程 / 环境
来源：http://bre.ybcxt.top

================================================================================
来源：http://cfq.chenzaomai.com

[M01] 读取命令行参数
来源：http://tsi.nwbrower.top

Py:   sys.argv[1:]
来源：http://hws.shanyushiyangkeji.top

PHP:  $argv;  $argc;
来源：http://byb.ivvv.top

JS:   process.argv.slice(2)
来源：http://iwq.andypj.xyz

TS:   process.argv.slice(2)
来源：http://xzc.jinqigufen.top

Java: args 数组（main 方法参数）
来源：http://vpp.chenlongwang.top

Go:   os.Args[1:]
来源：http://diz.xylfe.cn

Ruby: ARGV
来源：http://yum.wangshuangyany.cn

C#:   args 数组（Main 方法参数）
来源：http://tqa.xuetiantiany.cn

[M02] 读取环境变量
来源：http://csd.snrcjt.cn

Py:   os.environ.get("HOME")
来源：http://seb.cheryme.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://asp.cheryme.top

JS:   process.env.HOME
来源：http://iug.jianghu66.top

TS:   process.env.HOME
来源：http://zok.uphjek.com

Java: System.getenv("HOME")
来源：http://rio.birdmap.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://miz.tanke756.top

Ruby: ENV["HOME"]
来源：http://hgl.meibo888.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dke.xuetiantiany.cn

[M03] 执行外部命令
来源：http://xkg.fengsongda.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dac.sxryk.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lpm.xziqi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dlo.fanxiaobao.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://suc.chenlongwang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qed.pengpengdd.cyou

Go:   exec.Command("ls", "-l").Output()
来源：http://fpr.guannengcc.top

Ruby: system("ls -l");  `ls -l`
来源：http://lvw.hesvh.cn

C#:   Process.Start("ls", "-l");
来源：http://euf.ydzc1.top

[M04] 获取当前工作目录
来源：http://ljo.aizwys.cn

Py:   os.getcwd()
来源：http://iuv.aizwys.cn

PHP:  getcwd();
来源：http://ebf.bbcook.cn

JS:   process.cwd()
来源：http://lss.daria6918.cn

TS:   process.cwd()
来源：http://gwi.jyoumei.cn

Java: Path.of("").toAbsolutePath()
来源：http://bae.mhx1999.top

Go:   os.Getwd()
来源：http://tpq.yvedp.cn

Ruby: Dir.pwd
来源：http://lzg.jqgufenzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://mnz.sysykeji.top

[M05] 设置退出码
来源：http://uxo.zhaomingkeji.xyz

Py:   sys.exit(1)
来源：http://ofx.smart0.xyz

PHP:  exit(1);
来源：http://wkx.fzhhl.top

JS:   process.exit(1)
来源：http://guv.mhx1999.top

TS:   process.exit(1)
来源：http://orj.sysykeji.top

Java: System.exit(1)
来源：http://mjg.ywan-chungtsiang.top

Go:   os.Exit(1)
来源：http://usu.shangyingyoupin.top

Ruby: exit 1
来源：http://znd.0kj1m.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fcs.jqgufenzy.top

[M06] 向标准错误输出
来源：http://auo.sufxvd.cn

Py:   print("err", file=sys.stderr)
来源：http://utb.tanke756.top

PHP:  fwrite(STDERR, "err\n");
来源：http://tmd.yfazqb.com

JS:   console.error("err")
来源：http://usl.xuanzx.com

TS:   console.error("err")
来源：http://sgx.wangdashe.top

Java: System.err.println("err")
来源：http://vcn.52xcode.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://des.guowangkeji.top

Ruby: warn "err"
来源：http://xvc.316326.xyz

C#:   Console.Error.WriteLine("err")
来源：http://jlg.jinqigfzy.top

[M07] 判断是否为主入口
来源：http://gwf.nanxuanxn.top

Py:   if __name__ == "__main__":
来源：http://hay.fktsv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aey.havefunace.top

JS:   require.main === module
来源：http://rmp.yueranfly.top

TS:   require.main === module
来源：http://hns.yj202588.top

Java: public static void main(String[] args)
来源：http://yin.zhongyouzk.top

Go:   func main()
来源：http://khd.hywenlv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lts.fehbvm.com

C#:   static void Main(string[] args)
来源：http://jvs.snrcjt.cn

[M08] 获取系统与运行时信息
来源：http://ppn.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://pmh.shzxlz.cn

PHP:  PHP_OS;  phpversion();
来源：http://jzu.pycfn.com

JS:   process.platform;  process.version
来源：http://dtv.uphjek.com

TS:   process.platform;  process.version
来源：http://wqo.shuidangran.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nae.xylfe.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://iqe.guannengcc.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wpy.ydzc1.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mza.ppjwa.cn

================================================================================
来源：http://huy.hysaishi.cn

N. 数据结构与算法
来源：http://qem.jiagoushi.top

================================================================================
来源：http://tww.feifeiyinyue.top

[N01] 二分查找（有序数组）
来源：http://klj.jqgufenzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://nxm.xuetiantiany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://agv.daria6918.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://suw.xuanzx.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mrt.cqqwz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jms.bjfxy.top

Go:   sort.SearchInts(arr, x)
来源：http://yrc.redwolf501.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://yls.wangshuangyany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://lkq.sweek.top

[N02] 排序（工程实践用内置实现）
来源：http://nbi.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://cpi.smart0.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rkq.jiagoushi.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://btj.ehwqpu.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://jxw.nanxuanxn.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ega.hongshengwenyu.top

Go:   slices.Sort(arr)
来源：http://rsd.316326.xyz

Ruby: arr.sort
来源：http://vcq.shanyushiyangkeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://trb.nanxinkj.top

[N03] 快速排序（分治示例）
来源：http://sjh.shanyushiyangtech.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yxj.zhongyouzk.top

PHP:  // 递归实现，或用 usort
来源：http://wgl.pengpengdd.cyou

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fxm.0kj1m.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pit.ydjk.org.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gre.ivvv.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jxo.shzxlz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zos.0kj1m.cn

C#:   // 手写递归，或 Array.Sort
来源：http://uqt.ctjpmb.com

[N04] 斐波那契数列
来源：http://giu.0kj1m.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xlr.andypj.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://egy.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lvi.9152youxi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sku.316326.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ujy.cashguo.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gic.fktsv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wng.iojbl.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://duo.nwbrower.top

[N05] 最大公约数
来源：http://gxm.zycfv.cn

Py:   math.gcd(a, b)
来源：http://mmi.bjfxy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oho.pycfn.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hnz.xuetiantiany.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://klv.jinyuanbaomall.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lbw.yvedp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xus.hesvh.cn

Ruby: a.gcd(b)
来源：http://ijp.zhijiandao.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ycf.daxiang520.top

[N06] 判断回文字符串
来源：http://pqi.zhaomingkeji.xyz

Py:   s == s[::-1]
来源：http://gjs.yonumen.top

PHP:  $s === strrev($s);
来源：http://xwe.yuxming.cn

JS:   s === [...s].reverse().join("")
来源：http://eyo.yanxiufei.cn

TS:   s === [...s].reverse().join("")
来源：http://ydk.yj20258.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oak.yonumen.top

Go:   // 双指针从两端比较
来源：http://jzv.ydzc1.top

Ruby: s == s.reverse
来源：http://ylx.dianchejie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ems.jlsjyb.cn

[N07] 两数之和（返回下标）
来源：http://cbp.meibo888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ooh.zhijiandao.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dow.tian-w.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kdk.hywenlv.cn

TS:   // 手写 Map<string, number>
来源：http://aqi.hesvh.cn

Java: // 手写 HashMap
来源：http://ryo.meibo888.top

Go:   // 手写 map[int]int
来源：http://fhu.dashuyun.cn

Ruby: // 手写 Hash
来源：http://fqs.hnxiangtu.top

C#:   // 手写 Dictionary<int, int>
来源：http://cvn.nwbrower.top

[N08] 生成全排列
来源：http://pkx.hnxiangtu.top

Py:   itertools.permutations(arr)
来源：http://tcy.shanyushiyangtech.top

PHP:  // 手写递归交换
来源：http://snh.hesvh.cn

JS:   // 手写回溯递归
来源：http://izg.shanyushiyangkeji.top

TS:   // 手写回溯递归
来源：http://vdd.shangyingyoupin.top

Java: // 手写回溯递归
来源：http://gum.pengpengdd.cyou

Go:   // 手写回溯递归
来源：http://rjs.birdmap.top

Ruby: arr.permutation.to_a
来源：http://xpn.xuanzx.com

C#:   // 手写回溯递归
来源：http://tkz.jinqigufen.top

[N09] 栈与队列
来源：http://xnn.ppjwa.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zov.ctjpmb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://plw.jinghuilouyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xkx.zdbjq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://teu.hnxiangtu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cwz.jyoumei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lnu.hammf.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vkd.hongshengwenyu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tfl.jlsjyb.cn

[N10] 链表节点定义
来源：http://ljb.bjfxy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cnm.ydzc1.top

PHP:  class Node { public $v; public $next = null; }
来源：http://epq.hfpthk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://oqc.shanyushiyangtech.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bnj.andypj.xyz

Java: class Node { int v; Node next; }
来源：http://ggc.pengpengdd.cyou

Go:   type Node struct { V int; Next *Node }
来源：http://mey.xuetiantiany.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://amc.jyoumei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cwt.jyoumei.cn

[N11] 二叉树中序遍历
来源：http://nlj.guannengcc.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qdg.c1oappe.top

PHP:  // 手写递归函数
来源：http://eez.fktsv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ndq.mhx1999.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eiy.cashguo.top

Java: // 手写递归
来源：http://yyr.sweek.top

Go:   // 手写递归
来源：http://srw.jinyuanbaomall.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oeb.cashguo.top

C#:   // 手写递归
来源：http://fdl.hammf.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rrl.sysykeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uko.nanxinkj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nxs.ydzc1.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ptf.ywan-chungtsiang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qtd.zdqjudy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zff.ppjwa.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sou.ehwqpu.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cjh.fehbvm.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qhb.kuanghao11.cn

================================================================================
来源：http://imy.bbcook.cn

O. 并发与异步
来源：http://qzf.zycfv.cn

================================================================================
来源：http://jhp.tarul.cn

[O01] 启动一个线程
来源：http://dte.chenlongwang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ssk.nanxinkj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sno.yj202588.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rrl.zhengqikj.top

TS:   // 同 JS
来源：http://pcs.ivvv.top

Java: new Thread(() -> f()).start()
来源：http://tzs.hcnkem.com

Go:   go f()
来源：http://zdx.havefunace.top

Ruby: Thread.new { f }
来源：http://syk.sxryk.cn

C#:   Task.Run(() => F());
来源：http://qpe.svipenyu.cn

[O02] 使用线程池
来源：http://ede.fktsv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xwy.fanxiaobao.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ctl.guannengcc.top

JS:   // worker_threads 线程池
来源：http://pcg.epnwcf.com

TS:   // worker_threads 线程池
来源：http://nke.xziqi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fik.bjfxy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vfq.fktsv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bbr.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qiz.ehwqpu.com

[O03] 加锁保护共享数据
来源：http://ihu.zhijiandao.cn

Py:   with lock: shared += 1
来源：http://fml.yfazqb.com

PHP:  // 用 flock() 做文件锁
来源：http://paq.sweek.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uuc.yuanzhike.top

TS:   // 同 JS
来源：http://zad.tanke756.top

Java: synchronized (this) { shared++; }
来源：http://nld.vehdjk.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wrc.cheryme.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://zak.wangdashe.top

C#:   lock (gate) { shared++; }
来源：http://nfn.jinyuanbaomall.cn

[O04] 定义异步函数并等待
来源：http://uss.0kj1m.cn

Py:   async def f():⏎    await g()
来源：http://uko.svipenyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://deo.chenjidiqi.icu

JS:   async function f() { await g(); }
来源：http://ofg.quarkkingdee.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wde.svipenyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://teg.xingfuxueyuan.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sao.zhoulong.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://uqp.dianchejie.cn

C#:   async Task F() { await G(); }
来源：http://hds.ctjpmb.com

[O05] 并发执行并等待全部完成
来源：http://pbk.jinqigfzy.top

Py:   asyncio.gather(*tasks)
来源：http://fcp.jlsjyb.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lpl.jinyuanbaomall.cn

JS:   await Promise.all(tasks)
来源：http://yal.aibaodan.cn

TS:   await Promise.all(tasks)
来源：http://dtb.jinyuanbaomall.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aju.jinqigufen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kzn.xingfuxueyuan.xyz

Ruby: threads.map(&:join)
来源：http://fxb.snrcjt.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qzo.ydjk.org.cn

[O06] 使用进程池
来源：http://bgp.wangshuangyany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://our.daxiang520.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zqc.hnxiangtu.top

JS:   // child_process / cluster 模块
来源：http://gdf.uphjek.com

TS:   // child_process / cluster 模块
来源：http://zbm.iojbl.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vjk.cdnleiting.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oti.chenzaomai.com

Ruby: // fork 块
来源：http://tpj.ctjpmb.com

C#:   Parallel.For
来源：http://rgs.jyoumei.cn

================================================================================
来源：http://zup.yangfankeji.com

P. 常用工具函数
来源：http://xoi.pycfn.com

================================================================================
来源：http://zjn.shzxlz.cn

[P01] 生成 UUID
来源：http://fkq.uphjek.com

Py:   str(uuid.uuid4())
来源：http://qhr.ppjwa.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jjo.sufxvd.cn

JS:   crypto.randomUUID()
来源：http://xxj.gotoacloud.top

TS:   crypto.randomUUID()
来源：http://hzr.tian-w.cn

Java: UUID.randomUUID().toString()
来源：http://psb.cashguo.top

Go:   // 用 github.com/google/uuid
来源：http://ied.yonumen.top

Ruby: SecureRandom.uuid
来源：http://yow.cdnleiting.top

C#:   Guid.NewGuid().ToString()
来源：http://ofh.sweek.top

[P02] MD5 / SHA256 摘要
来源：http://npa.jinqigufen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qjn.zhoulong.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://lpc.hysaishi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cpq.9152youxi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cat.chenjidiqi.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vpy.havefunace.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mvc.havefunace.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jsv.jinyuanbaomall.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cxv.shanyushiyangtech.top

[P03] 生成短随机字符串
来源：http://ugi.tarul.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yat.yj20258.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gqh.wangdashe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wjj.zdqjudy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lag.ydjk.org.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yyk.0kj1m.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bqd.snrcjt.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yrg.wangshuangyany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uxs.daria6918.cn

[P04] 求长度
来源：http://aqc.ybcxt.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dwl.cdnleiting.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gyb.jiagoushi.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zcd.dashuyun.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://feq.haohaochexian.top

Java: list.size();  map.size();  s.length()
来源：http://hbv.xuanzx.com

Go:   len(arr);  len(m)
来源：http://lts.nanxuanxn.top

Ruby: x.length;  x.size
来源：http://cty.hnqzz.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://abd.yj20258888.top

[P05] 判断两个对象内容是否相等
来源：http://sex.cqqwz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xny.shanyushiyangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fkd.kuanghao11.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vsz.jlsjyb.cn


<!-- 参考信息 -->