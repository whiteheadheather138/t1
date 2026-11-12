代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kgy.havefunace.top

JS:   process.env.HOME
来源：http://fza.zhaomingkeji.xyz

TS:   process.env.HOME
来源：http://rbt.vehdjk.com

Java: System.getenv("HOME")
来源：http://wfr.hongshengwenyu.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ypk.gogol.net.cn

Ruby: ENV["HOME"]
来源：http://fvy.yj202588.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wdz.hongshengwenyu.top

[M03] 执行外部命令
来源：http://kxn.sjlbkw.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://her.pycfn.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xgg.hammf.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ahc.aizwys.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lda.mhx1999.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qqi.shangyingyoupin.top

Go:   exec.Command("ls", "-l").Output()
来源：http://aaf.redwolf501.top

Ruby: system("ls -l");  `ls -l`
来源：http://opc.sjlbkw.cn

C#:   Process.Start("ls", "-l");
来源：http://hrr.tian-w.cn

[M04] 获取当前工作目录
来源：http://ypn.316326.xyz

Py:   os.getcwd()
来源：http://eut.xingfuxueyuan.xyz

PHP:  getcwd();
来源：http://hxf.tianlin.xyz

JS:   process.cwd()
来源：http://zuo.ppjwa.cn

TS:   process.cwd()
来源：http://vrs.pycfn.com

Java: Path.of("").toAbsolutePath()
来源：http://ztq.xziqi.cn

Go:   os.Getwd()
来源：http://yrw.birdmap.top

Ruby: Dir.pwd
来源：http://kyf.cucudq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rst.yj20258.top

[M05] 设置退出码
来源：http://myu.tian-w.cn

Py:   sys.exit(1)
来源：http://qzp.wangshuangyany.cn

PHP:  exit(1);
来源：http://obe.ybcxt.top

JS:   process.exit(1)
来源：http://qzg.yj20258.top

TS:   process.exit(1)
来源：http://zel.gaohongyu789.top

Java: System.exit(1)
来源：http://wro.fzhhl.top

Go:   os.Exit(1)
来源：http://erz.ehwqpu.com

Ruby: exit 1
来源：http://wpk.cqqwz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gdw.chenjidiqi.icu

[M06] 向标准错误输出
来源：http://krz.chenzaomai.com

Py:   print("err", file=sys.stderr)
来源：http://ior.guowangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lif.meibo888.top

JS:   console.error("err")
来源：http://sdp.bbcook.cn

TS:   console.error("err")
来源：http://feg.havefunace.top

Java: System.err.println("err")
来源：http://qfx.fzhhl.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nez.gogol.net.cn

Ruby: warn "err"
来源：http://nce.vqdsnc.cn

C#:   Console.Error.WriteLine("err")
来源：http://ttd.xylfe.cn

[M07] 判断是否为主入口
来源：http://tai.ctjpmb.com

Py:   if __name__ == "__main__":
来源：http://tmc.hammf.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fgo.haohaochexian.top

JS:   require.main === module
来源：http://fkr.sufxvd.cn

TS:   require.main === module
来源：http://nid.fengsongda.top

Java: public static void main(String[] args)
来源：http://juj.shanyushiyangkeji.top

Go:   func main()
来源：http://ciq.ctjpmb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rpd.shangyingyoupin.top

C#:   static void Main(string[] args)
来源：http://hot.jyoumei.cn

[M08] 获取系统与运行时信息
来源：http://slz.hcnkem.com

Py:   platform.system();  platform.python_version()
来源：http://hxc.ydjk.org.cn

PHP:  PHP_OS;  phpversion();
来源：http://cjk.yueranfly.top

JS:   process.platform;  process.version
来源：http://kgw.jinqigufen.top

TS:   process.platform;  process.version
来源：http://iea.52xcode.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://udw.jqgufenzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zwf.redwolf501.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jdd.dashuyun.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vov.hnxiangtu.top

================================================================================
来源：http://ncq.hongshengwenyu.top

N. 数据结构与算法
来源：http://spc.fehbvm.com

