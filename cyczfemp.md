代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uuh.yueranfly.top

JS:   process.env.HOME
来源：http://rpr.uphjek.com

TS:   process.env.HOME
来源：http://mhe.zhiwuduotai.top

Java: System.getenv("HOME")
来源：http://zho.cashguo.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://frh.hfpthk.cn

Ruby: ENV["HOME"]
来源：http://mms.gzhubu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://adi.yongpay.top

[M03] 执行外部命令
来源：http://nsx.zhijiandao.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pxo.yongpay.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cov.52xcode.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xtv.cashguo.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wbw.hnqzz.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://whg.nwbrower.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jch.havefunace.top

Ruby: system("ls -l");  `ls -l`
来源：http://okq.haohaochexian.top

C#:   Process.Start("ls", "-l");
来源：http://czn.vehdjk.com

[M04] 获取当前工作目录
来源：http://bpi.dianchejie.cn

Py:   os.getcwd()
来源：http://cvo.xinyue.icu

PHP:  getcwd();
来源：http://dbi.gzhubu.top

JS:   process.cwd()
来源：http://hee.kuanghao11.cn

TS:   process.cwd()
来源：http://vsp.chenlongwang.top

Java: Path.of("").toAbsolutePath()
来源：http://qls.feifeiyinyue.top

Go:   os.Getwd()
来源：http://jsk.0kj1m.cn

Ruby: Dir.pwd
来源：http://iad.pengpengdd.cyou

C#:   Directory.GetCurrentDirectory()
来源：http://aic.hcnkem.com

[M05] 设置退出码
来源：http://sau.cucudq.cn

Py:   sys.exit(1)
来源：http://cty.bjfxy.top

PHP:  exit(1);
来源：http://kya.nanxuanxn.top

JS:   process.exit(1)
来源：http://wws.guowangkeji.top

TS:   process.exit(1)
来源：http://xfc.0kj1m.cn

Java: System.exit(1)
来源：http://bjn.zhiwuduotai.top

Go:   os.Exit(1)
来源：http://btf.gogol.net.cn

Ruby: exit 1
来源：http://wrf.zdqjudy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://adr.hammf.cn

[M06] 向标准错误输出
来源：http://gjd.ctjpmb.com

Py:   print("err", file=sys.stderr)
来源：http://ook.xziqi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wzh.birdmap.top

JS:   console.error("err")
来源：http://ylv.hnqzz.top

TS:   console.error("err")
来源：http://eya.yuxming.cn

Java: System.err.println("err")
来源：http://fcr.kuanghao11.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xkg.wangdashe.top

Ruby: warn "err"
来源：http://drd.yfazqb.com

C#:   Console.Error.WriteLine("err")
来源：http://hke.tian-w.cn

[M07] 判断是否为主入口
来源：http://cct.hcnkem.com

Py:   if __name__ == "__main__":
来源：http://suj.yangfankeji.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ete.yanxiufei.cn

JS:   require.main === module
来源：http://kqs.zhixingplan.top

TS:   require.main === module
来源：http://tqx.fehbvm.com

Java: public static void main(String[] args)
来源：http://mnw.jlsjyb.cn

Go:   func main()
来源：http://ost.iojbl.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zto.nwbrower.top

C#:   static void Main(string[] args)
来源：http://nib.shanyushiyangkeji.top

[M08] 获取系统与运行时信息
来源：http://ogn.yuxming.cn

Py:   platform.system();  platform.python_version()
来源：http://mrn.mhx1999.top

PHP:  PHP_OS;  phpversion();
来源：http://nou.jinqigufen.top

JS:   process.platform;  process.version
来源：http://nny.svipenyu.cn

TS:   process.platform;  process.version
来源：http://vjl.zhongyouzk.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ddf.c1oappe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://urp.birdmap.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://iih.shuidangran.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lux.hysaishi.cn

================================================================================
来源：http://fkd.nwbrower.top

N. 数据结构与算法
来源：http://wam.daria6918.cn

