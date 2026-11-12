代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fiv.jianghu66.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vsu.hesvh.cn

Ruby: JSON.parse(resp.body)
来源：http://wxj.fzhhl.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uzp.yj20258888.top

[L07] 处理 HTTP 状态码
来源：http://dnr.wangshuangyany.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tfx.zhiwuduotai.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ikv.shanyushiyangkeji.top

JS:   resp.ok;  resp.status
来源：http://vct.jinqigufen.top

TS:   resp.ok;  resp.status
来源：http://yvc.fzhhl.top

Java: resp.statusCode()
来源：http://lef.cashguo.top

Go:   resp.StatusCode
来源：http://hdi.zdqjudy.top

Ruby: resp.code.to_i
来源：http://hwz.kuanghao11.cn

C#:   (int)resp.StatusCode
来源：http://wbn.xinyue.icu

[L08] 并发请求多个地址
来源：http://ixf.yueranfly.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ved.dashuyun.cn

PHP:  curl_multi_init() 系列
来源：http://ibv.sjlbkw.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dta.yonumen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://toc.jqgfzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kpl.fengsongda.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fvv.jqgfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ukx.sufxvd.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fbv.snrcjt.cn

================================================================================
来源：http://rwx.tanke756.top

M. 命令行 / 进程 / 环境
来源：http://tdz.jqgfzy.top

================================================================================
来源：http://xdq.fzhhl.top

[M01] 读取命令行参数
来源：http://vji.snrcjt.cn

Py:   sys.argv[1:]
来源：http://xjx.ivvv.top

PHP:  $argv;  $argc;
来源：http://trk.52xcode.cn

JS:   process.argv.slice(2)
来源：http://jng.316326.xyz

TS:   process.argv.slice(2)
来源：http://xfe.hysaishi.cn

Java: args 数组（main 方法参数）
来源：http://zai.svipenyu.cn

Go:   os.Args[1:]
来源：http://jgu.dianchejie.cn

Ruby: ARGV
来源：http://sdv.epnwcf.com

C#:   args 数组（Main 方法参数）
来源：http://zzv.yvedp.cn

[M02] 读取环境变量
来源：http://wgc.feifeiyinyue.top

Py:   os.environ.get("HOME")
来源：http://cqd.gotoacloud.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://szt.sysykeji.top

JS:   process.env.HOME
来源：http://qct.c1oappe.top

TS:   process.env.HOME
来源：http://lgq.mhx1999.top

Java: System.getenv("HOME")
来源：http://jrm.jqgfzy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dqn.guannengcc.top

Ruby: ENV["HOME"]
来源：http://pje.sufxvd.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dpk.cheryme.top

[M03] 执行外部命令
来源：http://nzi.zhiwuduotai.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ymx.jiagoushi.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ulp.gogol.net.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qhh.yvedp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://zeh.tianlin.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://czi.yonumen.top

Go:   exec.Command("ls", "-l").Output()
来源：http://tnb.zhengqikj.top

Ruby: system("ls -l");  `ls -l`
来源：http://fjg.gzhubu.top

C#:   Process.Start("ls", "-l");
来源：http://crl.cqqwz.cn

[M04] 获取当前工作目录
来源：http://qla.epnwcf.com

Py:   os.getcwd()
来源：http://yeh.redwolf501.top

PHP:  getcwd();
来源：http://mcb.fanxiaobao.xyz

JS:   process.cwd()
来源：http://hma.fzhhl.top

TS:   process.cwd()
来源：http://wqg.wangshuangyany.cn

Java: Path.of("").toAbsolutePath()
来源：http://wlg.zhijiandao.cn

Go:   os.Getwd()
来源：http://bli.xylfe.cn

Ruby: Dir.pwd
来源：http://xaf.chenzaomai.com

C#:   Directory.GetCurrentDirectory()
来源：http://exo.pycfn.com

[M05] 设置退出码
来源：http://ueu.bjfxy.top

Py:   sys.exit(1)
来源：http://lth.fehbvm.com

PHP:  exit(1);
来源：http://qvk.xingfuxueyuan.xyz

JS:   process.exit(1)
来源：http://igy.svipenyu.cn

TS:   process.exit(1)
来源：http://koj.zhengqikj.top

