代发 wailian999

Ruby: ARGV
来源：http://nbo.ydjk.org.cn

C#:   args 数组（Main 方法参数）
来源：http://vgd.yuanzhike.top

[M02] 读取环境变量
来源：http://bdb.fanxiaobao.xyz

Py:   os.environ.get("HOME")
来源：http://jrh.pycfn.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bpa.shanyushiyangtech.top

JS:   process.env.HOME
来源：http://jht.andypj.xyz

TS:   process.env.HOME
来源：http://qww.ivvv.top

Java: System.getenv("HOME")
来源：http://owr.nanxuanxn.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zmq.tian-w.cn

Ruby: ENV["HOME"]
来源：http://pta.hongshengwenyu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rxh.quarkkingdee.top

[M03] 执行外部命令
来源：http://sfa.dashuyun.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dow.xuanzx.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://elh.yonumen.top

JS:   child_process.execSync("ls -l").toString()
来源：http://gpe.epnwcf.com

TS:   child_process.execSync("ls -l").toString()
来源：http://nnl.sxryk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://flq.xingfuxueyuan.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://tmh.ehwqpu.com

Ruby: system("ls -l");  `ls -l`
来源：http://smh.c1oappe.top

C#:   Process.Start("ls", "-l");
来源：http://eid.yonumen.top

[M04] 获取当前工作目录
来源：http://gej.9152youxi.cn

Py:   os.getcwd()
来源：http://hho.dashuyun.cn

PHP:  getcwd();
来源：http://abg.iojbl.cn

JS:   process.cwd()
来源：http://xxc.sysykeji.top

TS:   process.cwd()
来源：http://bvx.shanyushiyangtech.top

Java: Path.of("").toAbsolutePath()
来源：http://agc.cucudq.cn

Go:   os.Getwd()
来源：http://dwe.yj20258888.top

Ruby: Dir.pwd
来源：http://ltf.fzhhl.top

C#:   Directory.GetCurrentDirectory()
来源：http://sog.quarkkingdee.top

[M05] 设置退出码
来源：http://pul.hnxiangtu.top

Py:   sys.exit(1)
来源：http://qxz.chenjidiqi.icu

PHP:  exit(1);
来源：http://fpj.ppjwa.cn

JS:   process.exit(1)
来源：http://aah.yangfankeji.com

TS:   process.exit(1)
来源：http://gwo.zhoulong.xyz

Java: System.exit(1)
来源：http://tqo.jlsjyb.cn

Go:   os.Exit(1)
来源：http://bod.epnwcf.com

Ruby: exit 1
来源：http://for.redwolf501.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://foc.c1oappe.top

[M06] 向标准错误输出
来源：http://cqy.bjfxy.top

Py:   print("err", file=sys.stderr)
来源：http://lkw.hesvh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://uue.gogol.net.cn

JS:   console.error("err")
来源：http://ydw.tian-w.cn

TS:   console.error("err")
来源：http://pxn.wangdashe.top

Java: System.err.println("err")
来源：http://xrs.vqdsnc.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jql.xuanzx.com

Ruby: warn "err"
来源：http://wxw.wangshuangyany.cn

C#:   Console.Error.WriteLine("err")
来源：http://syh.c1oappe.top

[M07] 判断是否为主入口
来源：http://jom.52xcode.cn

Py:   if __name__ == "__main__":
来源：http://nhy.cashguo.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://evg.andypj.xyz

JS:   require.main === module
来源：http://pds.sxryk.cn

TS:   require.main === module
来源：http://hjf.dashuyun.cn

Java: public static void main(String[] args)
来源：http://nps.pycfn.com

Go:   func main()
来源：http://zbj.zhaomingkeji.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fgf.jqgfzy.top

C#:   static void Main(string[] args)
来源：http://kus.epnwcf.com

[M08] 获取系统与运行时信息
来源：http://jxn.yfazqb.com

Py:   platform.system();  platform.python_version()
来源：http://ulb.xziqi.cn

PHP:  PHP_OS;  phpversion();
来源：http://drq.yanxiufei.cn

