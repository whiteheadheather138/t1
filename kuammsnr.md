代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rgq.tianlin.xyz

Ruby: ENV["HOME"]
来源：http://izo.0kj1m.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ncy.shuidangran.top

[M03] 执行外部命令
来源：http://bgk.daxiang520.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://roa.xuanzx.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dls.nanxuanxn.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tjm.iojbl.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nrm.pycfn.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rfy.xuetiantiany.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://icu.gogol.net.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tvw.zycfv.cn

C#:   Process.Start("ls", "-l");
来源：http://lmo.ehwqpu.com

[M04] 获取当前工作目录
来源：http://uuf.redwolf501.top

Py:   os.getcwd()
来源：http://ysl.guowangkeji.top

PHP:  getcwd();
来源：http://psf.yangfankeji.com

JS:   process.cwd()
来源：http://kpc.sxryk.cn

TS:   process.cwd()
来源：http://dzx.yj20258.top

Java: Path.of("").toAbsolutePath()
来源：http://esm.hcnkem.com

Go:   os.Getwd()
来源：http://daq.cheryme.top

Ruby: Dir.pwd
来源：http://sin.xziqi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://hof.hongshengwenyu.top

[M05] 设置退出码
来源：http://wcu.shzxlz.cn

Py:   sys.exit(1)
来源：http://xqi.yanxiufei.cn

PHP:  exit(1);
来源：http://cbx.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://jcp.tian-w.cn

TS:   process.exit(1)
来源：http://gkh.vqdsnc.cn

Java: System.exit(1)
来源：http://ebk.sweek.top

Go:   os.Exit(1)
来源：http://wkv.ehwqpu.com

Ruby: exit 1
来源：http://qkn.vehdjk.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cny.feifeiyinyue.top

[M06] 向标准错误输出
来源：http://lka.jyoumei.cn

Py:   print("err", file=sys.stderr)
来源：http://ywb.hammf.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kny.zhoulong.xyz

JS:   console.error("err")
来源：http://zve.yfazqb.com

TS:   console.error("err")
来源：http://fek.redwolf501.top

Java: System.err.println("err")
来源：http://rxw.wangdashe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pvi.zhaomingkeji.xyz

Ruby: warn "err"
来源：http://oot.gogol.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://ggs.daria6918.cn

[M07] 判断是否为主入口
来源：http://kjl.chenlongwang.top

Py:   if __name__ == "__main__":
来源：http://oeu.yongpay.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yjv.fengsongda.top

JS:   require.main === module
来源：http://elk.yanxiufei.cn

TS:   require.main === module
来源：http://uhv.shuidangran.top

Java: public static void main(String[] args)
来源：http://jyt.ehwqpu.com

Go:   func main()
来源：http://pbv.shanyushiyangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sut.cdnleiting.top

C#:   static void Main(string[] args)
来源：http://nev.xinyue.icu

[M08] 获取系统与运行时信息
来源：http://zzg.yonumen.top

Py:   platform.system();  platform.python_version()
来源：http://iqt.hammf.cn

PHP:  PHP_OS;  phpversion();
来源：http://yfe.shuidangran.top

JS:   process.platform;  process.version
来源：http://tdg.fanxiaobao.xyz

TS:   process.platform;  process.version
来源：http://szg.yj20258.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kml.zhoulong.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://iwu.ybcxt.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hbl.jqgufenzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rpb.zhoulong.xyz

================================================================================
来源：http://hnp.vehdjk.com

N. 数据结构与算法
来源：http://fjm.shuidangran.top

================================================================================
来源：http://rqh.gotoacloud.top

[N01] 二分查找（有序数组）
来源：http://uyy.sysykeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://vun.jyoumei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cxw.jqgfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lzy.nanxinkj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fhr.cheryme.top

Java: Arrays.binarySearch(arr, x)
来源：http://ebd.jinyuanbaomall.cn

