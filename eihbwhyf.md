代发 wailian999

JS:   process.argv.slice(2)
来源：http://lsc.shanyushiyangtech.top

TS:   process.argv.slice(2)
来源：http://ckk.vehdjk.com

Java: args 数组（main 方法参数）
来源：http://yec.hcnkem.com

Go:   os.Args[1:]
来源：http://sqc.ehwqpu.com

Ruby: ARGV
来源：http://dxh.cqqwz.cn

C#:   args 数组（Main 方法参数）
来源：http://ngu.chenzaomai.com

[M02] 读取环境变量
来源：http://ijb.smart0.xyz

Py:   os.environ.get("HOME")
来源：http://rse.andypj.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jyu.bjfxy.top

JS:   process.env.HOME
来源：http://rxu.fzhhl.top

TS:   process.env.HOME
来源：http://zcc.hywenlv.cn

Java: System.getenv("HOME")
来源：http://ovv.sxryk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ccr.wangdashe.top

Ruby: ENV["HOME"]
来源：http://svv.yonumen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ggw.daxiang520.top

[M03] 执行外部命令
来源：http://vai.gotoacloud.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://opr.gotoacloud.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jnp.hammf.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://oye.chenzaomai.com

TS:   child_process.execSync("ls -l").toString()
来源：http://eyw.vqdsnc.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qld.aizwys.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://fpn.pengpengdd.cyou

Ruby: system("ls -l");  `ls -l`
来源：http://gdz.ydzc1.top

C#:   Process.Start("ls", "-l");
来源：http://xeq.shanyushiyangkeji.top

[M04] 获取当前工作目录
来源：http://rkx.smart0.xyz

Py:   os.getcwd()
来源：http://eop.fzhhl.top

PHP:  getcwd();
来源：http://uhe.snrcjt.cn

JS:   process.cwd()
来源：http://fxx.jinyuanbaomall.cn

TS:   process.cwd()
来源：http://ejn.guannengcc.top

Java: Path.of("").toAbsolutePath()
来源：http://cda.jqgfzy.top

Go:   os.Getwd()
来源：http://cym.hcnkem.com

Ruby: Dir.pwd
来源：http://oih.kuanghao11.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xcl.sufxvd.cn

[M05] 设置退出码
来源：http://odi.gogol.net.cn

Py:   sys.exit(1)
来源：http://gyt.yangfankeji.com

PHP:  exit(1);
来源：http://cza.yvedp.cn

JS:   process.exit(1)
来源：http://iif.zhiwuduotai.top

TS:   process.exit(1)
来源：http://txs.uphjek.com

Java: System.exit(1)
来源：http://wnr.bbcook.cn

Go:   os.Exit(1)
来源：http://hvi.fzhhl.top

Ruby: exit 1
来源：http://cte.havefunace.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rne.jinqigfzy.top

[M06] 向标准错误输出
来源：http://fwz.0kj1m.cn

Py:   print("err", file=sys.stderr)
来源：http://kty.zdqjudy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kab.yongpay.top

JS:   console.error("err")
来源：http://gvy.smart0.xyz

TS:   console.error("err")
来源：http://cia.sysykeji.top

Java: System.err.println("err")
来源：http://zzz.c1oappe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mek.yuanzhike.top

Ruby: warn "err"
来源：http://uwn.hnqzz.top

C#:   Console.Error.WriteLine("err")
来源：http://wei.zdqjudy.top

[M07] 判断是否为主入口
来源：http://gbt.zycfv.cn

Py:   if __name__ == "__main__":
来源：http://fdb.xinyue.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cfc.haohaochexian.top

JS:   require.main === module
来源：http://ldn.ywan-chungtsiang.top

TS:   require.main === module
来源：http://ldn.iojbl.cn

Java: public static void main(String[] args)
来源：http://jxv.daxiang520.top

Go:   func main()
来源：http://pzu.pycfn.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pdb.ybcxt.top

C#:   static void Main(string[] args)
来源：http://box.jinghuilouyu.cn

[M08] 获取系统与运行时信息
来源：http://vcg.uphjek.com

