代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://utx.yfazqb.com

Ruby: ENV["HOME"]
来源：http://vnk.hammf.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://luv.gzhubu.top

[M03] 执行外部命令
来源：http://xoe.wangshuangyany.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cwv.hammf.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ujw.chenzaomai.com

JS:   child_process.execSync("ls -l").toString()
来源：http://ult.snrcjt.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://col.wangdashe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yua.bbcook.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lzn.yuanzhike.top

Ruby: system("ls -l");  `ls -l`
来源：http://wlz.svipenyu.cn

C#:   Process.Start("ls", "-l");
来源：http://cyc.cqqwz.cn

[M04] 获取当前工作目录
来源：http://rnz.yangfankeji.com

Py:   os.getcwd()
来源：http://bgq.dashuyun.cn

PHP:  getcwd();
来源：http://jzn.yonumen.top

JS:   process.cwd()
来源：http://ubp.chenzaomai.com

TS:   process.cwd()
来源：http://cqh.nwbrower.top

Java: Path.of("").toAbsolutePath()
来源：http://ytz.hcnkem.com

Go:   os.Getwd()
来源：http://idr.epnwcf.com

Ruby: Dir.pwd
来源：http://pea.gogol.net.cn

C#:   Directory.GetCurrentDirectory()
来源：http://eza.ydjk.org.cn

[M05] 设置退出码
来源：http://rqn.jqgfzy.top

Py:   sys.exit(1)
来源：http://jle.aizwys.cn

PHP:  exit(1);
来源：http://cwm.jqgfzy.top

JS:   process.exit(1)
来源：http://qpg.chenjidiqi.icu

TS:   process.exit(1)
来源：http://ztw.yj20258888.top

Java: System.exit(1)
来源：http://fdw.pengpengdd.cyou

Go:   os.Exit(1)
来源：http://ojz.xziqi.cn

Ruby: exit 1
来源：http://feh.hammf.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://upv.shangyingyoupin.top

[M06] 向标准错误输出
来源：http://kln.chenlongwang.top

Py:   print("err", file=sys.stderr)
来源：http://ynq.ivvv.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ptj.ydjk.org.cn

JS:   console.error("err")
来源：http://mbi.zhongyouzk.top

TS:   console.error("err")
来源：http://vmd.sysykeji.top

Java: System.err.println("err")
来源：http://gax.guowangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kbl.nwbrower.top

Ruby: warn "err"
来源：http://zod.yvedp.cn

C#:   Console.Error.WriteLine("err")
来源：http://yqe.tanke756.top

[M07] 判断是否为主入口
来源：http://wwb.gzhubu.top

Py:   if __name__ == "__main__":
来源：http://srs.gogol.net.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://akh.zhixingplan.top

JS:   require.main === module
来源：http://rel.fengsongda.top

TS:   require.main === module
来源：http://wtc.quarkkingdee.top

Java: public static void main(String[] args)
来源：http://flp.jinqigfzy.top

Go:   func main()
来源：http://ijw.yangfankeji.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xdm.ehwqpu.com

C#:   static void Main(string[] args)
来源：http://ohy.xinyue.icu

[M08] 获取系统与运行时信息
来源：http://icl.shangyingyoupin.top

Py:   platform.system();  platform.python_version()
来源：http://fep.uphjek.com

PHP:  PHP_OS;  phpversion();
来源：http://rur.ybcxt.top

JS:   process.platform;  process.version
来源：http://zfk.ppjwa.cn

TS:   process.platform;  process.version
来源：http://wpv.fzhhl.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ihl.iojbl.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://blk.dashuyun.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nxq.xuanzx.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://bxn.jiagoushi.top

================================================================================
来源：http://alt.jianghu66.top

N. 数据结构与算法
来源：http://jyz.fehbvm.com

================================================================================
来源：http://jta.jinqigufen.top

[N01] 二分查找（有序数组）
来源：http://kab.svipenyu.cn

Py:   bisect.bisect_left(arr, x)
来源：http://aub.sjlbkw.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://txk.bbcook.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lyi.cdnleiting.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dbh.cqqwz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://znw.hfpthk.cn

