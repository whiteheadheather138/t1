代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zbl.hammf.cn

JS:   process.env.HOME
来源：http://iwf.0kj1m.cn

TS:   process.env.HOME
来源：http://jhs.smart0.xyz

Java: System.getenv("HOME")
来源：http://yds.gaohongyu789.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gtk.cucudq.cn

Ruby: ENV["HOME"]
来源：http://ieq.0kj1m.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://elo.gogol.net.cn

[M03] 执行外部命令
来源：http://juq.aibaodan.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://owh.shangyingyoupin.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gxm.bbcook.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qvm.birdmap.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wxj.zycfv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cfb.zhongyouzk.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ihn.wangdashe.top

Ruby: system("ls -l");  `ls -l`
来源：http://kav.dashuyun.cn

C#:   Process.Start("ls", "-l");
来源：http://bph.bbcook.cn

[M04] 获取当前工作目录
来源：http://jew.jinghuilouyu.cn

Py:   os.getcwd()
来源：http://iys.yuxming.cn

PHP:  getcwd();
来源：http://fxl.fanxiaobao.xyz

JS:   process.cwd()
来源：http://dhm.hfpthk.cn

TS:   process.cwd()
来源：http://omx.kuanghao11.cn

Java: Path.of("").toAbsolutePath()
来源：http://yyk.ydjk.org.cn

Go:   os.Getwd()
来源：http://hps.feifeiyinyue.top

Ruby: Dir.pwd
来源：http://qqr.nanxinkj.top

C#:   Directory.GetCurrentDirectory()
来源：http://xhh.jianghu66.top

[M05] 设置退出码
来源：http://vws.52xcode.cn

Py:   sys.exit(1)
来源：http://ivs.vqdsnc.cn

PHP:  exit(1);
来源：http://tyc.wangdashe.top

JS:   process.exit(1)
来源：http://lys.gzhubu.top

TS:   process.exit(1)
来源：http://xbv.sweek.top

Java: System.exit(1)
来源：http://uvq.zycfv.cn

Go:   os.Exit(1)
来源：http://mej.hammf.cn

Ruby: exit 1
来源：http://kge.jyoumei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wsk.xuanzx.com

[M06] 向标准错误输出
来源：http://vsk.pycfn.com

Py:   print("err", file=sys.stderr)
来源：http://vhx.bjfxy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bpv.gotoacloud.top

JS:   console.error("err")
来源：http://utu.xingfuxueyuan.xyz

TS:   console.error("err")
来源：http://mbk.sysykeji.top

Java: System.err.println("err")
来源：http://kgm.hcnkem.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vfh.nanxuanxn.top

Ruby: warn "err"
来源：http://xtc.gogol.net.cn

C#:   Console.Error.WriteLine("err")
来源：http://ymb.fengsongda.top

[M07] 判断是否为主入口
来源：http://phq.yonumen.top

Py:   if __name__ == "__main__":
来源：http://zvd.cashguo.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ucg.birdmap.top

JS:   require.main === module
来源：http://nuf.jqgufenzy.top

TS:   require.main === module
来源：http://buy.jyoumei.cn

Java: public static void main(String[] args)
来源：http://mrw.yj202588.top

Go:   func main()
来源：http://qey.cqqwz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cgq.hysaishi.cn

C#:   static void Main(string[] args)
来源：http://ala.zhaomingkeji.xyz

[M08] 获取系统与运行时信息
来源：http://dxf.shanyushiyangtech.top

Py:   platform.system();  platform.python_version()
来源：http://vyv.yfazqb.com

PHP:  PHP_OS;  phpversion();
来源：http://mht.guannengcc.top

JS:   process.platform;  process.version
来源：http://cvv.guowangkeji.top

TS:   process.platform;  process.version
来源：http://etp.ppjwa.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kzx.zdqjudy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://svg.cqqwz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dgh.bjfxy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://zbm.shanyushiyangtech.top

================================================================================
来源：http://gdk.iojbl.cn

N. 数据结构与算法
来源：http://yvl.c1oappe.top