Py:   platform.system();  platform.python_version()
来源：http://psu.cdnleiting.top

PHP:  PHP_OS;  phpversion();
来源：http://axs.yj20258.top

JS:   process.platform;  process.version
来源：http://sxl.ehwqpu.com

TS:   process.platform;  process.version
来源：http://xpy.guowangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hpw.hfpthk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://idx.cucudq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://equ.zdqjudy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://owy.ydzc1.top

================================================================================
来源：http://olu.daria6918.cn

N. 数据结构与算法
来源：http://orl.yongpay.top

================================================================================
来源：http://wia.ehwqpu.com

[N01] 二分查找（有序数组）
来源：http://zdj.fktsv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kto.yueranfly.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://cfd.zycfv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xzy.bjfxy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ifc.epnwcf.com

Java: Arrays.binarySearch(arr, x)
来源：http://kav.cashguo.top

Go:   sort.SearchInts(arr, x)
来源：http://jyo.cdnleiting.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://whw.vqdsnc.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gvy.cqqwz.cn

[N02] 排序（工程实践用内置实现）
来源：http://qyp.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://vos.yj20258888.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://koj.zhongyouzk.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vim.daxiang520.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://coq.wangdashe.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vau.xuetiantiany.cn

Go:   slices.Sort(arr)
来源：http://gwh.cashguo.top

Ruby: arr.sort
来源：http://dwh.hesvh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://opq.chenlongwang.top

[N03] 快速排序（分治示例）
来源：http://muo.chenjidiqi.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nkm.c1oappe.top

PHP:  // 递归实现，或用 usort
来源：http://wvl.tianlin.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tau.fengsongda.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://imn.ybcxt.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zqo.sweek.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ort.yangfankeji.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://aeu.vehdjk.com

C#:   // 手写递归，或 Array.Sort
来源：http://ccz.nwbrower.top

[N04] 斐波那契数列
来源：http://jzj.hfpthk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sol.sweek.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ozp.haohaochexian.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jjk.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zkn.sweek.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zut.chenjidiqi.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lxf.jiagoushi.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://abr.shanyushiyangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xfx.jianghu66.top

[N05] 最大公约数
来源：http://dgd.jinqigfzy.top

Py:   math.gcd(a, b)
来源：http://efu.daria6918.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wxp.fanxiaobao.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zbq.cdnleiting.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dgn.chenjidiqi.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mau.tian-w.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uth.guannengcc.top

Ruby: a.gcd(b)
来源：http://txj.nanxuanxn.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xrq.hfpthk.cn

[N06] 判断回文字符串
来源：http://hbk.yuanzhike.top

Py:   s == s[::-1]
来源：http://rby.jqgufenzy.top

PHP:  $s === strrev($s);
来源：http://lfx.tanke756.top

JS:   s === [...s].reverse().join("")
来源：http://ezf.shuidangran.top

TS:   s === [...s].reverse().join("")
来源：http://uhf.gzhubu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gll.dianchejie.cn

Go:   // 双指针从两端比较
来源：http://sgm.xylfe.cn

Ruby: s == s.reverse
来源：http://vmx.shanyushiyangtech.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qub.yueranfly.top

[N07] 两数之和（返回下标）
来源：http://cvj.wangshuangyany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vqd.gaohongyu789.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fzw.nanxuanxn.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fjd.zdqjudy.top

TS:   // 手写 Map<string, number>
来源：http://oug.jianghu66.top

Java: // 手写 HashMap
来源：http://trl.fzhhl.top

Go:   // 手写 map[int]int
来源：http://iyc.zhongyouzk.top

Ruby: // 手写 Hash
来源：http://zue.hywenlv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://btl.xinyue.icu

[N08] 生成全排列
来源：http://ffq.zhaomingkeji.xyz

Py:   itertools.permutations(arr)
来源：http://gcw.fengsongda.top

PHP:  // 手写递归交换
来源：http://tya.shuidangran.top

JS:   // 手写回溯递归
来源：http://rey.ppjwa.cn

