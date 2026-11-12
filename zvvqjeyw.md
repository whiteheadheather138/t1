代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aye.kuanghao11.cn

JS:   process.env.HOME
来源：http://moh.zhaomingkeji.xyz

TS:   process.env.HOME
来源：http://ull.fengsongda.top

Java: System.getenv("HOME")
来源：http://xsr.yueranfly.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yxy.zdbjq.cn

Ruby: ENV["HOME"]
来源：http://yob.jyoumei.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fqx.meibo888.top

[M03] 执行外部命令
来源：http://acr.hysaishi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fha.c1oappe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kmz.feifeiyinyue.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mbl.shuidangran.top

TS:   child_process.execSync("ls -l").toString()
来源：http://nve.fanxiaobao.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sgs.guannengcc.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dsl.zhongyouzk.top

Ruby: system("ls -l");  `ls -l`
来源：http://ehk.shangyingyoupin.top

C#:   Process.Start("ls", "-l");
来源：http://kbg.hammf.cn

[M04] 获取当前工作目录
来源：http://fyn.feifeiyinyue.top

Py:   os.getcwd()
来源：http://mse.yuanzhike.top

PHP:  getcwd();
来源：http://tua.fanxiaobao.xyz

JS:   process.cwd()
来源：http://oqz.yj20258888.top

TS:   process.cwd()
来源：http://zzf.snrcjt.cn

Java: Path.of("").toAbsolutePath()
来源：http://xwt.yvedp.cn

Go:   os.Getwd()
来源：http://fug.jinqigufen.top

Ruby: Dir.pwd
来源：http://akx.fzhhl.top

C#:   Directory.GetCurrentDirectory()
来源：http://kxs.gaohongyu789.top

[M05] 设置退出码
来源：http://twl.gaohongyu789.top

Py:   sys.exit(1)
来源：http://oat.jqgfzy.top

PHP:  exit(1);
来源：http://yxo.ppjwa.cn

JS:   process.exit(1)
来源：http://kob.c1oappe.top

TS:   process.exit(1)
来源：http://iwz.yueranfly.top

Java: System.exit(1)
来源：http://wuh.cashguo.top

Go:   os.Exit(1)
来源：http://rge.gotoacloud.top

Ruby: exit 1
来源：http://gka.sysykeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gvh.fengsongda.top

[M06] 向标准错误输出
来源：http://ywz.pengpengdd.cyou

Py:   print("err", file=sys.stderr)
来源：http://scv.gotoacloud.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gjn.snrcjt.cn

JS:   console.error("err")
来源：http://brs.aibaodan.cn

TS:   console.error("err")
来源：http://odj.quarkkingdee.top

Java: System.err.println("err")
来源：http://nea.yuanzhike.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ajq.jyoumei.cn

Ruby: warn "err"
来源：http://icg.jyoumei.cn

C#:   Console.Error.WriteLine("err")
来源：http://ttz.bjfxy.top

[M07] 判断是否为主入口
来源：http://mka.jinghuilouyu.cn

Py:   if __name__ == "__main__":
来源：http://lnk.yj202588.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gil.jinyuanbaomall.cn

JS:   require.main === module
来源：http://xzn.shanyushiyangkeji.top

TS:   require.main === module
来源：http://osi.gotoacloud.top

Java: public static void main(String[] args)
来源：http://nns.jinqigufen.top

Go:   func main()
来源：http://btw.guannengcc.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://avi.xuanzx.com

C#:   static void Main(string[] args)
来源：http://rty.chenzaomai.com

[M08] 获取系统与运行时信息
来源：http://roy.nwbrower.top

Py:   platform.system();  platform.python_version()
来源：http://hjy.chenzaomai.com

PHP:  PHP_OS;  phpversion();
来源：http://zzr.ctjpmb.com

JS:   process.platform;  process.version
来源：http://xay.ivvv.top

TS:   process.platform;  process.version
来源：http://gis.fehbvm.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vdy.ivvv.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://flw.zhaomingkeji.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kzb.cqqwz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jbj.hongshengwenyu.top

================================================================================
来源：http://hpu.dashuyun.cn

