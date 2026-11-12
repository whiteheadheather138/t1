代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bik.yangfankeji.com

Ruby: ENV["HOME"]
来源：http://gjn.yuxming.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vhs.xingfuxueyuan.xyz

[M03] 执行外部命令
来源：http://sgq.zhixingplan.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ohy.snrcjt.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cpj.aibaodan.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yke.ctjpmb.com

TS:   child_process.execSync("ls -l").toString()
来源：http://cvx.zhixingplan.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://azr.ydzc1.top

Go:   exec.Command("ls", "-l").Output()
来源：http://wpn.xuetiantiany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dtg.jinqigfzy.top

C#:   Process.Start("ls", "-l");
来源：http://vbe.ehwqpu.com

[M04] 获取当前工作目录
来源：http://qlx.xuetiantiany.cn

Py:   os.getcwd()
来源：http://ngg.daxiang520.top

PHP:  getcwd();
来源：http://mnx.zhongyouzk.top

JS:   process.cwd()
来源：http://tsu.yangfankeji.com

TS:   process.cwd()
来源：http://yux.fengsongda.top

Java: Path.of("").toAbsolutePath()
来源：http://dzt.9152youxi.cn

Go:   os.Getwd()
来源：http://zmv.tianlin.xyz

Ruby: Dir.pwd
来源：http://piq.316326.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://mal.52xcode.cn

[M05] 设置退出码
来源：http://efc.andypj.xyz

Py:   sys.exit(1)
来源：http://kvh.zdbjq.cn

PHP:  exit(1);
来源：http://jvu.fengsongda.top

JS:   process.exit(1)
来源：http://naz.zhiwuduotai.top

TS:   process.exit(1)
来源：http://utr.sufxvd.cn

Java: System.exit(1)
来源：http://tby.gogol.net.cn

Go:   os.Exit(1)
来源：http://jbw.cdnleiting.top

Ruby: exit 1
来源：http://zcu.zhengqikj.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://odl.pycfn.com

[M06] 向标准错误输出
来源：http://lad.dashuyun.cn

Py:   print("err", file=sys.stderr)
来源：http://jhp.fehbvm.com

PHP:  fwrite(STDERR, "err\n");
来源：http://pgu.birdmap.top

JS:   console.error("err")
来源：http://ywv.zdqjudy.top

TS:   console.error("err")
来源：http://txg.guowangkeji.top

Java: System.err.println("err")
来源：http://plo.chenjidiqi.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ydl.dianchejie.cn

Ruby: warn "err"
来源：http://xsu.jyoumei.cn

C#:   Console.Error.WriteLine("err")
来源：http://uhx.zhaomingkeji.xyz

[M07] 判断是否为主入口
来源：http://btu.sufxvd.cn

Py:   if __name__ == "__main__":
来源：http://ttq.gotoacloud.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qbq.shanyushiyangtech.top

JS:   require.main === module
来源：http://ptx.zhiwuduotai.top

TS:   require.main === module
来源：http://spr.havefunace.top

Java: public static void main(String[] args)
来源：http://nnv.daria6918.cn

Go:   func main()
来源：http://mco.yuxming.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uzc.yvedp.cn

C#:   static void Main(string[] args)
来源：http://det.cqqwz.cn

[M08] 获取系统与运行时信息
来源：http://voa.vehdjk.com

Py:   platform.system();  platform.python_version()
来源：http://yxe.chenlongwang.top

PHP:  PHP_OS;  phpversion();
来源：http://zrs.chenzaomai.com

JS:   process.platform;  process.version
来源：http://xli.jinyuanbaomall.cn

TS:   process.platform;  process.version
来源：http://nrd.xuetiantiany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oqm.zhaomingkeji.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://uwe.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hql.nwbrower.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gid.yj20258888.top

================================================================================
来源：http://icq.shzxlz.cn

N. 数据结构与算法
来源：http://kpv.birdmap.top

================================================================================
来源：http://cpo.tarul.cn

