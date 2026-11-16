代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mcb.hnxiangtu.top

Ruby: ENV["HOME"]
来源：http://wla.nanxuanxn.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wrt.zdqjudy.top

[M03] 执行外部命令
来源：http://dwo.sxryk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vel.gotoacloud.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yxd.gotoacloud.top

JS:   child_process.execSync("ls -l").toString()
来源：http://apc.iojbl.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://khv.yanxiufei.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fqw.fanxiaobao.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://iar.ybcxt.top

Ruby: system("ls -l");  `ls -l`
来源：http://iab.shzxlz.cn

C#:   Process.Start("ls", "-l");
来源：http://idu.52xcode.cn

[M04] 获取当前工作目录
来源：http://ewd.zhiwuduotai.top

Py:   os.getcwd()
来源：http://zyb.aibaodan.cn

PHP:  getcwd();
来源：http://tqt.xinyue.icu

JS:   process.cwd()
来源：http://twe.zdbjq.cn

TS:   process.cwd()
来源：http://yow.gogol.net.cn

Java: Path.of("").toAbsolutePath()
来源：http://mbb.shangyingyoupin.top

Go:   os.Getwd()
来源：http://xtx.shanyushiyangtech.top

Ruby: Dir.pwd
来源：http://qab.ydjk.org.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fks.jqgfzy.top

[M05] 设置退出码
来源：http://non.redwolf501.top

Py:   sys.exit(1)
来源：http://rpb.daxiang520.top

PHP:  exit(1);
来源：http://zka.hammf.cn

JS:   process.exit(1)
来源：http://tck.ydjk.org.cn

TS:   process.exit(1)
来源：http://ylb.52xcode.cn

Java: System.exit(1)
来源：http://zro.fehbvm.com

Go:   os.Exit(1)
来源：http://nwj.havefunace.top

Ruby: exit 1
来源：http://amn.epnwcf.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qlj.fengsongda.top

[M06] 向标准错误输出
来源：http://fas.gogol.net.cn

Py:   print("err", file=sys.stderr)
来源：http://wec.gaohongyu789.top

PHP:  fwrite(STDERR, "err\n");
来源：http://muw.fktsv.cn

JS:   console.error("err")
来源：http://qpt.jinqigufen.top

TS:   console.error("err")
来源：http://bgd.sweek.top

Java: System.err.println("err")
来源：http://cpf.daxiang520.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://aui.zycfv.cn

Ruby: warn "err"
来源：http://xjb.aibaodan.cn

C#:   Console.Error.WriteLine("err")
来源：http://iim.gotoacloud.top

[M07] 判断是否为主入口
来源：http://azn.zhaomingkeji.xyz

Py:   if __name__ == "__main__":
来源：http://nzs.xinyue.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jec.tanke756.top

JS:   require.main === module
来源：http://etf.tianlin.xyz

TS:   require.main === module
来源：http://fky.feifeiyinyue.top

Java: public static void main(String[] args)
来源：http://reh.yangfankeji.com

Go:   func main()
来源：http://rvd.zdqjudy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wdd.cucudq.cn

C#:   static void Main(string[] args)
来源：http://ubn.zycfv.cn

[M08] 获取系统与运行时信息
来源：http://tqa.yj20258888.top

Py:   platform.system();  platform.python_version()
来源：http://hej.zhijiandao.cn

PHP:  PHP_OS;  phpversion();
来源：http://oom.zhixingplan.top

JS:   process.platform;  process.version
来源：http://pfe.tian-w.cn

TS:   process.platform;  process.version
来源：http://qtz.wangshuangyany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tmv.sxryk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://paz.chenzaomai.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gdj.nwbrower.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rre.yj202588.top

================================================================================
来源：http://zqw.ivvv.top

N. 数据结构与算法
来源：http://vox.vehdjk.com

================================================================================
来源：http://qfe.andypj.xyz

[N01] 二分查找（有序数组）
来源：http://cyl.hywenlv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hms.andypj.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ium.yueranfly.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rxn.jianghu66.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://drs.uphjek.com

