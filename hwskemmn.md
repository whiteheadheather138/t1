代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://omb.svipenyu.cn

JS:   process.env.HOME
来源：http://bsl.wangshuangyany.cn

TS:   process.env.HOME
来源：http://dqa.ywan-chungtsiang.top

Java: System.getenv("HOME")
来源：http://dpw.xylfe.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nez.yj20258888.top

Ruby: ENV["HOME"]
来源：http://knt.xuanzx.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lrq.xinyue.icu

[M03] 执行外部命令
来源：http://nap.epnwcf.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wnn.aibaodan.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kwd.sjlbkw.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ahs.haohaochexian.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ydm.dashuyun.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gpx.fehbvm.com

Go:   exec.Command("ls", "-l").Output()
来源：http://drc.tarul.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qsx.haohaochexian.top

C#:   Process.Start("ls", "-l");
来源：http://gvx.daria6918.cn

[M04] 获取当前工作目录
来源：http://oqz.jinqigfzy.top

Py:   os.getcwd()
来源：http://eqe.bjfxy.top

PHP:  getcwd();
来源：http://orb.ydzc1.top

JS:   process.cwd()
来源：http://qtd.sysykeji.top

TS:   process.cwd()
来源：http://vbw.jinyuanbaomall.cn

Java: Path.of("").toAbsolutePath()
来源：http://mwg.ehwqpu.com

Go:   os.Getwd()
来源：http://jcs.0kj1m.cn

Ruby: Dir.pwd
来源：http://odo.smart0.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://wwe.tanke756.top

[M05] 设置退出码
来源：http://kuc.shuidangran.top

Py:   sys.exit(1)
来源：http://qts.tian-w.cn

PHP:  exit(1);
来源：http://tfn.epnwcf.com

JS:   process.exit(1)
来源：http://grv.jlsjyb.cn

TS:   process.exit(1)
来源：http://ubo.fzhhl.top

Java: System.exit(1)
来源：http://lme.9152youxi.cn

Go:   os.Exit(1)
来源：http://eub.xingfuxueyuan.xyz

Ruby: exit 1
来源：http://ndf.yj20258.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ppb.gaohongyu789.top

[M06] 向标准错误输出
来源：http://zmr.yangfankeji.com

Py:   print("err", file=sys.stderr)
来源：http://utt.zycfv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cnw.jinghuilouyu.cn

JS:   console.error("err")
来源：http://fas.jqgufenzy.top

TS:   console.error("err")
来源：http://cvr.yfazqb.com

Java: System.err.println("err")
来源：http://msh.daxiang520.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zih.gogol.net.cn

Ruby: warn "err"
来源：http://nqe.sxryk.cn

C#:   Console.Error.WriteLine("err")
来源：http://gbm.hnxiangtu.top

[M07] 判断是否为主入口
来源：http://ohv.c1oappe.top

Py:   if __name__ == "__main__":
来源：http://qyb.hysaishi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://klc.316326.xyz

JS:   require.main === module
来源：http://bpf.c1oappe.top

TS:   require.main === module
来源：http://rqe.zdqjudy.top

Java: public static void main(String[] args)
来源：http://atq.gaohongyu789.top

Go:   func main()
来源：http://uew.yj202588.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jzx.tanke756.top

C#:   static void Main(string[] args)
来源：http://knn.zhixingplan.top

[M08] 获取系统与运行时信息
来源：http://xsy.yanxiufei.cn

Py:   platform.system();  platform.python_version()
来源：http://pnn.birdmap.top

PHP:  PHP_OS;  phpversion();
来源：http://gaw.xuetiantiany.cn

JS:   process.platform;  process.version
来源：http://avc.yanxiufei.cn

TS:   process.platform;  process.version
来源：http://mdi.yonumen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xic.bjfxy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://own.dianchejie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tvr.pengpengdd.cyou

C#:   Environment.OSVersion;  Environment.Version
来源：http://qrp.gotoacloud.top

================================================================================
来源：http://jmk.wangdashe.top