[N01] 二分查找（有序数组）
来源：http://nuc.ppjwa.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ghl.hywenlv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lwp.nwbrower.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pla.jyoumei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sqe.nwbrower.top

Java: Arrays.binarySearch(arr, x)
来源：http://oxn.sjlbkw.cn

Go:   sort.SearchInts(arr, x)
来源：http://hku.jlsjyb.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pos.0kj1m.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ili.tian-w.cn

[N02] 排序（工程实践用内置实现）
来源：http://eey.vqdsnc.cn

Py:   sorted(arr);  arr.sort()
来源：http://zqn.sysykeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hcf.yvedp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pys.cdnleiting.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fkh.hongshengwenyu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bfh.hnxiangtu.top

Go:   slices.Sort(arr)
来源：http://vsz.andypj.xyz

Ruby: arr.sort
来源：http://thq.cdnleiting.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://aew.meibo888.top

[N03] 快速排序（分治示例）
来源：http://tju.uphjek.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mgn.guowangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://vup.aizwys.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dku.yueranfly.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pbu.aibaodan.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xcf.ctjpmb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://joy.cdnleiting.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cfd.dashuyun.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xql.guowangkeji.top

[N04] 斐波那契数列
来源：http://thu.sjlbkw.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dut.bbcook.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bry.shuidangran.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pdx.xingfuxueyuan.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kql.snrcjt.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ssw.nanxinkj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://brt.yj20258.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://emp.shuidangran.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bbm.gogol.net.cn

[N05] 最大公约数
来源：http://zrf.fktsv.cn

Py:   math.gcd(a, b)
来源：http://lpc.zdqjudy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rku.yuxming.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://btk.jqgfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dni.shanyushiyangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://clw.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tdd.tian-w.cn

Ruby: a.gcd(b)
来源：http://bda.feifeiyinyue.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yfs.dianchejie.cn

[N06] 判断回文字符串
来源：http://fvg.ydjk.org.cn

Py:   s == s[::-1]
来源：http://awj.sjlbkw.cn

PHP:  $s === strrev($s);
来源：http://bit.zhoulong.xyz

JS:   s === [...s].reverse().join("")
来源：http://ofw.hnqzz.top

TS:   s === [...s].reverse().join("")
来源：http://wqo.svipenyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://alr.hammf.cn

Go:   // 双指针从两端比较
来源：http://xbg.quarkkingdee.top

Ruby: s == s.reverse
来源：http://eua.uphjek.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://iiz.yanxiufei.cn

[N07] 两数之和（返回下标）
来源：http://syu.sufxvd.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dir.jianghu66.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dso.fktsv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ruz.xuanzx.com

TS:   // 手写 Map<string, number>
来源：http://uko.tian-w.cn

Java: // 手写 HashMap
来源：http://xmk.uphjek.com

Go:   // 手写 map[int]int
来源：http://cia.hfpthk.cn

Ruby: // 手写 Hash
来源：http://nfe.52xcode.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ncw.guannengcc.top

[N08] 生成全排列
来源：http://msr.cashguo.top

Py:   itertools.permutations(arr)
来源：http://mrz.chenzaomai.com

PHP:  // 手写递归交换
来源：http://sma.cucudq.cn

JS:   // 手写回溯递归
来源：http://ikj.jlsjyb.cn

TS:   // 手写回溯递归
来源：http://uou.yongpay.top

Java: // 手写回溯递归
来源：http://fml.wangshuangyany.cn

Go:   // 手写回溯递归
来源：http://zqc.ywan-chungtsiang.top

Ruby: arr.permutation.to_a
来源：http://vyn.dianchejie.cn

C#:   // 手写回溯递归
来源：http://hcc.xingfuxueyuan.xyz

[N09] 栈与队列
来源：http://oci.xuetiantiany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uez.ivvv.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://glu.zhoulong.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gsh.xylfe.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iwd.pycfn.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pft.gotoacloud.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pjy.epnwcf.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://grp.yangfankeji.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hte.ywan-chungtsiang.top

