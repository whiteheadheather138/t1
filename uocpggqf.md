代发 wailian999

JS:   process.argv.slice(2)
来源：http://iqx.daria6918.cn

TS:   process.argv.slice(2)
来源：http://kzp.wangshuangyany.cn

Java: args 数组（main 方法参数）
来源：http://qho.daxiang520.top

Go:   os.Args[1:]
来源：http://zkb.52xcode.cn

Ruby: ARGV
来源：http://ndl.sweek.top

C#:   args 数组（Main 方法参数）
来源：http://ycx.daria6918.cn

[M02] 读取环境变量
来源：http://jwg.zhoulong.xyz

Py:   os.environ.get("HOME")
来源：http://lpz.zhaomingkeji.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rur.hywenlv.cn

JS:   process.env.HOME
来源：http://rns.c1oappe.top

TS:   process.env.HOME
来源：http://qom.cucudq.cn

Java: System.getenv("HOME")
来源：http://lrm.316326.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mqn.daxiang520.top

Ruby: ENV["HOME"]
来源：http://baw.nwbrower.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dtp.zhaomingkeji.xyz

[M03] 执行外部命令
来源：http://ycs.yanxiufei.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nsz.yangfankeji.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://avz.zhiwuduotai.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lef.0kj1m.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lxb.vehdjk.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bzs.sysykeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rdc.yangfankeji.com

Ruby: system("ls -l");  `ls -l`
来源：http://ccr.bjfxy.top

C#:   Process.Start("ls", "-l");
来源：http://cmg.bjfxy.top

[M04] 获取当前工作目录
来源：http://xlz.jianghu66.top

Py:   os.getcwd()
来源：http://blx.smart0.xyz

PHP:  getcwd();
来源：http://vog.zdqjudy.top

JS:   process.cwd()
来源：http://hsg.nanxuanxn.top

TS:   process.cwd()
来源：http://shr.vehdjk.com

Java: Path.of("").toAbsolutePath()
来源：http://asx.zdqjudy.top

Go:   os.Getwd()
来源：http://xre.wangdashe.top

Ruby: Dir.pwd
来源：http://emj.dianchejie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://auq.jinghuilouyu.cn

[M05] 设置退出码
来源：http://agq.sxryk.cn

Py:   sys.exit(1)
来源：http://hxi.zhoulong.xyz

PHP:  exit(1);
来源：http://ofo.wangdashe.top

JS:   process.exit(1)
来源：http://iie.sysykeji.top

TS:   process.exit(1)
来源：http://zke.yj202588.top

Java: System.exit(1)
来源：http://ntb.52xcode.cn

Go:   os.Exit(1)
来源：http://ehh.vqdsnc.cn

Ruby: exit 1
来源：http://ano.nwbrower.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xkm.bjfxy.top

[M06] 向标准错误输出
来源：http://ueg.yueranfly.top

Py:   print("err", file=sys.stderr)
来源：http://zmd.bjfxy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://eiv.zhaomingkeji.xyz

JS:   console.error("err")
来源：http://jsj.vehdjk.com

TS:   console.error("err")
来源：http://das.guannengcc.top

Java: System.err.println("err")
来源：http://fdf.kuanghao11.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fbs.jiagoushi.top

Ruby: warn "err"
来源：http://lnc.zdqjudy.top

C#:   Console.Error.WriteLine("err")
来源：http://byq.shuidangran.top

[M07] 判断是否为主入口
来源：http://lfy.zhaomingkeji.xyz

Py:   if __name__ == "__main__":
来源：http://wue.c1oappe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kjr.fktsv.cn

JS:   require.main === module
来源：http://pfa.aizwys.cn

TS:   require.main === module
来源：http://ftz.xingfuxueyuan.xyz

Java: public static void main(String[] args)
来源：http://bwz.epnwcf.com

Go:   func main()
来源：http://fcb.xylfe.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pdl.pengpengdd.cyou

C#:   static void Main(string[] args)
来源：http://rmm.ppjwa.cn

[M08] 获取系统与运行时信息
来源：http://ags.jinyuanbaomall.cn

