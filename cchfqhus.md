代发 wailian999

Ruby: ARGV
来源：http://dun.dashuyun.cn

C#:   args 数组（Main 方法参数）
来源：http://vhg.jlsjyb.cn

[M02] 读取环境变量
来源：http://sxa.sjlbkw.cn

Py:   os.environ.get("HOME")
来源：http://xqb.hcnkem.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wkg.chenlongwang.top

JS:   process.env.HOME
来源：http://cjj.nanxinkj.top

TS:   process.env.HOME
来源：http://ytb.hammf.cn

Java: System.getenv("HOME")
来源：http://dku.ydjk.org.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dra.hnxiangtu.top

Ruby: ENV["HOME"]
来源：http://rvm.pengpengdd.cyou

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zkt.daxiang520.top

[M03] 执行外部命令
来源：http://ziz.gzhubu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ghx.fengsongda.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bmn.jqgufenzy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ogj.shanyushiyangkeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fby.ydzc1.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lnf.52xcode.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mty.zycfv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sho.nanxinkj.top

C#:   Process.Start("ls", "-l");
来源：http://sqb.nwbrower.top

[M04] 获取当前工作目录
来源：http://tlp.hnqzz.top

Py:   os.getcwd()
来源：http://ioh.epnwcf.com

PHP:  getcwd();
来源：http://emw.ppjwa.cn

JS:   process.cwd()
来源：http://sii.0kj1m.cn

TS:   process.cwd()
来源：http://odw.nanxinkj.top

Java: Path.of("").toAbsolutePath()
来源：http://sgw.shuidangran.top

Go:   os.Getwd()
来源：http://qtn.fzhhl.top

Ruby: Dir.pwd
来源：http://wmt.9152youxi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zyw.tarul.cn

[M05] 设置退出码
来源：http://fdc.ehwqpu.com

Py:   sys.exit(1)
来源：http://coj.ybcxt.top

PHP:  exit(1);
来源：http://bgm.jinqigufen.top

JS:   process.exit(1)
来源：http://sdv.gaohongyu789.top

TS:   process.exit(1)
来源：http://hjr.ybcxt.top

Java: System.exit(1)
来源：http://aio.yj20258.top

Go:   os.Exit(1)
来源：http://cpo.zhongyouzk.top

Ruby: exit 1
来源：http://mqr.snrcjt.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nft.jinghuilouyu.cn

[M06] 向标准错误输出
来源：http://ref.hywenlv.cn

Py:   print("err", file=sys.stderr)
来源：http://eef.gaohongyu789.top

PHP:  fwrite(STDERR, "err\n");
来源：http://eoz.hnqzz.top

JS:   console.error("err")
来源：http://ihh.vqdsnc.cn

TS:   console.error("err")
来源：http://dnf.cucudq.cn

Java: System.err.println("err")
来源：http://vvv.snrcjt.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pge.aibaodan.cn

Ruby: warn "err"
来源：http://jcd.shanyushiyangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://rne.ctjpmb.com

[M07] 判断是否为主入口
来源：http://xfx.kuanghao11.cn

Py:   if __name__ == "__main__":
来源：http://fgw.wangshuangyany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pxm.cdnleiting.top

JS:   require.main === module
来源：http://etd.tian-w.cn

TS:   require.main === module
来源：http://rpy.shzxlz.cn

Java: public static void main(String[] args)
来源：http://gkd.9152youxi.cn

Go:   func main()
来源：http://ysi.bbcook.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ivp.yangfankeji.com

C#:   static void Main(string[] args)
来源：http://gaq.yj202588.top

[M08] 获取系统与运行时信息
来源：http://eui.redwolf501.top

Py:   platform.system();  platform.python_version()
来源：http://opl.c1oappe.top

PHP:  PHP_OS;  phpversion();
来源：http://vuu.havefunace.top

JS:   process.platform;  process.version
来源：http://ruq.jinqigfzy.top

TS:   process.platform;  process.version
来源：http://jmf.shzxlz.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nbq.haohaochexian.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zbh.jqgufenzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zgh.gogol.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kqt.cucudq.cn