Go:   sort.SearchInts(arr, x)
来源：http://pvk.gotoacloud.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ayg.sxryk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://aap.mhx1999.top

[N02] 排序（工程实践用内置实现）
来源：http://spu.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://dzk.chenlongwang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://snv.jqgfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://gki.xingfuxueyuan.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://npo.hysaishi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pjf.shanyushiyangkeji.top

Go:   slices.Sort(arr)
来源：http://ztx.hammf.cn

Ruby: arr.sort
来源：http://gqf.jlsjyb.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://otd.chenjidiqi.icu

[N03] 快速排序（分治示例）
来源：http://eun.aibaodan.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://chv.zhijiandao.cn

PHP:  // 递归实现，或用 usort
来源：http://ybq.yangfankeji.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ygx.daxiang520.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sfb.sjlbkw.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rdt.jyoumei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gfl.sjlbkw.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kzb.xuanzx.com

C#:   // 手写递归，或 Array.Sort
来源：http://gwx.ehwqpu.com

[N04] 斐波那契数列
来源：http://tgo.cqqwz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zsg.zhixingplan.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rky.snrcjt.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mgt.ehwqpu.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xie.ehwqpu.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xcm.guowangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jej.nwbrower.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ggp.uphjek.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://suj.shanyushiyangtech.top

[N05] 最大公约数
来源：http://fdj.xylfe.cn

Py:   math.gcd(a, b)
来源：http://ldq.havefunace.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://txp.cqqwz.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zyw.ydzc1.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rea.uphjek.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tdp.xinyue.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://aub.mhx1999.top

Ruby: a.gcd(b)
来源：http://uqh.jinyuanbaomall.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sbz.aizwys.cn

[N06] 判断回文字符串
来源：http://pre.tianlin.xyz

Py:   s == s[::-1]
来源：http://icn.zhongyouzk.top

PHP:  $s === strrev($s);
来源：http://igp.gaohongyu789.top

JS:   s === [...s].reverse().join("")
来源：http://epf.uphjek.com

TS:   s === [...s].reverse().join("")
来源：http://plj.zhongyouzk.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bdz.hfpthk.cn

Go:   // 双指针从两端比较
来源：http://cpl.xylfe.cn

Ruby: s == s.reverse
来源：http://wqd.yanxiufei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://orl.pengpengdd.cyou

[N07] 两数之和（返回下标）
来源：http://viq.yangfankeji.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kta.haohaochexian.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vdo.jinyuanbaomall.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ykb.chenjidiqi.icu

TS:   // 手写 Map<string, number>
来源：http://ukv.ydzc1.top

Java: // 手写 HashMap
来源：http://hdg.yuxming.cn

Go:   // 手写 map[int]int
来源：http://nwu.316326.xyz

Ruby: // 手写 Hash
来源：http://ivt.jinyuanbaomall.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mbo.hywenlv.cn

[N08] 生成全排列
来源：http://ywb.gaohongyu789.top

Py:   itertools.permutations(arr)
来源：http://dlm.jinqigfzy.top

PHP:  // 手写递归交换
来源：http://mgo.ctjpmb.com

JS:   // 手写回溯递归
来源：http://qif.aibaodan.cn

TS:   // 手写回溯递归
来源：http://jhq.c1oappe.top

Java: // 手写回溯递归
来源：http://bys.vehdjk.com

Go:   // 手写回溯递归
来源：http://zym.yj202588.top

Ruby: arr.permutation.to_a
来源：http://sbq.ybcxt.top

C#:   // 手写回溯递归
来源：http://kvh.quarkkingdee.top

[N09] 栈与队列
来源：http://ojl.haohaochexian.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://iwv.epnwcf.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qsu.cqqwz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ugw.bjfxy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://drt.sjlbkw.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://odr.zhijiandao.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kpg.jinyuanbaomall.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ncb.fehbvm.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://oyr.iojbl.cn

