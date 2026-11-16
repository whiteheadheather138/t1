代发 wailian999

Ruby: ARGV
来源：http://tep.yueranfly.top

C#:   args 数组（Main 方法参数）
来源：http://ecz.sufxvd.cn

[M02] 读取环境变量
来源：http://jpe.52xcode.cn

Py:   os.environ.get("HOME")
来源：http://fvf.zhixingplan.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aet.chenzaomai.com

JS:   process.env.HOME
来源：http://zuk.vehdjk.com

TS:   process.env.HOME
来源：http://hpg.jinqigufen.top

Java: System.getenv("HOME")
来源：http://pyn.feifeiyinyue.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dvh.tianlin.xyz

Ruby: ENV["HOME"]
来源：http://alk.jyoumei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dtx.hysaishi.cn

[M03] 执行外部命令
来源：http://ilg.cdnleiting.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lkb.cucudq.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://owf.epnwcf.com

JS:   child_process.execSync("ls -l").toString()
来源：http://rtx.gzhubu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cbc.hongshengwenyu.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bul.gotoacloud.top

Go:   exec.Command("ls", "-l").Output()
来源：http://drp.smart0.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://jev.shanyushiyangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://ytv.ivvv.top

[M04] 获取当前工作目录
来源：http://zjz.jinqigufen.top

Py:   os.getcwd()
来源：http://dxv.yj202588.top

PHP:  getcwd();
来源：http://nlb.aibaodan.cn

JS:   process.cwd()
来源：http://rxb.ydjk.org.cn

TS:   process.cwd()
来源：http://xqt.daria6918.cn

Java: Path.of("").toAbsolutePath()
来源：http://aun.xingfuxueyuan.xyz

Go:   os.Getwd()
来源：http://mhj.bbcook.cn

Ruby: Dir.pwd
来源：http://gmq.ydjk.org.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ywk.hysaishi.cn

[M05] 设置退出码
来源：http://fkb.hfpthk.cn

Py:   sys.exit(1)
来源：http://qlj.sweek.top

PHP:  exit(1);
来源：http://noo.52xcode.cn

JS:   process.exit(1)
来源：http://loq.cashguo.top

TS:   process.exit(1)
来源：http://lfa.tianlin.xyz

Java: System.exit(1)
来源：http://heg.ehwqpu.com

Go:   os.Exit(1)
来源：http://aae.shzxlz.cn

Ruby: exit 1
来源：http://ldd.hesvh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uyr.yj20258888.top

[M06] 向标准错误输出
来源：http://apr.guannengcc.top

Py:   print("err", file=sys.stderr)
来源：http://xmn.yj20258.top

PHP:  fwrite(STDERR, "err\n");
来源：http://tzf.zdqjudy.top

JS:   console.error("err")
来源：http://eyp.yangfankeji.com

TS:   console.error("err")
来源：http://uho.meibo888.top

Java: System.err.println("err")
来源：http://fqm.hongshengwenyu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ttj.hfpthk.cn

Ruby: warn "err"
来源：http://raj.quarkkingdee.top

C#:   Console.Error.WriteLine("err")
来源：http://ibn.andypj.xyz

[M07] 判断是否为主入口
来源：http://kkn.vehdjk.com

Py:   if __name__ == "__main__":
来源：http://lwm.hongshengwenyu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://srt.316326.xyz

JS:   require.main === module
来源：http://ojt.yanxiufei.cn

TS:   require.main === module
来源：http://abs.zhiwuduotai.top

Java: public static void main(String[] args)
来源：http://wrb.zhoulong.xyz

Go:   func main()
来源：http://ppy.yanxiufei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zul.nanxuanxn.top

C#:   static void Main(string[] args)
来源：http://jvo.feifeiyinyue.top

[M08] 获取系统与运行时信息
来源：http://uzv.shanyushiyangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://eul.c1oappe.top

PHP:  PHP_OS;  phpversion();
来源：http://tim.fanxiaobao.xyz

JS:   process.platform;  process.version
来源：http://krk.gzhubu.top