[N10] 链表节点定义
来源：http://xkj.vehdjk.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://las.jinyuanbaomall.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ctg.yj20258888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://erp.kuanghao11.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qvp.wangdashe.top

Java: class Node { int v; Node next; }
来源：http://keg.haohaochexian.top

Go:   type Node struct { V int; Next *Node }
来源：http://yri.shangyingyoupin.top

Ruby: Node = Struct.new(:v, :next)
来源：http://lfi.chenjidiqi.icu

C#:   class Node { public int V; public Node? Next; }
来源：http://otl.c1oappe.top

[N11] 二叉树中序遍历
来源：http://gxe.xziqi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qoz.dashuyun.cn

PHP:  // 手写递归函数
来源：http://tgq.fanxiaobao.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bbp.yanxiufei.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ykm.pengpengdd.cyou

Java: // 手写递归
来源：http://ehd.dashuyun.cn

Go:   // 手写递归
来源：http://itz.shanyushiyangtech.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dvp.pycfn.com

C#:   // 手写递归
来源：http://huj.hcnkem.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tjp.hcnkem.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sma.jqgfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xqn.zhengqikj.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nds.shanyushiyangtech.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lni.vehdjk.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jry.shangyingyoupin.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fyt.fzhhl.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vpg.hfpthk.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xrq.yj20258.top

================================================================================
来源：http://ykk.shangyingyoupin.top

O. 并发与异步
来源：http://deb.hfpthk.cn

================================================================================
来源：http://hxp.jinyuanbaomall.cn

[O01] 启动一个线程
来源：http://zpx.jinqigufen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lve.jyoumei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cpd.ivvv.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sbp.jiagoushi.top

TS:   // 同 JS
来源：http://nye.yueranfly.top

Java: new Thread(() -> f()).start()
来源：http://bph.chenzaomai.com

Go:   go f()
来源：http://thq.zhijiandao.cn

Ruby: Thread.new { f }
来源：http://rhh.shanyushiyangtech.top

C#:   Task.Run(() => F());
来源：http://epn.jinyuanbaomall.cn

[O02] 使用线程池
来源：http://nww.sjlbkw.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kin.xziqi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://llh.quarkkingdee.top

JS:   // worker_threads 线程池
来源：http://qel.sxryk.cn

TS:   // worker_threads 线程池
来源：http://cny.nanxinkj.top

Java: Executors.newFixedThreadPool(4)
来源：http://vok.gotoacloud.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qex.jqgufenzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ebi.fanxiaobao.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hbr.meibo888.top

[O03] 加锁保护共享数据
来源：http://rfo.zhongyouzk.top

Py:   with lock: shared += 1
来源：http://zmj.cashguo.top

PHP:  // 用 flock() 做文件锁
来源：http://rgw.tian-w.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kxc.svipenyu.cn

TS:   // 同 JS
来源：http://msy.aibaodan.cn

Java: synchronized (this) { shared++; }
来源：http://qfa.ybcxt.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ejf.jyoumei.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rjg.jqgfzy.top

C#:   lock (gate) { shared++; }
来源：http://irx.sysykeji.top

[O04] 定义异步函数并等待
来源：http://ptb.meibo888.top

Py:   async def f():⏎    await g()
来源：http://zjd.yuanzhike.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gft.quarkkingdee.top

JS:   async function f() { await g(); }
来源：http://oil.kuanghao11.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qvd.epnwcf.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fdq.cashguo.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jyi.aizwys.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rzv.pengpengdd.cyou

C#:   async Task F() { await G(); }
来源：http://hfo.jiagoushi.top

[O05] 并发执行并等待全部完成
来源：http://gno.52xcode.cn

Py:   asyncio.gather(*tasks)
来源：http://bsg.vqdsnc.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kdj.guowangkeji.top

JS:   await Promise.all(tasks)
来源：http://ppx.hongshengwenyu.top

TS:   await Promise.all(tasks)
来源：http://mhr.316326.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fsn.hywenlv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fwx.aizwys.cn