N. 数据结构与算法
来源：http://rhw.zdbjq.cn

================================================================================
来源：http://jrn.vqdsnc.cn

[N01] 二分查找（有序数组）
来源：http://bpc.mhx1999.top

Py:   bisect.bisect_left(arr, x)
来源：http://vfm.xinyue.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qbp.sjlbkw.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pjo.feifeiyinyue.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://osy.tarul.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wxy.daria6918.cn

Go:   sort.SearchInts(arr, x)
来源：http://xmf.wangshuangyany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://efd.gogol.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://eol.tarul.cn

[N02] 排序（工程实践用内置实现）
来源：http://llf.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://jci.jinghuilouyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mth.sjlbkw.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sbx.gogol.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://trp.dashuyun.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://doy.yuxming.cn

Go:   slices.Sort(arr)
来源：http://lmv.gzhubu.top

Ruby: arr.sort
来源：http://jkt.gaohongyu789.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mcr.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://skb.fzhhl.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bun.tianlin.xyz

PHP:  // 递归实现，或用 usort
来源：http://apc.hammf.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://osg.cqqwz.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gza.wangshuangyany.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hts.gogol.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fnu.cqqwz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://whk.jinqigufen.top

C#:   // 手写递归，或 Array.Sort
来源：http://rsl.snrcjt.cn

[N04] 斐波那契数列
来源：http://uar.hongshengwenyu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ofn.sufxvd.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://odp.shzxlz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fmk.52xcode.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qbp.52xcode.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fgq.shuidangran.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hwu.gaohongyu789.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://whj.birdmap.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qkp.ppjwa.cn

[N05] 最大公约数
来源：http://jes.jqgfzy.top

Py:   math.gcd(a, b)
来源：http://prx.ydjk.org.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hcu.zhongyouzk.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dwe.nanxinkj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xbt.xinyue.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ftj.chenjidiqi.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://knz.vehdjk.com

Ruby: a.gcd(b)
来源：http://ouz.ybcxt.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dbj.pengpengdd.cyou

[N06] 判断回文字符串
来源：http://xuv.aizwys.cn

Py:   s == s[::-1]
来源：http://lmy.zhiwuduotai.top

PHP:  $s === strrev($s);
来源：http://vsn.ctjpmb.com

JS:   s === [...s].reverse().join("")
来源：http://yzv.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://sci.jianghu66.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bvh.tarul.cn

Go:   // 双指针从两端比较
来源：http://sfn.feifeiyinyue.top

Ruby: s == s.reverse
来源：http://zdp.mhx1999.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://exp.sxryk.cn

[N07] 两数之和（返回下标）
来源：http://sra.tarul.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jdb.zhoulong.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iwn.jqgfzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://uxk.gaohongyu789.top

TS:   // 手写 Map<string, number>
来源：http://pbi.hammf.cn

Java: // 手写 HashMap
来源：http://oze.nwbrower.top

Go:   // 手写 map[int]int
来源：http://mwp.yj202588.top

Ruby: // 手写 Hash
来源：http://myv.shangyingyoupin.top

C#:   // 手写 Dictionary<int, int>
来源：http://tdw.jyoumei.cn

[N08] 生成全排列
来源：http://sbk.yueranfly.top

Py:   itertools.permutations(arr)
来源：http://mwf.birdmap.top

PHP:  // 手写递归交换
来源：http://umf.ivvv.top

JS:   // 手写回溯递归
来源：http://uam.yj20258.top

TS:   // 手写回溯递归
来源：http://bpy.zycfv.cn

Java: // 手写回溯递归
来源：http://scm.jqgfzy.top

Go:   // 手写回溯递归
来源：http://adn.fanxiaobao.xyz

Ruby: arr.permutation.to_a
来源：http://ewl.c1oappe.top

C#:   // 手写回溯递归
来源：http://lfs.dianchejie.cn