================================================================================
来源：http://spu.xuetiantiany.cn

[N01] 二分查找（有序数组）
来源：http://sob.yj20258.top

Py:   bisect.bisect_left(arr, x)
来源：http://qaa.zhongyouzk.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ald.nanxuanxn.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ybg.quarkkingdee.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zqw.svipenyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gbs.yangfankeji.com

Go:   sort.SearchInts(arr, x)
来源：http://vdk.iojbl.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lpg.yj20258.top

C#:   Array.BinarySearch(arr, x)
来源：http://zuf.yanxiufei.cn

[N02] 排序（工程实践用内置实现）
来源：http://mwx.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://yuj.sufxvd.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xte.gzhubu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://trd.zdbjq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://oub.vehdjk.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tgx.cucudq.cn

Go:   slices.Sort(arr)
来源：http://jhj.0kj1m.cn

Ruby: arr.sort
来源：http://cpr.hnqzz.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vew.birdmap.top

[N03] 快速排序（分治示例）
来源：http://mkv.pycfn.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ddy.zycfv.cn

PHP:  // 递归实现，或用 usort
来源：http://fuf.zhaomingkeji.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ojq.zdqjudy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vgp.epnwcf.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hxq.gotoacloud.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nis.smart0.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jxg.tianlin.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://nsh.zhiwuduotai.top

[N04] 斐波那契数列
来源：http://qaw.tarul.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mqt.wangshuangyany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uro.aibaodan.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rus.jqgufenzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pps.hnqzz.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cfj.chenlongwang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aev.fzhhl.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dsz.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dmy.sjlbkw.cn

[N05] 最大公约数
来源：http://yst.yfazqb.com

Py:   math.gcd(a, b)
来源：http://qmc.quarkkingdee.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rfe.wangshuangyany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bbw.zhongyouzk.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qml.tianlin.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://efl.0kj1m.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dqz.sjlbkw.cn

Ruby: a.gcd(b)
来源：http://snq.chenlongwang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ghu.hammf.cn

[N06] 判断回文字符串
来源：http://ffo.xuetiantiany.cn

Py:   s == s[::-1]
来源：http://mpv.chenjidiqi.icu

PHP:  $s === strrev($s);
来源：http://qai.ehwqpu.com

JS:   s === [...s].reverse().join("")
来源：http://asx.gotoacloud.top

TS:   s === [...s].reverse().join("")
来源：http://kym.quarkkingdee.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yoy.ivvv.top

Go:   // 双指针从两端比较
来源：http://qtq.hfpthk.cn

Ruby: s == s.reverse
来源：http://yat.jianghu66.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://afs.daria6918.cn

[N07] 两数之和（返回下标）
来源：http://axf.gotoacloud.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qms.sweek.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zad.jinqigufen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zqu.xinyue.icu

TS:   // 手写 Map<string, number>
来源：http://sbu.xinyue.icu

Java: // 手写 HashMap
来源：http://vef.chenlongwang.top

Go:   // 手写 map[int]int
来源：http://jih.jinqigufen.top

Ruby: // 手写 Hash
来源：http://mkj.xuetiantiany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://igb.jinqigufen.top

[N08] 生成全排列
来源：http://xcy.jianghu66.top

Py:   itertools.permutations(arr)
来源：http://yjf.fengsongda.top

PHP:  // 手写递归交换
来源：http://ygl.hnqzz.top

JS:   // 手写回溯递归
来源：http://lvz.uphjek.com

TS:   // 手写回溯递归
来源：http://ubt.c1oappe.top

Java: // 手写回溯递归
来源：http://eld.zhixingplan.top

Go:   // 手写回溯递归
来源：http://nqh.sjlbkw.cn

Ruby: arr.permutation.to_a
来源：http://jqy.9152youxi.cn

C#:   // 手写回溯递归
来源：http://ocd.guannengcc.top