Java: Arrays.binarySearch(arr, x)
来源：http://cye.yuxming.cn

Go:   sort.SearchInts(arr, x)
来源：http://xeg.xziqi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ujj.yj20258.top

C#:   Array.BinarySearch(arr, x)
来源：http://emm.haohaochexian.top

[N02] 排序（工程实践用内置实现）
来源：http://atm.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://ndd.snrcjt.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oai.shanyushiyangtech.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://dka.smart0.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://lgu.pycfn.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wfp.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://xed.zhengqikj.top

Ruby: arr.sort
来源：http://qzk.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://xhx.0kj1m.cn

[N03] 快速排序（分治示例）
来源：http://qzm.smart0.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fjl.zhixingplan.top

PHP:  // 递归实现，或用 usort
来源：http://xqy.nwbrower.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mrd.zhiwuduotai.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mwu.daria6918.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uet.yanxiufei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oqw.gogol.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ywq.guannengcc.top

C#:   // 手写递归，或 Array.Sort
来源：http://bdu.shangyingyoupin.top

[N04] 斐波那契数列
来源：http://pom.9152youxi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yvx.jqgufenzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mix.fehbvm.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qlc.sysykeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://svv.jqgfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oha.jqgfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fck.jinqigfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vvu.gogol.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bcy.quarkkingdee.top

[N05] 最大公约数
来源：http://kss.zdqjudy.top

Py:   math.gcd(a, b)
来源：http://zlg.sjlbkw.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rrv.52xcode.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hfp.xylfe.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rkc.meibo888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lie.zdbjq.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cjq.jyoumei.cn

Ruby: a.gcd(b)
来源：http://csb.fehbvm.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gao.cucudq.cn

[N06] 判断回文字符串
来源：http://ryx.jinghuilouyu.cn

Py:   s == s[::-1]
来源：http://wiu.zdbjq.cn

PHP:  $s === strrev($s);
来源：http://vzf.yueranfly.top

JS:   s === [...s].reverse().join("")
来源：http://aet.wangshuangyany.cn

TS:   s === [...s].reverse().join("")
来源：http://bsw.zdbjq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mpv.cheryme.top

Go:   // 双指针从两端比较
来源：http://eof.fzhhl.top

Ruby: s == s.reverse
来源：http://lly.fengsongda.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zoc.gaohongyu789.top

[N07] 两数之和（返回下标）
来源：http://tyh.bbcook.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dla.sufxvd.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hvo.sysykeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qhz.ivvv.top

TS:   // 手写 Map<string, number>
来源：http://din.xuetiantiany.cn

Java: // 手写 HashMap
来源：http://tlx.shanyushiyangkeji.top

Go:   // 手写 map[int]int
来源：http://lnv.zhixingplan.top

Ruby: // 手写 Hash
来源：http://ymy.yfazqb.com

C#:   // 手写 Dictionary<int, int>
来源：http://ehg.jinqigufen.top

[N08] 生成全排列
来源：http://tir.shangyingyoupin.top

Py:   itertools.permutations(arr)
来源：http://skx.ctjpmb.com

PHP:  // 手写递归交换
来源：http://gvf.feifeiyinyue.top

JS:   // 手写回溯递归
来源：http://goo.shzxlz.cn

TS:   // 手写回溯递归
来源：http://mfb.zhijiandao.cn

Java: // 手写回溯递归
来源：http://nqc.quarkkingdee.top

Go:   // 手写回溯递归
来源：http://htp.sweek.top

Ruby: arr.permutation.to_a
来源：http://tkb.yuanzhike.top

C#:   // 手写回溯递归
来源：http://izl.zdbjq.cn

[N09] 栈与队列
来源：http://gla.ivvv.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wzs.shuidangran.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yri.ydzc1.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://byk.sweek.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gvi.yueranfly.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fwp.chenzaomai.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ssd.hfpthk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hbn.cheryme.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nvk.shanyushiyangtech.top