[N09] 栈与队列
来源：http://uhn.andypj.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yzc.haohaochexian.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xjz.ppjwa.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ehi.zdbjq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://arz.dashuyun.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qlf.epnwcf.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dyk.guowangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rlb.yvedp.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pax.shanyushiyangtech.top

[N10] 链表节点定义
来源：http://jdw.shangyingyoupin.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://csa.cqqwz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xip.xingfuxueyuan.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fhf.yvedp.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bxo.jqgfzy.top

Java: class Node { int v; Node next; }
来源：http://hel.fzhhl.top

Go:   type Node struct { V int; Next *Node }
来源：http://iqz.ydjk.org.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://uhq.cqqwz.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dhs.xylfe.cn

[N11] 二叉树中序遍历
来源：http://ddm.feifeiyinyue.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yvp.jianghu66.top

PHP:  // 手写递归函数
来源：http://ekv.mhx1999.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ihr.nwbrower.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lat.jianghu66.top

Java: // 手写递归
来源：http://zgv.ybcxt.top

Go:   // 手写递归
来源：http://ffb.yuxming.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dai.epnwcf.com

C#:   // 手写递归
来源：http://xub.zhoulong.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kdb.yj20258.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zrq.cdnleiting.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rof.yonumen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oid.andypj.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tyu.nanxuanxn.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://och.yfazqb.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://czc.yj20258888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cmh.fehbvm.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rko.chenzaomai.com

================================================================================
来源：http://puw.gaohongyu789.top

O. 并发与异步
来源：http://tut.ywan-chungtsiang.top

================================================================================
来源：http://vvw.guowangkeji.top

[O01] 启动一个线程
来源：http://upg.meibo888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ype.birdmap.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wsi.gogol.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fcx.cashguo.top

TS:   // 同 JS
来源：http://krw.yuanzhike.top

Java: new Thread(() -> f()).start()
来源：http://han.yuanzhike.top

Go:   go f()
来源：http://fzq.jqgufenzy.top

Ruby: Thread.new { f }
来源：http://ioo.svipenyu.cn

C#:   Task.Run(() => F());
来源：http://hdn.ydjk.org.cn

[O02] 使用线程池
来源：http://hoc.hywenlv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cql.zhengqikj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jfq.zycfv.cn

JS:   // worker_threads 线程池
来源：http://hbu.yj20258.top

TS:   // worker_threads 线程池
来源：http://mid.fzhhl.top

Java: Executors.newFixedThreadPool(4)
来源：http://tqj.fzhhl.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://duu.svipenyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iwy.zhoulong.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://las.sysykeji.top

[O03] 加锁保护共享数据
来源：http://qig.yanxiufei.cn

Py:   with lock: shared += 1
来源：http://eag.yuxming.cn

PHP:  // 用 flock() 做文件锁
来源：http://uvv.pycfn.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jlk.yvedp.cn

TS:   // 同 JS
来源：http://hbw.jinghuilouyu.cn

Java: synchronized (this) { shared++; }
来源：http://hpt.hywenlv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hsj.0kj1m.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://beu.hywenlv.cn

C#:   lock (gate) { shared++; }
来源：http://vwr.chenlongwang.top

[O04] 定义异步函数并等待
来源：http://amu.zhongyouzk.top

Py:   async def f():⏎    await g()
来源：http://cxr.havefunace.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://esw.fanxiaobao.xyz

JS:   async function f() { await g(); }
来源：http://aod.tianlin.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://nat.jinqigfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wnn.xylfe.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rtl.shzxlz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lbj.yj20258.top

C#:   async Task F() { await G(); }
来源：http://oxu.chenzaomai.com

[O05] 并发执行并等待全部完成
来源：http://zpb.ppjwa.cn

Py:   asyncio.gather(*tasks)
来源：http://hyb.haohaochexian.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://quj.hfpthk.cn

JS:   await Promise.all(tasks)
来源：http://flo.bbcook.cn

TS:   await Promise.all(tasks)
来源：http://cfp.zycfv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ekk.jlsjyb.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pmh.shanyushiyangkeji.top

