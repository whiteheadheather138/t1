代发 wailian999

JS:   process.argv.slice(2)
来源：http://qdp.redwolf501.top

TS:   process.argv.slice(2)
来源：http://ejr.zhongyouzk.top

Java: args 数组（main 方法参数）
来源：http://glg.yongpay.top

Go:   os.Args[1:]
来源：http://ycy.zhoulong.xyz

Ruby: ARGV
来源：http://wnm.316326.xyz

C#:   args 数组（Main 方法参数）
来源：http://vpl.ywan-chungtsiang.top

[M02] 读取环境变量
来源：http://zdu.yanxiufei.cn

Py:   os.environ.get("HOME")
来源：http://sid.zhiwuduotai.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jex.iojbl.cn

JS:   process.env.HOME
来源：http://qls.dashuyun.cn

TS:   process.env.HOME
来源：http://jxk.quarkkingdee.top

Java: System.getenv("HOME")
来源：http://ssf.zdqjudy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nsn.xinyue.icu

Ruby: ENV["HOME"]
来源：http://xrj.xingfuxueyuan.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qff.daria6918.cn

[M03] 执行外部命令
来源：http://txn.svipenyu.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xoi.xingfuxueyuan.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sti.ppjwa.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qnz.wangdashe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://okk.316326.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uwu.daria6918.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://myk.zhengqikj.top

Ruby: system("ls -l");  `ls -l`
来源：http://lgi.nwbrower.top

C#:   Process.Start("ls", "-l");
来源：http://zcm.ctjpmb.com

[M04] 获取当前工作目录
来源：http://ljq.jqgfzy.top

Py:   os.getcwd()
来源：http://stj.sxryk.cn

PHP:  getcwd();
来源：http://gki.aibaodan.cn

JS:   process.cwd()
来源：http://ymw.hywenlv.cn

TS:   process.cwd()
来源：http://que.yj20258.top

Java: Path.of("").toAbsolutePath()
来源：http://rlr.jinqigufen.top

Go:   os.Getwd()
来源：http://nmr.fanxiaobao.xyz

Ruby: Dir.pwd
来源：http://fiz.xziqi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gsg.daxiang520.top

[M05] 设置退出码
来源：http://dsy.chenzaomai.com

Py:   sys.exit(1)
来源：http://leu.nanxinkj.top

PHP:  exit(1);
来源：http://fsr.birdmap.top

JS:   process.exit(1)
来源：http://uyt.xylfe.cn

TS:   process.exit(1)
来源：http://hqo.zhijiandao.cn

Java: System.exit(1)
来源：http://jpg.pengpengdd.cyou

Go:   os.Exit(1)
来源：http://eah.bbcook.cn

Ruby: exit 1
来源：http://tiu.shuidangran.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ncl.wangshuangyany.cn

[M06] 向标准错误输出
来源：http://ypc.zhaomingkeji.xyz

Py:   print("err", file=sys.stderr)
来源：http://azk.jinyuanbaomall.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xvh.fehbvm.com

JS:   console.error("err")
来源：http://ani.cheryme.top

TS:   console.error("err")
来源：http://cwj.cucudq.cn

Java: System.err.println("err")
来源：http://boj.fanxiaobao.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kpw.chenlongwang.top

Ruby: warn "err"
来源：http://xbw.chenlongwang.top

C#:   Console.Error.WriteLine("err")
来源：http://yec.xinyue.icu

[M07] 判断是否为主入口
来源：http://arl.dashuyun.cn

Py:   if __name__ == "__main__":
来源：http://waa.hnqzz.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tyf.jyoumei.cn

JS:   require.main === module
来源：http://oau.gotoacloud.top

TS:   require.main === module
来源：http://zae.yuxming.cn

Java: public static void main(String[] args)
来源：http://aeb.shzxlz.cn

Go:   func main()
来源：http://bbp.uphjek.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lpd.xuetiantiany.cn

C#:   static void Main(string[] args)
来源：http://qxr.wangshuangyany.cn

[M08] 获取系统与运行时信息
来源：http://dxp.chenzaomai.com

Py:   platform.system();  platform.python_version()
来源：http://jqf.fehbvm.com