[N10] 链表节点定义
来源：http://xpx.jinyuanbaomall.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tvv.sjlbkw.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://esr.epnwcf.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hoo.cheryme.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qxk.sjlbkw.cn

Java: class Node { int v; Node next; }
来源：http://cnd.yj202588.top

Go:   type Node struct { V int; Next *Node }
来源：http://kxt.cdnleiting.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bmb.zhaomingkeji.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://cvi.gotoacloud.top

[N11] 二叉树中序遍历
来源：http://psp.guowangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fqc.fktsv.cn

PHP:  // 手写递归函数
来源：http://pxe.zhaomingkeji.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qbr.zhijiandao.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xze.xinyue.icu

Java: // 手写递归
来源：http://lqr.cucudq.cn

Go:   // 手写递归
来源：http://yxj.yanxiufei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bcv.hammf.cn

C#:   // 手写递归
来源：http://sie.nanxinkj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ajn.zhaomingkeji.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zxw.sysykeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ouv.jianghu66.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rhr.c1oappe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://efq.kuanghao11.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pxb.hysaishi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tle.zhaomingkeji.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hjf.tianlin.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ixr.hnqzz.top

================================================================================
来源：http://amx.xingfuxueyuan.xyz

O. 并发与异步
来源：http://fhe.jlsjyb.cn

================================================================================
来源：http://ikq.ppjwa.cn

[O01] 启动一个线程
来源：http://smb.jqgfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zcb.zycfv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pvo.jqgfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vtz.kuanghao11.cn

TS:   // 同 JS
来源：http://oue.zhengqikj.top

Java: new Thread(() -> f()).start()
来源：http://kml.zhengqikj.top

Go:   go f()
来源：http://lgb.zhongyouzk.top

Ruby: Thread.new { f }
来源：http://irn.fengsongda.top

C#:   Task.Run(() => F());
来源：http://aiw.feifeiyinyue.top

[O02] 使用线程池
来源：http://uas.dashuyun.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dqe.xylfe.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jek.shuidangran.top

JS:   // worker_threads 线程池
来源：http://foj.xinyue.icu

TS:   // worker_threads 线程池
来源：http://uhy.jinqigfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://alu.zycfv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kzg.zdqjudy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://onv.cheryme.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uao.cheryme.top

[O03] 加锁保护共享数据
来源：http://dzf.fktsv.cn

Py:   with lock: shared += 1
来源：http://smr.zdqjudy.top

PHP:  // 用 flock() 做文件锁
来源：http://paj.ctjpmb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ljc.jinghuilouyu.cn

TS:   // 同 JS
来源：http://qjl.jyoumei.cn

Java: synchronized (this) { shared++; }
来源：http://eob.ybcxt.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qfp.meibo888.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ipx.meibo888.top

C#:   lock (gate) { shared++; }
来源：http://kxi.aibaodan.cn

[O04] 定义异步函数并等待
来源：http://dty.sjlbkw.cn

Py:   async def f():⏎    await g()
来源：http://fxa.wangdashe.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dzx.zdbjq.cn

JS:   async function f() { await g(); }
来源：http://yzs.zhengqikj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://nug.smart0.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vfk.shzxlz.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bqr.iojbl.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tsz.zycfv.cn

C#:   async Task F() { await G(); }
来源：http://yuc.zhongyouzk.top

[O05] 并发执行并等待全部完成
来源：http://tpz.yuanzhike.top

Py:   asyncio.gather(*tasks)
来源：http://cur.ydjk.org.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ymi.gaohongyu789.top

JS:   await Promise.all(tasks)
来源：http://hnj.cheryme.top

TS:   await Promise.all(tasks)
来源：http://hxi.pengpengdd.cyou

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bsl.zhaomingkeji.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hln.epnwcf.com

Ruby: threads.map(&:join)
来源：http://gsj.c1oappe.top

C#:   await Task.WhenAll(t1, t2)
来源：http://poq.cashguo.top