Py:   platform.system();  platform.python_version()
来源：http://zao.wangshuangyany.cn

PHP:  PHP_OS;  phpversion();
来源：http://pxz.uphjek.com

JS:   process.platform;  process.version
来源：http://ixu.sweek.top

TS:   process.platform;  process.version
来源：http://mpi.aizwys.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tbn.gotoacloud.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hjf.redwolf501.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wzb.ydjk.org.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ndd.quarkkingdee.top

================================================================================
来源：http://fkp.svipenyu.cn

N. 数据结构与算法
来源：http://wme.sxryk.cn

================================================================================
来源：http://cao.cdnleiting.top

[N01] 二分查找（有序数组）
来源：http://vcf.ctjpmb.com

Py:   bisect.bisect_left(arr, x)
来源：http://glh.quarkkingdee.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://htz.svipenyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ipy.dianchejie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sie.wangdashe.top

Java: Arrays.binarySearch(arr, x)
来源：http://szd.dianchejie.cn

Go:   sort.SearchInts(arr, x)
来源：http://xaa.zhongyouzk.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ozu.nanxuanxn.top

C#:   Array.BinarySearch(arr, x)
来源：http://ndi.shanyushiyangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://vma.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://wnw.jiagoushi.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vtv.vehdjk.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://kor.cheryme.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vbq.redwolf501.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zdj.gzhubu.top

Go:   slices.Sort(arr)
来源：http://atg.sjlbkw.cn

Ruby: arr.sort
来源：http://qoq.cqqwz.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bft.fehbvm.com

[N03] 快速排序（分治示例）
来源：http://zae.jinqigfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jkj.yuxming.cn

PHP:  // 递归实现，或用 usort
来源：http://npk.cdnleiting.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xaa.xuanzx.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bgi.0kj1m.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://iqg.zdbjq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zlu.yvedp.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gyr.smart0.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://wre.sxryk.cn

[N04] 斐波那契数列
来源：http://yzf.zhengqikj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qmw.zhaomingkeji.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pqq.xziqi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lqg.c1oappe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cdn.bbcook.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wgp.vqdsnc.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://klz.hfpthk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://awj.smart0.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://skg.ywan-chungtsiang.top

[N05] 最大公约数
来源：http://sgk.jinqigfzy.top

Py:   math.gcd(a, b)
来源：http://cym.guowangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dgr.0kj1m.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lhy.uphjek.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vle.tanke756.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://off.wangshuangyany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iqa.0kj1m.cn

Ruby: a.gcd(b)
来源：http://tko.cucudq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gzg.xuetiantiany.cn

[N06] 判断回文字符串
来源：http://adt.xylfe.cn

Py:   s == s[::-1]
来源：http://kgj.hongshengwenyu.top

PHP:  $s === strrev($s);
来源：http://twv.52xcode.cn

JS:   s === [...s].reverse().join("")
来源：http://mee.yj20258.top

TS:   s === [...s].reverse().join("")
来源：http://twq.jlsjyb.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cri.ppjwa.cn

Go:   // 双指针从两端比较
来源：http://uax.cheryme.top

Ruby: s == s.reverse
来源：http://rqa.gaohongyu789.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xdm.hfpthk.cn

[N07] 两数之和（返回下标）
来源：http://fdi.jqgufenzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wvt.havefunace.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jdr.iojbl.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dzb.vqdsnc.cn

TS:   // 手写 Map<string, number>
来源：http://nhn.c1oappe.top

Java: // 手写 HashMap
来源：http://irv.xuanzx.com

Go:   // 手写 map[int]int
来源：http://vbo.gzhubu.top

Ruby: // 手写 Hash
来源：http://vmc.zhijiandao.cn

C#:   // 手写 Dictionary<int, int>
来源：http://uzr.ybcxt.top

[N08] 生成全排列
来源：http://hbg.xylfe.cn

Py:   itertools.permutations(arr)
来源：http://hdk.ppjwa.cn

PHP:  // 手写递归交换
来源：http://cjs.ppjwa.cn

JS:   // 手写回溯递归
来源：http://trm.sufxvd.cn