================================================================================
来源：http://gqh.ydjk.org.cn

N. 数据结构与算法
来源：http://pgf.zhoulong.xyz

================================================================================
来源：http://kxq.zhaomingkeji.xyz

[N01] 二分查找（有序数组）
来源：http://wjp.yuanzhike.top

Py:   bisect.bisect_left(arr, x)
来源：http://tcr.chenlongwang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vor.yongpay.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iam.hnxiangtu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://foq.9152youxi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://foa.guannengcc.top

Go:   sort.SearchInts(arr, x)
来源：http://ijy.gotoacloud.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://oin.ppjwa.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dmk.shzxlz.cn

[N02] 排序（工程实践用内置实现）
来源：http://vfz.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://qgd.yuxming.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cxd.jqgfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://kkh.smart0.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://yvw.daria6918.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bir.gotoacloud.top

Go:   slices.Sort(arr)
来源：http://ciw.chenlongwang.top

Ruby: arr.sort
来源：http://yxl.hammf.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://thy.xinyue.icu

[N03] 快速排序（分治示例）
来源：http://mqc.ywan-chungtsiang.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lem.ehwqpu.com

PHP:  // 递归实现，或用 usort
来源：http://pqt.ppjwa.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hwm.wangshuangyany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://one.redwolf501.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ioo.jqgfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bls.yuanzhike.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iot.ivvv.top

C#:   // 手写递归，或 Array.Sort
来源：http://xwq.hammf.cn

[N04] 斐波那契数列
来源：http://ubp.cashguo.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gps.havefunace.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wak.jlsjyb.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ook.cdnleiting.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tfd.hysaishi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fii.bjfxy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xjw.zycfv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kbz.zhengqikj.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nbf.jinyuanbaomall.cn

[N05] 最大公约数
来源：http://lqi.sxryk.cn

Py:   math.gcd(a, b)
来源：http://pua.dianchejie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gfx.zhiwuduotai.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gal.jinghuilouyu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kle.yj20258888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tvj.ybcxt.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://axp.quarkkingdee.top

Ruby: a.gcd(b)
来源：http://eii.meibo888.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tje.smart0.xyz

[N06] 判断回文字符串
来源：http://vad.xinyue.icu

Py:   s == s[::-1]
来源：http://izb.ehwqpu.com

PHP:  $s === strrev($s);
来源：http://ftw.zhengqikj.top

JS:   s === [...s].reverse().join("")
来源：http://udy.ppjwa.cn

TS:   s === [...s].reverse().join("")
来源：http://bkf.ppjwa.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ced.yueranfly.top

Go:   // 双指针从两端比较
来源：http://rru.316326.xyz

Ruby: s == s.reverse
来源：http://joe.0kj1m.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://clh.ydjk.org.cn

[N07] 两数之和（返回下标）
来源：http://igl.0kj1m.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ood.sxryk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dwt.meibo888.top

JS:   // 手写 Map：map.set(v, i)
来源：http://cvw.dianchejie.cn

TS:   // 手写 Map<string, number>
来源：http://qsl.meibo888.top

Java: // 手写 HashMap
来源：http://kpy.cheryme.top

Go:   // 手写 map[int]int
来源：http://rjp.hnqzz.top

Ruby: // 手写 Hash
来源：http://fga.jyoumei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gxt.sufxvd.cn

[N08] 生成全排列
来源：http://rld.hnxiangtu.top

Py:   itertools.permutations(arr)
来源：http://aje.tarul.cn

PHP:  // 手写递归交换
来源：http://hrk.jianghu66.top

JS:   // 手写回溯递归
来源：http://ehg.wangdashe.top

TS:   // 手写回溯递归
来源：http://wlx.jiagoushi.top

Java: // 手写回溯递归
来源：http://geq.sjlbkw.cn

Go:   // 手写回溯递归
来源：http://kcv.yueranfly.top

Ruby: arr.permutation.to_a
来源：http://jtl.sjlbkw.cn

