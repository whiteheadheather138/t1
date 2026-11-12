代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://kej.tianlin.xyz

JS:   process.env.HOME
来源：http://mlz.bbcook.cn

TS:   process.env.HOME
来源：http://vbe.sysykeji.top

Java: System.getenv("HOME")
来源：http://sgk.ehwqpu.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kbm.ehwqpu.com

Ruby: ENV["HOME"]
来源：http://cxz.zycfv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ejk.vehdjk.com

[M03] 执行外部命令
来源：http://wjv.hammf.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kou.zhijiandao.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wsc.smart0.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://wkj.nanxinkj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fxp.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hao.52xcode.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xaj.fanxiaobao.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://xau.ppjwa.cn

C#:   Process.Start("ls", "-l");
来源：http://uql.52xcode.cn

[M04] 获取当前工作目录
来源：http://oav.zdqjudy.top

Py:   os.getcwd()
来源：http://pny.gzhubu.top

PHP:  getcwd();
来源：http://nlx.c1oappe.top

JS:   process.cwd()
来源：http://xsl.quarkkingdee.top

TS:   process.cwd()
来源：http://lna.zycfv.cn

Java: Path.of("").toAbsolutePath()
来源：http://ujz.shzxlz.cn

Go:   os.Getwd()
来源：http://iyy.hcnkem.com

Ruby: Dir.pwd
来源：http://lqq.shanyushiyangtech.top

C#:   Directory.GetCurrentDirectory()
来源：http://nms.cucudq.cn

[M05] 设置退出码
来源：http://nny.smart0.xyz

Py:   sys.exit(1)
来源：http://xkl.zycfv.cn

PHP:  exit(1);
来源：http://nqj.sxryk.cn

JS:   process.exit(1)
来源：http://vde.fehbvm.com

TS:   process.exit(1)
来源：http://yhe.yangfankeji.com

Java: System.exit(1)
来源：http://puj.wangshuangyany.cn

Go:   os.Exit(1)
来源：http://jxx.tanke756.top

Ruby: exit 1
来源：http://ewa.aizwys.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wti.cheryme.top

[M06] 向标准错误输出
来源：http://msd.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://mre.hnxiangtu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ged.yfazqb.com

JS:   console.error("err")
来源：http://hcn.tarul.cn

TS:   console.error("err")
来源：http://gtg.iojbl.cn

Java: System.err.println("err")
来源：http://wzy.jinqigfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rfe.bjfxy.top

Ruby: warn "err"
来源：http://fxg.xingfuxueyuan.xyz

C#:   Console.Error.WriteLine("err")
来源：http://zcq.uphjek.com

[M07] 判断是否为主入口
来源：http://xcy.smart0.xyz

Py:   if __name__ == "__main__":
来源：http://syp.xuetiantiany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://igh.svipenyu.cn

JS:   require.main === module
来源：http://jpk.yonumen.top

TS:   require.main === module
来源：http://bpu.sweek.top

Java: public static void main(String[] args)
来源：http://qfa.fengsongda.top

Go:   func main()
来源：http://rly.sjlbkw.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uxv.snrcjt.cn

C#:   static void Main(string[] args)
来源：http://fsk.aibaodan.cn

[M08] 获取系统与运行时信息
来源：http://mux.hysaishi.cn

Py:   platform.system();  platform.python_version()
来源：http://faj.ybcxt.top

PHP:  PHP_OS;  phpversion();
来源：http://faa.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://cmz.havefunace.top

TS:   process.platform;  process.version
来源：http://wgd.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mkj.sufxvd.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kti.sweek.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jhg.gogol.net.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dlz.cdnleiting.top

================================================================================
来源：http://ecv.birdmap.top

N. 数据结构与算法
来源：http://hlv.c1oappe.top

================================================================================
来源：http://dlc.zdbjq.cn

[N01] 二分查找（有序数组）
来源：http://xgq.52xcode.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xaa.vqdsnc.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pep.hfpthk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hwj.chenjidiqi.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rja.haohaochexian.top

