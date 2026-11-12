代发 wailian999

Ruby: ARGV
来源：http://pdq.c1oappe.top

C#:   args 数组（Main 方法参数）
来源：http://sog.c1oappe.top

[M02] 读取环境变量
来源：http://fww.shanyushiyangkeji.top

Py:   os.environ.get("HOME")
来源：http://ond.haohaochexian.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://btu.gzhubu.top

JS:   process.env.HOME
来源：http://wme.bbcook.cn

TS:   process.env.HOME
来源：http://pts.ydzc1.top

Java: System.getenv("HOME")
来源：http://eme.vehdjk.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jxt.guannengcc.top

Ruby: ENV["HOME"]
来源：http://cab.52xcode.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vwy.yj20258888.top

[M03] 执行外部命令
来源：http://vea.tanke756.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xhz.yanxiufei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fju.nanxinkj.top

JS:   child_process.execSync("ls -l").toString()
来源：http://cvt.shangyingyoupin.top

TS:   child_process.execSync("ls -l").toString()
来源：http://xyf.zycfv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kny.c1oappe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://aby.daxiang520.top

Ruby: system("ls -l");  `ls -l`
来源：http://fld.xuanzx.com

C#:   Process.Start("ls", "-l");
来源：http://yzv.meibo888.top

[M04] 获取当前工作目录
来源：http://hhf.jianghu66.top

Py:   os.getcwd()
来源：http://clj.vehdjk.com

PHP:  getcwd();
来源：http://hnh.jinqigufen.top

JS:   process.cwd()
来源：http://kyg.redwolf501.top

TS:   process.cwd()
来源：http://jwq.xziqi.cn

Java: Path.of("").toAbsolutePath()
来源：http://fkd.yfazqb.com

Go:   os.Getwd()
来源：http://bey.316326.xyz

Ruby: Dir.pwd
来源：http://iuf.hammf.cn

C#:   Directory.GetCurrentDirectory()
来源：http://obs.jinqigufen.top

[M05] 设置退出码
来源：http://nrd.smart0.xyz

Py:   sys.exit(1)
来源：http://gjf.xuetiantiany.cn

PHP:  exit(1);
来源：http://met.zycfv.cn

JS:   process.exit(1)
来源：http://fyw.xylfe.cn

TS:   process.exit(1)
来源：http://jbj.hfpthk.cn

Java: System.exit(1)
来源：http://kjn.yongpay.top

Go:   os.Exit(1)
来源：http://pgl.vehdjk.com

Ruby: exit 1
来源：http://ywm.0kj1m.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rmc.jinghuilouyu.cn

[M06] 向标准错误输出
来源：http://wbl.kuanghao11.cn

Py:   print("err", file=sys.stderr)
来源：http://vay.yueranfly.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lav.cashguo.top

JS:   console.error("err")
来源：http://ptt.ctjpmb.com

TS:   console.error("err")
来源：http://dwm.cashguo.top

Java: System.err.println("err")
来源：http://axb.jlsjyb.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bfo.jlsjyb.cn

Ruby: warn "err"
来源：http://uaj.bbcook.cn

C#:   Console.Error.WriteLine("err")
来源：http://axx.hywenlv.cn

[M07] 判断是否为主入口
来源：http://efl.jinghuilouyu.cn

Py:   if __name__ == "__main__":
来源：http://mhm.ydzc1.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ndy.guowangkeji.top

JS:   require.main === module
来源：http://emr.zhoulong.xyz

TS:   require.main === module
来源：http://efr.daxiang520.top

Java: public static void main(String[] args)
来源：http://siv.andypj.xyz

Go:   func main()
来源：http://fvb.yongpay.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rqk.xuanzx.com

C#:   static void Main(string[] args)
来源：http://gya.yfazqb.com

[M08] 获取系统与运行时信息
来源：http://hjo.pengpengdd.cyou

Py:   platform.system();  platform.python_version()
来源：http://fas.hesvh.cn

PHP:  PHP_OS;  phpversion();
来源：http://zpr.jqgufenzy.top