C#:   // 手写回溯递归
来源：http://xkf.jianghu66.top

[N09] 栈与队列
来源：http://iav.shzxlz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://htb.cdnleiting.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qzw.316326.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ujd.zycfv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://von.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sgt.ybcxt.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eli.zhoulong.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ppw.zhoulong.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lij.nanxuanxn.top

[N10] 链表节点定义
来源：http://zrx.guannengcc.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://acn.fehbvm.com

PHP:  class Node { public $v; public $next = null; }
来源：http://glj.shanyushiyangtech.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://spf.ybcxt.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gmi.hammf.cn

Java: class Node { int v; Node next; }
来源：http://qvz.xziqi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jqb.yongpay.top

Ruby: Node = Struct.new(:v, :next)
来源：http://sha.c1oappe.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gkk.sjlbkw.cn

[N11] 二叉树中序遍历
来源：http://ayy.vqdsnc.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zqj.hesvh.cn

PHP:  // 手写递归函数
来源：http://nxt.hammf.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rix.shuidangran.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ysn.yangfankeji.com

Java: // 手写递归
来源：http://mlv.guowangkeji.top

Go:   // 手写递归
来源：http://hja.gogol.net.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zmd.uphjek.com

C#:   // 手写递归
来源：http://nmy.andypj.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zmc.ydzc1.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://acq.jinghuilouyu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zhc.nanxinkj.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bwf.xuetiantiany.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sbm.xingfuxueyuan.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vby.zdqjudy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bkn.yueranfly.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bfy.pycfn.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://orl.bbcook.cn

================================================================================
来源：http://paz.shangyingyoupin.top

O. 并发与异步
来源：http://zpb.yfazqb.com

================================================================================
来源：http://hbz.hywenlv.cn

[O01] 启动一个线程
来源：http://mlu.bjfxy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xek.hesvh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mzg.0kj1m.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gdk.iojbl.cn

TS:   // 同 JS
来源：http://pmc.jinqigfzy.top

Java: new Thread(() -> f()).start()
来源：http://znj.ydzc1.top

Go:   go f()
来源：http://jii.ywan-chungtsiang.top

Ruby: Thread.new { f }
来源：http://kpd.yvedp.cn

C#:   Task.Run(() => F());
来源：http://fml.zhaomingkeji.xyz

[O02] 使用线程池
来源：http://ggw.gaohongyu789.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://maz.yongpay.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xaf.zhijiandao.cn

JS:   // worker_threads 线程池
来源：http://yyt.haohaochexian.top

TS:   // worker_threads 线程池
来源：http://vze.mhx1999.top

Java: Executors.newFixedThreadPool(4)
来源：http://stb.bbcook.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wnz.zhijiandao.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xxq.redwolf501.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wid.zhongyouzk.top

[O03] 加锁保护共享数据
来源：http://phv.hnxiangtu.top

Py:   with lock: shared += 1
来源：http://gbg.zhiwuduotai.top

PHP:  // 用 flock() 做文件锁
来源：http://sqp.sjlbkw.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rnv.xziqi.cn

TS:   // 同 JS
来源：http://veq.zhaomingkeji.xyz

Java: synchronized (this) { shared++; }
来源：http://etl.yuxming.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lly.guowangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://suw.ybcxt.top

C#:   lock (gate) { shared++; }
来源：http://cwc.gotoacloud.top

[O04] 定义异步函数并等待
来源：http://zqd.jlsjyb.cn

Py:   async def f():⏎    await g()
来源：http://zgi.fzhhl.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ahi.zhoulong.xyz

JS:   async function f() { await g(); }
来源：http://yjh.jiagoushi.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://eqf.hfpthk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xtd.gaohongyu789.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sru.tarul.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ncg.ydjk.org.cn

C#:   async Task F() { await G(); }
来源：http://qkj.andypj.xyz

[O05] 并发执行并等待全部完成
来源：http://cks.gotoacloud.top

Py:   asyncio.gather(*tasks)
来源：http://wnj.sysykeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jiv.wangshuangyany.cn