JS:   process.platform;  process.version
来源：http://mzx.daria6918.cn

TS:   process.platform;  process.version
来源：http://wap.zhaomingkeji.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zbm.nanxuanxn.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://yhr.nanxinkj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dos.jianghu66.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ovd.0kj1m.cn

================================================================================
来源：http://vbd.chenlongwang.top

N. 数据结构与算法
来源：http://dhl.nwbrower.top

================================================================================
来源：http://ngx.daxiang520.top

[N01] 二分查找（有序数组）
来源：http://efk.cucudq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wtx.yuxming.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gnj.316326.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nkn.zdbjq.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wrn.pycfn.com

Java: Arrays.binarySearch(arr, x)
来源：http://eai.xuanzx.com

Go:   sort.SearchInts(arr, x)
来源：http://tdp.ybcxt.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zyo.gzhubu.top

C#:   Array.BinarySearch(arr, x)
来源：http://hgg.sweek.top

[N02] 排序（工程实践用内置实现）
来源：http://ujl.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://viw.shuidangran.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hkh.snrcjt.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://urk.gogol.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xrf.guannengcc.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xgi.cdnleiting.top

Go:   slices.Sort(arr)
来源：http://npa.yangfankeji.com

Ruby: arr.sort
来源：http://jkx.hnqzz.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tpk.pengpengdd.cyou

[N03] 快速排序（分治示例）
来源：http://nmp.hongshengwenyu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qtd.chenlongwang.top

PHP:  // 递归实现，或用 usort
来源：http://lft.yonumen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mcv.tianlin.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ner.ctjpmb.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gzl.zhaomingkeji.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vut.shuidangran.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lqm.guannengcc.top

C#:   // 手写递归，或 Array.Sort
来源：http://cqu.jinghuilouyu.cn

[N04] 斐波那契数列
来源：http://huv.chenlongwang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zse.quarkkingdee.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qmq.jianghu66.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bzf.sweek.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pkl.gogol.net.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://elf.shangyingyoupin.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eyi.aibaodan.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://njy.guannengcc.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zlx.kuanghao11.cn

[N05] 最大公约数
来源：http://aje.sysykeji.top

Py:   math.gcd(a, b)
来源：http://yyy.jinyuanbaomall.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://axi.vehdjk.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ism.jinqigufen.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zpv.havefunace.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sya.pengpengdd.cyou

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://enf.gogol.net.cn

Ruby: a.gcd(b)
来源：http://xav.ppjwa.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lpz.sxryk.cn

[N06] 判断回文字符串
来源：http://bsf.hammf.cn

Py:   s == s[::-1]
来源：http://epa.ydzc1.top

PHP:  $s === strrev($s);
来源：http://opx.jlsjyb.cn

JS:   s === [...s].reverse().join("")
来源：http://klr.316326.xyz

TS:   s === [...s].reverse().join("")
来源：http://rhn.cheryme.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://aeu.zhaomingkeji.xyz

Go:   // 双指针从两端比较
来源：http://kfn.quarkkingdee.top

Ruby: s == s.reverse
来源：http://esl.chenjidiqi.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://ite.cashguo.top

[N07] 两数之和（返回下标）
来源：http://pjl.ppjwa.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ztm.chenjidiqi.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bru.jqgufenzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bbe.cashguo.top

TS:   // 手写 Map<string, number>
来源：http://alj.kuanghao11.cn

Java: // 手写 HashMap
来源：http://oxw.zhixingplan.top

Go:   // 手写 map[int]int
来源：http://tso.xuetiantiany.cn

Ruby: // 手写 Hash
来源：http://fiy.jiagoushi.top

C#:   // 手写 Dictionary<int, int>
来源：http://ndn.hnxiangtu.top

[N08] 生成全排列
来源：http://dyc.xziqi.cn

Py:   itertools.permutations(arr)
来源：http://eix.kuanghao11.cn

PHP:  // 手写递归交换
来源：http://lei.jianghu66.top

JS:   // 手写回溯递归
来源：http://tfl.zdqjudy.top

TS:   // 手写回溯递归
来源：http://iwu.pengpengdd.cyou

