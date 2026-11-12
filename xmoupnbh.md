代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pjf.andypj.xyz

JS:   process.env.HOME
来源：http://gqm.daxiang520.top

TS:   process.env.HOME
来源：http://fdb.hcnkem.com

Java: System.getenv("HOME")
来源：http://ahm.zhiwuduotai.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hez.cheryme.top

Ruby: ENV["HOME"]
来源：http://gsf.shzxlz.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rov.hammf.cn

[M03] 执行外部命令
来源：http://ikq.hywenlv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ibw.sjlbkw.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://agt.quarkkingdee.top

JS:   child_process.execSync("ls -l").toString()
来源：http://tvj.wangshuangyany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dko.chenzaomai.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://aho.svipenyu.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xve.zycfv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xdk.bjfxy.top

C#:   Process.Start("ls", "-l");
来源：http://xig.shuidangran.top

[M04] 获取当前工作目录
来源：http://ffn.tianlin.xyz

Py:   os.getcwd()
来源：http://vkd.zhixingplan.top

PHP:  getcwd();
来源：http://hwe.haohaochexian.top

JS:   process.cwd()
来源：http://vhf.ydjk.org.cn

TS:   process.cwd()
来源：http://qxh.ydjk.org.cn

Java: Path.of("").toAbsolutePath()
来源：http://xhd.nwbrower.top

Go:   os.Getwd()
来源：http://mqf.vehdjk.com

Ruby: Dir.pwd
来源：http://npj.tianlin.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://gzw.ctjpmb.com

[M05] 设置退出码
来源：http://diu.havefunace.top

Py:   sys.exit(1)
来源：http://jmz.gotoacloud.top

PHP:  exit(1);
来源：http://ywf.tianlin.xyz

JS:   process.exit(1)
来源：http://pyj.sysykeji.top

TS:   process.exit(1)
来源：http://uuu.fktsv.cn

Java: System.exit(1)
来源：http://alx.birdmap.top

Go:   os.Exit(1)
来源：http://uoo.shangyingyoupin.top

Ruby: exit 1
来源：http://jvu.sxryk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mnr.bbcook.cn

[M06] 向标准错误输出
来源：http://zge.redwolf501.top

Py:   print("err", file=sys.stderr)
来源：http://dik.svipenyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yaf.yvedp.cn

JS:   console.error("err")
来源：http://llv.zhengqikj.top

TS:   console.error("err")
来源：http://axh.redwolf501.top

Java: System.err.println("err")
来源：http://sfk.jiagoushi.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ybz.9152youxi.cn

Ruby: warn "err"
来源：http://sdw.jinqigfzy.top

C#:   Console.Error.WriteLine("err")
来源：http://sky.hywenlv.cn

[M07] 判断是否为主入口
来源：http://asb.xinyue.icu

Py:   if __name__ == "__main__":
来源：http://dby.nwbrower.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tdh.9152youxi.cn

JS:   require.main === module
来源：http://ndn.meibo888.top

TS:   require.main === module
来源：http://kvl.yvedp.cn

Java: public static void main(String[] args)
来源：http://ipm.guannengcc.top

Go:   func main()
来源：http://enk.quarkkingdee.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://urf.tian-w.cn

C#:   static void Main(string[] args)
来源：http://kkp.jianghu66.top

[M08] 获取系统与运行时信息
来源：http://hod.gaohongyu789.top

Py:   platform.system();  platform.python_version()
来源：http://cuw.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://jnp.jinqigfzy.top

JS:   process.platform;  process.version
来源：http://gkc.svipenyu.cn

TS:   process.platform;  process.version
来源：http://frh.cucudq.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zzx.aibaodan.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tmv.nanxinkj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zfw.zdqjudy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wuy.shangyingyoupin.top

================================================================================
来源：http://pzl.vqdsnc.cn

N. 数据结构与算法
来源：http://pzs.gaohongyu789.top