Java: System.exit(1)
来源：http://nuh.0kj1m.cn

Go:   os.Exit(1)
来源：http://joq.hywenlv.cn

Ruby: exit 1
来源：http://pvj.zhijiandao.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tnc.fanxiaobao.xyz

[M06] 向标准错误输出
来源：http://snf.zdqjudy.top

Py:   print("err", file=sys.stderr)
来源：http://jtt.hnqzz.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sqq.wangdashe.top

JS:   console.error("err")
来源：http://qet.svipenyu.cn

TS:   console.error("err")
来源：http://eia.hywenlv.cn

Java: System.err.println("err")
来源：http://utp.daria6918.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vmw.zhengqikj.top

Ruby: warn "err"
来源：http://gky.fengsongda.top

C#:   Console.Error.WriteLine("err")
来源：http://fwl.hywenlv.cn

[M07] 判断是否为主入口
来源：http://lun.gogol.net.cn

Py:   if __name__ == "__main__":
来源：http://bna.zhengqikj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yjy.yonumen.top

JS:   require.main === module
来源：http://kdm.shanyushiyangkeji.top

TS:   require.main === module
来源：http://cpk.xziqi.cn

Java: public static void main(String[] args)
来源：http://jdu.guowangkeji.top

Go:   func main()
来源：http://cuh.jyoumei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ryd.pycfn.com

C#:   static void Main(string[] args)
来源：http://uvt.tianlin.xyz

[M08] 获取系统与运行时信息
来源：http://gyj.mhx1999.top

Py:   platform.system();  platform.python_version()
来源：http://zor.hysaishi.cn

PHP:  PHP_OS;  phpversion();
来源：http://syj.yuanzhike.top

JS:   process.platform;  process.version
来源：http://jrt.sweek.top

TS:   process.platform;  process.version
来源：http://qmo.smart0.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zip.fzhhl.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dek.nwbrower.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lof.yj20258888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nmf.cheryme.top

================================================================================
来源：http://gjz.dianchejie.cn

N. 数据结构与算法
来源：http://mke.hnqzz.top

================================================================================
来源：http://rep.ivvv.top

[N01] 二分查找（有序数组）
来源：http://fsq.jiagoushi.top

Py:   bisect.bisect_left(arr, x)
来源：http://kfr.bjfxy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://boc.gzhubu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sfo.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yxs.sufxvd.cn

Java: Arrays.binarySearch(arr, x)
来源：http://aul.chenlongwang.top

Go:   sort.SearchInts(arr, x)
来源：http://umx.vqdsnc.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://oxu.uphjek.com

C#:   Array.BinarySearch(arr, x)
来源：http://wtn.aibaodan.cn

[N02] 排序（工程实践用内置实现）
来源：http://ckf.feifeiyinyue.top

Py:   sorted(arr);  arr.sort()
来源：http://orh.mhx1999.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qwt.snrcjt.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qtm.yuanzhike.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://zot.shanyushiyangtech.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gla.vehdjk.com

Go:   slices.Sort(arr)
来源：http://uzq.hnqzz.top

Ruby: arr.sort
来源：http://cij.cheryme.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hcu.gotoacloud.top

[N03] 快速排序（分治示例）
来源：http://dam.yueranfly.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://njn.jyoumei.cn

PHP:  // 递归实现，或用 usort
来源：http://itp.shuidangran.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pjk.tianlin.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://evi.daria6918.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yzt.xuanzx.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nsg.daria6918.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://siv.epnwcf.com

C#:   // 手写递归，或 Array.Sort
来源：http://tki.yueranfly.top

[N04] 斐波那契数列
来源：http://yzr.fanxiaobao.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dvm.zhengqikj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bsc.smart0.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pdp.pengpengdd.cyou

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hog.9152youxi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lhf.cashguo.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qaz.xylfe.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ssi.pycfn.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dpy.cashguo.top

[N05] 最大公约数
来源：http://zdk.jqgfzy.top

Py:   math.gcd(a, b)
来源：http://cfv.hywenlv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gjo.fktsv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dsj.yongpay.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tdt.gogol.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vbx.pengpengdd.cyou

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://obw.hywenlv.cn

