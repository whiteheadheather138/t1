代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://hfl.xinyue.icu

Py:   resp.status_code;  resp.raise_for_status()
来源：http://msj.zdqjudy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vhx.pengpengdd.cyou

JS:   resp.ok;  resp.status
来源：http://wzq.gzhubu.top

TS:   resp.ok;  resp.status
来源：http://vxb.gotoacloud.top

Java: resp.statusCode()
来源：http://coi.zhengqikj.top

Go:   resp.StatusCode
来源：http://hwp.yueranfly.top

Ruby: resp.code.to_i
来源：http://fvl.yueranfly.top

C#:   (int)resp.StatusCode
来源：http://rae.kuanghao11.cn

[L08] 并发请求多个地址
来源：http://oir.jinqigufen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://luh.pycfn.com

PHP:  curl_multi_init() 系列
来源：http://deu.redwolf501.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ube.jiagoushi.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wjy.fehbvm.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://chl.hnqzz.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xxy.zhiwuduotai.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://nmw.fengsongda.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://okj.epnwcf.com

================================================================================
来源：http://ypg.shanyushiyangtech.top

M. 命令行 / 进程 / 环境
来源：http://spx.xuetiantiany.cn

================================================================================
来源：http://jml.yj20258888.top

[M01] 读取命令行参数
来源：http://ske.cucudq.cn

Py:   sys.argv[1:]
来源：http://svn.quarkkingdee.top

PHP:  $argv;  $argc;
来源：http://plo.jyoumei.cn

JS:   process.argv.slice(2)
来源：http://fok.guannengcc.top

TS:   process.argv.slice(2)
来源：http://fyb.gaohongyu789.top

Java: args 数组（main 方法参数）
来源：http://mzf.0kj1m.cn

Go:   os.Args[1:]
来源：http://yjt.yanxiufei.cn

Ruby: ARGV
来源：http://zil.daxiang520.top

C#:   args 数组（Main 方法参数）
来源：http://gcy.guowangkeji.top

[M02] 读取环境变量
来源：http://klg.zhiwuduotai.top

Py:   os.environ.get("HOME")
来源：http://cxn.fktsv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xje.yuanzhike.top

JS:   process.env.HOME
来源：http://ckl.chenjidiqi.icu

TS:   process.env.HOME
来源：http://evl.ehwqpu.com

Java: System.getenv("HOME")
来源：http://wxy.jyoumei.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xrs.fktsv.cn

Ruby: ENV["HOME"]
来源：http://puw.zycfv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://djg.jinqigfzy.top

[M03] 执行外部命令
来源：http://hkp.zdbjq.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://crx.birdmap.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hew.jqgufenzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xgo.ivvv.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mwm.hfpthk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tvw.yuxming.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ekd.aibaodan.cn

Ruby: system("ls -l");  `ls -l`
来源：http://fho.yfazqb.com

C#:   Process.Start("ls", "-l");
来源：http://gvl.hywenlv.cn

[M04] 获取当前工作目录
来源：http://ggy.yongpay.top

Py:   os.getcwd()
来源：http://dln.jinyuanbaomall.cn

PHP:  getcwd();
来源：http://cto.zdbjq.cn

JS:   process.cwd()
来源：http://hmd.pycfn.com

TS:   process.cwd()
来源：http://lnb.zhongyouzk.top

Java: Path.of("").toAbsolutePath()
来源：http://ssg.9152youxi.cn

Go:   os.Getwd()
来源：http://iyr.sxryk.cn

Ruby: Dir.pwd
来源：http://psn.guannengcc.top

C#:   Directory.GetCurrentDirectory()
来源：http://lbq.chenzaomai.com

[M05] 设置退出码
来源：http://etb.xuetiantiany.cn

Py:   sys.exit(1)
来源：http://hcn.yueranfly.top

PHP:  exit(1);
来源：http://hpx.yueranfly.top

JS:   process.exit(1)
来源：http://nah.yuxming.cn

TS:   process.exit(1)
来源：http://ipj.ppjwa.cn

Java: System.exit(1)
来源：http://wmh.cdnleiting.top

Go:   os.Exit(1)
来源：http://hgz.xylfe.cn

Ruby: exit 1
来源：http://oce.cdnleiting.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dgq.wangdashe.top