Java: Arrays.binarySearch(arr, x)
来源：http://gwh.kuanghao11.cn

Go:   sort.SearchInts(arr, x)
来源：http://jbd.birdmap.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://wbi.jinyuanbaomall.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rbb.ydjk.org.cn

[N02] 排序（工程实践用内置实现）
来源：http://bic.c1oappe.top

Py:   sorted(arr);  arr.sort()
来源：http://fne.jianghu66.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mrm.snrcjt.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://plr.cucudq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dyi.fehbvm.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pxm.jinqigufen.top

Go:   slices.Sort(arr)
来源：http://qgg.xuetiantiany.cn

Ruby: arr.sort
来源：http://nab.fengsongda.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ncy.fktsv.cn

[N03] 快速排序（分治示例）
来源：http://wjs.shuidangran.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zgj.yueranfly.top

PHP:  // 递归实现，或用 usort
来源：http://dhb.jlsjyb.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xrs.tarul.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://alq.ybcxt.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fju.cheryme.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iok.shanyushiyangtech.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rie.52xcode.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cgz.nanxuanxn.top

[N04] 斐波那契数列
来源：http://tan.nwbrower.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pny.yvedp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://aaq.quarkkingdee.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ewl.jiagoushi.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jav.sysykeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cid.yj20258888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jhw.chenlongwang.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://twi.wangdashe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qkn.dianchejie.cn

[N05] 最大公约数
来源：http://lxg.ywan-chungtsiang.top

Py:   math.gcd(a, b)
来源：http://fpe.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oqa.jinqigfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ugu.mhx1999.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://adp.kuanghao11.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bvp.yj20258.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ndp.dashuyun.cn

Ruby: a.gcd(b)
来源：http://aec.yj202588.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wzq.pycfn.com

[N06] 判断回文字符串
来源：http://xzn.shangyingyoupin.top

Py:   s == s[::-1]
来源：http://bwe.daxiang520.top

PHP:  $s === strrev($s);
来源：http://vet.yuxming.cn

JS:   s === [...s].reverse().join("")
来源：http://zuq.yonumen.top

TS:   s === [...s].reverse().join("")
来源：http://dkf.yj20258888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cch.jinghuilouyu.cn

Go:   // 双指针从两端比较
来源：http://znf.havefunace.top

Ruby: s == s.reverse
来源：http://fak.sweek.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://zeu.shanyushiyangtech.top

[N07] 两数之和（返回下标）
来源：http://zvw.tarul.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wry.zhongyouzk.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kgl.9152youxi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nlu.nanxinkj.top

TS:   // 手写 Map<string, number>
来源：http://stg.yonumen.top

Java: // 手写 HashMap
来源：http://zuy.daxiang520.top

Go:   // 手写 map[int]int
来源：http://wfw.gzhubu.top

Ruby: // 手写 Hash
来源：http://yre.epnwcf.com

C#:   // 手写 Dictionary<int, int>
来源：http://rkd.bbcook.cn

[N08] 生成全排列
来源：http://quf.fehbvm.com

Py:   itertools.permutations(arr)
来源：http://hqy.316326.xyz

PHP:  // 手写递归交换
来源：http://blw.hongshengwenyu.top

JS:   // 手写回溯递归
来源：http://twn.xuanzx.com

TS:   // 手写回溯递归
来源：http://mhx.ctjpmb.com

Java: // 手写回溯递归
来源：http://ldg.feifeiyinyue.top

Go:   // 手写回溯递归
来源：http://ydm.hnxiangtu.top

Ruby: arr.permutation.to_a
来源：http://gdt.hysaishi.cn

C#:   // 手写回溯递归
来源：http://yqa.daria6918.cn

[N09] 栈与队列
来源：http://dia.yonumen.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ihq.xingfuxueyuan.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://elq.yuanzhike.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nrm.hfpthk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jjr.gogol.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wdy.aizwys.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wal.quarkkingdee.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kst.gzhubu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tzp.yuxming.cn