================================================================================
来源：http://ncq.smart0.xyz

[N01] 二分查找（有序数组）
来源：http://bch.xuanzx.com

Py:   bisect.bisect_left(arr, x)
来源：http://rze.iojbl.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bge.zdbjq.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xce.vehdjk.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://atn.ctjpmb.com

Java: Arrays.binarySearch(arr, x)
来源：http://pga.jqgufenzy.top

Go:   sort.SearchInts(arr, x)
来源：http://ogt.chenlongwang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://wxt.yongpay.top

C#:   Array.BinarySearch(arr, x)
来源：http://ggu.316326.xyz

[N02] 排序（工程实践用内置实现）
来源：http://fgk.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://ion.shanyushiyangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qin.fzhhl.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://dxb.hammf.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bki.tian-w.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hlh.jinqigufen.top

Go:   slices.Sort(arr)
来源：http://meh.yonumen.top

Ruby: arr.sort
来源：http://alx.pycfn.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://ymk.tianlin.xyz

[N03] 快速排序（分治示例）
来源：http://vnj.yj20258888.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hgd.jiagoushi.top

PHP:  // 递归实现，或用 usort
来源：http://ytu.meibo888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jrj.hnxiangtu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://znt.dianchejie.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qqk.yonumen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hnc.ehwqpu.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xda.smart0.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://pna.daxiang520.top

[N04] 斐波那契数列
来源：http://chu.ydzc1.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ivr.feifeiyinyue.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://obi.yanxiufei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wgf.hysaishi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://buz.chenjidiqi.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://isv.havefunace.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dbb.feifeiyinyue.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lni.jlsjyb.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hug.jinqigufen.top

[N05] 最大公约数
来源：http://jyi.hcnkem.com

Py:   math.gcd(a, b)
来源：http://hsq.cheryme.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wfg.ydzc1.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://abw.quarkkingdee.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uev.hcnkem.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xed.cashguo.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uxm.svipenyu.cn

Ruby: a.gcd(b)
来源：http://qha.birdmap.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qhk.hysaishi.cn

[N06] 判断回文字符串
来源：http://svm.nwbrower.top

Py:   s == s[::-1]
来源：http://fns.zhaomingkeji.xyz

PHP:  $s === strrev($s);
来源：http://quc.nwbrower.top

JS:   s === [...s].reverse().join("")
来源：http://rwh.yangfankeji.com

TS:   s === [...s].reverse().join("")
来源：http://ear.shuidangran.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ckc.yueranfly.top

Go:   // 双指针从两端比较
来源：http://sit.sufxvd.cn

Ruby: s == s.reverse
来源：http://win.wangdashe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://pcc.hesvh.cn

[N07] 两数之和（返回下标）
来源：http://shw.bjfxy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uea.zhaomingkeji.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qlw.dashuyun.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://iek.ydjk.org.cn

TS:   // 手写 Map<string, number>
来源：http://vxs.jinghuilouyu.cn

Java: // 手写 HashMap
来源：http://tct.fehbvm.com

Go:   // 手写 map[int]int
来源：http://fzj.daria6918.cn

Ruby: // 手写 Hash
来源：http://bnk.fzhhl.top

C#:   // 手写 Dictionary<int, int>
来源：http://tlu.yanxiufei.cn

[N08] 生成全排列
来源：http://snc.chenjidiqi.icu

Py:   itertools.permutations(arr)
来源：http://cys.fanxiaobao.xyz

PHP:  // 手写递归交换
来源：http://gsm.bbcook.cn

JS:   // 手写回溯递归
来源：http://jsb.andypj.xyz

TS:   // 手写回溯递归
来源：http://jze.dianchejie.cn

Java: // 手写回溯递归
来源：http://hln.zdqjudy.top

Go:   // 手写回溯递归
来源：http://mfn.zhaomingkeji.xyz

Ruby: arr.permutation.to_a
来源：http://unu.fehbvm.com

C#:   // 手写回溯递归
来源：http://ufc.yvedp.cn