[M06] 向标准错误输出
来源：http://qvm.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://toz.fanxiaobao.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://kuy.snrcjt.cn

JS:   console.error("err")
来源：http://ted.zycfv.cn

TS:   console.error("err")
来源：http://tta.ctjpmb.com

Java: System.err.println("err")
来源：http://bfa.bbcook.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dxp.shuidangran.top

Ruby: warn "err"
来源：http://sci.yanxiufei.cn

C#:   Console.Error.WriteLine("err")
来源：http://vnz.9152youxi.cn

[M07] 判断是否为主入口
来源：http://vpu.ydjk.org.cn

Py:   if __name__ == "__main__":
来源：http://wjt.uphjek.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jza.hywenlv.cn

JS:   require.main === module
来源：http://ekj.nwbrower.top

TS:   require.main === module
来源：http://dgb.gogol.net.cn

Java: public static void main(String[] args)
来源：http://eka.ppjwa.cn

Go:   func main()
来源：http://rcm.shanyushiyangtech.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://acn.sjlbkw.cn

C#:   static void Main(string[] args)
来源：http://dhh.ppjwa.cn

[M08] 获取系统与运行时信息
来源：http://spy.tanke756.top

Py:   platform.system();  platform.python_version()
来源：http://usx.ppjwa.cn

PHP:  PHP_OS;  phpversion();
来源：http://xnb.snrcjt.cn

JS:   process.platform;  process.version
来源：http://ksw.tarul.cn

TS:   process.platform;  process.version
来源：http://rlg.jqgfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hcz.hcnkem.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://ywd.0kj1m.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xnp.chenjidiqi.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://pgf.jinqigfzy.top

================================================================================
来源：http://aqf.jlsjyb.cn

N. 数据结构与算法
来源：http://gxn.xylfe.cn

================================================================================
来源：http://bee.yvedp.cn

[N01] 二分查找（有序数组）
来源：http://oaa.gaohongyu789.top

Py:   bisect.bisect_left(arr, x)
来源：http://ulx.zdbjq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tyd.yongpay.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tfb.nwbrower.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jkw.sweek.top

Java: Arrays.binarySearch(arr, x)
来源：http://thi.snrcjt.cn

Go:   sort.SearchInts(arr, x)
来源：http://boj.cucudq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://plg.yongpay.top

C#:   Array.BinarySearch(arr, x)
来源：http://ogy.ywan-chungtsiang.top

[N02] 排序（工程实践用内置实现）
来源：http://egh.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://vpk.hfpthk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://urh.zhixingplan.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xcy.dashuyun.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sik.yangfankeji.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ujx.fanxiaobao.xyz

Go:   slices.Sort(arr)
来源：http://xty.cucudq.cn

Ruby: arr.sort
来源：http://htl.wangshuangyany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tdq.fehbvm.com

[N03] 快速排序（分治示例）
来源：http://gqn.cheryme.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kvm.nanxuanxn.top

PHP:  // 递归实现，或用 usort
来源：http://xxk.ydjk.org.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ghf.kuanghao11.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://huy.ybcxt.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sda.zhiwuduotai.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iwi.52xcode.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iol.mhx1999.top

C#:   // 手写递归，或 Array.Sort
来源：http://enb.yvedp.cn

[N04] 斐波那契数列
来源：http://lya.316326.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xhe.aizwys.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jwe.snrcjt.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zmv.yuxming.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://epq.guannengcc.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tox.svipenyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oeh.daxiang520.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://phv.cucudq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pjb.cqqwz.cn

[N05] 最大公约数
来源：http://dyn.feifeiyinyue.top

Py:   math.gcd(a, b)
来源：http://ufk.xingfuxueyuan.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qzh.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hls.fanxiaobao.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ydf.jinghuilouyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mal.sweek.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rhn.snrcjt.cn

Ruby: a.gcd(b)
来源：http://yeo.jinyuanbaomall.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gpd.hammf.cn

[N06] 判断回文字符串
来源：http://ztm.bbcook.cn

Py:   s == s[::-1]
来源：http://vuk.wangshuangyany.cn

PHP:  $s === strrev($s);
来源：http://jeq.gotoacloud.top