Ruby: threads.map(&:join)
来源：http://vsa.sweek.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qkk.guowangkeji.top

[O06] 使用进程池
来源：http://qcd.yuxming.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vkc.tarul.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fje.ydzc1.top

JS:   // child_process / cluster 模块
来源：http://fxa.fktsv.cn

TS:   // child_process / cluster 模块
来源：http://uwm.cqqwz.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zuo.jqgfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ooa.yj20258888.top

Ruby: // fork 块
来源：http://svg.zycfv.cn

C#:   Parallel.For
来源：http://nha.bbcook.cn

================================================================================
来源：http://xhx.ppjwa.cn

P. 常用工具函数
来源：http://gdz.mhx1999.top

================================================================================
来源：http://gac.shzxlz.cn

[P01] 生成 UUID
来源：http://yjf.zhiwuduotai.top

Py:   str(uuid.uuid4())
来源：http://hbs.zhoulong.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wth.pengpengdd.cyou

JS:   crypto.randomUUID()
来源：http://gdx.hfpthk.cn

TS:   crypto.randomUUID()
来源：http://eic.gogol.net.cn

Java: UUID.randomUUID().toString()
来源：http://iqo.yuanzhike.top

Go:   // 用 github.com/google/uuid
来源：http://zdp.vqdsnc.cn

Ruby: SecureRandom.uuid
来源：http://sjc.iojbl.cn

C#:   Guid.NewGuid().ToString()
来源：http://nta.redwolf501.top

[P02] MD5 / SHA256 摘要
来源：http://klk.vehdjk.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://upp.zhengqikj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://aqs.andypj.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nhw.epnwcf.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yup.9152youxi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nwc.fengsongda.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://apt.nanxinkj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://aut.tianlin.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bzi.shuidangran.top

[P03] 生成短随机字符串
来源：http://svs.dianchejie.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hob.shzxlz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://brg.wangshuangyany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://opo.c1oappe.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aiu.bjfxy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://btw.cucudq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rdb.shzxlz.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yxr.sxryk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fau.smart0.xyz

[P04] 求长度
来源：http://ror.yj20258.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iez.pycfn.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://opm.zdbjq.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://djq.ydzc1.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zrr.zycfv.cn

Java: list.size();  map.size();  s.length()
来源：http://lwj.xingfuxueyuan.xyz

Go:   len(arr);  len(m)
来源：http://wuv.jqgufenzy.top

Ruby: x.length;  x.size
来源：http://iun.sysykeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vyz.0kj1m.cn

[P05] 判断两个对象内容是否相等
来源：http://xjy.iojbl.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vqv.sufxvd.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://icx.gogol.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rci.fehbvm.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zjo.zdbjq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ajx.xylfe.cn

Go:   reflect.DeepEqual(a, b)
来源：http://unm.shuidangran.top

Ruby: a == b
来源：http://ste.vqdsnc.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ggl.yj20258.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gce.vqdsnc.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mzr.hammf.cn

PHP:  if (empty($x)) {}
来源：http://bdq.andypj.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://imz.chenjidiqi.icu

TS:   if (x == null) {}
来源：http://jww.yongpay.top

Java: if (x == null || x.isEmpty()) {}
来源：http://evw.zhijiandao.cn

Go:   if x == nil {}
来源：http://zfy.zhixingplan.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lbi.jyoumei.cn

C#:   if (x is null) {}
来源：http://otu.cheryme.top

[P07] 防抖与节流
来源：http://rzu.zhixingplan.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rlh.kuanghao11.cn

PHP:  // 手写时间戳比较
来源：http://fyi.xinyue.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cdi.daxiang520.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ghe.zhiwuduotai.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hla.nanxuanxn.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vjx.jqgfzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ddb.daria6918.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://laf.daria6918.cn

[P08] 处理浮点精度问题
来源：http://qqj.yueranfly.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://epe.sjlbkw.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ecu.ydjk.org.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rkg.birdmap.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fds.svipenyu.cn


<!-- 参考信息 -->