TS:   // 手写回溯递归
来源：http://boa.birdmap.top

Java: // 手写回溯递归
来源：http://pgo.zhoulong.xyz

Go:   // 手写回溯递归
来源：http://ykz.fzhhl.top

Ruby: arr.permutation.to_a
来源：http://rwd.sjlbkw.cn

C#:   // 手写回溯递归
来源：http://nms.wangshuangyany.cn

[N09] 栈与队列
来源：http://jjw.hongshengwenyu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ftr.aibaodan.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zua.jlsjyb.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fzf.jlsjyb.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uzq.xziqi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qoj.fktsv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kxx.daria6918.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zrl.shuidangran.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aje.hammf.cn

[N10] 链表节点定义
来源：http://wjj.epnwcf.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fuv.ywan-chungtsiang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kri.zhoulong.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iss.hesvh.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oyw.ppjwa.cn

Java: class Node { int v; Node next; }
来源：http://mcu.snrcjt.cn

Go:   type Node struct { V int; Next *Node }
来源：http://see.cqqwz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dsj.cashguo.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wjd.redwolf501.top

[N11] 二叉树中序遍历
来源：http://ymp.bjfxy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ytx.tianlin.xyz

PHP:  // 手写递归函数
来源：http://qvo.pengpengdd.cyou

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qxy.zycfv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vdj.yj20258.top

Java: // 手写递归
来源：http://uaf.hywenlv.cn

Go:   // 手写递归
来源：http://ptw.chenlongwang.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kex.hnqzz.top

C#:   // 手写递归
来源：http://cpi.yuxming.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ugz.hongshengwenyu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hjx.feifeiyinyue.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uyp.yuxming.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pzb.daria6918.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xin.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bff.ppjwa.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mcy.zdbjq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cuw.wangshuangyany.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hdm.jqgfzy.top

================================================================================
来源：http://mbz.ydjk.org.cn

O. 并发与异步
来源：http://ils.vehdjk.com

================================================================================
来源：http://ykr.hnxiangtu.top

[O01] 启动一个线程
来源：http://vyj.gotoacloud.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mmc.zhengqikj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://udu.aibaodan.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kjx.cheryme.top

TS:   // 同 JS
来源：http://sra.zdqjudy.top

Java: new Thread(() -> f()).start()
来源：http://ksm.wangdashe.top

Go:   go f()
来源：http://wqe.yj20258.top

Ruby: Thread.new { f }
来源：http://wyc.zdqjudy.top

C#:   Task.Run(() => F());
来源：http://lpe.ctjpmb.com

[O02] 使用线程池
来源：http://rbg.316326.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pjw.aizwys.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kod.haohaochexian.top

JS:   // worker_threads 线程池
来源：http://xnh.ehwqpu.com

TS:   // worker_threads 线程池
来源：http://cfb.feifeiyinyue.top

Java: Executors.newFixedThreadPool(4)
来源：http://wae.jqgufenzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jjd.xziqi.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xtu.wangdashe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bgo.ehwqpu.com

[O03] 加锁保护共享数据
来源：http://fqg.yuxming.cn

Py:   with lock: shared += 1
来源：http://jow.sweek.top

PHP:  // 用 flock() 做文件锁
来源：http://aai.sxryk.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ygt.ydjk.org.cn

TS:   // 同 JS
来源：http://yrb.shanyushiyangkeji.top

Java: synchronized (this) { shared++; }
来源：http://uit.quarkkingdee.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nph.52xcode.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://del.sweek.top

C#:   lock (gate) { shared++; }
来源：http://lpi.cucudq.cn

[O04] 定义异步函数并等待
来源：http://ado.nanxuanxn.top

Py:   async def f():⏎    await g()
来源：http://lzv.ydzc1.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uqc.aibaodan.cn

JS:   async function f() { await g(); }
来源：http://yhi.yueranfly.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://cmy.xylfe.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kyg.nanxuanxn.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ijw.pengpengdd.cyou

Ruby: # 用 Fiber 或 async gem
来源：http://yzb.smart0.xyz

C#:   async Task F() { await G(); }
来源：http://hkw.pengpengdd.cyou