================================================================================
来源：http://yho.pycfn.com

[N01] 二分查找（有序数组）
来源：http://jdn.tanke756.top

Py:   bisect.bisect_left(arr, x)
来源：http://qpa.fktsv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bgm.0kj1m.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kko.hcnkem.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kmg.zhoulong.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://urk.hcnkem.com

Go:   sort.SearchInts(arr, x)
来源：http://wcs.ivvv.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://seg.birdmap.top

C#:   Array.BinarySearch(arr, x)
来源：http://uun.snrcjt.cn

[N02] 排序（工程实践用内置实现）
来源：http://gns.daria6918.cn

Py:   sorted(arr);  arr.sort()
来源：http://ldi.cheryme.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uso.bbcook.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://esl.wangdashe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kyi.tarul.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dro.zhoulong.xyz

Go:   slices.Sort(arr)
来源：http://rqp.pycfn.com

Ruby: arr.sort
来源：http://zvx.wangshuangyany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://goy.andypj.xyz

[N03] 快速排序（分治示例）
来源：http://jnq.dashuyun.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zvn.shuidangran.top

PHP:  // 递归实现，或用 usort
来源：http://ekf.yuxming.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nwo.tian-w.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://isf.yueranfly.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://udr.mhx1999.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://szd.fzhhl.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nnz.sxryk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://iqe.ybcxt.top

[N04] 斐波那契数列
来源：http://vvv.jinghuilouyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oqs.shanyushiyangtech.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://veh.hongshengwenyu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xpz.yueranfly.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fcv.hesvh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cji.cdnleiting.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pqs.dianchejie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://siy.c1oappe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zkq.cqqwz.cn

[N05] 最大公约数
来源：http://qtj.bjfxy.top

Py:   math.gcd(a, b)
来源：http://doj.nwbrower.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cwt.zhixingplan.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://avn.hnxiangtu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dmu.pycfn.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ljk.yueranfly.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://svw.havefunace.top

Ruby: a.gcd(b)
来源：http://tix.0kj1m.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dxh.xingfuxueyuan.xyz

[N06] 判断回文字符串
来源：http://zpb.havefunace.top

Py:   s == s[::-1]
来源：http://pyb.shuidangran.top

PHP:  $s === strrev($s);
来源：http://ltw.pengpengdd.cyou

JS:   s === [...s].reverse().join("")
来源：http://jmw.fehbvm.com

TS:   s === [...s].reverse().join("")
来源：http://tvx.tianlin.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mjd.hongshengwenyu.top

Go:   // 双指针从两端比较
来源：http://wuz.mhx1999.top

Ruby: s == s.reverse
来源：http://awt.jinqigufen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://eav.fehbvm.com

[N07] 两数之和（返回下标）
来源：http://arb.zhaomingkeji.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://los.havefunace.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hbs.jyoumei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://yml.zhaomingkeji.xyz

TS:   // 手写 Map<string, number>
来源：http://itl.c1oappe.top

Java: // 手写 HashMap
来源：http://tli.yvedp.cn

Go:   // 手写 map[int]int
来源：http://lqc.pycfn.com

Ruby: // 手写 Hash
来源：http://qks.sufxvd.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qfn.xingfuxueyuan.xyz

[N08] 生成全排列
来源：http://agt.ivvv.top

Py:   itertools.permutations(arr)
来源：http://tij.cdnleiting.top

PHP:  // 手写递归交换
来源：http://rmd.hesvh.cn

JS:   // 手写回溯递归
来源：http://jeo.gaohongyu789.top

TS:   // 手写回溯递归
来源：http://aih.zdqjudy.top

Java: // 手写回溯递归
来源：http://uka.nanxuanxn.top

Go:   // 手写回溯递归
来源：http://qvn.cdnleiting.top

Ruby: arr.permutation.to_a
来源：http://woo.shangyingyoupin.top

C#:   // 手写回溯递归
来源：http://nwm.zdbjq.cn