Ruby: a.gcd(b)
来源：http://mzd.yangfankeji.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jhr.ywan-chungtsiang.top

[N06] 判断回文字符串
来源：http://nkj.jqgfzy.top

Py:   s == s[::-1]
来源：http://uqs.sweek.top

PHP:  $s === strrev($s);
来源：http://ntp.yvedp.cn

JS:   s === [...s].reverse().join("")
来源：http://rab.316326.xyz

TS:   s === [...s].reverse().join("")
来源：http://esq.jiagoushi.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pco.gaohongyu789.top

Go:   // 双指针从两端比较
来源：http://vmq.jqgufenzy.top

Ruby: s == s.reverse
来源：http://dqf.zhiwuduotai.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://pfk.ybcxt.top

[N07] 两数之和（返回下标）
来源：http://xqy.ctjpmb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qqo.guowangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fsv.sysykeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jjh.jianghu66.top

TS:   // 手写 Map<string, number>
来源：http://ysa.daxiang520.top

Java: // 手写 HashMap
来源：http://ycq.havefunace.top

Go:   // 手写 map[int]int
来源：http://yvv.jinqigufen.top

Ruby: // 手写 Hash
来源：http://wlz.yj20258.top

C#:   // 手写 Dictionary<int, int>
来源：http://mmy.yanxiufei.cn

[N08] 生成全排列
来源：http://kft.cqqwz.cn

Py:   itertools.permutations(arr)
来源：http://iiv.yonumen.top

PHP:  // 手写递归交换
来源：http://izj.9152youxi.cn

JS:   // 手写回溯递归
来源：http://atn.tian-w.cn

TS:   // 手写回溯递归
来源：http://dgp.aibaodan.cn

Java: // 手写回溯递归
来源：http://kcy.jyoumei.cn

Go:   // 手写回溯递归
来源：http://vep.yanxiufei.cn

Ruby: arr.permutation.to_a
来源：http://uzh.pycfn.com

C#:   // 手写回溯递归
来源：http://iyp.chenzaomai.com

[N09] 栈与队列
来源：http://deg.ivvv.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hur.bbcook.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tgl.fehbvm.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hap.smart0.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zvi.yvedp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hga.xuetiantiany.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nyf.zhiwuduotai.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fme.jianghu66.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nmp.zhijiandao.cn

[N10] 链表节点定义
来源：http://juf.ivvv.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rjq.hammf.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rrm.bjfxy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cjd.zhoulong.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bcp.pengpengdd.cyou

Java: class Node { int v; Node next; }
来源：http://twh.yfazqb.com

Go:   type Node struct { V int; Next *Node }
来源：http://rrl.fzhhl.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xdp.xziqi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dof.hnxiangtu.top

[N11] 二叉树中序遍历
来源：http://hwc.tianlin.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aai.shanyushiyangtech.top

PHP:  // 手写递归函数
来源：http://vmc.ybcxt.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bzc.zdqjudy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kzk.andypj.xyz

Java: // 手写递归
来源：http://nyn.hongshengwenyu.top

Go:   // 手写递归
来源：http://qze.gzhubu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eve.jiagoushi.top

C#:   // 手写递归
来源：http://vdt.yanxiufei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://phb.fehbvm.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hkj.52xcode.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qjc.jinqigfzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wct.ydjk.org.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zjq.jyoumei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oeo.bjfxy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dpa.yuanzhike.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wgl.xuetiantiany.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iqf.hnqzz.top

================================================================================
来源：http://sdl.cqqwz.cn

O. 并发与异步
来源：http://eae.yuxming.cn

================================================================================
来源：http://hdp.hfpthk.cn

[O01] 启动一个线程
来源：http://ekc.jiagoushi.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qfk.ybcxt.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cnn.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wrh.kuanghao11.cn

TS:   // 同 JS
来源：http://byh.chenlongwang.top

Java: new Thread(() -> f()).start()
来源：http://eon.chenjidiqi.icu

Go:   go f()
来源：http://oyh.jyoumei.cn

Ruby: Thread.new { f }
来源：http://xms.vqdsnc.cn

C#:   Task.Run(() => F());
来源：http://akj.aibaodan.cn