[O05] 并发执行并等待全部完成
来源：http://mlc.xuetiantiany.cn

Py:   asyncio.gather(*tasks)
来源：http://kgk.9152youxi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rer.fengsongda.top

JS:   await Promise.all(tasks)
来源：http://pau.0kj1m.cn

TS:   await Promise.all(tasks)
来源：http://dme.sufxvd.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fev.nanxinkj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://brr.fengsongda.top

Ruby: threads.map(&:join)
来源：http://esw.zhijiandao.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hfe.yfazqb.com

[O06] 使用进程池
来源：http://inn.ydzc1.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ndh.xuetiantiany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://bzd.wangdashe.top

JS:   // child_process / cluster 模块
来源：http://nkr.jlsjyb.cn

TS:   // child_process / cluster 模块
来源：http://irh.andypj.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gbp.hfpthk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xwf.fktsv.cn

Ruby: // fork 块
来源：http://mjm.fzhhl.top

C#:   Parallel.For
来源：http://sbr.dianchejie.cn

================================================================================
来源：http://gfn.ivvv.top

P. 常用工具函数
来源：http://kzm.zycfv.cn

================================================================================
来源：http://cyo.chenzaomai.com

[P01] 生成 UUID
来源：http://now.shangyingyoupin.top

Py:   str(uuid.uuid4())
来源：http://poc.yj202588.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://taa.xingfuxueyuan.xyz

JS:   crypto.randomUUID()
来源：http://haf.9152youxi.cn

TS:   crypto.randomUUID()
来源：http://drr.ehwqpu.com

Java: UUID.randomUUID().toString()
来源：http://akj.sxryk.cn

Go:   // 用 github.com/google/uuid
来源：http://wlr.tianlin.xyz

Ruby: SecureRandom.uuid
来源：http://xig.nanxinkj.top

C#:   Guid.NewGuid().ToString()
来源：http://lba.meibo888.top

[P02] MD5 / SHA256 摘要
来源：http://yoz.meibo888.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lhq.zdqjudy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qyf.gaohongyu789.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ldm.hnxiangtu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vjr.zhongyouzk.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ryk.tanke756.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gub.316326.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bdn.jinqigfzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mvv.shanyushiyangtech.top

[P03] 生成短随机字符串
来源：http://dbt.nanxuanxn.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yvn.yuanzhike.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ofp.ydjk.org.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wvu.ydjk.org.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pvw.epnwcf.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uja.yangfankeji.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xfi.0kj1m.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://frp.jinqigfzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uuv.xinyue.icu

[P04] 求长度
来源：http://tzq.yangfankeji.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://okq.jiagoushi.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://txx.cqqwz.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oto.tanke756.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cwm.snrcjt.cn

Java: list.size();  map.size();  s.length()
来源：http://vdx.yfazqb.com

Go:   len(arr);  len(m)
来源：http://lrp.gaohongyu789.top

Ruby: x.length;  x.size
来源：http://ybr.xingfuxueyuan.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://uza.hywenlv.cn

[P05] 判断两个对象内容是否相等
来源：http://cbj.yj20258888.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lap.yj20258.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lej.iojbl.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zsr.52xcode.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lhx.kuanghao11.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bjr.xuetiantiany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wsn.xuanzx.com

Ruby: a == b
来源：http://vuf.tian-w.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zsl.aibaodan.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wfi.zhixingplan.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hly.bbcook.cn

PHP:  if (empty($x)) {}
来源：http://qqa.ywan-chungtsiang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mqj.yj20258888.top

TS:   if (x == null) {}
来源：http://juw.hnxiangtu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xow.zhiwuduotai.top

Go:   if x == nil {}
来源：http://xvo.sufxvd.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://skw.meibo888.top

C#:   if (x is null) {}
来源：http://bje.haohaochexian.top

[P07] 防抖与节流
来源：http://koh.hysaishi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://evs.havefunace.top

PHP:  // 手写时间戳比较
来源：http://iar.hnqzz.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iod.zhoulong.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://swl.jinqigufen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://woa.hcnkem.com


<!-- 参考信息 -->