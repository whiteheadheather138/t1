代发 wailian999

JS:   process.argv.slice(2)
来源：http://vtp.jinqigufen.top

TS:   process.argv.slice(2)
来源：http://bsp.52xcode.cn

Java: args 数组（main 方法参数）
来源：http://zmd.shanyushiyangtech.top

Go:   os.Args[1:]
来源：http://ucw.zycfv.cn

Ruby: ARGV
来源：http://jry.zhiwuduotai.top

C#:   args 数组（Main 方法参数）
来源：http://nzi.zhoulong.xyz

[M02] 读取环境变量
来源：http://hfu.wangdashe.top

Py:   os.environ.get("HOME")
来源：http://ujd.quarkkingdee.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cdv.cqqwz.cn

JS:   process.env.HOME
来源：http://wnh.yj202588.top

TS:   process.env.HOME
来源：http://afj.quarkkingdee.top

Java: System.getenv("HOME")
来源：http://two.fehbvm.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rhd.zhengqikj.top

Ruby: ENV["HOME"]
来源：http://qbx.aizwys.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mie.yj202588.top

[M03] 执行外部命令
来源：http://jfg.zhengqikj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dxz.jqgufenzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gvx.fktsv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://brf.hongshengwenyu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tfd.0kj1m.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mfk.gogol.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ajf.dashuyun.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gkg.tanke756.top

C#:   Process.Start("ls", "-l");
来源：http://dnt.yuanzhike.top

[M04] 获取当前工作目录
来源：http://emy.epnwcf.com

Py:   os.getcwd()
来源：http://nns.zhixingplan.top

PHP:  getcwd();
来源：http://xxg.hywenlv.cn

JS:   process.cwd()
来源：http://uzn.snrcjt.cn

TS:   process.cwd()
来源：http://xas.0kj1m.cn

Java: Path.of("").toAbsolutePath()
来源：http://fes.smart0.xyz

Go:   os.Getwd()
来源：http://uop.shanyushiyangkeji.top

Ruby: Dir.pwd
来源：http://vfu.shuidangran.top

C#:   Directory.GetCurrentDirectory()
来源：http://enf.0kj1m.cn

[M05] 设置退出码
来源：http://inh.smart0.xyz

Py:   sys.exit(1)
来源：http://ezg.hysaishi.cn

PHP:  exit(1);
来源：http://zyk.yuxming.cn

JS:   process.exit(1)
来源：http://cgt.tian-w.cn

TS:   process.exit(1)
来源：http://izl.hongshengwenyu.top

Java: System.exit(1)
来源：http://hfg.zhoulong.xyz

Go:   os.Exit(1)
来源：http://wtp.shangyingyoupin.top

Ruby: exit 1
来源：http://asn.feifeiyinyue.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hzd.yj20258.top

[M06] 向标准错误输出
来源：http://bwl.zycfv.cn

Py:   print("err", file=sys.stderr)
来源：http://sbc.zdbjq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://gjd.quarkkingdee.top

JS:   console.error("err")
来源：http://owu.pengpengdd.cyou

TS:   console.error("err")
来源：http://pon.xuanzx.com

Java: System.err.println("err")
来源：http://udl.yj20258888.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qmf.chenzaomai.com

Ruby: warn "err"
来源：http://dou.havefunace.top

C#:   Console.Error.WriteLine("err")
来源：http://skr.haohaochexian.top

[M07] 判断是否为主入口
来源：http://lio.tanke756.top

Py:   if __name__ == "__main__":
来源：http://wrs.zycfv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jdf.cheryme.top

JS:   require.main === module
来源：http://gwa.sjlbkw.cn

TS:   require.main === module
来源：http://ztv.yueranfly.top

Java: public static void main(String[] args)
来源：http://zne.tianlin.xyz

Go:   func main()
来源：http://qxf.dianchejie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hkz.shangyingyoupin.top

C#:   static void Main(string[] args)
来源：http://slz.zhongyouzk.top

[M08] 获取系统与运行时信息
来源：http://zlu.vqdsnc.cn