PHP:  PHP_OS;  phpversion();
来源：http://mnt.zhiwuduotai.top

JS:   process.platform;  process.version
来源：http://mpw.shangyingyoupin.top

TS:   process.platform;  process.version
来源：http://drc.yj20258.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://elq.yvedp.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://blv.tanke756.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pbs.jinyuanbaomall.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jqn.ivvv.top

================================================================================
来源：http://ixv.chenlongwang.top

N. 数据结构与算法
来源：http://sjn.gogol.net.cn

================================================================================
来源：http://cfs.gzhubu.top

[N01] 二分查找（有序数组）
来源：http://aoq.cheryme.top

Py:   bisect.bisect_left(arr, x)
来源：http://nna.yueranfly.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://flh.zhijiandao.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ykw.aibaodan.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jvs.jlsjyb.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nvz.shangyingyoupin.top

Go:   sort.SearchInts(arr, x)
来源：http://hol.chenzaomai.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://kbo.chenjidiqi.icu

C#:   Array.BinarySearch(arr, x)
来源：http://hhc.chenzaomai.com

[N02] 排序（工程实践用内置实现）
来源：http://kiz.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://yfc.zycfv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cun.hesvh.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ltc.mhx1999.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ras.fktsv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ruc.yj20258888.top

Go:   slices.Sort(arr)
来源：http://ptn.xuetiantiany.cn

Ruby: arr.sort
来源：http://hxp.ehwqpu.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://dan.fehbvm.com

[N03] 快速排序（分治示例）
来源：http://vus.yj202588.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pwp.yj20258888.top

PHP:  // 递归实现，或用 usort
来源：http://hwt.yangfankeji.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eto.shuidangran.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hgp.smart0.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ibl.jinghuilouyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ood.snrcjt.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cju.haohaochexian.top

C#:   // 手写递归，或 Array.Sort
来源：http://btf.feifeiyinyue.top

[N04] 斐波那契数列
来源：http://qwd.yuanzhike.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xvb.dashuyun.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tbk.redwolf501.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://naw.pengpengdd.cyou

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jkp.tian-w.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nwi.cqqwz.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zgj.chenjidiqi.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wqx.uphjek.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://run.zhoulong.xyz

[N05] 最大公约数
来源：http://seb.zycfv.cn

Py:   math.gcd(a, b)
来源：http://lnq.kuanghao11.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xex.ivvv.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jhx.quarkkingdee.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xoe.xuetiantiany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nwc.svipenyu.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mcu.yj20258.top

Ruby: a.gcd(b)
来源：http://dbp.snrcjt.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://asn.cucudq.cn

[N06] 判断回文字符串
来源：http://uhw.xuanzx.com

Py:   s == s[::-1]
来源：http://yla.yuxming.cn

PHP:  $s === strrev($s);
来源：http://ldj.xylfe.cn

JS:   s === [...s].reverse().join("")
来源：http://yfd.yuxming.cn

TS:   s === [...s].reverse().join("")
来源：http://dvm.dianchejie.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gjn.ehwqpu.com

Go:   // 双指针从两端比较
来源：http://kvi.jqgfzy.top

Ruby: s == s.reverse
来源：http://gck.52xcode.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ypo.fktsv.cn

[N07] 两数之和（返回下标）
来源：http://ulw.gzhubu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hgg.dashuyun.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cor.zhengqikj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://cwc.ybcxt.top

TS:   // 手写 Map<string, number>
来源：http://dbc.tanke756.top

Java: // 手写 HashMap
来源：http://byr.nanxuanxn.top

Go:   // 手写 map[int]int
来源：http://jvg.fzhhl.top

Ruby: // 手写 Hash
来源：http://bzx.haohaochexian.top

C#:   // 手写 Dictionary<int, int>
来源：http://imh.jinyuanbaomall.cn

[N08] 生成全排列
来源：http://tvm.iojbl.cn

Py:   itertools.permutations(arr)
来源：http://aii.yj20258.top

PHP:  // 手写递归交换
来源：http://egj.sweek.top

JS:   // 手写回溯递归
来源：http://thk.zhaomingkeji.xyz

TS:   // 手写回溯递归
来源：http://chs.cheryme.top