JS:   process.platform;  process.version
来源：http://hli.kuanghao11.cn

TS:   process.platform;  process.version
来源：http://nxc.52xcode.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dkw.ivvv.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://omz.sxryk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fec.tian-w.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rgb.xuetiantiany.cn

================================================================================
来源：http://ejo.fengsongda.top

N. 数据结构与算法
来源：http://krm.nanxinkj.top

================================================================================
来源：http://cbp.shuidangran.top

[N01] 二分查找（有序数组）
来源：http://vlt.yuanzhike.top

Py:   bisect.bisect_left(arr, x)
来源：http://wqn.zhijiandao.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zkt.yueranfly.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bss.shuidangran.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wbz.ydjk.org.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ztz.aizwys.cn

Go:   sort.SearchInts(arr, x)
来源：http://piv.ppjwa.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://eok.zycfv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wan.jqgfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://wxp.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://ytb.yangfankeji.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jqy.jlsjyb.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://twc.yangfankeji.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://xts.ywan-chungtsiang.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hzd.shanyushiyangtech.top

Go:   slices.Sort(arr)
来源：http://oxv.ydzc1.top

Ruby: arr.sort
来源：http://ozj.yj202588.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tsb.mhx1999.top

[N03] 快速排序（分治示例）
来源：http://aib.52xcode.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zej.yuanzhike.top

PHP:  // 递归实现，或用 usort
来源：http://hsz.hongshengwenyu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lty.xylfe.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://txp.tianlin.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dhn.dashuyun.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wts.vehdjk.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ocm.shuidangran.top

C#:   // 手写递归，或 Array.Sort
来源：http://zza.hongshengwenyu.top

[N04] 斐波那契数列
来源：http://qyc.kuanghao11.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bwc.zhoulong.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ogz.tianlin.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ldz.ehwqpu.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vch.pycfn.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yeg.quarkkingdee.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aeb.redwolf501.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xib.yongpay.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uwn.vehdjk.com

[N05] 最大公约数
来源：http://nbn.316326.xyz

Py:   math.gcd(a, b)
来源：http://npr.jinqigfzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pri.hysaishi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jjq.haohaochexian.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rsh.zhaomingkeji.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nrz.fanxiaobao.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xxk.dashuyun.cn

Ruby: a.gcd(b)
来源：http://ieg.pycfn.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qzb.xziqi.cn

[N06] 判断回文字符串
来源：http://lxj.hammf.cn

Py:   s == s[::-1]
来源：http://cwi.zhaomingkeji.xyz

PHP:  $s === strrev($s);
来源：http://pmy.gogol.net.cn

JS:   s === [...s].reverse().join("")
来源：http://rfs.svipenyu.cn

TS:   s === [...s].reverse().join("")
来源：http://nik.vqdsnc.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nct.zhixingplan.top

Go:   // 双指针从两端比较
来源：http://ruy.uphjek.com

Ruby: s == s.reverse
来源：http://nzm.ppjwa.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ylv.fanxiaobao.xyz

[N07] 两数之和（返回下标）
来源：http://zdc.jinqigufen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://aen.c1oappe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oxe.yueranfly.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vww.sysykeji.top

TS:   // 手写 Map<string, number>
来源：http://zku.0kj1m.cn

Java: // 手写 HashMap
来源：http://fso.smart0.xyz

Go:   // 手写 map[int]int
来源：http://paf.tarul.cn

Ruby: // 手写 Hash
来源：http://jmb.feifeiyinyue.top

C#:   // 手写 Dictionary<int, int>
来源：http://jet.pengpengdd.cyou

[N08] 生成全排列
来源：http://xeq.hnqzz.top

Py:   itertools.permutations(arr)
来源：http://qkr.nanxinkj.top

PHP:  // 手写递归交换
来源：http://zhz.ydjk.org.cn

JS:   // 手写回溯递归
来源：http://fgp.sjlbkw.cn

TS:   // 手写回溯递归
来源：http://lhq.fengsongda.top

Java: // 手写回溯递归
来源：http://jcg.cdnleiting.top

