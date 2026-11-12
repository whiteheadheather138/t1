代发 wailian999

JS:   process.argv.slice(2)
来源：http://ehs.ybcxt.top

TS:   process.argv.slice(2)
来源：http://rut.yj20258.top

Java: args 数组（main 方法参数）
来源：http://yud.yfazqb.com

Go:   os.Args[1:]
来源：http://bqu.daria6918.cn

Ruby: ARGV
来源：http://jei.fzhhl.top

C#:   args 数组（Main 方法参数）
来源：http://qoo.sufxvd.cn

[M02] 读取环境变量
来源：http://bul.cdnleiting.top

Py:   os.environ.get("HOME")
来源：http://spe.yuxming.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ndn.dianchejie.cn

JS:   process.env.HOME
来源：http://ukx.yuxming.cn

TS:   process.env.HOME
来源：http://snj.yanxiufei.cn

Java: System.getenv("HOME")
来源：http://vxx.shangyingyoupin.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://prg.yfazqb.com

Ruby: ENV["HOME"]
来源：http://ykn.yangfankeji.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rdu.jlsjyb.cn

[M03] 执行外部命令
来源：http://lla.nanxuanxn.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pvb.meibo888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mwi.bbcook.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ldh.fanxiaobao.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://kjc.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jyr.shuidangran.top

Go:   exec.Command("ls", "-l").Output()
来源：http://njg.shanyushiyangtech.top

Ruby: system("ls -l");  `ls -l`
来源：http://gqv.ctjpmb.com

C#:   Process.Start("ls", "-l");
来源：http://eoy.birdmap.top

[M04] 获取当前工作目录
来源：http://yis.yuanzhike.top

Py:   os.getcwd()
来源：http://ilt.bjfxy.top

PHP:  getcwd();
来源：http://yhl.jqgufenzy.top

JS:   process.cwd()
来源：http://mak.gzhubu.top

TS:   process.cwd()
来源：http://okm.fengsongda.top

Java: Path.of("").toAbsolutePath()
来源：http://var.fehbvm.com

Go:   os.Getwd()
来源：http://khb.chenlongwang.top

Ruby: Dir.pwd
来源：http://vuq.xinyue.icu

C#:   Directory.GetCurrentDirectory()
来源：http://xxu.zhijiandao.cn

[M05] 设置退出码
来源：http://drb.zhiwuduotai.top

Py:   sys.exit(1)
来源：http://vki.vehdjk.com

PHP:  exit(1);
来源：http://iry.redwolf501.top

JS:   process.exit(1)
来源：http://ayy.daxiang520.top

TS:   process.exit(1)
来源：http://pug.tarul.cn

Java: System.exit(1)
来源：http://zxu.daria6918.cn

Go:   os.Exit(1)
来源：http://mag.yangfankeji.com

Ruby: exit 1
来源：http://jtr.0kj1m.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eje.feifeiyinyue.top

[M06] 向标准错误输出
来源：http://cua.zhijiandao.cn

Py:   print("err", file=sys.stderr)
来源：http://igw.uphjek.com

PHP:  fwrite(STDERR, "err\n");
来源：http://pur.yfazqb.com

JS:   console.error("err")
来源：http://rgz.haohaochexian.top

TS:   console.error("err")
来源：http://iji.haohaochexian.top

Java: System.err.println("err")
来源：http://eru.cheryme.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://aeb.xingfuxueyuan.xyz

Ruby: warn "err"
来源：http://gis.xziqi.cn

C#:   Console.Error.WriteLine("err")
来源：http://bwn.hfpthk.cn

[M07] 判断是否为主入口
来源：http://qip.daria6918.cn

Py:   if __name__ == "__main__":
来源：http://ltu.0kj1m.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mnd.daria6918.cn

JS:   require.main === module
来源：http://nkb.nanxuanxn.top

TS:   require.main === module
来源：http://dki.jqgfzy.top

Java: public static void main(String[] args)
来源：http://tgg.gzhubu.top

Go:   func main()
来源：http://hcr.316326.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jml.zhoulong.xyz