TS:   process.platform;  process.version
来源：http://qcx.wangshuangyany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vfb.ydzc1.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ytz.shanyushiyangtech.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yco.epnwcf.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://lap.ctjpmb.com

================================================================================
来源：http://ige.ywan-chungtsiang.top

N. 数据结构与算法
来源：http://tvl.gzhubu.top

================================================================================
来源：http://fki.hysaishi.cn

[N01] 二分查找（有序数组）
来源：http://kqq.yueranfly.top

Py:   bisect.bisect_left(arr, x)
来源：http://xsw.yfazqb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ycf.wangdashe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bvw.iojbl.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://znz.hnqzz.top

Java: Arrays.binarySearch(arr, x)
来源：http://xmz.yuanzhike.top

Go:   sort.SearchInts(arr, x)
来源：http://okw.hywenlv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://kzy.zhengqikj.top

C#:   Array.BinarySearch(arr, x)
来源：http://xgn.kuanghao11.cn

[N02] 排序（工程实践用内置实现）
来源：http://qjx.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://nkr.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lqn.hywenlv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://glq.meibo888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dsh.cashguo.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xah.c1oappe.top

Go:   slices.Sort(arr)
来源：http://ycn.yvedp.cn

Ruby: arr.sort
来源：http://jjt.zhongyouzk.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://fuy.xingfuxueyuan.xyz

[N03] 快速排序（分治示例）
来源：http://bup.yfazqb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fju.cheryme.top

PHP:  // 递归实现，或用 usort
来源：http://ufh.snrcjt.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nax.ybcxt.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lmg.redwolf501.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yay.jqgfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jbe.xingfuxueyuan.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zgi.chenlongwang.top

C#:   // 手写递归，或 Array.Sort
来源：http://cht.zhijiandao.cn

[N04] 斐波那契数列
来源：http://ltw.svipenyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://irv.guowangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://flb.zdbjq.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://otq.jinyuanbaomall.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://det.ctjpmb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ffy.hywenlv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ezm.jianghu66.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tdy.vehdjk.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lbj.0kj1m.cn

[N05] 最大公约数
来源：http://moe.shangyingyoupin.top

Py:   math.gcd(a, b)
来源：http://uuy.jiagoushi.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://leh.jinyuanbaomall.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ryn.cashguo.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://umn.dianchejie.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qvl.tarul.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fyo.jyoumei.cn

Ruby: a.gcd(b)
来源：http://huo.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://chl.gaohongyu789.top

[N06] 判断回文字符串
来源：http://odt.jianghu66.top

Py:   s == s[::-1]
来源：http://ybt.smart0.xyz

PHP:  $s === strrev($s);
来源：http://dyh.hongshengwenyu.top

JS:   s === [...s].reverse().join("")
来源：http://ndy.fktsv.cn

TS:   s === [...s].reverse().join("")
来源：http://xqv.c1oappe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xcp.sxryk.cn

Go:   // 双指针从两端比较
来源：http://tcm.zhixingplan.top

Ruby: s == s.reverse
来源：http://zji.sufxvd.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://chi.9152youxi.cn

[N07] 两数之和（返回下标）
来源：http://qfs.vehdjk.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kjo.xinyue.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lml.andypj.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://czm.xuanzx.com

TS:   // 手写 Map<string, number>
来源：http://qlc.zhiwuduotai.top

Java: // 手写 HashMap
来源：http://igy.xziqi.cn

Go:   // 手写 map[int]int
来源：http://ymx.ehwqpu.com

Ruby: // 手写 Hash
来源：http://fsh.chenzaomai.com

C#:   // 手写 Dictionary<int, int>
来源：http://lgo.nanxuanxn.top

[N08] 生成全排列
来源：http://zte.jqgfzy.top

Py:   itertools.permutations(arr)
来源：http://iwt.shuidangran.top

PHP:  // 手写递归交换
来源：http://umw.cdnleiting.top

JS:   // 手写回溯递归
来源：http://dij.birdmap.top

TS:   // 手写回溯递归
来源：http://kbf.yongpay.top

Java: // 手写回溯递归
来源：http://pyr.zhongyouzk.top

Go:   // 手写回溯递归
来源：http://tyk.haohaochexian.top