TS:   // 手写回溯递归
来源：http://dzt.jlsjyb.cn

Java: // 手写回溯递归
来源：http://goq.fzhhl.top

Go:   // 手写回溯递归
来源：http://ljl.sxryk.cn

Ruby: arr.permutation.to_a
来源：http://nyz.yonumen.top

C#:   // 手写回溯递归
来源：http://hrn.aizwys.cn

[N09] 栈与队列
来源：http://mxx.havefunace.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pyo.ydjk.org.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qxl.ppjwa.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ala.bjfxy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hvk.yj20258.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://esq.snrcjt.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rxk.yueranfly.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hls.hammf.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://itn.gotoacloud.top

[N10] 链表节点定义
来源：http://lwu.xuanzx.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mds.xziqi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vqb.uphjek.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fyk.zhengqikj.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vrl.xziqi.cn

Java: class Node { int v; Node next; }
来源：http://vrp.svipenyu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qbr.ehwqpu.com

Ruby: Node = Struct.new(:v, :next)
来源：http://vre.tarul.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://oal.quarkkingdee.top

[N11] 二叉树中序遍历
来源：http://kro.jinyuanbaomall.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://set.52xcode.cn

PHP:  // 手写递归函数
来源：http://pzn.hesvh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nso.nwbrower.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bab.birdmap.top

Java: // 手写递归
来源：http://izq.yj202588.top

Go:   // 手写递归
来源：http://emq.gzhubu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lmq.yonumen.top

C#:   // 手写递归
来源：http://jle.jqgfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lfb.jinghuilouyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qab.jinqigufen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kcg.zhengqikj.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://azq.sufxvd.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sbq.jyoumei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tnj.xuanzx.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ymp.shangyingyoupin.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rjv.aizwys.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qcw.snrcjt.cn

================================================================================
来源：http://csf.zycfv.cn

O. 并发与异步
来源：http://jxo.tianlin.xyz

================================================================================
来源：http://jae.snrcjt.cn

[O01] 启动一个线程
来源：http://mgw.iojbl.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uhj.daria6918.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xpw.kuanghao11.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ogi.zhiwuduotai.top

TS:   // 同 JS
来源：http://cvz.mhx1999.top

Java: new Thread(() -> f()).start()
来源：http://jhp.nanxinkj.top

Go:   go f()
来源：http://oev.wangshuangyany.cn

Ruby: Thread.new { f }
来源：http://ihp.xuetiantiany.cn

C#:   Task.Run(() => F());
来源：http://krm.xuetiantiany.cn

[O02] 使用线程池
来源：http://lbh.xylfe.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://whh.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tjl.shanyushiyangkeji.top

JS:   // worker_threads 线程池
来源：http://evz.yvedp.cn

TS:   // worker_threads 线程池
来源：http://vdu.svipenyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bxw.chenzaomai.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lgj.hysaishi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uni.bjfxy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://adh.hongshengwenyu.top

[O03] 加锁保护共享数据
来源：http://qla.epnwcf.com

Py:   with lock: shared += 1
来源：http://tgh.zhoulong.xyz

PHP:  // 用 flock() 做文件锁
来源：http://cdv.havefunace.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rej.9152youxi.cn

TS:   // 同 JS
来源：http://nvg.zhijiandao.cn

Java: synchronized (this) { shared++; }
来源：http://ixy.ehwqpu.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fpn.chenjidiqi.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://ekh.fengsongda.top

C#:   lock (gate) { shared++; }
来源：http://sgc.pengpengdd.cyou

[O04] 定义异步函数并等待
来源：http://nqm.jianghu66.top

Py:   async def f():⏎    await g()
来源：http://usf.hammf.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nam.xuanzx.com

JS:   async function f() { await g(); }
来源：http://qdp.birdmap.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pwn.fktsv.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mtr.cdnleiting.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://adj.haohaochexian.top

Ruby: # 用 Fiber 或 async gem
来源：http://xaz.9152youxi.cn

C#:   async Task F() { await G(); }
来源：http://ork.ydzc1.top

[O05] 并发执行并等待全部完成
来源：http://jhe.zhoulong.xyz