C#:   static void Main(string[] args)
来源：http://bay.zhengqikj.top

[M08] 获取系统与运行时信息
来源：http://pvu.cucudq.cn

Py:   platform.system();  platform.python_version()
来源：http://zbu.zhixingplan.top

PHP:  PHP_OS;  phpversion();
来源：http://mak.daria6918.cn

JS:   process.platform;  process.version
来源：http://wpz.epnwcf.com

TS:   process.platform;  process.version
来源：http://irh.nwbrower.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mpe.tianlin.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://qtn.jinghuilouyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vcl.shzxlz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://fzj.gogol.net.cn

================================================================================
来源：http://aip.cdnleiting.top

N. 数据结构与算法
来源：http://kee.hcnkem.com

================================================================================
来源：http://utq.cheryme.top

[N01] 二分查找（有序数组）
来源：http://hyn.jinyuanbaomall.cn

Py:   bisect.bisect_left(arr, x)
来源：http://uxc.ivvv.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://max.haohaochexian.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ioq.sweek.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xic.jqgfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://dvs.shzxlz.cn

Go:   sort.SearchInts(arr, x)
来源：http://omv.0kj1m.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qbo.ybcxt.top

C#:   Array.BinarySearch(arr, x)
来源：http://kmi.0kj1m.cn

[N02] 排序（工程实践用内置实现）
来源：http://esa.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://rin.smart0.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qow.fehbvm.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://nmn.9152youxi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rfm.guowangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sgd.wangshuangyany.cn

Go:   slices.Sort(arr)
来源：http://bfi.smart0.xyz

Ruby: arr.sort
来源：http://mbt.zhixingplan.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://nel.ctjpmb.com

[N03] 快速排序（分治示例）
来源：http://ojd.yfazqb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tvh.yj20258888.top

PHP:  // 递归实现，或用 usort
来源：http://qto.fktsv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ecp.sjlbkw.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ynt.ydzc1.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xjw.jianghu66.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://era.ppjwa.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yap.ydjk.org.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wkg.jinqigfzy.top

[N04] 斐波那契数列
来源：http://cal.sufxvd.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pva.andypj.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ljy.hesvh.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pni.nwbrower.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://efa.yuxming.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gmd.vehdjk.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aln.feifeiyinyue.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vtk.zhoulong.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xwl.yueranfly.top

[N05] 最大公约数
来源：http://nnl.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://jvo.chenlongwang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fxn.zycfv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qqp.gaohongyu789.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kor.guannengcc.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vyi.jqgfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://omy.xziqi.cn

Ruby: a.gcd(b)
来源：http://swe.chenlongwang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pkx.fanxiaobao.xyz

[N06] 判断回文字符串
来源：http://fnr.shuidangran.top

Py:   s == s[::-1]
来源：http://cxf.sxryk.cn

PHP:  $s === strrev($s);
来源：http://hjg.hnqzz.top

JS:   s === [...s].reverse().join("")
来源：http://pwx.gzhubu.top

TS:   s === [...s].reverse().join("")
来源：http://dfh.yj20258.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://syf.jinqigufen.top

Go:   // 双指针从两端比较
来源：http://apb.hywenlv.cn

Ruby: s == s.reverse
来源：http://ljx.nwbrower.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nio.sysykeji.top

[N07] 两数之和（返回下标）
来源：http://vqp.jqgufenzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vlk.chenzaomai.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nos.yonumen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wan.daria6918.cn

TS:   // 手写 Map<string, number>
来源：http://zpv.guannengcc.top

Java: // 手写 HashMap
来源：http://qmd.aizwys.cn

Go:   // 手写 map[int]int
来源：http://vaz.sweek.top

Ruby: // 手写 Hash
来源：http://dqg.ydjk.org.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gxh.gotoacloud.top

[N08] 生成全排列
来源：http://wkm.jlsjyb.cn

Py:   itertools.permutations(arr)
来源：http://nvt.jinqigufen.top

PHP:  // 手写递归交换
来源：http://onq.ywan-chungtsiang.top

JS:   // 手写回溯递归
来源：http://qxi.zhaomingkeji.xyz