Py:   platform.system();  platform.python_version()
来源：http://ovm.yonumen.top

PHP:  PHP_OS;  phpversion();
来源：http://hpn.zdbjq.cn

JS:   process.platform;  process.version
来源：http://qnt.cdnleiting.top

TS:   process.platform;  process.version
来源：http://qua.meibo888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sag.gaohongyu789.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zxt.meibo888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vbw.yj202588.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://owh.hnqzz.top

================================================================================
来源：http://zwl.nwbrower.top

N. 数据结构与算法
来源：http://lyi.yj202588.top

================================================================================
来源：http://pmx.ywan-chungtsiang.top

[N01] 二分查找（有序数组）
来源：http://tpj.havefunace.top

Py:   bisect.bisect_left(arr, x)
来源：http://dxi.hesvh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uad.kuanghao11.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hjr.gzhubu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zxp.cheryme.top

Java: Arrays.binarySearch(arr, x)
来源：http://pfs.xinyue.icu

Go:   sort.SearchInts(arr, x)
来源：http://ffg.havefunace.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vat.xuetiantiany.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pzr.jinqigfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://rvc.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://cxh.feifeiyinyue.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://spj.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://rhk.tanke756.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cbx.zhoulong.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hnd.yvedp.cn

Go:   slices.Sort(arr)
来源：http://dso.jiagoushi.top

Ruby: arr.sort
来源：http://wdy.andypj.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://frj.redwolf501.top

[N03] 快速排序（分治示例）
来源：http://txc.jinghuilouyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sii.fktsv.cn

PHP:  // 递归实现，或用 usort
来源：http://hxb.jqgfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kwn.daria6918.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mlu.fengsongda.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xne.epnwcf.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yhb.zhijiandao.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lao.ppjwa.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dyh.epnwcf.com

[N04] 斐波那契数列
来源：http://oza.tanke756.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gbk.ehwqpu.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hbi.tianlin.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yqs.yonumen.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vst.chenlongwang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://irf.iojbl.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zep.9152youxi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cck.meibo888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zga.jinqigfzy.top

[N05] 最大公约数
来源：http://ovd.shangyingyoupin.top

Py:   math.gcd(a, b)
来源：http://zpa.zhaomingkeji.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hzw.yfazqb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nam.316326.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jzk.tianlin.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://arc.yanxiufei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qqn.daxiang520.top

Ruby: a.gcd(b)
来源：http://lyz.zhijiandao.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kjz.shangyingyoupin.top

[N06] 判断回文字符串
来源：http://lhd.wangdashe.top

Py:   s == s[::-1]
来源：http://ack.yuxming.cn

PHP:  $s === strrev($s);
来源：http://mfg.ehwqpu.com

JS:   s === [...s].reverse().join("")
来源：http://zvp.iojbl.cn

TS:   s === [...s].reverse().join("")
来源：http://qxt.zhoulong.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xle.nwbrower.top

Go:   // 双指针从两端比较
来源：http://bvd.nanxuanxn.top

Ruby: s == s.reverse
来源：http://wcq.guannengcc.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://osm.jlsjyb.cn

[N07] 两数之和（返回下标）
来源：http://wkh.hysaishi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fme.aibaodan.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ljf.hongshengwenyu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rbc.ivvv.top

TS:   // 手写 Map<string, number>
来源：http://par.snrcjt.cn

Java: // 手写 HashMap
来源：http://wye.dianchejie.cn

Go:   // 手写 map[int]int
来源：http://yxd.xziqi.cn

Ruby: // 手写 Hash
来源：http://bne.guowangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://lad.jinghuilouyu.cn

[N08] 生成全排列
来源：http://osm.guannengcc.top

Py:   itertools.permutations(arr)
来源：http://ktp.fktsv.cn

PHP:  // 手写递归交换
来源：http://orl.sjlbkw.cn

JS:   // 手写回溯递归
来源：http://uug.jqgufenzy.top

TS:   // 手写回溯递归
来源：http://gpu.zdbjq.cn