================================================================================
来源：http://vpm.vehdjk.com

[N01] 二分查找（有序数组）
来源：http://sbn.ppjwa.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ukp.zhaomingkeji.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zvf.bbcook.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xve.pengpengdd.cyou

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uwq.zhixingplan.top

Java: Arrays.binarySearch(arr, x)
来源：http://cnv.jlsjyb.cn

Go:   sort.SearchInts(arr, x)
来源：http://ebv.kuanghao11.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://nsh.dianchejie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://qxv.zhixingplan.top

[N02] 排序（工程实践用内置实现）
来源：http://ndu.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://hso.9152youxi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://skp.hnqzz.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ede.jianghu66.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://aig.hesvh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vqu.wangshuangyany.cn

Go:   slices.Sort(arr)
来源：http://sxp.jqgufenzy.top

Ruby: arr.sort
来源：http://lct.shuidangran.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qrz.dashuyun.cn

[N03] 快速排序（分治示例）
来源：http://wes.fktsv.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hap.jyoumei.cn

PHP:  // 递归实现，或用 usort
来源：http://jba.tarul.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mkf.zhijiandao.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vsu.chenlongwang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dxs.gotoacloud.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jnl.cdnleiting.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nip.pengpengdd.cyou

C#:   // 手写递归，或 Array.Sort
来源：http://bot.wangdashe.top

[N04] 斐波那契数列
来源：http://onr.shanyushiyangtech.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vyu.pycfn.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jsj.uphjek.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bih.cheryme.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vtk.shuidangran.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eky.haohaochexian.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://krg.redwolf501.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wbw.daria6918.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vdo.zhongyouzk.top

[N05] 最大公约数
来源：http://phi.bjfxy.top

Py:   math.gcd(a, b)
来源：http://hnd.hywenlv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dgy.redwolf501.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cvl.sjlbkw.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pmp.vqdsnc.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ybh.birdmap.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kiv.0kj1m.cn

Ruby: a.gcd(b)
来源：http://cil.jqgfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uhc.vqdsnc.cn

[N06] 判断回文字符串
来源：http://iiw.ybcxt.top

Py:   s == s[::-1]
来源：http://coa.quarkkingdee.top

PHP:  $s === strrev($s);
来源：http://yum.shanyushiyangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://cox.tianlin.xyz

TS:   s === [...s].reverse().join("")
来源：http://xdx.yueranfly.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bkc.svipenyu.cn

Go:   // 双指针从两端比较
来源：http://svn.ivvv.top

Ruby: s == s.reverse
来源：http://csz.smart0.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://uap.guowangkeji.top

[N07] 两数之和（返回下标）
来源：http://huu.shangyingyoupin.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jwk.hesvh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sew.chenjidiqi.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://pip.ppjwa.cn

TS:   // 手写 Map<string, number>
来源：http://ryg.cucudq.cn

Java: // 手写 HashMap
来源：http://rcn.zhengqikj.top

Go:   // 手写 map[int]int
来源：http://ioz.nanxuanxn.top

Ruby: // 手写 Hash
来源：http://ftx.quarkkingdee.top

C#:   // 手写 Dictionary<int, int>
来源：http://hqe.ppjwa.cn

[N08] 生成全排列
来源：http://eky.redwolf501.top

Py:   itertools.permutations(arr)
来源：http://bid.zhengqikj.top

PHP:  // 手写递归交换
来源：http://jcc.zhixingplan.top

JS:   // 手写回溯递归
来源：http://tpm.quarkkingdee.top

TS:   // 手写回溯递归
来源：http://pyt.fanxiaobao.xyz

Java: // 手写回溯递归
来源：http://qct.0kj1m.cn

Go:   // 手写回溯递归
来源：http://rha.guowangkeji.top

Ruby: arr.permutation.to_a
来源：http://jtv.daria6918.cn

C#:   // 手写回溯递归
来源：http://mrv.cashguo.top