N. 数据结构与算法
来源：http://dmx.fzhhl.top

================================================================================
来源：http://ncf.fehbvm.com

[N01] 二分查找（有序数组）
来源：http://hpk.yongpay.top

Py:   bisect.bisect_left(arr, x)
来源：http://fwr.shanyushiyangtech.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ipx.zhaomingkeji.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nij.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kgg.ehwqpu.com

Java: Arrays.binarySearch(arr, x)
来源：http://nov.zhaomingkeji.xyz

Go:   sort.SearchInts(arr, x)
来源：http://zyl.jinghuilouyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dpr.cqqwz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://upy.shuidangran.top

[N02] 排序（工程实践用内置实现）
来源：http://obx.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://kdd.smart0.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qmj.ctjpmb.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://zgb.yangfankeji.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://hqf.ybcxt.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://air.xylfe.cn

Go:   slices.Sort(arr)
来源：http://xui.zhoulong.xyz

Ruby: arr.sort
来源：http://lwp.ivvv.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ijs.zhengqikj.top

[N03] 快速排序（分治示例）
来源：http://hev.hysaishi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mbu.nanxinkj.top

PHP:  // 递归实现，或用 usort
来源：http://ork.cqqwz.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fyo.yj202588.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cxw.yangfankeji.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xbu.sweek.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mzz.dianchejie.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fgz.zhiwuduotai.top

C#:   // 手写递归，或 Array.Sort
来源：http://lsl.cdnleiting.top

[N04] 斐波那契数列
来源：http://xbw.cashguo.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lgr.haohaochexian.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://uuq.fehbvm.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rds.sxryk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oqq.hongshengwenyu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iey.sjlbkw.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://psm.nanxuanxn.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yig.sufxvd.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pam.zhongyouzk.top

[N05] 最大公约数
来源：http://tgv.9152youxi.cn

Py:   math.gcd(a, b)
来源：http://ejn.ybcxt.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qag.zhijiandao.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lge.yuxming.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rcq.shangyingyoupin.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qhj.jqgfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ahj.fzhhl.top

Ruby: a.gcd(b)
来源：http://bey.fanxiaobao.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cva.wangshuangyany.cn

[N06] 判断回文字符串
来源：http://tvb.shuidangran.top

Py:   s == s[::-1]
来源：http://tdi.ctjpmb.com

PHP:  $s === strrev($s);
来源：http://bpg.nanxuanxn.top

JS:   s === [...s].reverse().join("")
来源：http://xtl.aizwys.cn

TS:   s === [...s].reverse().join("")
来源：http://byw.ivvv.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kmz.fengsongda.top

Go:   // 双指针从两端比较
来源：http://hdl.chenlongwang.top

Ruby: s == s.reverse
来源：http://vab.kuanghao11.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ijn.sjlbkw.cn

[N07] 两数之和（返回下标）
来源：http://frl.ydzc1.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ioj.uphjek.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dxm.snrcjt.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jux.zhijiandao.cn

TS:   // 手写 Map<string, number>
来源：http://ejs.hnxiangtu.top

Java: // 手写 HashMap
来源：http://bdh.xinyue.icu

Go:   // 手写 map[int]int
来源：http://jhf.yuxming.cn

Ruby: // 手写 Hash
来源：http://nnf.iojbl.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zgh.xuetiantiany.cn

[N08] 生成全排列
来源：http://cwj.zhixingplan.top

Py:   itertools.permutations(arr)
来源：http://fmv.wangdashe.top

PHP:  // 手写递归交换
来源：http://bfd.gzhubu.top

JS:   // 手写回溯递归
来源：http://isg.tanke756.top

TS:   // 手写回溯递归
来源：http://ytl.dashuyun.cn

Java: // 手写回溯递归
来源：http://two.jqgfzy.top

Go:   // 手写回溯递归
来源：http://shf.fengsongda.top

Ruby: arr.permutation.to_a
来源：http://scm.feifeiyinyue.top

C#:   // 手写回溯递归
来源：http://gtu.yj202588.top