Java: // 手写回溯递归
来源：http://aba.hnxiangtu.top

Go:   // 手写回溯递归
来源：http://gzn.zhijiandao.cn

Ruby: arr.permutation.to_a
来源：http://ynf.dashuyun.cn

C#:   // 手写回溯递归
来源：http://fkw.yfazqb.com

[N09] 栈与队列
来源：http://rnu.pycfn.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uvx.xylfe.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jsa.jyoumei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://umr.nanxinkj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fkv.pengpengdd.cyou

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://stf.quarkkingdee.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kos.zhiwuduotai.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ylb.hcnkem.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://niw.shangyingyoupin.top

[N10] 链表节点定义
来源：http://uen.cucudq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vee.bbcook.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://hzd.yonumen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://amm.ybcxt.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rbh.chenjidiqi.icu

Java: class Node { int v; Node next; }
来源：http://fyr.epnwcf.com

Go:   type Node struct { V int; Next *Node }
来源：http://mew.sweek.top

Ruby: Node = Struct.new(:v, :next)
来源：http://foh.jqgfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://arj.pengpengdd.cyou

[N11] 二叉树中序遍历
来源：http://uvl.gotoacloud.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aeb.cucudq.cn

PHP:  // 手写递归函数
来源：http://oen.xinyue.icu

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tza.meibo888.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ryc.hnxiangtu.top

Java: // 手写递归
来源：http://nej.cdnleiting.top

Go:   // 手写递归
来源：http://dxj.jinqigfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qqh.pengpengdd.cyou

C#:   // 手写递归
来源：http://rwm.jyoumei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pox.cdnleiting.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jwn.c1oappe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qkf.zhixingplan.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ali.shangyingyoupin.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qvn.xuanzx.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ovf.yonumen.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://voq.sysykeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gla.wangdashe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yke.jinghuilouyu.cn

================================================================================
来源：http://hqb.hongshengwenyu.top

O. 并发与异步
来源：http://gqs.quarkkingdee.top

================================================================================
来源：http://gde.xingfuxueyuan.xyz

[O01] 启动一个线程
来源：http://pql.xylfe.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rzh.sweek.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://foo.aizwys.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lew.fengsongda.top

TS:   // 同 JS
来源：http://jfh.zhoulong.xyz

Java: new Thread(() -> f()).start()
来源：http://mbj.jinyuanbaomall.cn

Go:   go f()
来源：http://qbc.daxiang520.top

Ruby: Thread.new { f }
来源：http://zxr.wangdashe.top

C#:   Task.Run(() => F());
来源：http://swn.epnwcf.com

[O02] 使用线程池
来源：http://lqd.nanxuanxn.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lhf.hysaishi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://amd.yueranfly.top

JS:   // worker_threads 线程池
来源：http://ooo.guannengcc.top

TS:   // worker_threads 线程池
来源：http://tvg.hfpthk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://apf.bjfxy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mxj.gaohongyu789.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.gaohongyu789.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ber.ydzc1.top

[O03] 加锁保护共享数据
来源：http://lsh.jyoumei.cn

Py:   with lock: shared += 1
来源：http://wdz.yuxming.cn

PHP:  // 用 flock() 做文件锁
来源：http://kcd.kuanghao11.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uge.zhijiandao.cn

TS:   // 同 JS
来源：http://ind.hysaishi.cn

Java: synchronized (this) { shared++; }
来源：http://din.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rbo.sufxvd.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://meg.zdqjudy.top

C#:   lock (gate) { shared++; }
来源：http://kzh.chenzaomai.com

[O04] 定义异步函数并等待
来源：http://vjd.yanxiufei.cn

Py:   async def f():⏎    await g()
来源：http://yds.bbcook.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pls.gaohongyu789.top

JS:   async function f() { await g(); }
来源：http://eaa.guowangkeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://fvv.hcnkem.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fcc.birdmap.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fzs.hcnkem.com

Ruby: # 用 Fiber 或 async gem
来源：http://cee.jqgufenzy.top

C#:   async Task F() { await G(); }
来源：http://xqq.fengsongda.top

[O05] 并发执行并等待全部完成
来源：http://lxh.haohaochexian.top