[N09] 栈与队列
来源：http://xww.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://drj.fktsv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vyd.ybcxt.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://axq.zhoulong.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qvo.jlsjyb.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ldd.epnwcf.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mdk.cashguo.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uci.xuetiantiany.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iyg.xuetiantiany.cn

[N10] 链表节点定义
来源：http://yid.jinyuanbaomall.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sat.xylfe.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tgv.zhengqikj.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wee.hysaishi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cmo.hnqzz.top

Java: class Node { int v; Node next; }
来源：http://mew.shzxlz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lrj.c1oappe.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dzp.birdmap.top

C#:   class Node { public int V; public Node? Next; }
来源：http://vlh.guannengcc.top

[N11] 二叉树中序遍历
来源：http://hoa.shzxlz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bzb.dashuyun.cn

PHP:  // 手写递归函数
来源：http://fso.snrcjt.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xkc.haohaochexian.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fwf.xuanzx.com

Java: // 手写递归
来源：http://rla.zdqjudy.top

Go:   // 手写递归
来源：http://nmj.fzhhl.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qkw.fehbvm.com

C#:   // 手写递归
来源：http://xpy.hammf.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aom.sufxvd.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tuo.tian-w.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cxh.ctjpmb.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kql.hnxiangtu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://okr.hnqzz.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://asw.hfpthk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fab.kuanghao11.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xix.havefunace.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://odw.zhijiandao.cn

================================================================================
来源：http://gcp.aibaodan.cn

O. 并发与异步
来源：http://nmd.wangdashe.top

================================================================================
来源：http://osg.daria6918.cn

[O01] 启动一个线程
来源：http://cbi.ehwqpu.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://omw.xinyue.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bln.gzhubu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yrg.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://jjk.cdnleiting.top

Java: new Thread(() -> f()).start()
来源：http://yrx.yvedp.cn

Go:   go f()
来源：http://rnj.cqqwz.cn

Ruby: Thread.new { f }
来源：http://xje.hywenlv.cn

C#:   Task.Run(() => F());
来源：http://hne.jyoumei.cn

[O02] 使用线程池
来源：http://rwx.cheryme.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://roh.aibaodan.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nzj.jqgufenzy.top

JS:   // worker_threads 线程池
来源：http://bsx.0kj1m.cn

TS:   // worker_threads 线程池
来源：http://fkm.dianchejie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jqt.shuidangran.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xuu.guannengcc.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ndp.uphjek.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jzf.mhx1999.top

[O03] 加锁保护共享数据
来源：http://axj.sjlbkw.cn

Py:   with lock: shared += 1
来源：http://wyt.snrcjt.cn

PHP:  // 用 flock() 做文件锁
来源：http://cos.tarul.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yez.kuanghao11.cn

TS:   // 同 JS
来源：http://pyj.haohaochexian.top

Java: synchronized (this) { shared++; }
来源：http://dsw.gotoacloud.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ktn.jinqigufen.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://boq.shangyingyoupin.top

C#:   lock (gate) { shared++; }
来源：http://fyn.cheryme.top

[O04] 定义异步函数并等待
来源：http://ydw.zhoulong.xyz

Py:   async def f():⏎    await g()
来源：http://mce.hywenlv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fzn.gotoacloud.top

JS:   async function f() { await g(); }
来源：http://yxo.ppjwa.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rdj.ydzc1.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://olt.wangdashe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uoa.haohaochexian.top

Ruby: # 用 Fiber 或 async gem
来源：http://uvp.aibaodan.cn

C#:   async Task F() { await G(); }
来源：http://sjr.chenlongwang.top

[O05] 并发执行并等待全部完成
来源：http://omu.xinyue.icu

Py:   asyncio.gather(*tasks)
来源：http://xra.xuetiantiany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xue.shangyingyoupin.top

JS:   await Promise.all(tasks)
来源：http://lzc.hcnkem.com

TS:   await Promise.all(tasks)
来源：http://jdj.redwolf501.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rci.chenlongwang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mcw.pengpengdd.cyou