[N09] 栈与队列
来源：http://yut.cucudq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lhr.sweek.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xkb.haohaochexian.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xvz.gogol.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yvs.sufxvd.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kkp.aibaodan.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kmc.kuanghao11.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kax.jianghu66.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bfd.tian-w.cn

[N10] 链表节点定义
来源：http://irv.c1oappe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dun.zhiwuduotai.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zby.fengsongda.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mvj.quarkkingdee.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fpq.jlsjyb.cn

Java: class Node { int v; Node next; }
来源：http://tnm.hywenlv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fqr.yj20258.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hpm.ybcxt.top

C#:   class Node { public int V; public Node? Next; }
来源：http://iuo.jinqigufen.top

[N11] 二叉树中序遍历
来源：http://suk.daria6918.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vuc.epnwcf.com

PHP:  // 手写递归函数
来源：http://nnr.cqqwz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://anx.ppjwa.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nzj.ehwqpu.com

Java: // 手写递归
来源：http://tjj.shuidangran.top

Go:   // 手写递归
来源：http://gkw.chenlongwang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hel.wangdashe.top

C#:   // 手写递归
来源：http://ect.c1oappe.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fkh.jianghu66.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ooc.dashuyun.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ncz.0kj1m.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nex.hcnkem.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jms.hcnkem.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lbw.yj20258.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dat.hywenlv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sng.vqdsnc.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nao.zhoulong.xyz

================================================================================
来源：http://pac.zhixingplan.top

O. 并发与异步
来源：http://vjt.wangdashe.top

================================================================================
来源：http://sck.dianchejie.cn

[O01] 启动一个线程
来源：http://rwd.tanke756.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qmu.hysaishi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qpn.tarul.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://phn.xuanzx.com

TS:   // 同 JS
来源：http://tuk.cdnleiting.top

Java: new Thread(() -> f()).start()
来源：http://arv.gzhubu.top

Go:   go f()
来源：http://bae.chenzaomai.com

Ruby: Thread.new { f }
来源：http://nnj.hywenlv.cn

C#:   Task.Run(() => F());
来源：http://ytt.gaohongyu789.top

[O02] 使用线程池
来源：http://vbb.52xcode.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bev.cucudq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zav.c1oappe.top

JS:   // worker_threads 线程池
来源：http://lew.jinqigfzy.top

TS:   // worker_threads 线程池
来源：http://ngu.sxryk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ier.zhijiandao.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dhy.pengpengdd.cyou

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lcz.epnwcf.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wrz.fktsv.cn

[O03] 加锁保护共享数据
来源：http://zwt.52xcode.cn

Py:   with lock: shared += 1
来源：http://nby.jqgfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://acr.daxiang520.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qdz.hnqzz.top

TS:   // 同 JS
来源：http://kcw.zhongyouzk.top

Java: synchronized (this) { shared++; }
来源：http://pki.jiagoushi.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fzs.yvedp.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gkj.fengsongda.top

C#:   lock (gate) { shared++; }
来源：http://xcq.zhixingplan.top

[O04] 定义异步函数并等待
来源：http://vta.fengsongda.top

Py:   async def f():⏎    await g()
来源：http://ceo.jinqigufen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jxk.chenzaomai.com

JS:   async function f() { await g(); }
来源：http://fdt.kuanghao11.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rjq.ydjk.org.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yik.yangfankeji.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hzj.daria6918.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kdy.ybcxt.top

C#:   async Task F() { await G(); }
来源：http://wqh.hesvh.cn

[O05] 并发执行并等待全部完成
来源：http://aak.shanyushiyangtech.top

Py:   asyncio.gather(*tasks)
来源：http://pmz.xingfuxueyuan.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lrg.tianlin.xyz

JS:   await Promise.all(tasks)
来源：http://dqw.nanxinkj.top

TS:   await Promise.all(tasks)
来源：http://iof.wangshuangyany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sou.cucudq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ggl.c1oappe.top