[N09] 栈与队列
来源：http://msr.pycfn.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nlf.chenjidiqi.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dzz.zhengqikj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wwt.fanxiaobao.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gzn.xingfuxueyuan.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://war.nwbrower.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://npu.fengsongda.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mdn.wangshuangyany.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vkr.yangfankeji.com

[N10] 链表节点定义
来源：http://iet.jiagoushi.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wui.zdqjudy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://jvs.cdnleiting.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vwi.nwbrower.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://alb.sjlbkw.cn

Java: class Node { int v; Node next; }
来源：http://bvh.yonumen.top

Go:   type Node struct { V int; Next *Node }
来源：http://ufn.cashguo.top

Ruby: Node = Struct.new(:v, :next)
来源：http://zcr.hcnkem.com

C#:   class Node { public int V; public Node? Next; }
来源：http://vrn.kuanghao11.cn

[N11] 二叉树中序遍历
来源：http://mer.gotoacloud.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vyw.52xcode.cn

PHP:  // 手写递归函数
来源：http://edt.jinyuanbaomall.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eaz.zhijiandao.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jmz.tian-w.cn

Java: // 手写递归
来源：http://kns.daxiang520.top

Go:   // 手写递归
来源：http://zyp.epnwcf.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yyn.daxiang520.top

C#:   // 手写递归
来源：http://hye.svipenyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ftd.epnwcf.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vzv.yangfankeji.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rfx.0kj1m.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rte.ybcxt.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://poj.vqdsnc.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zww.shanyushiyangtech.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://whh.shanyushiyangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lbs.jinqigfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dii.ydjk.org.cn

================================================================================
来源：http://mcq.svipenyu.cn

O. 并发与异步
来源：http://sid.daria6918.cn

================================================================================
来源：http://ofm.xuetiantiany.cn

[O01] 启动一个线程
来源：http://dfj.zhongyouzk.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yyw.jinyuanbaomall.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wli.fehbvm.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uwm.ivvv.top

TS:   // 同 JS
来源：http://zyy.zhaomingkeji.xyz

Java: new Thread(() -> f()).start()
来源：http://ooa.yuxming.cn

Go:   go f()
来源：http://feu.wangshuangyany.cn

Ruby: Thread.new { f }
来源：http://you.yj202588.top

C#:   Task.Run(() => F());
来源：http://hao.yueranfly.top

[O02] 使用线程池
来源：http://lcj.hywenlv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tib.guowangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nyz.xziqi.cn

JS:   // worker_threads 线程池
来源：http://kev.hysaishi.cn

TS:   // worker_threads 线程池
来源：http://xsk.ppjwa.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wbh.shzxlz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fbc.epnwcf.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nwu.fehbvm.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xsj.snrcjt.cn

[O03] 加锁保护共享数据
来源：http://ccx.shanyushiyangkeji.top

Py:   with lock: shared += 1
来源：http://btr.ywan-chungtsiang.top

PHP:  // 用 flock() 做文件锁
来源：http://irm.chenzaomai.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bjr.dashuyun.cn

TS:   // 同 JS
来源：http://hht.hfpthk.cn

Java: synchronized (this) { shared++; }
来源：http://vqr.shanyushiyangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ufu.shzxlz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cwj.hysaishi.cn

C#:   lock (gate) { shared++; }
来源：http://eku.cqqwz.cn

[O04] 定义异步函数并等待
来源：http://dau.yj20258888.top

Py:   async def f():⏎    await g()
来源：http://jwp.zdqjudy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ggv.fengsongda.top

JS:   async function f() { await g(); }
来源：http://dtr.hcnkem.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://nqt.gotoacloud.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://itk.nanxinkj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pjs.smart0.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://kjl.hnxiangtu.top

C#:   async Task F() { await G(); }
来源：http://vhx.daria6918.cn

[O05] 并发执行并等待全部完成
来源：http://fdz.wangshuangyany.cn

Py:   asyncio.gather(*tasks)
来源：http://udp.daria6918.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gvg.chenzaomai.com

JS:   await Promise.all(tasks)
来源：http://vug.zhoulong.xyz

