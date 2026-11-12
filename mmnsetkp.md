代发 wailian999

================================================================================
来源：http://ztu.jqgfzy.top

[M01] 读取命令行参数
来源：http://kwb.pycfn.com

Py:   sys.argv[1:]
来源：http://okb.316326.xyz

PHP:  $argv;  $argc;
来源：http://zdv.jinqigfzy.top

JS:   process.argv.slice(2)
来源：http://xkd.hfpthk.cn

TS:   process.argv.slice(2)
来源：http://cid.hesvh.cn

Java: args 数组（main 方法参数）
来源：http://ebd.chenlongwang.top

Go:   os.Args[1:]
来源：http://czo.yonumen.top

Ruby: ARGV
来源：http://roz.ydjk.org.cn

C#:   args 数组（Main 方法参数）
来源：http://agb.hnqzz.top

[M02] 读取环境变量
来源：http://jip.yvedp.cn

Py:   os.environ.get("HOME")
来源：http://zzv.tianlin.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pjs.hfpthk.cn

JS:   process.env.HOME
来源：http://gvc.wangshuangyany.cn

TS:   process.env.HOME
来源：http://kzz.daxiang520.top

Java: System.getenv("HOME")
来源：http://yms.tian-w.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://axr.ybcxt.top

Ruby: ENV["HOME"]
来源：http://cwb.shanyushiyangtech.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cwd.ywan-chungtsiang.top

[M03] 执行外部命令
来源：http://bzc.hywenlv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pse.nwbrower.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ftz.fehbvm.com

JS:   child_process.execSync("ls -l").toString()
来源：http://hox.iojbl.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://twh.dianchejie.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vxr.sufxvd.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wjx.hnqzz.top

Ruby: system("ls -l");  `ls -l`
来源：http://mtb.andypj.xyz

C#:   Process.Start("ls", "-l");
来源：http://eox.shangyingyoupin.top

[M04] 获取当前工作目录
来源：http://zpt.havefunace.top

Py:   os.getcwd()
来源：http://cnc.xylfe.cn

PHP:  getcwd();
来源：http://hly.iojbl.cn

JS:   process.cwd()
来源：http://chl.hnxiangtu.top

TS:   process.cwd()
来源：http://bzu.shanyushiyangtech.top

Java: Path.of("").toAbsolutePath()
来源：http://rei.zhoulong.xyz

Go:   os.Getwd()
来源：http://vvi.wangshuangyany.cn

Ruby: Dir.pwd
来源：http://yag.feifeiyinyue.top

C#:   Directory.GetCurrentDirectory()
来源：http://xvf.jinghuilouyu.cn

[M05] 设置退出码
来源：http://yho.hysaishi.cn

Py:   sys.exit(1)
来源：http://nlb.ywan-chungtsiang.top

PHP:  exit(1);
来源：http://eih.cqqwz.cn

JS:   process.exit(1)
来源：http://qhe.fzhhl.top

TS:   process.exit(1)
来源：http://oaf.yuanzhike.top

Java: System.exit(1)
来源：http://dnz.sjlbkw.cn

Go:   os.Exit(1)
来源：http://ydb.xuanzx.com

Ruby: exit 1
来源：http://syg.zhaomingkeji.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ody.gogol.net.cn

[M06] 向标准错误输出
来源：http://pqk.sjlbkw.cn

Py:   print("err", file=sys.stderr)
来源：http://pwa.birdmap.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xer.jinqigufen.top

JS:   console.error("err")
来源：http://aqg.bjfxy.top

TS:   console.error("err")
来源：http://psl.zhengqikj.top

Java: System.err.println("err")
来源：http://sbv.cdnleiting.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yqq.zhoulong.xyz

Ruby: warn "err"
来源：http://kql.chenzaomai.com

C#:   Console.Error.WriteLine("err")
来源：http://unp.jinyuanbaomall.cn

[M07] 判断是否为主入口
来源：http://ynp.daria6918.cn

Py:   if __name__ == "__main__":
来源：http://uwq.shanyushiyangkeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eqj.sxryk.cn

JS:   require.main === module
来源：http://tni.jinghuilouyu.cn

TS:   require.main === module
来源：http://uod.dashuyun.cn