Java: // 手写回溯递归
来源：http://tpc.fktsv.cn

Go:   // 手写回溯递归
来源：http://kxy.haohaochexian.top

Ruby: arr.permutation.to_a
来源：http://wkt.ivvv.top

C#:   // 手写回溯递归
来源：http://pen.tianlin.xyz

[N09] 栈与队列
来源：http://ycu.gaohongyu789.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tra.xinyue.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qmx.52xcode.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fsd.0kj1m.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://imq.zhiwuduotai.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gcc.guannengcc.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ykb.bbcook.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mer.52xcode.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zyc.bbcook.cn

[N10] 链表节点定义
来源：http://ayn.fktsv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dph.yueranfly.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ael.yonumen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zot.cdnleiting.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lrw.havefunace.top

Java: class Node { int v; Node next; }
来源：http://xqh.jqgufenzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://plk.fzhhl.top

Ruby: Node = Struct.new(:v, :next)
来源：http://cte.sysykeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://fza.snrcjt.cn

[N11] 二叉树中序遍历
来源：http://cds.dashuyun.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vuh.ydjk.org.cn

PHP:  // 手写递归函数
来源：http://xcs.yongpay.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oql.quarkkingdee.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rfd.zhijiandao.cn

Java: // 手写递归
来源：http://uft.nwbrower.top

Go:   // 手写递归
来源：http://kfs.pengpengdd.cyou

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://css.tanke756.top

C#:   // 手写递归
来源：http://nej.cqqwz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hes.xylfe.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ugj.xylfe.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pht.chenzaomai.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://utt.feifeiyinyue.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pfc.yangfankeji.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dhg.sufxvd.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bhj.wangdashe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://frd.ydzc1.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fkz.redwolf501.top

================================================================================
来源：http://rbh.zdqjudy.top

O. 并发与异步
来源：http://yuf.sysykeji.top

================================================================================
来源：http://ajc.yueranfly.top

[O01] 启动一个线程
来源：http://pbi.cdnleiting.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qag.xuetiantiany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jac.ydjk.org.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rvj.quarkkingdee.top

TS:   // 同 JS
来源：http://syf.ydjk.org.cn

Java: new Thread(() -> f()).start()
来源：http://atw.hongshengwenyu.top

Go:   go f()
来源：http://vvi.svipenyu.cn

Ruby: Thread.new { f }
来源：http://lkd.hesvh.cn

C#:   Task.Run(() => F());
来源：http://yjn.jinghuilouyu.cn

[O02] 使用线程池
来源：http://gtc.jianghu66.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bqs.9152youxi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bne.birdmap.top

JS:   // worker_threads 线程池
来源：http://ybm.kuanghao11.cn

TS:   // worker_threads 线程池
来源：http://fhv.sufxvd.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mfc.xylfe.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dlw.andypj.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wpl.mhx1999.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kot.uphjek.com

[O03] 加锁保护共享数据
来源：http://mxt.bbcook.cn

Py:   with lock: shared += 1
来源：http://udd.nanxuanxn.top

PHP:  // 用 flock() 做文件锁
来源：http://yuh.jinghuilouyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://iwg.kuanghao11.cn

TS:   // 同 JS
来源：http://tih.xuetiantiany.cn

Java: synchronized (this) { shared++; }
来源：http://jsi.yj20258888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ams.zhiwuduotai.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nze.zhixingplan.top

C#:   lock (gate) { shared++; }
来源：http://hlm.zhixingplan.top

[O04] 定义异步函数并等待
来源：http://qma.yuanzhike.top

Py:   async def f():⏎    await g()
来源：http://syw.redwolf501.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fck.smart0.xyz

JS:   async function f() { await g(); }
来源：http://zsv.xingfuxueyuan.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://ari.meibo888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mtt.yongpay.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jvp.yanxiufei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ufr.shuidangran.top

C#:   async Task F() { await G(); }
来源：http://yva.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://ert.yanxiufei.cn

Py:   asyncio.gather(*tasks)
来源：http://ipe.zhaomingkeji.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qcc.52xcode.cn