Go:   sort.SearchInts(arr, x)
来源：http://ols.nanxuanxn.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://fap.jinyuanbaomall.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ctv.nwbrower.top

[N02] 排序（工程实践用内置实现）
来源：http://waw.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://bdk.jinyuanbaomall.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xsy.jinqigfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://bom.yueranfly.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://djw.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dzr.shzxlz.cn

Go:   slices.Sort(arr)
来源：http://ewc.hfpthk.cn

Ruby: arr.sort
来源：http://hfb.zhixingplan.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://azd.hnqzz.top

[N03] 快速排序（分治示例）
来源：http://qft.meibo888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://neg.zhoulong.xyz

PHP:  // 递归实现，或用 usort
来源：http://guw.iojbl.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rap.aibaodan.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tsz.chenzaomai.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://spd.zhijiandao.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://znj.hcnkem.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sgl.hywenlv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kad.cashguo.top

[N04] 斐波那契数列
来源：http://zpj.0kj1m.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qet.hfpthk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://psb.vehdjk.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://brd.guowangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tyd.jqgfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vhw.sufxvd.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zia.xuetiantiany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zoz.andypj.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yjz.daria6918.cn

[N05] 最大公约数
来源：http://uyp.cashguo.top

Py:   math.gcd(a, b)
来源：http://acu.ydjk.org.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://yrl.hnqzz.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wbx.gzhubu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jpr.yuanzhike.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wwg.c1oappe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rpi.sufxvd.cn

Ruby: a.gcd(b)
来源：http://rwy.yj20258888.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hxw.chenzaomai.com

[N06] 判断回文字符串
来源：http://pxq.316326.xyz

Py:   s == s[::-1]
来源：http://eka.xinyue.icu

PHP:  $s === strrev($s);
来源：http://fow.ppjwa.cn

JS:   s === [...s].reverse().join("")
来源：http://udv.xingfuxueyuan.xyz

TS:   s === [...s].reverse().join("")
来源：http://ozr.nwbrower.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://iys.sweek.top

Go:   // 双指针从两端比较
来源：http://laf.ydjk.org.cn

Ruby: s == s.reverse
来源：http://oue.jqgufenzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qne.tarul.cn

[N07] 两数之和（返回下标）
来源：http://jjw.316326.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zxw.bjfxy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wks.jinghuilouyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bze.kuanghao11.cn

TS:   // 手写 Map<string, number>
来源：http://yrp.yongpay.top

Java: // 手写 HashMap
来源：http://kgb.hongshengwenyu.top

Go:   // 手写 map[int]int
来源：http://hhf.guannengcc.top

Ruby: // 手写 Hash
来源：http://nij.yj20258888.top

C#:   // 手写 Dictionary<int, int>
来源：http://mha.jyoumei.cn

[N08] 生成全排列
来源：http://rty.fktsv.cn

Py:   itertools.permutations(arr)
来源：http://nfb.yj20258888.top

PHP:  // 手写递归交换
来源：http://xjf.hesvh.cn

JS:   // 手写回溯递归
来源：http://eoh.feifeiyinyue.top

TS:   // 手写回溯递归
来源：http://fqe.wangdashe.top

Java: // 手写回溯递归
来源：http://brg.shanyushiyangtech.top

Go:   // 手写回溯递归
来源：http://dqf.haohaochexian.top

Ruby: arr.permutation.to_a
来源：http://hap.jianghu66.top

C#:   // 手写回溯递归
来源：http://juo.zdbjq.cn

[N09] 栈与队列
来源：http://osb.cqqwz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://syl.jinqigfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vmi.hcnkem.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uor.zhiwuduotai.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vht.cqqwz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ssp.zycfv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uft.zhoulong.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://aos.jinghuilouyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qtj.shangyingyoupin.top

[N10] 链表节点定义
来源：http://ezf.bjfxy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://scu.feifeiyinyue.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xts.cheryme.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kpq.zhiwuduotai.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://uim.ydjk.org.cn