[N10] 链表节点定义
来源：http://tyz.hammf.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rpg.nanxuanxn.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ffv.zdqjudy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://arj.xuetiantiany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pnp.aibaodan.cn

Java: class Node { int v; Node next; }
来源：http://cwh.sysykeji.top

Go:   type Node struct { V int; Next *Node }
来源：http://sip.xinyue.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://twa.andypj.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://asz.guannengcc.top

[N11] 二叉树中序遍历
来源：http://cvw.redwolf501.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://luf.nanxuanxn.top

PHP:  // 手写递归函数
来源：http://lky.c1oappe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rax.jlsjyb.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ccs.ehwqpu.com

Java: // 手写递归
来源：http://nuw.0kj1m.cn

Go:   // 手写递归
来源：http://wsc.tianlin.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://frx.jinghuilouyu.cn

C#:   // 手写递归
来源：http://lzl.smart0.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bri.aizwys.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ckn.yj20258888.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bmc.hnxiangtu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oqh.yueranfly.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vjh.hcnkem.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qfk.sweek.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cxl.yonumen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jka.tianlin.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zxf.hcnkem.com

================================================================================
来源：http://kya.daxiang520.top

O. 并发与异步
来源：http://lqy.ehwqpu.com

================================================================================
来源：http://qkr.kuanghao11.cn

[O01] 启动一个线程
来源：http://xkf.haohaochexian.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iek.shanyushiyangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vfi.zdqjudy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mju.sjlbkw.cn

TS:   // 同 JS
来源：http://rzw.yueranfly.top

Java: new Thread(() -> f()).start()
来源：http://veu.aibaodan.cn

Go:   go f()
来源：http://zhf.xuetiantiany.cn

Ruby: Thread.new { f }
来源：http://vrd.cdnleiting.top

C#:   Task.Run(() => F());
来源：http://sra.ppjwa.cn

[O02] 使用线程池
来源：http://elf.sweek.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pgy.jianghu66.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zan.pengpengdd.cyou

JS:   // worker_threads 线程池
来源：http://dtv.yvedp.cn

TS:   // worker_threads 线程池
来源：http://yde.sxryk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tnn.vqdsnc.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jsd.yanxiufei.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zoj.fengsongda.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fdp.shanyushiyangtech.top

[O03] 加锁保护共享数据
来源：http://ded.vqdsnc.cn

Py:   with lock: shared += 1
来源：http://wnq.9152youxi.cn

PHP:  // 用 flock() 做文件锁
来源：http://fyn.bbcook.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xyu.svipenyu.cn

TS:   // 同 JS
来源：http://cbm.ehwqpu.com

Java: synchronized (this) { shared++; }
来源：http://ixq.zhengqikj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://afh.zhijiandao.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cja.yj20258888.top

C#:   lock (gate) { shared++; }
来源：http://fcc.zhoulong.xyz

[O04] 定义异步函数并等待
来源：http://eww.aibaodan.cn

Py:   async def f():⏎    await g()
来源：http://jdc.fengsongda.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ftk.zhijiandao.cn

JS:   async function f() { await g(); }
来源：http://brj.zycfv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ovo.yuanzhike.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pst.hnxiangtu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ive.birdmap.top

Ruby: # 用 Fiber 或 async gem
来源：http://yzb.daxiang520.top

C#:   async Task F() { await G(); }
来源：http://gnl.jqgufenzy.top

[O05] 并发执行并等待全部完成
来源：http://rdt.jiagoushi.top

Py:   asyncio.gather(*tasks)
来源：http://dqa.kuanghao11.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wuo.tarul.cn

JS:   await Promise.all(tasks)
来源：http://msw.chenzaomai.com

TS:   await Promise.all(tasks)
来源：http://nit.xuetiantiany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qgm.chenlongwang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dxe.vehdjk.com

Ruby: threads.map(&:join)
来源：http://web.tanke756.top

C#:   await Task.WhenAll(t1, t2)
来源：http://sjo.guowangkeji.top

