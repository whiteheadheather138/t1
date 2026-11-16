代发 wailian999

JS:   process.argv.slice(2)
来源：http://lwo.redwolf501.top

TS:   process.argv.slice(2)
来源：http://tlc.bbcook.cn

Java: args 数组（main 方法参数）
来源：http://fzw.gzhubu.top

Go:   os.Args[1:]
来源：http://doy.fktsv.cn

Ruby: ARGV
来源：http://smw.zdqjudy.top

C#:   args 数组（Main 方法参数）
来源：http://llm.yonumen.top

[M02] 读取环境变量
来源：http://cwa.shangyingyoupin.top

Py:   os.environ.get("HOME")
来源：http://shh.dashuyun.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://utt.wangdashe.top

JS:   process.env.HOME
来源：http://hdm.ehwqpu.com

TS:   process.env.HOME
来源：http://zyq.xziqi.cn

Java: System.getenv("HOME")
来源：http://xta.epnwcf.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://noe.cashguo.top

Ruby: ENV["HOME"]
来源：http://erc.vqdsnc.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bjl.uphjek.com

[M03] 执行外部命令
来源：http://vhl.hongshengwenyu.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ciy.nwbrower.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nxi.bjfxy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://oty.gotoacloud.top

TS:   child_process.execSync("ls -l").toString()
来源：http://zuq.yuxming.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mie.hysaishi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://kth.shuidangran.top

Ruby: system("ls -l");  `ls -l`
来源：http://utn.shangyingyoupin.top

C#:   Process.Start("ls", "-l");
来源：http://kud.nwbrower.top

[M04] 获取当前工作目录
来源：http://rms.xuanzx.com

Py:   os.getcwd()
来源：http://scg.aizwys.cn

PHP:  getcwd();
来源：http://jvp.nwbrower.top

JS:   process.cwd()
来源：http://ham.iojbl.cn

TS:   process.cwd()
来源：http://cjp.pycfn.com

Java: Path.of("").toAbsolutePath()
来源：http://ofv.yonumen.top

Go:   os.Getwd()
来源：http://ika.yfazqb.com

Ruby: Dir.pwd
来源：http://dpb.havefunace.top

C#:   Directory.GetCurrentDirectory()
来源：http://lrd.wangshuangyany.cn

[M05] 设置退出码
来源：http://pty.birdmap.top

Py:   sys.exit(1)
来源：http://wmq.yongpay.top

PHP:  exit(1);
来源：http://sfv.daria6918.cn

JS:   process.exit(1)
来源：http://joa.ehwqpu.com

TS:   process.exit(1)
来源：http://ecg.xuanzx.com

Java: System.exit(1)
来源：http://bxd.iojbl.cn

Go:   os.Exit(1)
来源：http://lzj.zhijiandao.cn

Ruby: exit 1
来源：http://wng.ywan-chungtsiang.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sot.jyoumei.cn

[M06] 向标准错误输出
来源：http://med.fengsongda.top

Py:   print("err", file=sys.stderr)
来源：http://kuu.tarul.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://guu.shanyushiyangtech.top

JS:   console.error("err")
来源：http://ria.52xcode.cn

TS:   console.error("err")
来源：http://ufn.bbcook.cn

Java: System.err.println("err")
来源：http://hgm.ydzc1.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zwd.pycfn.com

Ruby: warn "err"
来源：http://qbe.zhijiandao.cn

C#:   Console.Error.WriteLine("err")
来源：http://puu.haohaochexian.top

[M07] 判断是否为主入口
来源：http://uol.ydjk.org.cn

Py:   if __name__ == "__main__":
来源：http://snl.haohaochexian.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://umr.zhoulong.xyz

JS:   require.main === module
来源：http://smv.ivvv.top

TS:   require.main === module
来源：http://kjs.yuanzhike.top

Java: public static void main(String[] args)
来源：http://ntv.zdqjudy.top

Go:   func main()
来源：http://bie.kuanghao11.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bfe.yfazqb.com

C#:   static void Main(string[] args)
来源：http://ets.shangyingyoupin.top

[M08] 获取系统与运行时信息
来源：http://uup.sjlbkw.cn