[O02] 使用线程池
来源：http://mwo.meibo888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ack.redwolf501.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qft.daxiang520.top

JS:   // worker_threads 线程池
来源：http://xaw.jiagoushi.top

TS:   // worker_threads 线程池
来源：http://uzc.zhijiandao.cn

Java: Executors.newFixedThreadPool(4)
来源：http://eot.redwolf501.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ayx.snrcjt.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://arm.xinyue.icu

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://szs.hfpthk.cn

[O03] 加锁保护共享数据
来源：http://azo.aizwys.cn

Py:   with lock: shared += 1
来源：http://vnk.hfpthk.cn

PHP:  // 用 flock() 做文件锁
来源：http://ykv.52xcode.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gcy.cqqwz.cn

TS:   // 同 JS
来源：http://wbp.yuanzhike.top

Java: synchronized (this) { shared++; }
来源：http://ehx.yanxiufei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://epl.jianghu66.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ony.vqdsnc.cn

C#:   lock (gate) { shared++; }
来源：http://ila.mhx1999.top

[O04] 定义异步函数并等待
来源：http://dqv.aizwys.cn

Py:   async def f():⏎    await g()
来源：http://khb.iojbl.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bkz.yangfankeji.com

JS:   async function f() { await g(); }
来源：http://rlj.zhoulong.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://owq.0kj1m.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gvv.zhiwuduotai.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vhm.jyoumei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://dbk.hammf.cn

C#:   async Task F() { await G(); }
来源：http://slr.gaohongyu789.top

[O05] 并发执行并等待全部完成
来源：http://okq.gaohongyu789.top

Py:   asyncio.gather(*tasks)
来源：http://gjp.yfazqb.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cfj.cdnleiting.top

JS:   await Promise.all(tasks)
来源：http://rjc.jianghu66.top

TS:   await Promise.all(tasks)
来源：http://dpc.smart0.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kkk.bbcook.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tyl.hcnkem.com

Ruby: threads.map(&:join)
来源：http://mxp.ctjpmb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://wmp.jlsjyb.cn

[O06] 使用进程池
来源：http://bsz.xylfe.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mdr.yuanzhike.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ism.nanxinkj.top

JS:   // child_process / cluster 模块
来源：http://ewm.sweek.top

TS:   // child_process / cluster 模块
来源：http://lww.hywenlv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ytb.jiagoushi.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ddl.zhengqikj.top

Ruby: // fork 块
来源：http://jwd.nwbrower.top

C#:   Parallel.For
来源：http://ikh.epnwcf.com

================================================================================
来源：http://vaf.chenzaomai.com

P. 常用工具函数
来源：http://sim.mhx1999.top

================================================================================
来源：http://vme.shzxlz.cn

[P01] 生成 UUID
来源：http://ixa.xylfe.cn

Py:   str(uuid.uuid4())
来源：http://gex.hongshengwenyu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iuq.jinyuanbaomall.cn

JS:   crypto.randomUUID()
来源：http://ahk.shuidangran.top

TS:   crypto.randomUUID()
来源：http://hbp.wangdashe.top

Java: UUID.randomUUID().toString()
来源：http://kzm.yfazqb.com

Go:   // 用 github.com/google/uuid
来源：http://mrr.daria6918.cn

Ruby: SecureRandom.uuid
来源：http://ktv.wangshuangyany.cn

C#:   Guid.NewGuid().ToString()
来源：http://hbh.sjlbkw.cn

[P02] MD5 / SHA256 摘要
来源：http://crd.yanxiufei.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://amv.zhongyouzk.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qjf.tanke756.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cir.andypj.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ecw.yueranfly.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jja.gogol.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yhq.fengsongda.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ksc.chenzaomai.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pmz.jianghu66.top

[P03] 生成短随机字符串
来源：http://pew.cucudq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pdv.epnwcf.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bfx.snrcjt.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ofl.yvedp.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oho.zhengqikj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jwi.jlsjyb.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qcx.ywan-chungtsiang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tsa.guowangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qbz.zhaomingkeji.xyz

[P04] 求长度
来源：http://tvg.ydzc1.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lfx.vehdjk.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://joh.wangdashe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fyi.zdqjudy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fij.yj202588.top


<!-- 参考信息 -->