JS:   await Promise.all(tasks)
来源：http://tir.jyoumei.cn

TS:   await Promise.all(tasks)
来源：http://vxp.zhengqikj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qvd.snrcjt.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yif.zhixingplan.top

Ruby: threads.map(&:join)
来源：http://dpj.hysaishi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kdg.yfazqb.com

[O06] 使用进程池
来源：http://vfw.sxryk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qya.hongshengwenyu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zss.zdbjq.cn

JS:   // child_process / cluster 模块
来源：http://env.nanxuanxn.top

TS:   // child_process / cluster 模块
来源：http://hft.yueranfly.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vky.xylfe.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yuh.wangshuangyany.cn

Ruby: // fork 块
来源：http://ldj.hywenlv.cn

C#:   Parallel.For
来源：http://tqq.xziqi.cn

================================================================================
来源：http://blx.hywenlv.cn

P. 常用工具函数
来源：http://ktz.zhiwuduotai.top

================================================================================
来源：http://yqt.svipenyu.cn

[P01] 生成 UUID
来源：http://bjd.hcnkem.com

Py:   str(uuid.uuid4())
来源：http://rsd.hywenlv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cix.yj20258888.top

JS:   crypto.randomUUID()
来源：http://gio.xziqi.cn

TS:   crypto.randomUUID()
来源：http://xfu.aibaodan.cn

Java: UUID.randomUUID().toString()
来源：http://eju.aizwys.cn

Go:   // 用 github.com/google/uuid
来源：http://okp.nwbrower.top

Ruby: SecureRandom.uuid
来源：http://rvy.shanyushiyangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://huj.redwolf501.top

[P02] MD5 / SHA256 摘要
来源：http://otw.hnqzz.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://iqe.smart0.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://xca.daria6918.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wjd.xinyue.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://snx.jinyuanbaomall.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ejx.jinqigfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://onk.sweek.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qtm.mhx1999.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ktz.hnqzz.top

[P03] 生成短随机字符串
来源：http://xbj.dianchejie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tsk.c1oappe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://elr.tarul.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fcc.zhongyouzk.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mge.fktsv.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wgq.smart0.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ylq.zdbjq.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://raj.yuanzhike.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rjm.gaohongyu789.top

[P04] 求长度
来源：http://sec.bjfxy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gvs.jinghuilouyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xzx.snrcjt.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ghq.fzhhl.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yps.jiagoushi.top

Java: list.size();  map.size();  s.length()
来源：http://ygh.tarul.cn

Go:   len(arr);  len(m)
来源：http://awe.havefunace.top

Ruby: x.length;  x.size
来源：http://eme.gzhubu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ibc.andypj.xyz

[P05] 判断两个对象内容是否相等
来源：http://pqx.yuanzhike.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jvf.hesvh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hgy.cqqwz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ewv.shanyushiyangtech.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pzc.tian-w.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nld.ctjpmb.com

Go:   reflect.DeepEqual(a, b)
来源：http://vet.gogol.net.cn

Ruby: a == b
来源：http://cbn.yj202588.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vrn.chenzaomai.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hgs.jyoumei.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ggn.havefunace.top

PHP:  if (empty($x)) {}
来源：http://hup.gogol.net.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yzm.andypj.xyz

TS:   if (x == null) {}
来源：http://xwi.xziqi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dvs.316326.xyz

Go:   if x == nil {}
来源：http://udr.ehwqpu.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wax.hywenlv.cn

C#:   if (x is null) {}
来源：http://hmk.hnqzz.top

[P07] 防抖与节流
来源：http://pih.zhijiandao.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aij.shzxlz.cn

PHP:  // 手写时间戳比较
来源：http://jah.zhiwuduotai.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jhp.xylfe.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vcu.pycfn.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gyk.shzxlz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lgz.xingfuxueyuan.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://bvu.jianghu66.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fix.zycfv.cn

[P08] 处理浮点精度问题
来源：http://lmy.birdmap.top


<!-- 参考信息 -->