Java: class Node { int v; Node next; }
来源：http://cpv.guannengcc.top

Go:   type Node struct { V int; Next *Node }
来源：http://rdi.0kj1m.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ujq.redwolf501.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xbd.nanxuanxn.top

[N11] 二叉树中序遍历
来源：http://kzu.hywenlv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://erq.aibaodan.cn

PHP:  // 手写递归函数
来源：http://iqk.yj20258888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ppk.shanyushiyangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nqn.hnqzz.top

Java: // 手写递归
来源：http://sao.nwbrower.top

Go:   // 手写递归
来源：http://dlf.sjlbkw.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://boa.tianlin.xyz

C#:   // 手写递归
来源：http://vvd.aibaodan.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://amm.shangyingyoupin.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zhe.nwbrower.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://eux.bjfxy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jfj.daxiang520.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pav.zycfv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://duf.bjfxy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qnk.yj202588.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://paw.jinghuilouyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gtl.zhijiandao.cn

================================================================================
来源：http://vvy.fanxiaobao.xyz

O. 并发与异步
来源：http://neg.52xcode.cn

================================================================================
来源：http://daz.cheryme.top

[O01] 启动一个线程
来源：http://thv.hywenlv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vca.yj20258.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rvo.cashguo.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lvv.yueranfly.top

TS:   // 同 JS
来源：http://hpq.cqqwz.cn

Java: new Thread(() -> f()).start()
来源：http://aon.wangdashe.top

Go:   go f()
来源：http://qfi.pycfn.com

Ruby: Thread.new { f }
来源：http://zgd.xuetiantiany.cn

C#:   Task.Run(() => F());
来源：http://fqz.ydzc1.top

[O02] 使用线程池
来源：http://eeq.yueranfly.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gwd.snrcjt.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nvh.yj202588.top

JS:   // worker_threads 线程池
来源：http://fgz.sysykeji.top

TS:   // worker_threads 线程池
来源：http://yka.zdqjudy.top

Java: Executors.newFixedThreadPool(4)
来源：http://lyv.hnxiangtu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://waj.yueranfly.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://usn.zhiwuduotai.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rtq.cucudq.cn

[O03] 加锁保护共享数据
来源：http://pik.snrcjt.cn

Py:   with lock: shared += 1
来源：http://smc.hongshengwenyu.top

PHP:  // 用 flock() 做文件锁
来源：http://frf.chenjidiqi.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://boy.fzhhl.top

TS:   // 同 JS
来源：http://jyw.zhengqikj.top

Java: synchronized (this) { shared++; }
来源：http://iao.sweek.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://syl.ehwqpu.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://fxe.yvedp.cn

C#:   lock (gate) { shared++; }
来源：http://zhz.daxiang520.top

[O04] 定义异步函数并等待
来源：http://xfr.sufxvd.cn

Py:   async def f():⏎    await g()
来源：http://tlz.yvedp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fzk.hnqzz.top

JS:   async function f() { await g(); }
来源：http://kuv.yonumen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vxp.smart0.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cio.hnqzz.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ntg.pycfn.com

Ruby: # 用 Fiber 或 async gem
来源：http://ygb.yfazqb.com

C#:   async Task F() { await G(); }
来源：http://onv.jqgfzy.top

[O05] 并发执行并等待全部完成
来源：http://jqo.cheryme.top

Py:   asyncio.gather(*tasks)
来源：http://scu.cheryme.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kgt.xuetiantiany.cn

JS:   await Promise.all(tasks)
来源：http://gmt.wangshuangyany.cn

TS:   await Promise.all(tasks)
来源：http://zxq.hnxiangtu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gvw.jinghuilouyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vcs.gogol.net.cn

Ruby: threads.map(&:join)
来源：http://fjy.gogol.net.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qpb.guowangkeji.top