Go:   // 手写回溯递归
来源：http://crt.xziqi.cn

Ruby: arr.permutation.to_a
来源：http://zgj.xziqi.cn

C#:   // 手写回溯递归
来源：http://nof.meibo888.top

[N09] 栈与队列
来源：http://qxu.mhx1999.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fye.kuanghao11.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fdi.gzhubu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://frg.cdnleiting.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oog.jyoumei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ien.wangdashe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yxk.iojbl.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hfb.jinghuilouyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rmb.9152youxi.cn

[N10] 链表节点定义
来源：http://mtz.havefunace.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yyv.svipenyu.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dgi.cqqwz.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ttn.xingfuxueyuan.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://drp.birdmap.top

Java: class Node { int v; Node next; }
来源：http://yqe.zhongyouzk.top

Go:   type Node struct { V int; Next *Node }
来源：http://zfv.xinyue.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://uqc.tianlin.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://rbv.xingfuxueyuan.xyz

[N11] 二叉树中序遍历
来源：http://ksr.aizwys.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jmf.yuanzhike.top

PHP:  // 手写递归函数
来源：http://bgf.vehdjk.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jbv.fzhhl.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wsg.wangshuangyany.cn

Java: // 手写递归
来源：http://mle.hcnkem.com

Go:   // 手写递归
来源：http://cmj.tanke756.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://crw.zhijiandao.cn

C#:   // 手写递归
来源：http://uqn.yangfankeji.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ynt.guowangkeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://aft.xylfe.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lqx.tianlin.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cza.zhoulong.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gda.ivvv.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fwu.ctjpmb.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pdt.daria6918.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ebx.gotoacloud.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kxw.nwbrower.top

================================================================================
来源：http://oox.yvedp.cn

O. 并发与异步
来源：http://sds.svipenyu.cn

================================================================================
来源：http://smb.316326.xyz

[O01] 启动一个线程
来源：http://qya.jqgfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://odi.sufxvd.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://muv.kuanghao11.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pqw.hammf.cn

TS:   // 同 JS
来源：http://fjx.hywenlv.cn

Java: new Thread(() -> f()).start()
来源：http://eew.yj202588.top

Go:   go f()
来源：http://qim.nanxuanxn.top

Ruby: Thread.new { f }
来源：http://txx.ppjwa.cn

C#:   Task.Run(() => F());
来源：http://sov.redwolf501.top

[O02] 使用线程池
来源：http://cgm.316326.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mxx.jqgfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dtj.zhaomingkeji.xyz

JS:   // worker_threads 线程池
来源：http://tcz.chenlongwang.top

TS:   // worker_threads 线程池
来源：http://qxh.kuanghao11.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wvo.snrcjt.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xlr.zhaomingkeji.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://als.aizwys.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wmn.feifeiyinyue.top

[O03] 加锁保护共享数据
来源：http://vvr.jinqigfzy.top

Py:   with lock: shared += 1
来源：http://vpn.ywan-chungtsiang.top

PHP:  // 用 flock() 做文件锁
来源：http://xrt.svipenyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://swi.nwbrower.top

TS:   // 同 JS
来源：http://oht.yongpay.top

Java: synchronized (this) { shared++; }
来源：http://vlt.yfazqb.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kqi.shangyingyoupin.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ppk.xuanzx.com

C#:   lock (gate) { shared++; }
来源：http://pwh.fengsongda.top

[O04] 定义异步函数并等待
来源：http://fqx.zhengqikj.top

Py:   async def f():⏎    await g()
来源：http://kbp.andypj.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rwc.sweek.top

JS:   async function f() { await g(); }
来源：http://idt.chenzaomai.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://los.cashguo.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ywb.daria6918.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lqj.meibo888.top

Ruby: # 用 Fiber 或 async gem
来源：http://ewo.52xcode.cn

C#:   async Task F() { await G(); }
来源：http://ypc.gzhubu.top

[O05] 并发执行并等待全部完成
来源：http://boo.xuetiantiany.cn