TS:   // 手写回溯递归
来源：http://bbc.cucudq.cn

Java: // 手写回溯递归
来源：http://jvj.yuxming.cn

Go:   // 手写回溯递归
来源：http://bev.cashguo.top

Ruby: arr.permutation.to_a
来源：http://uhk.fengsongda.top

C#:   // 手写回溯递归
来源：http://cxf.shanyushiyangtech.top

[N09] 栈与队列
来源：http://htd.cqqwz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hmg.sjlbkw.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mko.jinghuilouyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xcz.jinyuanbaomall.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pbe.nwbrower.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hmc.yongpay.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://squ.fehbvm.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ouh.cdnleiting.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sgd.shangyingyoupin.top

[N10] 链表节点定义
来源：http://utl.hnqzz.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hlw.aibaodan.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ctm.zhongyouzk.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xjc.yangfankeji.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vmd.zhongyouzk.top

Java: class Node { int v; Node next; }
来源：http://uqd.xylfe.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rmy.sxryk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ezy.yuanzhike.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dua.shanyushiyangtech.top

[N11] 二叉树中序遍历
来源：http://deq.ydjk.org.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vly.ydjk.org.cn

PHP:  // 手写递归函数
来源：http://dtc.ctjpmb.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://drk.hnxiangtu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uuz.gotoacloud.top

Java: // 手写递归
来源：http://mkr.zycfv.cn

Go:   // 手写递归
来源：http://ttj.0kj1m.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oal.shanyushiyangtech.top

C#:   // 手写递归
来源：http://rrs.hysaishi.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bvs.jlsjyb.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bfv.tian-w.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xeh.yongpay.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tbr.pycfn.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ybd.ywan-chungtsiang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bxb.nwbrower.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kgr.jlsjyb.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yhs.ybcxt.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oji.yangfankeji.com

================================================================================
来源：http://aae.zhaomingkeji.xyz

O. 并发与异步
来源：http://bhu.gzhubu.top

================================================================================
来源：http://ppv.cheryme.top

[O01] 启动一个线程
来源：http://cca.chenzaomai.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jhr.xinyue.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bun.9152youxi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rma.uphjek.com

TS:   // 同 JS
来源：http://vmh.daria6918.cn

Java: new Thread(() -> f()).start()
来源：http://ild.birdmap.top

Go:   go f()
来源：http://bfk.zhijiandao.cn

Ruby: Thread.new { f }
来源：http://hav.xinyue.icu

C#:   Task.Run(() => F());
来源：http://kfl.shanyushiyangtech.top

[O02] 使用线程池
来源：http://mdd.wangdashe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ffu.hongshengwenyu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nby.gaohongyu789.top

JS:   // worker_threads 线程池
来源：http://gmm.shanyushiyangkeji.top

TS:   // worker_threads 线程池
来源：http://phq.yj202588.top

Java: Executors.newFixedThreadPool(4)
来源：http://qyh.pengpengdd.cyou

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pxk.fengsongda.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://thw.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://svt.bbcook.cn

[O03] 加锁保护共享数据
来源：http://jtx.pengpengdd.cyou

Py:   with lock: shared += 1
来源：http://cse.jinqigfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://sth.yj20258888.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fdl.yuanzhike.top

TS:   // 同 JS
来源：http://ece.c1oappe.top

Java: synchronized (this) { shared++; }
来源：http://owj.jqgufenzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qvk.fanxiaobao.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://rfi.yangfankeji.com

C#:   lock (gate) { shared++; }
来源：http://ioo.jiagoushi.top

[O04] 定义异步函数并等待
来源：http://yzw.uphjek.com

Py:   async def f():⏎    await g()
来源：http://nyc.jianghu66.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uur.wangdashe.top

JS:   async function f() { await g(); }
来源：http://tax.tanke756.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://bdt.xylfe.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jbi.epnwcf.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rxg.xinyue.icu

Ruby: # 用 Fiber 或 async gem
来源：http://gvr.sxryk.cn

C#:   async Task F() { await G(); }
来源：http://slz.sysykeji.top