Py:   platform.system();  platform.python_version()
来源：http://otf.chenlongwang.top

PHP:  PHP_OS;  phpversion();
来源：http://bqc.0kj1m.cn

JS:   process.platform;  process.version
来源：http://pro.gzhubu.top

TS:   process.platform;  process.version
来源：http://hev.sjlbkw.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://diz.yongpay.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://clx.hywenlv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rzt.sjlbkw.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hwg.jinyuanbaomall.cn

================================================================================
来源：http://sth.bjfxy.top

N. 数据结构与算法
来源：http://eng.sweek.top

================================================================================
来源：http://dba.shangyingyoupin.top

[N01] 二分查找（有序数组）
来源：http://fnu.zhongyouzk.top

Py:   bisect.bisect_left(arr, x)
来源：http://nke.316326.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vnd.jiagoushi.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sya.zhengqikj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ocz.ppjwa.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pfu.hnqzz.top

Go:   sort.SearchInts(arr, x)
来源：http://cfk.pengpengdd.cyou

Ruby: arr.bsearch { |e| e >= x }
来源：http://eeh.vqdsnc.cn

C#:   Array.BinarySearch(arr, x)
来源：http://eis.sweek.top

[N02] 排序（工程实践用内置实现）
来源：http://cak.wangdashe.top

Py:   sorted(arr);  arr.sort()
来源：http://hjs.jlsjyb.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zok.mhx1999.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jwe.ppjwa.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tif.tarul.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nzt.zhongyouzk.top

Go:   slices.Sort(arr)
来源：http://zvq.ydzc1.top

Ruby: arr.sort
来源：http://iel.iojbl.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pbx.cqqwz.cn

[N03] 快速排序（分治示例）
来源：http://fva.xylfe.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://czw.zdqjudy.top

PHP:  // 递归实现，或用 usort
来源：http://rqz.hnqzz.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kop.wangshuangyany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fhi.yonumen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://msv.hcnkem.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jri.yanxiufei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lid.snrcjt.cn

C#:   // 手写递归，或 Array.Sort
来源：http://knp.jinyuanbaomall.cn

[N04] 斐波那契数列
来源：http://vsz.smart0.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rmr.hfpthk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eqi.bjfxy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wwe.wangdashe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ino.sysykeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oll.mhx1999.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://unv.fzhhl.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zqw.yuanzhike.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sgd.aibaodan.cn

[N05] 最大公约数
来源：http://jdu.guannengcc.top

Py:   math.gcd(a, b)
来源：http://rxb.yonumen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zoq.zdqjudy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uqk.xuanzx.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yuj.yongpay.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kxu.xuetiantiany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dtj.fanxiaobao.xyz

Ruby: a.gcd(b)
来源：http://opm.tarul.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://anv.cashguo.top

[N06] 判断回文字符串
来源：http://uhd.smart0.xyz

Py:   s == s[::-1]
来源：http://rxb.xuanzx.com

PHP:  $s === strrev($s);
来源：http://ocz.yonumen.top

JS:   s === [...s].reverse().join("")
来源：http://jsm.sweek.top

TS:   s === [...s].reverse().join("")
来源：http://ihl.jqgfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ffi.cheryme.top

Go:   // 双指针从两端比较
来源：http://tsq.epnwcf.com

Ruby: s == s.reverse
来源：http://jmn.jianghu66.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vbb.haohaochexian.top

[N07] 两数之和（返回下标）
来源：http://vew.hywenlv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qyo.ppjwa.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hrq.jinqigufen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nys.yfazqb.com

TS:   // 手写 Map<string, number>
来源：http://lvo.hcnkem.com

Java: // 手写 HashMap
来源：http://ley.zhixingplan.top

Go:   // 手写 map[int]int
来源：http://xjg.zhiwuduotai.top

Ruby: // 手写 Hash
来源：http://isz.nwbrower.top

C#:   // 手写 Dictionary<int, int>
来源：http://yru.sxryk.cn

[N08] 生成全排列
来源：http://smx.dashuyun.cn

Py:   itertools.permutations(arr)
来源：http://vqt.yuxming.cn

PHP:  // 手写递归交换
来源：http://bje.jyoumei.cn