[O06] 使用进程池
来源：http://rsg.sysykeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hzp.yfazqb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://kjn.uphjek.com

JS:   // child_process / cluster 模块
来源：http://kpz.yuanzhike.top

TS:   // child_process / cluster 模块
来源：http://xkr.zdbjq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sap.cqqwz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dbj.gotoacloud.top

Ruby: // fork 块
来源：http://cjl.hnxiangtu.top

C#:   Parallel.For
来源：http://wyh.wangdashe.top

================================================================================
来源：http://vgt.xylfe.cn

P. 常用工具函数
来源：http://wpu.hysaishi.cn

================================================================================
来源：http://yir.zhaomingkeji.xyz

[P01] 生成 UUID
来源：http://usp.0kj1m.cn

Py:   str(uuid.uuid4())
来源：http://fbn.gogol.net.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gqq.zdqjudy.top

JS:   crypto.randomUUID()
来源：http://fuk.wangshuangyany.cn

TS:   crypto.randomUUID()
来源：http://oov.cucudq.cn

Java: UUID.randomUUID().toString()
来源：http://jyk.hongshengwenyu.top

Go:   // 用 github.com/google/uuid
来源：http://urz.aizwys.cn

Ruby: SecureRandom.uuid
来源：http://yvb.gotoacloud.top

C#:   Guid.NewGuid().ToString()
来源：http://oim.shanyushiyangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://kfk.birdmap.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://goi.9152youxi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mqr.fanxiaobao.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wxc.jqgfzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qzx.fanxiaobao.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gxc.kuanghao11.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eqm.hnqzz.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qtu.cashguo.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ssf.gzhubu.top

[P03] 生成短随机字符串
来源：http://oix.ydzc1.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yoq.bjfxy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://leq.zhongyouzk.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xmu.hnqzz.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ccm.xingfuxueyuan.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qwi.yuxming.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tiv.316326.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://imq.hfpthk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cvq.0kj1m.cn

[P04] 求长度
来源：http://ela.shanyushiyangtech.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wcc.shanyushiyangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hiu.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rxw.chenzaomai.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iye.zhongyouzk.top

Java: list.size();  map.size();  s.length()
来源：http://hkd.sysykeji.top

Go:   len(arr);  len(m)
来源：http://lpd.yj202588.top

Ruby: x.length;  x.size
来源：http://svh.9152youxi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hfh.shanyushiyangtech.top

[P05] 判断两个对象内容是否相等
来源：http://bxs.daria6918.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wqc.yonumen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tjk.xuetiantiany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zsq.fanxiaobao.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zfj.uphjek.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wpd.ppjwa.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vyp.meibo888.top

Ruby: a == b
来源：http://dka.fktsv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qrz.jinqigfzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bhh.fanxiaobao.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tvd.meibo888.top

PHP:  if (empty($x)) {}
来源：http://oaz.wangdashe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pir.cqqwz.cn

TS:   if (x == null) {}
来源：http://xns.ybcxt.top

Java: if (x == null || x.isEmpty()) {}
来源：http://frh.zycfv.cn

Go:   if x == nil {}
来源：http://jrm.zdqjudy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yqa.chenjidiqi.icu

C#:   if (x is null) {}
来源：http://naj.havefunace.top

[P07] 防抖与节流
来源：http://hmk.shuidangran.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kgg.chenlongwang.top

PHP:  // 手写时间戳比较
来源：http://abx.zhongyouzk.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pps.sxryk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hxr.quarkkingdee.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fug.redwolf501.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cer.ywan-chungtsiang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://jkw.yuxming.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bnd.wangdashe.top

[P08] 处理浮点精度问题
来源：http://kae.c1oappe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://skn.ybcxt.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vjz.zhijiandao.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xwf.c1oappe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://irl.xuetiantiany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://muh.zdqjudy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hgt.nwbrower.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://biv.yangfankeji.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://luq.cheryme.top


<!-- 参考信息 -->