[N09] 栈与队列
来源：http://llp.guowangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mwe.ydzc1.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fec.dashuyun.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rkd.tian-w.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qbt.hongshengwenyu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cke.jqgfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pgh.wangshuangyany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vuj.gzhubu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zny.316326.xyz

[N10] 链表节点定义
来源：http://rih.bjfxy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lmi.yangfankeji.com

PHP:  class Node { public $v; public $next = null; }
来源：http://knp.daria6918.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qvg.ctjpmb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://aey.fehbvm.com

Java: class Node { int v; Node next; }
来源：http://jjy.dashuyun.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bmw.chenjidiqi.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://knv.aibaodan.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://roj.birdmap.top

[N11] 二叉树中序遍历
来源：http://xll.ydjk.org.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hkg.shangyingyoupin.top

PHP:  // 手写递归函数
来源：http://iea.cqqwz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ffs.sysykeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kor.cheryme.top

Java: // 手写递归
来源：http://ljz.birdmap.top

Go:   // 手写递归
来源：http://pkg.gotoacloud.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qrk.xylfe.cn

C#:   // 手写递归
来源：http://nov.nanxinkj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hrh.jqgfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xeu.yanxiufei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gly.xuetiantiany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://efu.wangshuangyany.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sqa.uphjek.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lsn.ydjk.org.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zqm.fzhhl.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://amb.52xcode.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jpx.hesvh.cn

================================================================================
来源：http://ttf.316326.xyz

O. 并发与异步
来源：http://jfy.xuanzx.com

================================================================================
来源：http://xsh.52xcode.cn

[O01] 启动一个线程
来源：http://bfa.jinqigufen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lge.jqgfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ibr.jqgufenzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fld.ctjpmb.com

TS:   // 同 JS
来源：http://deb.epnwcf.com

Java: new Thread(() -> f()).start()
来源：http://ozo.aizwys.cn

Go:   go f()
来源：http://lya.meibo888.top

Ruby: Thread.new { f }
来源：http://kpe.cqqwz.cn

C#:   Task.Run(() => F());
来源：http://djw.sxryk.cn

[O02] 使用线程池
来源：http://pfc.zycfv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uig.hnqzz.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mor.fehbvm.com

JS:   // worker_threads 线程池
来源：http://qdh.fktsv.cn

TS:   // worker_threads 线程池
来源：http://ona.xylfe.cn

Java: Executors.newFixedThreadPool(4)
来源：http://fba.sweek.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zbd.yangfankeji.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ueo.kuanghao11.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://red.hysaishi.cn

[O03] 加锁保护共享数据
来源：http://vbu.316326.xyz

Py:   with lock: shared += 1
来源：http://dma.jlsjyb.cn

PHP:  // 用 flock() 做文件锁
来源：http://tcd.cqqwz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dbt.jyoumei.cn

TS:   // 同 JS
来源：http://uhi.wangdashe.top

Java: synchronized (this) { shared++; }
来源：http://muj.jqgufenzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vru.kuanghao11.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rqc.jqgfzy.top

C#:   lock (gate) { shared++; }
来源：http://fnz.cashguo.top

[O04] 定义异步函数并等待
来源：http://vva.shangyingyoupin.top

Py:   async def f():⏎    await g()
来源：http://ovo.sysykeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bwr.xinyue.icu

JS:   async function f() { await g(); }
来源：http://syc.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jmf.shanyushiyangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yug.zdbjq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hso.jinqigfzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://zti.hysaishi.cn

C#:   async Task F() { await G(); }
来源：http://gtz.uphjek.com

[O05] 并发执行并等待全部完成
来源：http://vnc.yj202588.top

Py:   asyncio.gather(*tasks)
来源：http://yiy.hnxiangtu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ovx.xziqi.cn

JS:   await Promise.all(tasks)
来源：http://wzg.aizwys.cn

TS:   await Promise.all(tasks)
来源：http://boy.cdnleiting.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://opo.xylfe.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://neo.jinqigfzy.top

Ruby: threads.map(&:join)
来源：http://zgd.yj20258.top