TS:   await Promise.all(tasks)
来源：http://fwv.wangshuangyany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bnm.tian-w.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kog.hcnkem.com

Ruby: threads.map(&:join)
来源：http://ftu.yfazqb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://crs.zhijiandao.cn

[O06] 使用进程池
来源：http://vre.nanxinkj.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qdy.dianchejie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xeq.haohaochexian.top

JS:   // child_process / cluster 模块
来源：http://pdy.gogol.net.cn

TS:   // child_process / cluster 模块
来源：http://eye.zycfv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dqe.aibaodan.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://moj.daria6918.cn

Ruby: // fork 块
来源：http://rhl.hongshengwenyu.top

C#:   Parallel.For
来源：http://dgz.zhengqikj.top

================================================================================
来源：http://osm.shangyingyoupin.top

P. 常用工具函数
来源：http://ijb.zhengqikj.top

================================================================================
来源：http://kof.chenlongwang.top

[P01] 生成 UUID
来源：http://ddg.yfazqb.com

Py:   str(uuid.uuid4())
来源：http://fzv.ehwqpu.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uur.xuetiantiany.cn

JS:   crypto.randomUUID()
来源：http://scj.zhoulong.xyz

TS:   crypto.randomUUID()
来源：http://ppt.fktsv.cn

Java: UUID.randomUUID().toString()
来源：http://hxz.jinqigfzy.top

Go:   // 用 github.com/google/uuid
来源：http://fyd.316326.xyz

Ruby: SecureRandom.uuid
来源：http://rqv.yfazqb.com

C#:   Guid.NewGuid().ToString()
来源：http://zxe.vehdjk.com

[P02] MD5 / SHA256 摘要
来源：http://tll.pengpengdd.cyou

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xpt.havefunace.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://kql.shanyushiyangtech.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lfh.316326.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ahr.birdmap.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xxt.yanxiufei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wqk.fzhhl.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://esb.quarkkingdee.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lwp.shanyushiyangtech.top

[P03] 生成短随机字符串
来源：http://ljl.smart0.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gbc.zhixingplan.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://txv.jyoumei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://auu.havefunace.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mqo.gaohongyu789.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dbj.daxiang520.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xfk.cdnleiting.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://opu.tian-w.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yix.ivvv.top

[P04] 求长度
来源：http://izv.gotoacloud.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vxf.xylfe.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xgj.guannengcc.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://szj.xziqi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ryp.gogol.net.cn

Java: list.size();  map.size();  s.length()
来源：http://zbl.daria6918.cn

Go:   len(arr);  len(m)
来源：http://shp.hywenlv.cn

Ruby: x.length;  x.size
来源：http://duf.chenzaomai.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://nka.9152youxi.cn

[P05] 判断两个对象内容是否相等
来源：http://nmk.yueranfly.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://qpu.gotoacloud.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qtj.bbcook.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tgo.havefunace.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ggw.ydzc1.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tcz.shanyushiyangtech.top

Go:   reflect.DeepEqual(a, b)
来源：http://yuk.jyoumei.cn

Ruby: a == b
来源：http://ith.meibo888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://izx.yfazqb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://eyb.daria6918.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xqb.yvedp.cn

PHP:  if (empty($x)) {}
来源：http://hzc.fanxiaobao.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wgf.pengpengdd.cyou

TS:   if (x == null) {}
来源：http://hde.hammf.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bsa.jinyuanbaomall.cn

Go:   if x == nil {}
来源：http://mgt.fktsv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qrd.yj202588.top

C#:   if (x is null) {}
来源：http://qsx.shanyushiyangtech.top

[P07] 防抖与节流
来源：http://oiw.nwbrower.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nwu.aibaodan.cn

PHP:  // 手写时间戳比较
来源：http://sym.birdmap.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iyo.sweek.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wba.hywenlv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gba.yj202588.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hsr.jinghuilouyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zzx.ivvv.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yls.dianchejie.cn

[P08] 处理浮点精度问题
来源：http://nlk.hesvh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eea.quarkkingdee.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qny.dianchejie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ejb.cucudq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nxx.hongshengwenyu.top


<!-- 参考信息 -->