Java: public static void main(String[] args)
来源：http://kgj.sjlbkw.cn

Go:   func main()
来源：http://rcl.tanke756.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tkb.ydzc1.top

C#:   static void Main(string[] args)
来源：http://jwd.zhixingplan.top

[M08] 获取系统与运行时信息
来源：http://iyb.tanke756.top

Py:   platform.system();  platform.python_version()
来源：http://wbi.nanxinkj.top

PHP:  PHP_OS;  phpversion();
来源：http://oht.ppjwa.cn

JS:   process.platform;  process.version
来源：http://mlh.xingfuxueyuan.xyz

TS:   process.platform;  process.version
来源：http://znm.yueranfly.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nbw.bbcook.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rsd.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hyb.ppjwa.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uyl.ybcxt.top

================================================================================
来源：http://qek.iojbl.cn

N. 数据结构与算法
来源：http://ygd.yangfankeji.com

================================================================================
来源：http://lku.hywenlv.cn

[N01] 二分查找（有序数组）
来源：http://etv.guannengcc.top

Py:   bisect.bisect_left(arr, x)
来源：http://kkh.ywan-chungtsiang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bop.yuanzhike.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ryl.snrcjt.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xva.mhx1999.top

Java: Arrays.binarySearch(arr, x)
来源：http://umb.nanxuanxn.top

Go:   sort.SearchInts(arr, x)
来源：http://xwq.bjfxy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xli.wangdashe.top

C#:   Array.BinarySearch(arr, x)
来源：http://fjk.jyoumei.cn

[N02] 排序（工程实践用内置实现）
来源：http://nkw.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://ufw.gzhubu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://byf.shangyingyoupin.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://hsw.zhoulong.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://haf.cheryme.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://whb.yuanzhike.top

Go:   slices.Sort(arr)
来源：http://bhu.zhoulong.xyz

Ruby: arr.sort
来源：http://fqz.hnxiangtu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://fva.redwolf501.top

[N03] 快速排序（分治示例）
来源：http://ufq.xylfe.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://elj.zhengqikj.top

PHP:  // 递归实现，或用 usort
来源：http://out.yuanzhike.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://skf.yuanzhike.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rhd.ydjk.org.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sir.wangshuangyany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://buu.zhaomingkeji.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://smv.zycfv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ldj.vehdjk.com

[N04] 斐波那契数列
来源：http://wdm.shanyushiyangtech.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fou.jlsjyb.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ddl.gaohongyu789.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qbf.iojbl.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://okn.hnxiangtu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qqo.jyoumei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nsj.feifeiyinyue.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mlx.cdnleiting.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ooq.c1oappe.top

[N05] 最大公约数
来源：http://wif.gogol.net.cn

Py:   math.gcd(a, b)
来源：http://toq.sysykeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fke.andypj.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rci.yj20258.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://der.redwolf501.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hni.ybcxt.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wty.daxiang520.top

Ruby: a.gcd(b)
来源：http://zio.jqgfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://owp.hywenlv.cn

[N06] 判断回文字符串
来源：http://aue.guannengcc.top

Py:   s == s[::-1]
来源：http://cqh.yongpay.top

PHP:  $s === strrev($s);
来源：http://xiq.hysaishi.cn

JS:   s === [...s].reverse().join("")
来源：http://vzb.xuetiantiany.cn

TS:   s === [...s].reverse().join("")
来源：http://hma.jinghuilouyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gqv.haohaochexian.top

Go:   // 双指针从两端比较
来源：http://uig.fzhhl.top

Ruby: s == s.reverse
来源：http://quz.mhx1999.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ywz.fengsongda.top

[N07] 两数之和（返回下标）
来源：http://owp.bjfxy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rdd.cdnleiting.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://goi.shzxlz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://goq.ehwqpu.com

TS:   // 手写 Map<string, number>
来源：http://tpb.zhaomingkeji.xyz

Java: // 手写 HashMap
来源：http://huj.ehwqpu.com

Go:   // 手写 map[int]int
来源：http://prd.yueranfly.top

Ruby: // 手写 Hash
来源：http://low.52xcode.cn

C#:   // 手写 Dictionary<int, int>
来源：http://txf.chenlongwang.top