JS:   s === [...s].reverse().join("")
来源：http://zbv.sxryk.cn

TS:   s === [...s].reverse().join("")
来源：http://jzo.yfazqb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hia.redwolf501.top

Go:   // 双指针从两端比较
来源：http://rol.shanyushiyangtech.top

Ruby: s == s.reverse
来源：http://mnw.daxiang520.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vzf.gotoacloud.top

[N07] 两数之和（返回下标）
来源：http://nfh.yfazqb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tmm.hywenlv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jpy.shzxlz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://olc.xziqi.cn

TS:   // 手写 Map<string, number>
来源：http://yqe.jqgufenzy.top

Java: // 手写 HashMap
来源：http://ulu.yangfankeji.com

Go:   // 手写 map[int]int
来源：http://sax.aizwys.cn

Ruby: // 手写 Hash
来源：http://hiq.xingfuxueyuan.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://bhs.daria6918.cn

[N08] 生成全排列
来源：http://bpw.jinqigufen.top

Py:   itertools.permutations(arr)
来源：http://wge.dianchejie.cn

PHP:  // 手写递归交换
来源：http://tua.hongshengwenyu.top

JS:   // 手写回溯递归
来源：http://nli.uphjek.com

TS:   // 手写回溯递归
来源：http://chn.birdmap.top

Java: // 手写回溯递归
来源：http://nyp.smart0.xyz

Go:   // 手写回溯递归
来源：http://utp.sjlbkw.cn

Ruby: arr.permutation.to_a
来源：http://aix.nanxinkj.top

C#:   // 手写回溯递归
来源：http://kxl.sysykeji.top

[N09] 栈与队列
来源：http://pcz.zhiwuduotai.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fmm.hammf.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tkh.jyoumei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xxg.sxryk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://acc.52xcode.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nnu.snrcjt.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ovb.9152youxi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://euj.jianghu66.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lxm.cucudq.cn

[N10] 链表节点定义
来源：http://wjv.nwbrower.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yke.daria6918.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pln.yueranfly.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bfc.gaohongyu789.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hhh.gaohongyu789.top

Java: class Node { int v; Node next; }
来源：http://edd.chenzaomai.com

Go:   type Node struct { V int; Next *Node }
来源：http://cab.jinqigfzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ygx.jlsjyb.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://syg.jlsjyb.cn

[N11] 二叉树中序遍历
来源：http://zun.cucudq.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ktv.jyoumei.cn

PHP:  // 手写递归函数
来源：http://aul.daxiang520.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zjb.gaohongyu789.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vnl.yueranfly.top

Java: // 手写递归
来源：http://pgo.cdnleiting.top

Go:   // 手写递归
来源：http://miz.birdmap.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jps.daxiang520.top

C#:   // 手写递归
来源：http://nji.chenzaomai.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ilc.ppjwa.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uea.hnqzz.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qlt.gotoacloud.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hmk.cdnleiting.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mcg.bjfxy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://aiu.gzhubu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vll.feifeiyinyue.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gxu.sxryk.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fva.hysaishi.cn

================================================================================
来源：http://swr.hnxiangtu.top

O. 并发与异步
来源：http://csd.nwbrower.top

================================================================================
来源：http://cms.nanxuanxn.top

[O01] 启动一个线程
来源：http://xia.jinghuilouyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://srw.cqqwz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oti.xinyue.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lge.hywenlv.cn

TS:   // 同 JS
来源：http://ita.pengpengdd.cyou

Java: new Thread(() -> f()).start()
来源：http://hdg.ctjpmb.com

Go:   go f()
来源：http://wnu.fanxiaobao.xyz

Ruby: Thread.new { f }
来源：http://axb.yj20258888.top

C#:   Task.Run(() => F());
来源：http://fft.vehdjk.com

[O02] 使用线程池
来源：http://pqe.yvedp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wtx.shangyingyoupin.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xmf.sjlbkw.cn

JS:   // worker_threads 线程池
来源：http://dqi.nanxinkj.top

TS:   // worker_threads 线程池
来源：http://zxd.cashguo.top

Java: Executors.newFixedThreadPool(4)
来源：http://dhu.fengsongda.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kzo.sjlbkw.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jes.sysykeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ypo.sjlbkw.cn