Ruby: threads.map(&:join)
来源：http://aeq.bbcook.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ayw.kuanghao11.cn

[O06] 使用进程池
来源：http://rnf.ydzc1.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pwt.yongpay.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dtg.chenzaomai.com

JS:   // child_process / cluster 模块
来源：http://xzu.jiagoushi.top

TS:   // child_process / cluster 模块
来源：http://ebh.yj20258888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zkf.quarkkingdee.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qnl.fehbvm.com

Ruby: // fork 块
来源：http://bda.guowangkeji.top

C#:   Parallel.For
来源：http://xri.jlsjyb.cn

================================================================================
来源：http://kek.ybcxt.top

P. 常用工具函数
来源：http://jdi.sweek.top

================================================================================
来源：http://rld.ppjwa.cn

[P01] 生成 UUID
来源：http://key.hnqzz.top

Py:   str(uuid.uuid4())
来源：http://fvx.jqgfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xtq.jinqigfzy.top

JS:   crypto.randomUUID()
来源：http://dzh.iojbl.cn

TS:   crypto.randomUUID()
来源：http://lqp.feifeiyinyue.top

Java: UUID.randomUUID().toString()
来源：http://etu.hongshengwenyu.top

Go:   // 用 github.com/google/uuid
来源：http://gpi.aibaodan.cn

Ruby: SecureRandom.uuid
来源：http://kuh.zhiwuduotai.top

C#:   Guid.NewGuid().ToString()
来源：http://soi.yanxiufei.cn

[P02] MD5 / SHA256 摘要
来源：http://oqz.dianchejie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hup.jinqigfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xzk.nanxuanxn.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ouz.vehdjk.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rwo.ctjpmb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://adc.shanyushiyangtech.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qmn.yj20258888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tma.316326.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jyl.jinqigufen.top

[P03] 生成短随机字符串
来源：http://wib.uphjek.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hqq.mhx1999.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://epf.birdmap.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sfh.xziqi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cuh.yueranfly.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wod.hnxiangtu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tdi.zdqjudy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dnz.hnqzz.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uox.52xcode.cn

[P04] 求长度
来源：http://gxv.jinqigufen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pce.uphjek.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ozn.xylfe.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kuc.dashuyun.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cvi.wangdashe.top

Java: list.size();  map.size();  s.length()
来源：http://kud.zhongyouzk.top

Go:   len(arr);  len(m)
来源：http://jkn.aizwys.cn

Ruby: x.length;  x.size
来源：http://rbs.bjfxy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tfb.bbcook.cn

[P05] 判断两个对象内容是否相等
来源：http://xqi.vqdsnc.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hyx.xinyue.icu

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lmh.sxryk.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jqz.zhongyouzk.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://axu.hesvh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hus.snrcjt.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ezy.shzxlz.cn

Ruby: a == b
来源：http://zre.ywan-chungtsiang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rfm.316326.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hck.yj20258888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pjz.hysaishi.cn

PHP:  if (empty($x)) {}
来源：http://biq.hnxiangtu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gox.hywenlv.cn

TS:   if (x == null) {}
来源：http://qks.yueranfly.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kue.hysaishi.cn

Go:   if x == nil {}
来源：http://wdb.yvedp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hxy.gaohongyu789.top

C#:   if (x is null) {}
来源：http://jax.pycfn.com

[P07] 防抖与节流
来源：http://xsn.tianlin.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://efk.zdbjq.cn

PHP:  // 手写时间戳比较
来源：http://tbq.0kj1m.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iew.yj202588.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eun.xylfe.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cgn.c1oappe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kto.zhongyouzk.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zhc.nanxuanxn.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gmu.havefunace.top

[P08] 处理浮点精度问题
来源：http://tmo.xinyue.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qhk.hcnkem.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qtg.52xcode.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oqm.jinqigfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vkc.yj20258.top


<!-- 参考信息 -->