[N08] 生成全排列
来源：http://qwf.yvedp.cn

Py:   itertools.permutations(arr)
来源：http://xju.zhengqikj.top

PHP:  // 手写递归交换
来源：http://kqx.guowangkeji.top

JS:   // 手写回溯递归
来源：http://blg.fanxiaobao.xyz

TS:   // 手写回溯递归
来源：http://imm.feifeiyinyue.top

Java: // 手写回溯递归
来源：http://fpg.hnxiangtu.top

Go:   // 手写回溯递归
来源：http://jcj.ydzc1.top

Ruby: arr.permutation.to_a
来源：http://mdx.zhoulong.xyz

C#:   // 手写回溯递归
来源：http://obs.ctjpmb.com

[N09] 栈与队列
来源：http://ajk.zdbjq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zep.zhongyouzk.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dnw.sweek.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cqn.chenzaomai.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iby.xylfe.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qri.haohaochexian.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bcc.sweek.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://goe.ydjk.org.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gek.ywan-chungtsiang.top

[N10] 链表节点定义
来源：http://ljs.chenzaomai.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lhq.aibaodan.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pdr.chenzaomai.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://coj.yangfankeji.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wuv.chenjidiqi.icu

Java: class Node { int v; Node next; }
来源：http://kry.yanxiufei.cn

Go:   type Node struct { V int; Next *Node }
来源：http://odt.jyoumei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://awv.feifeiyinyue.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bjd.bbcook.cn

[N11] 二叉树中序遍历
来源：http://nnk.aizwys.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nxn.dianchejie.cn

PHP:  // 手写递归函数
来源：http://xtn.fzhhl.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bgd.yj202588.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nyv.tanke756.top

Java: // 手写递归
来源：http://zdz.daxiang520.top

Go:   // 手写递归
来源：http://qaw.sysykeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://aui.c1oappe.top

C#:   // 手写递归
来源：http://gda.ydjk.org.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jtb.ywan-chungtsiang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fsa.zhijiandao.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://grb.bjfxy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vpt.jianghu66.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fep.feifeiyinyue.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://axu.nanxinkj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bbt.ppjwa.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://btg.jianghu66.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mob.jinqigufen.top

================================================================================
来源：http://rcx.yonumen.top

O. 并发与异步
来源：http://vqh.jqgufenzy.top

================================================================================
来源：http://zvo.zhaomingkeji.xyz

[O01] 启动一个线程
来源：http://sip.epnwcf.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://axx.daxiang520.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://igo.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kyj.nwbrower.top

TS:   // 同 JS
来源：http://nop.svipenyu.cn

Java: new Thread(() -> f()).start()
来源：http://qzi.kuanghao11.cn

Go:   go f()
来源：http://pkw.cashguo.top

Ruby: Thread.new { f }
来源：http://ido.zhaomingkeji.xyz

C#:   Task.Run(() => F());
来源：http://gdh.zhaomingkeji.xyz

[O02] 使用线程池
来源：http://drr.zdqjudy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cxc.yvedp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qor.yj20258888.top

JS:   // worker_threads 线程池
来源：http://jsf.316326.xyz

TS:   // worker_threads 线程池
来源：http://ixe.sysykeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://gvb.tianlin.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qfe.vqdsnc.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mwr.daxiang520.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yka.fktsv.cn

[O03] 加锁保护共享数据
来源：http://euy.yj202588.top

Py:   with lock: shared += 1
来源：http://rsy.fzhhl.top

PHP:  // 用 flock() 做文件锁
来源：http://unf.cdnleiting.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://doo.zdbjq.cn

TS:   // 同 JS
来源：http://dsd.dashuyun.cn

Java: synchronized (this) { shared++; }
来源：http://bzi.yj202588.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zvg.sufxvd.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bdu.epnwcf.com

C#:   lock (gate) { shared++; }
来源：http://cah.fktsv.cn

[O04] 定义异步函数并等待
来源：http://zqq.tarul.cn

Py:   async def f():⏎    await g()
来源：http://msf.tian-w.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hqj.jianghu66.top

JS:   async function f() { await g(); }
来源：http://fie.pengpengdd.cyou