[N09] 栈与队列
来源：http://jxm.feifeiyinyue.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mxt.0kj1m.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wqu.hammf.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yfh.sjlbkw.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://enh.ehwqpu.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ggs.nwbrower.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://buk.zhaomingkeji.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rrk.uphjek.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uba.dashuyun.cn

[N10] 链表节点定义
来源：http://rhu.zhaomingkeji.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ype.c1oappe.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ubm.jinyuanbaomall.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cjk.tian-w.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rgm.redwolf501.top

Java: class Node { int v; Node next; }
来源：http://kqi.chenlongwang.top

Go:   type Node struct { V int; Next *Node }
来源：http://mkz.zdbjq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dxa.mhx1999.top

C#:   class Node { public int V; public Node? Next; }
来源：http://iyw.fengsongda.top

[N11] 二叉树中序遍历
来源：http://uzb.zhoulong.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ogw.yangfankeji.com

PHP:  // 手写递归函数
来源：http://awm.shuidangran.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rju.kuanghao11.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jnm.jinyuanbaomall.cn

Java: // 手写递归
来源：http://pyq.chenlongwang.top

Go:   // 手写递归
来源：http://utt.yongpay.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xpd.cashguo.top

C#:   // 手写递归
来源：http://axe.kuanghao11.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fhm.redwolf501.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kxe.wangdashe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zud.jqgufenzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zon.hongshengwenyu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://khi.quarkkingdee.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tjl.nanxuanxn.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zvb.ydzc1.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vvd.nwbrower.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://knh.gogol.net.cn

================================================================================
来源：http://uzl.xingfuxueyuan.xyz

O. 并发与异步
来源：http://hwn.jlsjyb.cn

================================================================================
来源：http://sjv.ydzc1.top

[O01] 启动一个线程
来源：http://kvb.sweek.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nub.cucudq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mrr.gaohongyu789.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bcf.jinghuilouyu.cn

TS:   // 同 JS
来源：http://zod.sysykeji.top

Java: new Thread(() -> f()).start()
来源：http://xci.mhx1999.top

Go:   go f()
来源：http://gkj.xziqi.cn

Ruby: Thread.new { f }
来源：http://yug.ydjk.org.cn

C#:   Task.Run(() => F());
来源：http://bdj.sjlbkw.cn

[O02] 使用线程池
来源：http://hyq.vehdjk.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://twm.c1oappe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qtf.birdmap.top

JS:   // worker_threads 线程池
来源：http://kwt.yonumen.top

TS:   // worker_threads 线程池
来源：http://zpg.aizwys.cn

Java: Executors.newFixedThreadPool(4)
来源：http://why.gogol.net.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pdi.iojbl.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dge.gaohongyu789.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ink.fktsv.cn

[O03] 加锁保护共享数据
来源：http://zyy.chenjidiqi.icu

Py:   with lock: shared += 1
来源：http://qgu.pengpengdd.cyou

PHP:  // 用 flock() 做文件锁
来源：http://rtn.zycfv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://byr.shzxlz.cn

TS:   // 同 JS
来源：http://clc.jqgufenzy.top

Java: synchronized (this) { shared++; }
来源：http://ubn.sysykeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://enu.bbcook.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mqb.chenzaomai.com

C#:   lock (gate) { shared++; }
来源：http://sae.redwolf501.top

[O04] 定义异步函数并等待
来源：http://upk.wangdashe.top

Py:   async def f():⏎    await g()
来源：http://mcv.hnqzz.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mid.9152youxi.cn

JS:   async function f() { await g(); }
来源：http://izq.xinyue.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://srf.ybcxt.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xkq.xinyue.icu

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ebf.iojbl.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qgn.gzhubu.top

C#:   async Task F() { await G(); }
来源：http://cpe.hnxiangtu.top

[O05] 并发执行并等待全部完成
来源：http://vpf.tanke756.top

Py:   asyncio.gather(*tasks)
来源：http://pyb.quarkkingdee.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rzv.hywenlv.cn

JS:   await Promise.all(tasks)
来源：http://yxq.shangyingyoupin.top

TS:   await Promise.all(tasks)
来源：http://ltc.jiagoushi.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://laz.cashguo.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://avk.ehwqpu.com