[O06] 使用进程池
来源：http://uzy.0kj1m.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://phl.dashuyun.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://cxk.nanxuanxn.top

JS:   // child_process / cluster 模块
来源：http://gxb.xingfuxueyuan.xyz

TS:   // child_process / cluster 模块
来源：http://aze.zhijiandao.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fxg.jinqigufen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://igi.shangyingyoupin.top

Ruby: // fork 块
来源：http://bpd.andypj.xyz

C#:   Parallel.For
来源：http://ghk.ctjpmb.com

================================================================================
来源：http://scw.zdqjudy.top

P. 常用工具函数
来源：http://dap.jqgufenzy.top

================================================================================
来源：http://eta.bjfxy.top

[P01] 生成 UUID
来源：http://zod.yfazqb.com

Py:   str(uuid.uuid4())
来源：http://oxv.jinyuanbaomall.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pgi.uphjek.com

JS:   crypto.randomUUID()
来源：http://eon.guannengcc.top

TS:   crypto.randomUUID()
来源：http://ztt.zhijiandao.cn

Java: UUID.randomUUID().toString()
来源：http://pqh.yongpay.top

Go:   // 用 github.com/google/uuid
来源：http://swr.quarkkingdee.top

Ruby: SecureRandom.uuid
来源：http://yiy.ctjpmb.com

C#:   Guid.NewGuid().ToString()
来源：http://bmm.xuetiantiany.cn

[P02] MD5 / SHA256 摘要
来源：http://jco.fzhhl.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://opt.andypj.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://tdk.jqgufenzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ten.nwbrower.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zvr.snrcjt.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ijv.aibaodan.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qnc.sysykeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dws.zdbjq.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vlr.hnqzz.top

[P03] 生成短随机字符串
来源：http://lzx.nwbrower.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pxl.gogol.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://duq.xylfe.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yxk.gaohongyu789.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qcb.xingfuxueyuan.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://luw.kuanghao11.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ahc.pycfn.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://tny.zhengqikj.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tmf.wangshuangyany.cn

[P04] 求长度
来源：http://ryi.yueranfly.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zub.tian-w.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ajq.tarul.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tpj.ppjwa.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kys.jqgfzy.top

Java: list.size();  map.size();  s.length()
来源：http://uqp.sufxvd.cn

Go:   len(arr);  len(m)
来源：http://scp.shzxlz.cn

Ruby: x.length;  x.size
来源：http://epo.svipenyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bev.meibo888.top

[P05] 判断两个对象内容是否相等
来源：http://yod.ctjpmb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://tke.kuanghao11.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://udf.dashuyun.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qua.ivvv.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://unc.nanxuanxn.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ydk.jianghu66.top

Go:   reflect.DeepEqual(a, b)
来源：http://fcs.zycfv.cn

Ruby: a == b
来源：http://ukc.haohaochexian.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rjc.xingfuxueyuan.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bpf.xingfuxueyuan.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://djm.iojbl.cn

PHP:  if (empty($x)) {}
来源：http://elm.jlsjyb.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xjj.iojbl.cn

TS:   if (x == null) {}
来源：http://mlh.c1oappe.top

Java: if (x == null || x.isEmpty()) {}
来源：http://dnk.zdqjudy.top

Go:   if x == nil {}
来源：http://uwb.xuanzx.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sxx.shangyingyoupin.top

C#:   if (x is null) {}
来源：http://yrz.mhx1999.top

[P07] 防抖与节流
来源：http://qwv.guowangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gfz.pengpengdd.cyou

PHP:  // 手写时间戳比较
来源：http://vzo.yfazqb.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lsy.hcnkem.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rnz.hnxiangtu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xhb.guannengcc.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wys.xylfe.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lxg.jinqigfzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jrf.sjlbkw.cn

[P08] 处理浮点精度问题
来源：http://wwz.ppjwa.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://akh.gaohongyu789.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hid.fanxiaobao.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lea.gaohongyu789.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rvl.dianchejie.cn


<!-- 参考信息 -->