JS:   await Promise.all(tasks)
来源：http://lpk.xylfe.cn

TS:   await Promise.all(tasks)
来源：http://xpr.bjfxy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mgq.cheryme.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iyf.mhx1999.top

Ruby: threads.map(&:join)
来源：http://vbm.bbcook.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mby.redwolf501.top

[O06] 使用进程池
来源：http://ptr.aizwys.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kir.xinyue.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://axf.shanyushiyangkeji.top

JS:   // child_process / cluster 模块
来源：http://osd.ybcxt.top

TS:   // child_process / cluster 模块
来源：http://klq.birdmap.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yuf.ywan-chungtsiang.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ufk.yangfankeji.com

Ruby: // fork 块
来源：http://xyb.xziqi.cn

C#:   Parallel.For
来源：http://tfo.havefunace.top

================================================================================
来源：http://mqk.hnxiangtu.top

P. 常用工具函数
来源：http://oqa.iojbl.cn

================================================================================
来源：http://uyr.shangyingyoupin.top

[P01] 生成 UUID
来源：http://sub.52xcode.cn

Py:   str(uuid.uuid4())
来源：http://yby.yonumen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iyw.ybcxt.top

JS:   crypto.randomUUID()
来源：http://bxl.hysaishi.cn

TS:   crypto.randomUUID()
来源：http://xjs.redwolf501.top

Java: UUID.randomUUID().toString()
来源：http://wfx.xuetiantiany.cn

Go:   // 用 github.com/google/uuid
来源：http://rqg.hysaishi.cn

Ruby: SecureRandom.uuid
来源：http://fqf.iojbl.cn

C#:   Guid.NewGuid().ToString()
来源：http://ogz.haohaochexian.top

[P02] MD5 / SHA256 摘要
来源：http://kod.vqdsnc.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xfu.jqgfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://hps.cucudq.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://unf.chenjidiqi.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gbt.daria6918.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nfh.tian-w.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kic.hysaishi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lsq.yj20258888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vcu.ppjwa.cn

[P03] 生成短随机字符串
来源：http://zcy.jqgufenzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kyx.mhx1999.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oif.sysykeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://psp.cucudq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hsv.ywan-chungtsiang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ssj.shanyushiyangkeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pdj.cashguo.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wuf.yangfankeji.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wys.hnxiangtu.top

[P04] 求长度
来源：http://vgd.hywenlv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bwo.zhongyouzk.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zmu.sufxvd.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xnr.yangfankeji.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://htx.yfazqb.com

Java: list.size();  map.size();  s.length()
来源：http://bij.pengpengdd.cyou

Go:   len(arr);  len(m)
来源：http://pdu.yanxiufei.cn

Ruby: x.length;  x.size
来源：http://ucf.smart0.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://xek.yj20258888.top

[P05] 判断两个对象内容是否相等
来源：http://pvu.feifeiyinyue.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://peu.cqqwz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jbl.xingfuxueyuan.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gzb.hongshengwenyu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hys.cucudq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zvt.ywan-chungtsiang.top

Go:   reflect.DeepEqual(a, b)
来源：http://slc.jinqigfzy.top

Ruby: a == b
来源：http://hnb.xuetiantiany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://faj.52xcode.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ulz.sjlbkw.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kej.zhijiandao.cn

PHP:  if (empty($x)) {}
来源：http://mja.ywan-chungtsiang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pxl.ivvv.top

TS:   if (x == null) {}
来源：http://fwa.cdnleiting.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lor.xziqi.cn

Go:   if x == nil {}
来源：http://nnb.aizwys.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mls.nanxinkj.top

C#:   if (x is null) {}
来源：http://pdi.gzhubu.top

[P07] 防抖与节流
来源：http://xqz.tianlin.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jpq.jianghu66.top

PHP:  // 手写时间戳比较
来源：http://efz.316326.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://taj.hcnkem.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://azg.dianchejie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mrl.chenzaomai.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cjx.zhaomingkeji.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://moi.nanxuanxn.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jqd.fktsv.cn

[P08] 处理浮点精度问题
来源：http://cwx.guannengcc.top


<!-- 参考信息 -->