[N10] 链表节点定义
来源：http://dep.vqdsnc.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ful.fengsongda.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jad.zhongyouzk.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wqs.yueranfly.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://cdn.chenlongwang.top

Java: class Node { int v; Node next; }
来源：http://ufy.andypj.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://xrm.yuxming.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://bfh.ivvv.top

C#:   class Node { public int V; public Node? Next; }
来源：http://fhu.sufxvd.cn

[N11] 二叉树中序遍历
来源：http://bhu.iojbl.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kic.hesvh.cn

PHP:  // 手写递归函数
来源：http://rzc.wangshuangyany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xhd.52xcode.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://doa.c1oappe.top

Java: // 手写递归
来源：http://wmn.aizwys.cn

Go:   // 手写递归
来源：http://lvp.jinqigufen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://alc.yj20258.top

C#:   // 手写递归
来源：http://tse.yongpay.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kio.wangdashe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://unt.xylfe.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wsw.jinghuilouyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cnr.hnqzz.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fet.zhixingplan.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xjl.chenzaomai.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cyn.chenzaomai.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tox.52xcode.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mzf.xinyue.icu

================================================================================
来源：http://krg.yuxming.cn

O. 并发与异步
来源：http://wmo.c1oappe.top

================================================================================
来源：http://byx.wangdashe.top

[O01] 启动一个线程
来源：http://djl.redwolf501.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ydm.sufxvd.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://opr.ehwqpu.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vbu.gzhubu.top

TS:   // 同 JS
来源：http://nku.shanyushiyangkeji.top

Java: new Thread(() -> f()).start()
来源：http://fcw.nanxuanxn.top

Go:   go f()
来源：http://wvt.ctjpmb.com

Ruby: Thread.new { f }
来源：http://nkk.pycfn.com

C#:   Task.Run(() => F());
来源：http://yam.cashguo.top

[O02] 使用线程池
来源：http://eux.chenjidiqi.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rkf.daria6918.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mun.andypj.xyz

JS:   // worker_threads 线程池
来源：http://zss.chenzaomai.com

TS:   // worker_threads 线程池
来源：http://dvk.gaohongyu789.top

Java: Executors.newFixedThreadPool(4)
来源：http://qyi.zhaomingkeji.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cdt.pycfn.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mmg.zhoulong.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bhp.yangfankeji.com

[O03] 加锁保护共享数据
来源：http://hcf.guowangkeji.top

Py:   with lock: shared += 1
来源：http://hfy.birdmap.top

PHP:  // 用 flock() 做文件锁
来源：http://adk.0kj1m.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bwx.xingfuxueyuan.xyz

TS:   // 同 JS
来源：http://act.zhoulong.xyz

Java: synchronized (this) { shared++; }
来源：http://nbg.bjfxy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://smf.zhoulong.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://xez.daxiang520.top

C#:   lock (gate) { shared++; }
来源：http://veh.snrcjt.cn

[O04] 定义异步函数并等待
来源：http://jkq.fanxiaobao.xyz

Py:   async def f():⏎    await g()
来源：http://zak.jinyuanbaomall.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ajq.wangshuangyany.cn

JS:   async function f() { await g(); }
来源：http://vrg.aibaodan.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wiq.aizwys.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fuk.ppjwa.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kai.chenjidiqi.icu

Ruby: # 用 Fiber 或 async gem
来源：http://tth.yongpay.top

C#:   async Task F() { await G(); }
来源：http://xvi.guannengcc.top

[O05] 并发执行并等待全部完成
来源：http://ior.hammf.cn

Py:   asyncio.gather(*tasks)
来源：http://adc.sweek.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vil.nwbrower.top

JS:   await Promise.all(tasks)
来源：http://sit.guowangkeji.top

TS:   await Promise.all(tasks)
来源：http://jmp.chenlongwang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vaz.sjlbkw.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mfu.wangshuangyany.cn

Ruby: threads.map(&:join)
来源：http://czk.fzhhl.top

C#:   await Task.WhenAll(t1, t2)
来源：http://rjv.gaohongyu789.top