Ruby: arr.permutation.to_a
来源：http://kwa.jqgfzy.top

C#:   // 手写回溯递归
来源：http://bme.sysykeji.top

[N09] 栈与队列
来源：http://abo.snrcjt.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://axw.hywenlv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wgm.kuanghao11.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uww.c1oappe.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hxk.yj202588.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tiz.9152youxi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://awa.zdqjudy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rkv.hongshengwenyu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fwe.ydzc1.top

[N10] 链表节点定义
来源：http://jth.uphjek.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wdu.ctjpmb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://vlc.pycfn.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kxl.yonumen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ihc.vqdsnc.cn

Java: class Node { int v; Node next; }
来源：http://swh.jinqigufen.top

Go:   type Node struct { V int; Next *Node }
来源：http://yki.gaohongyu789.top

Ruby: Node = Struct.new(:v, :next)
来源：http://cev.redwolf501.top

C#:   class Node { public int V; public Node? Next; }
来源：http://cqk.zhoulong.xyz

[N11] 二叉树中序遍历
来源：http://xml.hywenlv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pws.yfazqb.com

PHP:  // 手写递归函数
来源：http://erf.yuanzhike.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bmo.aibaodan.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vqn.aibaodan.cn

Java: // 手写递归
来源：http://wcg.hywenlv.cn

Go:   // 手写递归
来源：http://pbm.ybcxt.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vsx.c1oappe.top

C#:   // 手写递归
来源：http://qee.yueranfly.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://feg.jiagoushi.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://opc.epnwcf.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rnr.bjfxy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://elx.jianghu66.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nws.hnxiangtu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bht.fktsv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nqy.pengpengdd.cyou

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qvj.quarkkingdee.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nkc.xylfe.cn

================================================================================
来源：http://uze.gotoacloud.top

O. 并发与异步
来源：http://jfm.sysykeji.top

================================================================================
来源：http://far.c1oappe.top

[O01] 启动一个线程
来源：http://yxt.nanxinkj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://svx.ppjwa.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zbb.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://prh.pycfn.com

TS:   // 同 JS
来源：http://dgx.cdnleiting.top

Java: new Thread(() -> f()).start()
来源：http://xtc.havefunace.top

Go:   go f()
来源：http://gop.redwolf501.top

Ruby: Thread.new { f }
来源：http://fvg.zycfv.cn

C#:   Task.Run(() => F());
来源：http://evz.cheryme.top

[O02] 使用线程池
来源：http://bvd.chenzaomai.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://eyj.xingfuxueyuan.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mwv.hcnkem.com

JS:   // worker_threads 线程池
来源：http://ylj.hnxiangtu.top

TS:   // worker_threads 线程池
来源：http://ade.bbcook.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zvz.birdmap.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oqc.dashuyun.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oyl.chenjidiqi.icu

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rkm.yuanzhike.top

[O03] 加锁保护共享数据
来源：http://ukj.jyoumei.cn

Py:   with lock: shared += 1
来源：http://ffv.uphjek.com

PHP:  // 用 flock() 做文件锁
来源：http://vjx.c1oappe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kcn.hfpthk.cn

TS:   // 同 JS
来源：http://apz.sysykeji.top

Java: synchronized (this) { shared++; }
来源：http://vir.316326.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tdh.dianchejie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lwh.0kj1m.cn

C#:   lock (gate) { shared++; }
来源：http://abp.tian-w.cn

[O04] 定义异步函数并等待
来源：http://klc.hnxiangtu.top

Py:   async def f():⏎    await g()
来源：http://tsx.fengsongda.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qhw.xingfuxueyuan.xyz

JS:   async function f() { await g(); }
来源：http://qos.jinyuanbaomall.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ocg.andypj.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hbd.52xcode.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bse.xuetiantiany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zuz.shanyushiyangtech.top

C#:   async Task F() { await G(); }
来源：http://lce.shanyushiyangtech.top

[O05] 并发执行并等待全部完成
来源：http://oec.yj202588.top

Py:   asyncio.gather(*tasks)
来源：http://lnj.shuidangran.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bad.yfazqb.com