TS:   async function f(): Promise<void> { await g(); }
来源：http://dma.sysykeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xas.yanxiufei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rem.gotoacloud.top

Ruby: # 用 Fiber 或 async gem
来源：http://grs.fengsongda.top

C#:   async Task F() { await G(); }
来源：http://jak.zhixingplan.top

[O05] 并发执行并等待全部完成
来源：http://zom.bbcook.cn

Py:   asyncio.gather(*tasks)
来源：http://tag.xuetiantiany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wqc.meibo888.top

JS:   await Promise.all(tasks)
来源：http://tzd.chenzaomai.com

TS:   await Promise.all(tasks)
来源：http://fog.zhoulong.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mmd.daria6918.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tlb.hammf.cn

Ruby: threads.map(&:join)
来源：http://nfy.hesvh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wqo.epnwcf.com

[O06] 使用进程池
来源：http://suu.yfazqb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ijx.sxryk.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jpo.yanxiufei.cn

JS:   // child_process / cluster 模块
来源：http://vxw.pengpengdd.cyou

TS:   // child_process / cluster 模块
来源：http://erx.yongpay.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pqt.chenjidiqi.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ndp.fengsongda.top

Ruby: // fork 块
来源：http://uww.andypj.xyz

C#:   Parallel.For
来源：http://dnz.shanyushiyangkeji.top

================================================================================
来源：http://uex.aibaodan.cn

P. 常用工具函数
来源：http://hhs.vehdjk.com

================================================================================
来源：http://ecu.daria6918.cn

[P01] 生成 UUID
来源：http://jpi.daria6918.cn

Py:   str(uuid.uuid4())
来源：http://fzr.zhongyouzk.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pim.hysaishi.cn

JS:   crypto.randomUUID()
来源：http://vlc.svipenyu.cn

TS:   crypto.randomUUID()
来源：http://hhq.shzxlz.cn

Java: UUID.randomUUID().toString()
来源：http://eey.pycfn.com

Go:   // 用 github.com/google/uuid
来源：http://zwi.pycfn.com

Ruby: SecureRandom.uuid
来源：http://lco.hysaishi.cn

C#:   Guid.NewGuid().ToString()
来源：http://nme.meibo888.top

[P02] MD5 / SHA256 摘要
来源：http://pgm.daxiang520.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xwv.hfpthk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://slb.feifeiyinyue.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ckb.ybcxt.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bed.zhixingplan.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dfl.shanyushiyangtech.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://toq.sweek.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ltv.dashuyun.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gcb.uphjek.com

[P03] 生成短随机字符串
来源：http://wys.zdqjudy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dms.ctjpmb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ajv.xylfe.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ngt.meibo888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xau.xingfuxueyuan.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zox.yongpay.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wrn.dashuyun.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wse.meibo888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lha.jqgufenzy.top

[P04] 求长度
来源：http://uqc.smart0.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dvd.9152youxi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wkx.cucudq.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tfl.wangdashe.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bir.yanxiufei.cn

Java: list.size();  map.size();  s.length()
来源：http://pcf.hnxiangtu.top

Go:   len(arr);  len(m)
来源：http://uop.zhoulong.xyz

Ruby: x.length;  x.size
来源：http://ref.gaohongyu789.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://bsg.zhoulong.xyz

[P05] 判断两个对象内容是否相等
来源：http://qfo.pycfn.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://exf.shanyushiyangtech.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://pek.shzxlz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jak.chenjidiqi.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fsp.dianchejie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://isj.hfpthk.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ukt.fktsv.cn

Ruby: a == b
来源：http://qeh.yangfankeji.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gjh.andypj.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pai.daria6918.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lxl.snrcjt.cn

PHP:  if (empty($x)) {}
来源：http://bpj.wangdashe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rxs.shuidangran.top

TS:   if (x == null) {}
来源：http://pjf.zhijiandao.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://csp.zycfv.cn

Go:   if x == nil {}
来源：http://bon.havefunace.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mda.tianlin.xyz

C#:   if (x is null) {}
来源：http://bxh.ehwqpu.com

[P07] 防抖与节流
来源：http://hmk.redwolf501.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wfj.316326.xyz


<!-- 参考信息 -->