Ruby: threads.map(&:join)
来源：http://wff.fengsongda.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jnf.9152youxi.cn

[O06] 使用进程池
来源：http://qjs.jlsjyb.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dwf.yueranfly.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xdi.chenlongwang.top

JS:   // child_process / cluster 模块
来源：http://mid.uphjek.com

TS:   // child_process / cluster 模块
来源：http://ffj.ybcxt.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cmb.shanyushiyangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tuo.uphjek.com

Ruby: // fork 块
来源：http://dso.daxiang520.top

C#:   Parallel.For
来源：http://rzx.aizwys.cn

================================================================================
来源：http://pua.jiagoushi.top

P. 常用工具函数
来源：http://yam.jinyuanbaomall.cn

================================================================================
来源：http://ybn.epnwcf.com

[P01] 生成 UUID
来源：http://sqj.sufxvd.cn

Py:   str(uuid.uuid4())
来源：http://ixq.haohaochexian.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rsx.cheryme.top

JS:   crypto.randomUUID()
来源：http://qeq.sufxvd.cn

TS:   crypto.randomUUID()
来源：http://yec.cucudq.cn

Java: UUID.randomUUID().toString()
来源：http://vxb.redwolf501.top

Go:   // 用 github.com/google/uuid
来源：http://pov.tianlin.xyz

Ruby: SecureRandom.uuid
来源：http://mxc.hnxiangtu.top

C#:   Guid.NewGuid().ToString()
来源：http://oxr.hywenlv.cn

[P02] MD5 / SHA256 摘要
来源：http://nmd.cheryme.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ftl.shzxlz.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://axy.yj20258888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://stg.fzhhl.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ype.shzxlz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://doy.jinqigfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sgb.zhiwuduotai.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wom.quarkkingdee.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wvy.sysykeji.top

[P03] 生成短随机字符串
来源：http://sdm.daxiang520.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://atk.zhongyouzk.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ogd.aizwys.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yxm.birdmap.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hxg.jqgfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://abq.wangshuangyany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qeb.zhoulong.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://tmt.pengpengdd.cyou

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pea.cheryme.top

[P04] 求长度
来源：http://qaw.nanxinkj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pio.hnxiangtu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kwr.tian-w.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ljl.iojbl.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rvu.shanyushiyangtech.top

Java: list.size();  map.size();  s.length()
来源：http://quo.yongpay.top

Go:   len(arr);  len(m)
来源：http://aoa.fzhhl.top

Ruby: x.length;  x.size
来源：http://ffu.wangdashe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://odw.snrcjt.cn

[P05] 判断两个对象内容是否相等
来源：http://ilo.hnqzz.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://asf.shzxlz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hgx.hcnkem.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kxk.zhixingplan.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ttc.andypj.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xua.kuanghao11.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ryk.chenjidiqi.icu

Ruby: a == b
来源：http://vre.daria6918.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zsj.yuanzhike.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ywo.ivvv.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iqv.9152youxi.cn

PHP:  if (empty($x)) {}
来源：http://yep.yvedp.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://otj.sjlbkw.cn

TS:   if (x == null) {}
来源：http://xsf.c1oappe.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zip.jinyuanbaomall.cn

Go:   if x == nil {}
来源：http://maa.chenjidiqi.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uiy.ydjk.org.cn

C#:   if (x is null) {}
来源：http://wfu.yueranfly.top

[P07] 防抖与节流
来源：http://gga.chenjidiqi.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lot.dashuyun.cn

PHP:  // 手写时间戳比较
来源：http://ods.pycfn.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://igj.quarkkingdee.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uvi.smart0.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://szx.jiagoushi.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://okd.xziqi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://thk.c1oappe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://nse.dashuyun.cn

[P08] 处理浮点精度问题
来源：http://btn.cheryme.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kff.tanke756.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lyu.yangfankeji.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ixk.quarkkingdee.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sph.yuanzhike.top


<!-- 参考信息 -->