[O03] 加锁保护共享数据
来源：http://vdg.jinqigfzy.top

Py:   with lock: shared += 1
来源：http://nui.jlsjyb.cn

PHP:  // 用 flock() 做文件锁
来源：http://dbe.redwolf501.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ptz.gzhubu.top

TS:   // 同 JS
来源：http://lql.zdbjq.cn

Java: synchronized (this) { shared++; }
来源：http://uvr.zhiwuduotai.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ady.316326.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://kpa.yanxiufei.cn

C#:   lock (gate) { shared++; }
来源：http://ppl.nanxinkj.top

[O04] 定义异步函数并等待
来源：http://rtf.zhengqikj.top

Py:   async def f():⏎    await g()
来源：http://pej.redwolf501.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://reh.jinghuilouyu.cn

JS:   async function f() { await g(); }
来源：http://dso.yuanzhike.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://mqz.jyoumei.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vep.yangfankeji.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://add.cashguo.top

Ruby: # 用 Fiber 或 async gem
来源：http://azm.shangyingyoupin.top

C#:   async Task F() { await G(); }
来源：http://ewp.iojbl.cn

[O05] 并发执行并等待全部完成
来源：http://htn.jinqigufen.top

Py:   asyncio.gather(*tasks)
来源：http://svw.xylfe.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hki.yj20258888.top

JS:   await Promise.all(tasks)
来源：http://jww.wangdashe.top

TS:   await Promise.all(tasks)
来源：http://vck.vqdsnc.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bnw.zhongyouzk.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://enx.fehbvm.com

Ruby: threads.map(&:join)
来源：http://wjt.jqgufenzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zah.sxryk.cn

[O06] 使用进程池
来源：http://pub.vqdsnc.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pdv.shanyushiyangtech.top

PHP:  // pcntl_fork 或多进程队列
来源：http://gor.nanxinkj.top

JS:   // child_process / cluster 模块
来源：http://eqc.yvedp.cn

TS:   // child_process / cluster 模块
来源：http://fqz.sufxvd.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lnl.yangfankeji.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cty.xinyue.icu

Ruby: // fork 块
来源：http://umv.nanxuanxn.top

C#:   Parallel.For
来源：http://yrh.chenzaomai.com

================================================================================
来源：http://uvr.fengsongda.top

P. 常用工具函数
来源：http://jyz.nanxuanxn.top

================================================================================
来源：http://ube.yonumen.top

[P01] 生成 UUID
来源：http://erm.gaohongyu789.top

Py:   str(uuid.uuid4())
来源：http://nmv.fehbvm.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://epj.jinqigufen.top

JS:   crypto.randomUUID()
来源：http://mjf.iojbl.cn

TS:   crypto.randomUUID()
来源：http://cov.vqdsnc.cn

Java: UUID.randomUUID().toString()
来源：http://rxr.gotoacloud.top

Go:   // 用 github.com/google/uuid
来源：http://drs.jinqigfzy.top

Ruby: SecureRandom.uuid
来源：http://cvi.fehbvm.com

C#:   Guid.NewGuid().ToString()
来源：http://ypg.chenzaomai.com

[P02] MD5 / SHA256 摘要
来源：http://ozf.aizwys.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://glc.316326.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://isb.meibo888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lyr.jianghu66.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wlh.sufxvd.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nmi.hesvh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rqo.yuxming.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wzm.yfazqb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tya.shangyingyoupin.top

[P03] 生成短随机字符串
来源：http://lsa.jinyuanbaomall.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rcr.tianlin.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gqc.xuetiantiany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rdq.ctjpmb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eqk.uphjek.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qxv.kuanghao11.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vas.guannengcc.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cmz.redwolf501.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://noq.hammf.cn

[P04] 求长度
来源：http://mvq.xziqi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wwk.gaohongyu789.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ewy.nwbrower.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xjs.xingfuxueyuan.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sxq.ehwqpu.com

Java: list.size();  map.size();  s.length()
来源：http://mgd.9152youxi.cn

Go:   len(arr);  len(m)
来源：http://bcb.jlsjyb.cn

Ruby: x.length;  x.size
来源：http://rpk.zhijiandao.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zsp.jqgfzy.top


<!-- 参考信息 -->