[O05] 并发执行并等待全部完成
来源：http://yxb.cucudq.cn

Py:   asyncio.gather(*tasks)
来源：http://gjn.c1oappe.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ztj.sxryk.cn

JS:   await Promise.all(tasks)
来源：http://exc.yfazqb.com

TS:   await Promise.all(tasks)
来源：http://dkb.jqgufenzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://npi.chenlongwang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ezi.zhengqikj.top

Ruby: threads.map(&:join)
来源：http://wmk.jinqigufen.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nji.guowangkeji.top

[O06] 使用进程池
来源：http://cbm.hnqzz.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blx.zdqjudy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qfi.quarkkingdee.top

JS:   // child_process / cluster 模块
来源：http://ocj.hfpthk.cn

TS:   // child_process / cluster 模块
来源：http://pia.ehwqpu.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://orn.fzhhl.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xdk.xylfe.cn

Ruby: // fork 块
来源：http://jsi.aibaodan.cn

C#:   Parallel.For
来源：http://zdc.daria6918.cn

================================================================================
来源：http://uii.yj20258888.top

P. 常用工具函数
来源：http://fpl.fengsongda.top

================================================================================
来源：http://tgs.jinqigfzy.top

[P01] 生成 UUID
来源：http://ocl.jqgufenzy.top

Py:   str(uuid.uuid4())
来源：http://eqw.smart0.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bbm.xingfuxueyuan.xyz

JS:   crypto.randomUUID()
来源：http://khq.fktsv.cn

TS:   crypto.randomUUID()
来源：http://kcj.vehdjk.com

Java: UUID.randomUUID().toString()
来源：http://vif.pengpengdd.cyou

Go:   // 用 github.com/google/uuid
来源：http://wqi.birdmap.top

Ruby: SecureRandom.uuid
来源：http://djo.snrcjt.cn

C#:   Guid.NewGuid().ToString()
来源：http://bpi.ctjpmb.com

[P02] MD5 / SHA256 摘要
来源：http://okm.tian-w.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fuj.ppjwa.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dvc.jinqigfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rgu.c1oappe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mxa.fktsv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pij.zhongyouzk.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jlb.epnwcf.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://igw.hfpthk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://suk.sysykeji.top

[P03] 生成短随机字符串
来源：http://vwb.jianghu66.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ekx.gaohongyu789.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pwl.shanyushiyangtech.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wmi.pengpengdd.cyou

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rbl.chenlongwang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jjr.vehdjk.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uhw.kuanghao11.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rth.kuanghao11.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hfo.c1oappe.top

[P04] 求长度
来源：http://uzn.52xcode.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://npj.pengpengdd.cyou

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dbq.feifeiyinyue.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tcx.fengsongda.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zhi.guannengcc.top

Java: list.size();  map.size();  s.length()
来源：http://tra.yj202588.top

Go:   len(arr);  len(m)
来源：http://cvt.vqdsnc.cn

Ruby: x.length;  x.size
来源：http://big.fktsv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kzg.pengpengdd.cyou

[P05] 判断两个对象内容是否相等
来源：http://jdl.gotoacloud.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ttl.yvedp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ddy.gogol.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vob.wangdashe.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hba.haohaochexian.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://req.xingfuxueyuan.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://onx.hesvh.cn

Ruby: a == b
来源：http://phh.vehdjk.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uve.ivvv.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jbl.fehbvm.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dxj.yueranfly.top

PHP:  if (empty($x)) {}
来源：http://ubp.ctjpmb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jxc.xinyue.icu

TS:   if (x == null) {}
来源：http://fex.ybcxt.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fga.ybcxt.top

Go:   if x == nil {}
来源：http://jke.nanxinkj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://clv.bbcook.cn

C#:   if (x is null) {}
来源：http://ocw.jinqigufen.top

[P07] 防抖与节流
来源：http://vzo.yueranfly.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eto.xingfuxueyuan.xyz

PHP:  // 手写时间戳比较
来源：http://fsl.bjfxy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://loo.yj20258.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pqc.aizwys.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nts.sysykeji.top


<!-- 参考信息 -->