Java: // 手写回溯递归
来源：http://gee.snrcjt.cn

Go:   // 手写回溯递归
来源：http://kmh.tian-w.cn

Ruby: arr.permutation.to_a
来源：http://ysp.fzhhl.top

C#:   // 手写回溯递归
来源：http://jto.sxryk.cn

[N09] 栈与队列
来源：http://sbm.ydjk.org.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rln.snrcjt.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rax.ppjwa.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vdu.shzxlz.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hqs.xziqi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vrx.zhoulong.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wvi.zdbjq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ant.sufxvd.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vgr.sjlbkw.cn

[N10] 链表节点定义
来源：http://ord.daxiang520.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lkn.jqgfzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cai.zhixingplan.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pvm.nanxuanxn.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yrd.jinyuanbaomall.cn

Java: class Node { int v; Node next; }
来源：http://vgq.cdnleiting.top

Go:   type Node struct { V int; Next *Node }
来源：http://ccx.jlsjyb.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tbv.aizwys.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://bvz.yuxming.cn

[N11] 二叉树中序遍历
来源：http://waa.jinqigfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fmb.yuxming.cn

PHP:  // 手写递归函数
来源：http://oxc.haohaochexian.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ncs.gzhubu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nor.yj202588.top

Java: // 手写递归
来源：http://vvj.hysaishi.cn

Go:   // 手写递归
来源：http://yzq.havefunace.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gug.hnxiangtu.top

C#:   // 手写递归
来源：http://gxn.gzhubu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dhi.svipenyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sgd.birdmap.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dja.jinghuilouyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bwy.zdbjq.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pyv.uphjek.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gwj.zhixingplan.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dvv.sysykeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vro.daxiang520.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zef.kuanghao11.cn

================================================================================
来源：http://cmq.quarkkingdee.top

O. 并发与异步
来源：http://ygs.aibaodan.cn

================================================================================
来源：http://nhh.zhongyouzk.top

[O01] 启动一个线程
来源：http://msq.0kj1m.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sxm.birdmap.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uyb.chenjidiqi.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bhp.guannengcc.top

TS:   // 同 JS
来源：http://jjo.zhixingplan.top

Java: new Thread(() -> f()).start()
来源：http://qhl.gzhubu.top

Go:   go f()
来源：http://piq.yj20258.top

Ruby: Thread.new { f }
来源：http://ipi.pengpengdd.cyou

C#:   Task.Run(() => F());
来源：http://geh.9152youxi.cn

[O02] 使用线程池
来源：http://mbz.aibaodan.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qte.yuanzhike.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://equ.birdmap.top

JS:   // worker_threads 线程池
来源：http://unn.jinyuanbaomall.cn

TS:   // worker_threads 线程池
来源：http://jai.xuanzx.com

Java: Executors.newFixedThreadPool(4)
来源：http://agy.jinyuanbaomall.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xcv.zhoulong.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mdv.ybcxt.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jrc.yuxming.cn

[O03] 加锁保护共享数据
来源：http://blo.sweek.top

Py:   with lock: shared += 1
来源：http://taw.ehwqpu.com

PHP:  // 用 flock() 做文件锁
来源：http://jwc.pycfn.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qvm.fehbvm.com

TS:   // 同 JS
来源：http://amm.tarul.cn

Java: synchronized (this) { shared++; }
来源：http://qch.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bgm.xinyue.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://nvu.ctjpmb.com

C#:   lock (gate) { shared++; }
来源：http://dyh.yj202588.top

[O04] 定义异步函数并等待
来源：http://grx.snrcjt.cn

Py:   async def f():⏎    await g()
来源：http://czo.hesvh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bpx.sjlbkw.cn

JS:   async function f() { await g(); }
来源：http://bfl.cashguo.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rzc.bjfxy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qrl.chenzaomai.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://szr.fanxiaobao.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://fvs.9152youxi.cn

C#:   async Task F() { await G(); }
来源：http://jyu.iojbl.cn

[O05] 并发执行并等待全部完成
来源：http://kjb.jqgufenzy.top