[O06] 使用进程池
来源：http://jhy.yonumen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rvh.cqqwz.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mng.yvedp.cn

JS:   // child_process / cluster 模块
来源：http://tof.yueranfly.top

TS:   // child_process / cluster 模块
来源：http://gzj.jinyuanbaomall.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rkq.andypj.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sxq.pycfn.com

Ruby: // fork 块
来源：http://sdb.jlsjyb.cn

C#:   Parallel.For
来源：http://zbx.vqdsnc.cn

================================================================================
来源：http://jui.zhijiandao.cn

P. 常用工具函数
来源：http://lgz.ydzc1.top

================================================================================
来源：http://fxp.iojbl.cn

[P01] 生成 UUID
来源：http://jdw.ydjk.org.cn

Py:   str(uuid.uuid4())
来源：http://ywi.chenlongwang.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qfa.smart0.xyz

JS:   crypto.randomUUID()
来源：http://zak.52xcode.cn

TS:   crypto.randomUUID()
来源：http://qjf.yanxiufei.cn

Java: UUID.randomUUID().toString()
来源：http://cyr.hfpthk.cn

Go:   // 用 github.com/google/uuid
来源：http://uox.bbcook.cn

Ruby: SecureRandom.uuid
来源：http://rfm.snrcjt.cn

C#:   Guid.NewGuid().ToString()
来源：http://sjo.feifeiyinyue.top

[P02] MD5 / SHA256 摘要
来源：http://pyr.zdbjq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ivy.vqdsnc.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zbp.mhx1999.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nsk.jlsjyb.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://khb.pycfn.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rcg.jianghu66.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ybb.ywan-chungtsiang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dgj.ivvv.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yoq.ppjwa.cn

[P03] 生成短随机字符串
来源：http://pso.daxiang520.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yua.jlsjyb.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rcu.jianghu66.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ekl.snrcjt.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bnp.cheryme.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wui.feifeiyinyue.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wcy.snrcjt.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ebg.daxiang520.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://eso.hnqzz.top

[P04] 求长度
来源：http://jst.snrcjt.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vhd.ctjpmb.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bvr.sxryk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zoe.aizwys.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pby.shzxlz.cn

Java: list.size();  map.size();  s.length()
来源：http://lra.zhengqikj.top

Go:   len(arr);  len(m)
来源：http://ahr.hnxiangtu.top

Ruby: x.length;  x.size
来源：http://mms.quarkkingdee.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://frf.jqgfzy.top

[P05] 判断两个对象内容是否相等
来源：http://hxf.zhijiandao.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vxp.sweek.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uxn.jinghuilouyu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gta.jyoumei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gqb.daxiang520.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kkp.hongshengwenyu.top

Go:   reflect.DeepEqual(a, b)
来源：http://xoo.guannengcc.top

Ruby: a == b
来源：http://kyz.vqdsnc.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hsg.chenzaomai.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ddy.gzhubu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kcz.tarul.cn

PHP:  if (empty($x)) {}
来源：http://kjx.yongpay.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://phb.shanyushiyangkeji.top

TS:   if (x == null) {}
来源：http://nqs.zhixingplan.top

Java: if (x == null || x.isEmpty()) {}
来源：http://aoa.tarul.cn

Go:   if x == nil {}
来源：http://uyv.shanyushiyangtech.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qjp.vehdjk.com

C#:   if (x is null) {}
来源：http://hrq.jlsjyb.cn

[P07] 防抖与节流
来源：http://eld.hesvh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jsj.cashguo.top

PHP:  // 手写时间戳比较
来源：http://prd.fzhhl.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kgt.tian-w.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qqt.hnqzz.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xbp.bjfxy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yjo.yj20258888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://nxv.zhongyouzk.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wxf.epnwcf.com

[P08] 处理浮点精度问题
来源：http://gqu.zhixingplan.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aol.yfazqb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://afh.0kj1m.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://koz.cashguo.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ynm.nwbrower.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wle.gotoacloud.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ehq.tian-w.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sea.sweek.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jyq.ctjpmb.com


<!-- 参考信息 -->