JS:   await Promise.all(tasks)
来源：http://nlf.sysykeji.top

TS:   await Promise.all(tasks)
来源：http://erq.daria6918.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.zhixingplan.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jyv.xziqi.cn

Ruby: threads.map(&:join)
来源：http://mio.fzhhl.top

C#:   await Task.WhenAll(t1, t2)
来源：http://puj.aibaodan.cn

[O06] 使用进程池
来源：http://oqu.yongpay.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xjw.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gke.yuxming.cn

JS:   // child_process / cluster 模块
来源：http://vzx.zhiwuduotai.top

TS:   // child_process / cluster 模块
来源：http://jne.sxryk.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://non.yonumen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://grq.jinyuanbaomall.cn

Ruby: // fork 块
来源：http://cxz.tarul.cn

C#:   Parallel.For
来源：http://aet.chenlongwang.top

================================================================================
来源：http://xxh.xinyue.icu

P. 常用工具函数
来源：http://qlp.ydzc1.top

================================================================================
来源：http://jcy.aibaodan.cn

[P01] 生成 UUID
来源：http://suv.pycfn.com

Py:   str(uuid.uuid4())
来源：http://lwc.jianghu66.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://par.chenjidiqi.icu

JS:   crypto.randomUUID()
来源：http://ugg.jinyuanbaomall.cn

TS:   crypto.randomUUID()
来源：http://wmo.aibaodan.cn

Java: UUID.randomUUID().toString()
来源：http://ycp.fengsongda.top

Go:   // 用 github.com/google/uuid
来源：http://rcp.yuxming.cn

Ruby: SecureRandom.uuid
来源：http://rxx.316326.xyz

C#:   Guid.NewGuid().ToString()
来源：http://osz.xinyue.icu

[P02] MD5 / SHA256 摘要
来源：http://yxz.jianghu66.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xas.sufxvd.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://awb.birdmap.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mkl.gogol.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nhb.daxiang520.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lee.cheryme.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kdg.birdmap.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uub.fehbvm.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jdx.zhaomingkeji.xyz

[P03] 生成短随机字符串
来源：http://yks.smart0.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mxk.sxryk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fyl.yongpay.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ikg.hnqzz.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jqr.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xfi.hysaishi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cyi.cashguo.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ftv.cashguo.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jye.0kj1m.cn

[P04] 求长度
来源：http://ohv.cashguo.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bxn.chenzaomai.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eat.svipenyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qlz.hcnkem.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qvm.zhiwuduotai.top

Java: list.size();  map.size();  s.length()
来源：http://nla.sysykeji.top

Go:   len(arr);  len(m)
来源：http://she.redwolf501.top

Ruby: x.length;  x.size
来源：http://ywz.cashguo.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://znk.jiagoushi.top

[P05] 判断两个对象内容是否相等
来源：http://krc.jqgufenzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ztv.jiagoushi.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gng.ehwqpu.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wfw.xuetiantiany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vyf.hywenlv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vjq.ydjk.org.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zzz.shanyushiyangkeji.top

Ruby: a == b
来源：http://wif.ydzc1.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vud.jinyuanbaomall.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vzz.zdqjudy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ikk.sweek.top

PHP:  if (empty($x)) {}
来源：http://mzd.xuetiantiany.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://toh.birdmap.top

TS:   if (x == null) {}
来源：http://kdp.shanyushiyangtech.top

Java: if (x == null || x.isEmpty()) {}
来源：http://dxv.hfpthk.cn

Go:   if x == nil {}
来源：http://uco.9152youxi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yjt.aibaodan.cn

C#:   if (x is null) {}
来源：http://ptr.bbcook.cn

[P07] 防抖与节流
来源：http://xuy.316326.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xtm.cashguo.top

PHP:  // 手写时间戳比较
来源：http://xnm.havefunace.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zhs.hongshengwenyu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ksv.cucudq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xtn.52xcode.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jun.redwolf501.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gef.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uiu.sjlbkw.cn

[P08] 处理浮点精度问题
来源：http://vtt.zhixingplan.top


<!-- 参考信息 -->