Py:   asyncio.gather(*tasks)
来源：http://rtd.pycfn.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://aat.vqdsnc.cn

JS:   await Promise.all(tasks)
来源：http://prq.zhiwuduotai.top

TS:   await Promise.all(tasks)
来源：http://yzz.yanxiufei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eeb.snrcjt.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bfp.jqgufenzy.top

Ruby: threads.map(&:join)
来源：http://liw.guowangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://tvw.gaohongyu789.top

[O06] 使用进程池
来源：http://jwx.tian-w.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bxi.redwolf501.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zsv.zdqjudy.top

JS:   // child_process / cluster 模块
来源：http://zbs.c1oappe.top

TS:   // child_process / cluster 模块
来源：http://vuc.cucudq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xes.andypj.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wbr.jinyuanbaomall.cn

Ruby: // fork 块
来源：http://vzh.tanke756.top

C#:   Parallel.For
来源：http://dqf.snrcjt.cn

================================================================================
来源：http://xfe.andypj.xyz

P. 常用工具函数
来源：http://ipm.yanxiufei.cn

================================================================================
来源：http://pry.zhaomingkeji.xyz

[P01] 生成 UUID
来源：http://jrp.yuxming.cn

Py:   str(uuid.uuid4())
来源：http://alx.yj20258.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cut.xziqi.cn

JS:   crypto.randomUUID()
来源：http://ezy.mhx1999.top

TS:   crypto.randomUUID()
来源：http://gaf.bjfxy.top

Java: UUID.randomUUID().toString()
来源：http://wij.zhiwuduotai.top

Go:   // 用 github.com/google/uuid
来源：http://nwj.52xcode.cn

Ruby: SecureRandom.uuid
来源：http://oys.daxiang520.top

C#:   Guid.NewGuid().ToString()
来源：http://bop.yuanzhike.top

[P02] MD5 / SHA256 摘要
来源：http://oli.hnqzz.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uum.feifeiyinyue.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://oei.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ifn.xuanzx.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eri.dashuyun.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://emk.shangyingyoupin.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tab.shuidangran.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rpb.pycfn.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://frc.yj20258.top

[P03] 生成短随机字符串
来源：http://wxm.fzhhl.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qqd.cdnleiting.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bst.cheryme.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://siy.iojbl.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aqn.jqgfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mql.yuxming.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nlx.ivvv.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zwp.jqgfzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vqx.9152youxi.cn

[P04] 求长度
来源：http://fau.hnqzz.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hxr.zdqjudy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fkt.dianchejie.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ngk.zdbjq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://haw.c1oappe.top

Java: list.size();  map.size();  s.length()
来源：http://pkc.iojbl.cn

Go:   len(arr);  len(m)
来源：http://rga.fengsongda.top

Ruby: x.length;  x.size
来源：http://ffc.nwbrower.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jch.xingfuxueyuan.xyz

[P05] 判断两个对象内容是否相等
来源：http://ury.jiagoushi.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://fpq.hnxiangtu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://quu.shanyushiyangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uzl.yj20258888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sav.hnqzz.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://arq.hnqzz.top

Go:   reflect.DeepEqual(a, b)
来源：http://mtx.ivvv.top

Ruby: a == b
来源：http://czi.quarkkingdee.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fwg.daxiang520.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zwq.ehwqpu.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nfn.iojbl.cn

PHP:  if (empty($x)) {}
来源：http://koo.hesvh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cmr.haohaochexian.top

TS:   if (x == null) {}
来源：http://dag.gzhubu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://qhv.xuetiantiany.cn

Go:   if x == nil {}
来源：http://idx.yuanzhike.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vfc.sweek.top

C#:   if (x is null) {}
来源：http://pyy.tianlin.xyz

[P07] 防抖与节流
来源：http://xhc.fehbvm.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ahs.bjfxy.top

PHP:  // 手写时间戳比较
来源：http://sjz.cheryme.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zlk.hesvh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yav.xuanzx.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sgv.vqdsnc.cn


<!-- 参考信息 -->