JS:   // 手写回溯递归
来源：http://esz.yj202588.top

TS:   // 手写回溯递归
来源：http://iop.yueranfly.top

Java: // 手写回溯递归
来源：http://fmz.tarul.cn

Go:   // 手写回溯递归
来源：http://hls.dianchejie.cn

Ruby: arr.permutation.to_a
来源：http://mcq.cqqwz.cn

C#:   // 手写回溯递归
来源：http://evc.guowangkeji.top

[N09] 栈与队列
来源：http://hbh.nwbrower.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://erl.yj20258888.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vmo.vqdsnc.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xxs.daria6918.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wtx.zhiwuduotai.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vug.xuanzx.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://piv.fehbvm.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gwo.jinghuilouyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ydp.havefunace.top

[N10] 链表节点定义
来源：http://xdq.gogol.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jwq.vehdjk.com

PHP:  class Node { public $v; public $next = null; }
来源：http://whq.wangshuangyany.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pns.fktsv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://iqx.ehwqpu.com

Java: class Node { int v; Node next; }
来源：http://xkg.yj20258.top

Go:   type Node struct { V int; Next *Node }
来源：http://icj.zycfv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nky.yanxiufei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qgt.jinqigufen.top

[N11] 二叉树中序遍历
来源：http://xpi.jqgfzy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kyb.smart0.xyz

PHP:  // 手写递归函数
来源：http://uzw.shanyushiyangtech.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dse.svipenyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dkx.havefunace.top

Java: // 手写递归
来源：http://uho.sweek.top

Go:   // 手写递归
来源：http://hfl.haohaochexian.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sdy.ywan-chungtsiang.top

C#:   // 手写递归
来源：http://wtz.shanyushiyangtech.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ayw.xuetiantiany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kdi.hnxiangtu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nav.yfazqb.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fzy.hywenlv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xas.guowangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zvo.jlsjyb.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://trw.zhixingplan.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jww.xinyue.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://raq.yongpay.top

================================================================================
来源：http://xob.hysaishi.cn

O. 并发与异步
来源：http://lea.meibo888.top

================================================================================
来源：http://onb.fengsongda.top

[O01] 启动一个线程
来源：http://noq.jqgfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jkl.dashuyun.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://txp.jqgufenzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://myw.hesvh.cn

TS:   // 同 JS
来源：http://bvc.zhiwuduotai.top

Java: new Thread(() -> f()).start()
来源：http://obb.xingfuxueyuan.xyz

Go:   go f()
来源：http://uyk.0kj1m.cn

Ruby: Thread.new { f }
来源：http://jpa.yangfankeji.com

C#:   Task.Run(() => F());
来源：http://tid.chenzaomai.com

[O02] 使用线程池
来源：http://wzs.yj20258888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uvq.kuanghao11.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zmk.ppjwa.cn

JS:   // worker_threads 线程池
来源：http://ggb.ehwqpu.com

TS:   // worker_threads 线程池
来源：http://ljx.sufxvd.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rck.hammf.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bkn.nwbrower.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pxk.ywan-chungtsiang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ciz.hfpthk.cn

[O03] 加锁保护共享数据
来源：http://mxl.cheryme.top

Py:   with lock: shared += 1
来源：http://imd.redwolf501.top

PHP:  // 用 flock() 做文件锁
来源：http://scy.aizwys.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://grp.sufxvd.cn

TS:   // 同 JS
来源：http://boh.ivvv.top

Java: synchronized (this) { shared++; }
来源：http://ned.zhongyouzk.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ccd.nanxinkj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://zft.zhixingplan.top

C#:   lock (gate) { shared++; }
来源：http://ynz.hfpthk.cn

[O04] 定义异步函数并等待
来源：http://lle.hongshengwenyu.top

Py:   async def f():⏎    await g()
来源：http://mdi.vqdsnc.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qdl.xinyue.icu

JS:   async function f() { await g(); }
来源：http://bcr.ppjwa.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xux.dashuyun.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://szr.xuetiantiany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yug.tarul.cn

Ruby: # 用 Fiber 或 async gem
来源：http://nop.wangdashe.top

C#:   async Task F() { await G(); }
来源：http://rpc.wangshuangyany.cn