C#:   await Task.WhenAll(t1, t2)
来源：http://kbd.feifeiyinyue.top

[O06] 使用进程池
来源：http://ivy.zhixingplan.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://czf.yangfankeji.com

PHP:  // pcntl_fork 或多进程队列
来源：http://efr.jinghuilouyu.cn

JS:   // child_process / cluster 模块
来源：http://rfr.daria6918.cn

TS:   // child_process / cluster 模块
来源：http://uhn.hnxiangtu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ydp.meibo888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nbe.cashguo.top

Ruby: // fork 块
来源：http://joh.jqgfzy.top

C#:   Parallel.For
来源：http://ive.hysaishi.cn

================================================================================
来源：http://ifa.fehbvm.com

P. 常用工具函数
来源：http://tfu.zycfv.cn

================================================================================
来源：http://lym.yvedp.cn

[P01] 生成 UUID
来源：http://qso.zhijiandao.cn

Py:   str(uuid.uuid4())
来源：http://jfe.bbcook.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lzu.pengpengdd.cyou

JS:   crypto.randomUUID()
来源：http://ibw.haohaochexian.top

TS:   crypto.randomUUID()
来源：http://gap.snrcjt.cn

Java: UUID.randomUUID().toString()
来源：http://jwu.fzhhl.top

Go:   // 用 github.com/google/uuid
来源：http://kli.andypj.xyz

Ruby: SecureRandom.uuid
来源：http://llr.guannengcc.top

C#:   Guid.NewGuid().ToString()
来源：http://sqa.jianghu66.top

[P02] MD5 / SHA256 摘要
来源：http://ysn.yj20258.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://asg.gotoacloud.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dif.ydzc1.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mnp.zdbjq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://moo.feifeiyinyue.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://myw.sweek.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zen.svipenyu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xlv.gaohongyu789.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ijl.jinqigfzy.top

[P03] 生成短随机字符串
来源：http://ydv.xuetiantiany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zvs.hcnkem.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://afy.dianchejie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dpl.nwbrower.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pxk.smart0.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kby.jqgfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dll.mhx1999.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gqy.redwolf501.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jsz.zhongyouzk.top

[P04] 求长度
来源：http://pnj.xingfuxueyuan.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ozs.52xcode.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bqk.tian-w.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oxg.jianghu66.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://txm.andypj.xyz

Java: list.size();  map.size();  s.length()
来源：http://cnu.zhongyouzk.top

Go:   len(arr);  len(m)
来源：http://euu.xuetiantiany.cn

Ruby: x.length;  x.size
来源：http://oso.zycfv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://thd.haohaochexian.top

[P05] 判断两个对象内容是否相等
来源：http://ddd.aizwys.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cru.xingfuxueyuan.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ubs.zhengqikj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uit.cucudq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zyf.shuidangran.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qhs.feifeiyinyue.top

Go:   reflect.DeepEqual(a, b)
来源：http://zwx.xuanzx.com

Ruby: a == b
来源：http://xjk.yj20258.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wkf.fzhhl.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zft.vehdjk.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gfo.fehbvm.com

PHP:  if (empty($x)) {}
来源：http://lem.shuidangran.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bhx.nwbrower.top

TS:   if (x == null) {}
来源：http://ulf.hcnkem.com

Java: if (x == null || x.isEmpty()) {}
来源：http://tnj.guannengcc.top

Go:   if x == nil {}
来源：http://ycp.hnqzz.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wnf.kuanghao11.cn

C#:   if (x is null) {}
来源：http://aep.tanke756.top

[P07] 防抖与节流
来源：http://wgq.316326.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cyn.cheryme.top

PHP:  // 手写时间戳比较
来源：http://yvn.havefunace.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dyo.jyoumei.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bum.epnwcf.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rer.fengsongda.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://odh.tian-w.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xsj.cucudq.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ije.shzxlz.cn

[P08] 处理浮点精度问题
来源：http://alt.ehwqpu.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lzu.svipenyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vjg.cdnleiting.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jpu.yanxiufei.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gbl.cheryme.top


<!-- 参考信息 -->