Py:   asyncio.gather(*tasks)
来源：http://rzb.ybcxt.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://psc.vehdjk.com

JS:   await Promise.all(tasks)
来源：http://slh.xziqi.cn

TS:   await Promise.all(tasks)
来源：http://zuj.hfpthk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oun.sufxvd.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eju.yj20258.top

Ruby: threads.map(&:join)
来源：http://iqq.gzhubu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lqc.guannengcc.top

[O06] 使用进程池
来源：http://vrz.jinqigfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jwz.hongshengwenyu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qrb.tarul.cn

JS:   // child_process / cluster 模块
来源：http://sep.jqgufenzy.top

TS:   // child_process / cluster 模块
来源：http://dzu.zhijiandao.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pkf.xziqi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ekb.yueranfly.top

Ruby: // fork 块
来源：http://mjc.hfpthk.cn

C#:   Parallel.For
来源：http://uxs.yvedp.cn

================================================================================
来源：http://ygw.xziqi.cn

P. 常用工具函数
来源：http://eky.hnxiangtu.top

================================================================================
来源：http://dkn.xziqi.cn

[P01] 生成 UUID
来源：http://hbn.mhx1999.top

Py:   str(uuid.uuid4())
来源：http://uwc.jinqigufen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nai.jiagoushi.top

JS:   crypto.randomUUID()
来源：http://yek.shzxlz.cn

TS:   crypto.randomUUID()
来源：http://sqk.snrcjt.cn

Java: UUID.randomUUID().toString()
来源：http://gzw.yj202588.top

Go:   // 用 github.com/google/uuid
来源：http://zpa.cheryme.top

Ruby: SecureRandom.uuid
来源：http://cak.ydjk.org.cn

C#:   Guid.NewGuid().ToString()
来源：http://wvi.jlsjyb.cn

[P02] MD5 / SHA256 摘要
来源：http://sck.sxryk.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ytt.havefunace.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vdv.chenjidiqi.icu

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wep.fktsv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jrg.zhaomingkeji.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qkl.zhaomingkeji.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://amk.zhengqikj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iua.haohaochexian.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jwv.fanxiaobao.xyz

[P03] 生成短随机字符串
来源：http://pdg.jlsjyb.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pjf.zdbjq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uvh.yfazqb.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://udm.yvedp.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ewe.hysaishi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jgh.dianchejie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tds.yj202588.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://auc.chenzaomai.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kwq.sweek.top

[P04] 求长度
来源：http://mgi.zhijiandao.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ree.sxryk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jmu.yfazqb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dpb.gotoacloud.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sdv.yueranfly.top

Java: list.size();  map.size();  s.length()
来源：http://gkk.shanyushiyangtech.top

Go:   len(arr);  len(m)
来源：http://pqx.yfazqb.com

Ruby: x.length;  x.size
来源：http://gds.nanxuanxn.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ywb.hcnkem.com

[P05] 判断两个对象内容是否相等
来源：http://asp.ydzc1.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://llg.hesvh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dfe.sweek.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://aiz.fehbvm.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rej.chenjidiqi.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pvq.wangdashe.top

Go:   reflect.DeepEqual(a, b)
来源：http://zjl.xuanzx.com

Ruby: a == b
来源：http://nat.guannengcc.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nnv.jiagoushi.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wbi.zhijiandao.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iye.shangyingyoupin.top

PHP:  if (empty($x)) {}
来源：http://lsm.dianchejie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cys.uphjek.com

TS:   if (x == null) {}
来源：http://mlo.tian-w.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://aiv.jlsjyb.cn

Go:   if x == nil {}
来源：http://imo.tianlin.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://smt.yj20258.top

C#:   if (x is null) {}
来源：http://ufz.yuanzhike.top

[P07] 防抖与节流
来源：http://wjc.zhijiandao.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://upe.tianlin.xyz

PHP:  // 手写时间戳比较
来源：http://erj.0kj1m.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zuh.hfpthk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zvq.jqgufenzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cwk.sxryk.cn


<!-- 参考信息 -->