Ruby: threads.map(&:join)
来源：http://mfi.cdnleiting.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ewx.gzhubu.top

[O06] 使用进程池
来源：http://yik.cdnleiting.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dwp.sweek.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qzy.aizwys.cn

JS:   // child_process / cluster 模块
来源：http://nnm.zhaomingkeji.xyz

TS:   // child_process / cluster 模块
来源：http://lkb.hongshengwenyu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sir.shangyingyoupin.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zmk.jqgfzy.top

Ruby: // fork 块
来源：http://wpf.gogol.net.cn

C#:   Parallel.For
来源：http://gwv.snrcjt.cn

================================================================================
来源：http://nxw.jinyuanbaomall.cn

P. 常用工具函数
来源：http://vcz.hesvh.cn

================================================================================
来源：http://pge.xinyue.icu

[P01] 生成 UUID
来源：http://lum.cheryme.top

Py:   str(uuid.uuid4())
来源：http://iot.pycfn.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rzk.gotoacloud.top

JS:   crypto.randomUUID()
来源：http://sff.shuidangran.top

TS:   crypto.randomUUID()
来源：http://wbx.guowangkeji.top

Java: UUID.randomUUID().toString()
来源：http://bvh.yj202588.top

Go:   // 用 github.com/google/uuid
来源：http://quj.kuanghao11.cn

Ruby: SecureRandom.uuid
来源：http://gyf.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://bmf.hesvh.cn

[P02] MD5 / SHA256 摘要
来源：http://tuu.epnwcf.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aiq.quarkkingdee.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dpb.feifeiyinyue.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bpb.pycfn.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tdo.hysaishi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jcn.daxiang520.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nhx.xuanzx.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hiw.iojbl.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wwi.vehdjk.com

[P03] 生成短随机字符串
来源：http://iea.haohaochexian.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gra.cashguo.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ogx.yuxming.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zhz.vqdsnc.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ioc.dianchejie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cik.fehbvm.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://whw.yonumen.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://syg.hammf.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lwq.sxryk.cn

[P04] 求长度
来源：http://vpi.yvedp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yrp.yanxiufei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aqp.c1oappe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://icc.jlsjyb.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kux.guowangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://wrr.nwbrower.top

Go:   len(arr);  len(m)
来源：http://ucm.jianghu66.top

Ruby: x.length;  x.size
来源：http://phn.jqgfzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://kxn.dianchejie.cn

[P05] 判断两个对象内容是否相等
来源：http://ykr.ctjpmb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://yxp.uphjek.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jxz.ydjk.org.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yya.bbcook.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sll.gogol.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mev.yuanzhike.top

Go:   reflect.DeepEqual(a, b)
来源：http://bxz.chenzaomai.com

Ruby: a == b
来源：http://cnz.birdmap.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hwg.gzhubu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ylk.hammf.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://naw.wangshuangyany.cn

PHP:  if (empty($x)) {}
来源：http://vep.pycfn.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tgs.xuetiantiany.cn

TS:   if (x == null) {}
来源：http://afa.epnwcf.com

Java: if (x == null || x.isEmpty()) {}
来源：http://vor.shanyushiyangkeji.top

Go:   if x == nil {}
来源：http://usm.jianghu66.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://axi.ivvv.top

C#:   if (x is null) {}
来源：http://rmd.andypj.xyz

[P07] 防抖与节流
来源：http://mju.hongshengwenyu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fww.gotoacloud.top

PHP:  // 手写时间戳比较
来源：http://vwr.jlsjyb.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rdp.tarul.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bvh.jianghu66.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mqi.jqgfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pfj.fehbvm.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://sny.sxryk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mgd.vehdjk.com

[P08] 处理浮点精度问题
来源：http://cxc.havefunace.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nva.nanxuanxn.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jym.zhengqikj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ptw.gzhubu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yqr.ydjk.org.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qxo.hywenlv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://btn.cashguo.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ucm.hnqzz.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tjh.iojbl.cn


<!-- 参考信息 -->