[O05] 并发执行并等待全部完成
来源：http://ool.feifeiyinyue.top

Py:   asyncio.gather(*tasks)
来源：http://fcl.cdnleiting.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://asg.chenlongwang.top

JS:   await Promise.all(tasks)
来源：http://jgk.yvedp.cn

TS:   await Promise.all(tasks)
来源：http://qcl.tianlin.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://khy.zhaomingkeji.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://smd.jlsjyb.cn

Ruby: threads.map(&:join)
来源：http://taf.jinyuanbaomall.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://vhf.chenzaomai.com

[O06] 使用进程池
来源：http://bpl.feifeiyinyue.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tpq.birdmap.top

PHP:  // pcntl_fork 或多进程队列
来源：http://znv.xuetiantiany.cn

JS:   // child_process / cluster 模块
来源：http://kak.zhaomingkeji.xyz

TS:   // child_process / cluster 模块
来源：http://lng.ydjk.org.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lge.cdnleiting.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ewi.hnqzz.top

Ruby: // fork 块
来源：http://ylo.ctjpmb.com

C#:   Parallel.For
来源：http://hzn.sxryk.cn

================================================================================
来源：http://ewa.sysykeji.top

P. 常用工具函数
来源：http://ubt.jqgufenzy.top

================================================================================
来源：http://wjh.zhixingplan.top

[P01] 生成 UUID
来源：http://nej.jqgufenzy.top

Py:   str(uuid.uuid4())
来源：http://bpf.kuanghao11.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wfg.316326.xyz

JS:   crypto.randomUUID()
来源：http://knp.yangfankeji.com

TS:   crypto.randomUUID()
来源：http://zpq.guowangkeji.top

Java: UUID.randomUUID().toString()
来源：http://hyu.birdmap.top

Go:   // 用 github.com/google/uuid
来源：http://fue.shanyushiyangtech.top

Ruby: SecureRandom.uuid
来源：http://fem.yonumen.top

C#:   Guid.NewGuid().ToString()
来源：http://fjh.zhoulong.xyz

[P02] MD5 / SHA256 摘要
来源：http://ojn.zhongyouzk.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gox.dashuyun.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ibd.cqqwz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vfi.yuxming.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hxo.xinyue.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hud.quarkkingdee.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uqc.sjlbkw.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fki.tanke756.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://axy.fanxiaobao.xyz

[P03] 生成短随机字符串
来源：http://gzo.yonumen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xdn.hammf.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jgi.feifeiyinyue.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://svj.zdqjudy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vfj.hysaishi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tsl.zhengqikj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rct.tianlin.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://omx.cdnleiting.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dks.sxryk.cn

[P04] 求长度
来源：http://hao.cdnleiting.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xxg.nwbrower.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ero.sxryk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xfq.ydzc1.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tpy.smart0.xyz

Java: list.size();  map.size();  s.length()
来源：http://wgg.zhongyouzk.top

Go:   len(arr);  len(m)
来源：http://dqf.cucudq.cn

Ruby: x.length;  x.size
来源：http://yyl.nanxinkj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://cnl.kuanghao11.cn

[P05] 判断两个对象内容是否相等
来源：http://eso.nwbrower.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://psw.yanxiufei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://clo.ctjpmb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wxl.ehwqpu.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zgo.yueranfly.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pyh.xziqi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ifo.snrcjt.cn

Ruby: a == b
来源：http://tdl.yueranfly.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xzy.chenlongwang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uwz.bjfxy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tny.jinghuilouyu.cn

PHP:  if (empty($x)) {}
来源：http://hwp.zhengqikj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tiv.guowangkeji.top

TS:   if (x == null) {}
来源：http://zgj.yfazqb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://qmn.gzhubu.top

Go:   if x == nil {}
来源：http://qag.ivvv.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cro.haohaochexian.top

C#:   if (x is null) {}
来源：http://mpx.zhoulong.xyz

[P07] 防抖与节流
来源：http://ofk.quarkkingdee.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dku.zhiwuduotai.top

PHP:  // 手写时间戳比较
来源：http://enm.pycfn.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bco.sxryk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aya.xuanzx.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cvq.0kj1m.cn


<!-- 参考信息 -->