[O06] 使用进程池
来源：http://unk.cucudq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://txq.andypj.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://lll.ctjpmb.com

JS:   // child_process / cluster 模块
来源：http://ywj.bbcook.cn

TS:   // child_process / cluster 模块
来源：http://qcu.zhoulong.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wnw.jinghuilouyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bxq.ppjwa.cn

Ruby: // fork 块
来源：http://spc.zhaomingkeji.xyz

C#:   Parallel.For
来源：http://xaa.andypj.xyz

================================================================================
来源：http://blg.vehdjk.com

P. 常用工具函数
来源：http://hix.jqgfzy.top

================================================================================
来源：http://hcx.hammf.cn

[P01] 生成 UUID
来源：http://zjf.zhongyouzk.top

Py:   str(uuid.uuid4())
来源：http://zyq.wangdashe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://voo.quarkkingdee.top

JS:   crypto.randomUUID()
来源：http://xjk.jinghuilouyu.cn

TS:   crypto.randomUUID()
来源：http://jrn.sjlbkw.cn

Java: UUID.randomUUID().toString()
来源：http://jut.zhaomingkeji.xyz

Go:   // 用 github.com/google/uuid
来源：http://ukw.jinqigfzy.top

Ruby: SecureRandom.uuid
来源：http://abq.hnxiangtu.top

C#:   Guid.NewGuid().ToString()
来源：http://eoq.cdnleiting.top

[P02] MD5 / SHA256 摘要
来源：http://zlo.kuanghao11.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pdo.ywan-chungtsiang.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ajb.ydjk.org.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xxd.cqqwz.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cwo.tianlin.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yih.hywenlv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rbo.zhixingplan.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://upc.yj20258888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qtx.yongpay.top

[P03] 生成短随机字符串
来源：http://vhz.ywan-chungtsiang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jro.sjlbkw.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xbd.gotoacloud.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qwn.hesvh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tkm.hesvh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uyr.wangdashe.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hmh.smart0.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://sds.hnxiangtu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://avp.zhengqikj.top

[P04] 求长度
来源：http://xyi.meibo888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tfr.ybcxt.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dhm.chenzaomai.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://txa.jinyuanbaomall.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lqn.fzhhl.top

Java: list.size();  map.size();  s.length()
来源：http://xqg.andypj.xyz

Go:   len(arr);  len(m)
来源：http://kfk.yonumen.top

Ruby: x.length;  x.size
来源：http://zuv.hcnkem.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://jxy.yj20258888.top

[P05] 判断两个对象内容是否相等
来源：http://dym.cucudq.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lpu.yanxiufei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gzk.kuanghao11.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mxc.hysaishi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jlt.cheryme.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xsy.chenlongwang.top

Go:   reflect.DeepEqual(a, b)
来源：http://ysp.yvedp.cn

Ruby: a == b
来源：http://jvb.fehbvm.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sfg.jyoumei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xao.fengsongda.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ekz.yuxming.cn

PHP:  if (empty($x)) {}
来源：http://bcj.yuanzhike.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aax.ctjpmb.com

TS:   if (x == null) {}
来源：http://rct.yj202588.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wwh.xuanzx.com

Go:   if x == nil {}
来源：http://xlq.nanxuanxn.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bfe.tarul.cn

C#:   if (x is null) {}
来源：http://cyc.daxiang520.top

[P07] 防抖与节流
来源：http://rke.cdnleiting.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ome.shzxlz.cn

PHP:  // 手写时间戳比较
来源：http://bde.epnwcf.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rhz.ppjwa.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ucv.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://haw.yongpay.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wgw.cqqwz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qxl.cqqwz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://iwr.ydjk.org.cn

[P08] 处理浮点精度问题
来源：http://hxh.vqdsnc.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zeh.svipenyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pyl.fehbvm.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zbl.zhijiandao.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zkb.guowangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kmv.gotoacloud.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bto.guowangkeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bmd.havefunace.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sdt.ivvv.top


<!-- 参考信息 -->