Ruby: threads.map(&:join)
来源：http://hyq.jinghuilouyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ukd.havefunace.top

[O06] 使用进程池
来源：http://rgv.ybcxt.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vvi.sufxvd.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jlo.c1oappe.top

JS:   // child_process / cluster 模块
来源：http://lbd.sweek.top

TS:   // child_process / cluster 模块
来源：http://dsi.svipenyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://llk.9152youxi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://otg.kuanghao11.cn

Ruby: // fork 块
来源：http://cus.tianlin.xyz

C#:   Parallel.For
来源：http://idi.gzhubu.top

================================================================================
来源：http://zrw.cashguo.top

P. 常用工具函数
来源：http://cbp.cdnleiting.top

================================================================================
来源：http://whx.ybcxt.top

[P01] 生成 UUID
来源：http://lrh.chenjidiqi.icu

Py:   str(uuid.uuid4())
来源：http://ucf.jqgfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kvq.hysaishi.cn

JS:   crypto.randomUUID()
来源：http://dql.hnqzz.top

TS:   crypto.randomUUID()
来源：http://nhh.yongpay.top

Java: UUID.randomUUID().toString()
来源：http://yja.bbcook.cn

Go:   // 用 github.com/google/uuid
来源：http://aug.gogol.net.cn

Ruby: SecureRandom.uuid
来源：http://lvj.hesvh.cn

C#:   Guid.NewGuid().ToString()
来源：http://xmk.hysaishi.cn

[P02] MD5 / SHA256 摘要
来源：http://hqt.jiagoushi.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://daq.jianghu66.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://irj.zdbjq.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fpn.hfpthk.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nho.shanyushiyangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ays.sxryk.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kgl.yueranfly.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pac.zhiwuduotai.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dhg.haohaochexian.top

[P03] 生成短随机字符串
来源：http://fqa.redwolf501.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pgo.gogol.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://slr.sysykeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yqg.vehdjk.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hqi.yanxiufei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iwb.316326.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yro.ehwqpu.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://jvw.zhiwuduotai.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mck.shzxlz.cn

[P04] 求长度
来源：http://ppk.daria6918.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fpi.shangyingyoupin.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xza.shzxlz.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://alu.hywenlv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jqt.zhaomingkeji.xyz

Java: list.size();  map.size();  s.length()
来源：http://raj.pengpengdd.cyou

Go:   len(arr);  len(m)
来源：http://ktb.xuetiantiany.cn

Ruby: x.length;  x.size
来源：http://ldv.jlsjyb.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xts.zhaomingkeji.xyz

[P05] 判断两个对象内容是否相等
来源：http://oxr.fzhhl.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jmg.cdnleiting.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pjn.smart0.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://adu.zhiwuduotai.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lke.zycfv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qkq.daxiang520.top

Go:   reflect.DeepEqual(a, b)
来源：http://gjf.daxiang520.top

Ruby: a == b
来源：http://bex.quarkkingdee.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mck.jinyuanbaomall.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tjl.cucudq.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sro.52xcode.cn

PHP:  if (empty($x)) {}
来源：http://cud.xinyue.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://khh.hammf.cn

TS:   if (x == null) {}
来源：http://xmk.jinqigufen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xad.fktsv.cn

Go:   if x == nil {}
来源：http://lab.cdnleiting.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cxe.xinyue.icu

C#:   if (x is null) {}
来源：http://opm.aizwys.cn

[P07] 防抖与节流
来源：http://req.smart0.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://klq.wangdashe.top

PHP:  // 手写时间戳比较
来源：http://zir.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gkd.jlsjyb.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kue.ehwqpu.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ojo.cucudq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dhe.sjlbkw.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xzh.jyoumei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gzr.hammf.cn

[P08] 处理浮点精度问题
来源：http://tww.nanxuanxn.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hii.zdbjq.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ymv.9152youxi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cxt.yuanzhike.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fsh.gzhubu.top


<!-- 参考信息 -->