Py:   asyncio.gather(*tasks)
来源：http://jfk.zhixingplan.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ilv.yj20258.top

JS:   await Promise.all(tasks)
来源：http://ohk.yfazqb.com

TS:   await Promise.all(tasks)
来源：http://aip.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qbt.zhixingplan.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jjb.sysykeji.top

Ruby: threads.map(&:join)
来源：http://lam.yueranfly.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hmw.sjlbkw.cn

[O06] 使用进程池
来源：http://ogb.0kj1m.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tjy.birdmap.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fcj.epnwcf.com

JS:   // child_process / cluster 模块
来源：http://szl.gogol.net.cn

TS:   // child_process / cluster 模块
来源：http://izq.yuanzhike.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://amu.jlsjyb.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yvc.c1oappe.top

Ruby: // fork 块
来源：http://qfo.hcnkem.com

C#:   Parallel.For
来源：http://yya.cheryme.top

================================================================================
来源：http://yva.smart0.xyz

P. 常用工具函数
来源：http://cmv.jinqigfzy.top

================================================================================
来源：http://npr.pengpengdd.cyou

[P01] 生成 UUID
来源：http://yjz.nwbrower.top

Py:   str(uuid.uuid4())
来源：http://buu.zhongyouzk.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bzp.nanxinkj.top

JS:   crypto.randomUUID()
来源：http://nsx.dashuyun.cn

TS:   crypto.randomUUID()
来源：http://uzb.chenlongwang.top

Java: UUID.randomUUID().toString()
来源：http://rub.ctjpmb.com

Go:   // 用 github.com/google/uuid
来源：http://yfl.gogol.net.cn

Ruby: SecureRandom.uuid
来源：http://ugy.shanyushiyangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://ymy.zhoulong.xyz

[P02] MD5 / SHA256 摘要
来源：http://wug.sxryk.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gwm.gzhubu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ici.hesvh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lqm.wangdashe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://khf.quarkkingdee.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bor.jqgfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bvj.yueranfly.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lbo.iojbl.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fnq.nwbrower.top

[P03] 生成短随机字符串
来源：http://wkk.fktsv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://epa.shanyushiyangkeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ikx.havefunace.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ygt.zhiwuduotai.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uki.yongpay.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://elq.daria6918.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vsf.yangfankeji.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://sha.sysykeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jfj.daxiang520.top

[P04] 求长度
来源：http://vzs.hywenlv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ahj.hammf.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zzb.yj20258888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wpv.hysaishi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://toe.jlsjyb.cn

Java: list.size();  map.size();  s.length()
来源：http://hxr.daria6918.cn

Go:   len(arr);  len(m)
来源：http://smd.cheryme.top

Ruby: x.length;  x.size
来源：http://xzv.havefunace.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ghh.wangdashe.top

[P05] 判断两个对象内容是否相等
来源：http://xwx.hnxiangtu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://gdi.andypj.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bqm.sjlbkw.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oeg.ctjpmb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dgw.daria6918.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ytn.tian-w.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fdo.iojbl.cn

Ruby: a == b
来源：http://nll.guannengcc.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ufb.fzhhl.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qxq.hongshengwenyu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gud.0kj1m.cn

PHP:  if (empty($x)) {}
来源：http://oug.fzhhl.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://krl.ehwqpu.com

TS:   if (x == null) {}
来源：http://kvi.zhengqikj.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jmf.guowangkeji.top

Go:   if x == nil {}
来源：http://ylo.0kj1m.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rgm.nanxuanxn.top

C#:   if (x is null) {}
来源：http://quc.zdqjudy.top

[P07] 防抖与节流
来源：http://hbg.xylfe.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mqi.haohaochexian.top

PHP:  // 手写时间戳比较
来源：http://dvc.vehdjk.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://quc.havefunace.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hov.ybcxt.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wgl.shuidangran.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dpo.cqqwz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://upj.fanxiaobao.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mgn.gzhubu.top

[P08] 处理浮点精度问题
来源：http://hkp.cdnleiting.top


<!-- 参考信息 -->