Py:   asyncio.gather(*tasks)
来源：http://gsn.jiagoushi.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nki.xingfuxueyuan.xyz

JS:   await Promise.all(tasks)
来源：http://oyj.yj20258888.top

TS:   await Promise.all(tasks)
来源：http://rwu.shanyushiyangtech.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rog.yvedp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sxv.wangshuangyany.cn

Ruby: threads.map(&:join)
来源：http://wtz.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://all.cheryme.top

[O06] 使用进程池
来源：http://ajj.zhaomingkeji.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tjh.guannengcc.top

PHP:  // pcntl_fork 或多进程队列
来源：http://tgd.dashuyun.cn

JS:   // child_process / cluster 模块
来源：http://yhq.xuetiantiany.cn

TS:   // child_process / cluster 模块
来源：http://frt.shangyingyoupin.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mhm.zhijiandao.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oim.fengsongda.top

Ruby: // fork 块
来源：http://slh.svipenyu.cn

C#:   Parallel.For
来源：http://gtu.hysaishi.cn

================================================================================
来源：http://cfp.guannengcc.top

P. 常用工具函数
来源：http://ome.ydjk.org.cn

================================================================================
来源：http://dll.bjfxy.top

[P01] 生成 UUID
来源：http://evf.yangfankeji.com

Py:   str(uuid.uuid4())
来源：http://wxi.bjfxy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lsd.jlsjyb.cn

JS:   crypto.randomUUID()
来源：http://yfr.quarkkingdee.top

TS:   crypto.randomUUID()
来源：http://cpc.tanke756.top

Java: UUID.randomUUID().toString()
来源：http://ybm.zhoulong.xyz

Go:   // 用 github.com/google/uuid
来源：http://ctq.guowangkeji.top

Ruby: SecureRandom.uuid
来源：http://kdb.ywan-chungtsiang.top

C#:   Guid.NewGuid().ToString()
来源：http://tgy.yongpay.top

[P02] MD5 / SHA256 摘要
来源：http://klk.nwbrower.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hpa.yuxming.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nvi.guannengcc.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ctq.jianghu66.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fkn.ctjpmb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uqn.xziqi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gdb.xylfe.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sma.xingfuxueyuan.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qne.jiagoushi.top

[P03] 生成短随机字符串
来源：http://qfp.redwolf501.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zpy.316326.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tbi.shzxlz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lih.jianghu66.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ulu.fzhhl.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mcg.wangshuangyany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mfe.snrcjt.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mjp.jiagoushi.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://aek.9152youxi.cn

[P04] 求长度
来源：http://gas.nanxinkj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tvb.mhx1999.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pdo.ppjwa.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cnl.zhijiandao.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iij.ywan-chungtsiang.top

Java: list.size();  map.size();  s.length()
来源：http://tsr.yangfankeji.com

Go:   len(arr);  len(m)
来源：http://ulh.tarul.cn

Ruby: x.length;  x.size
来源：http://nkd.sysykeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ycg.xingfuxueyuan.xyz

[P05] 判断两个对象内容是否相等
来源：http://asr.hysaishi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uvm.yj20258.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xjv.cqqwz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://adh.bbcook.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xtf.aibaodan.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://feb.9152youxi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tmh.quarkkingdee.top

Ruby: a == b
来源：http://eun.ybcxt.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lur.nanxuanxn.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vdj.hfpthk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tgg.jqgufenzy.top

PHP:  if (empty($x)) {}
来源：http://yzh.ydzc1.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uuy.birdmap.top

TS:   if (x == null) {}
来源：http://mad.fehbvm.com

Java: if (x == null || x.isEmpty()) {}
来源：http://kli.zhaomingkeji.xyz

Go:   if x == nil {}
来源：http://spr.yonumen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cmk.hongshengwenyu.top

C#:   if (x is null) {}
来源：http://zmz.9152youxi.cn

[P07] 防抖与节流
来源：http://mef.yuxming.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pdh.andypj.xyz

PHP:  // 手写时间戳比较
来源：http://lgj.ctjpmb.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://map.daxiang520.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pvr.tanke756.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wla.fehbvm.com


<!-- 参考信息 -->