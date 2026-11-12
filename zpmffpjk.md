代发 wailian999

Ruby: ARGV
来源：http://rig.zhixingplan.top

C#:   args 数组（Main 方法参数）
来源：http://fep.zycfv.cn

[M02] 读取环境变量
来源：http://fbd.zhixingplan.top

Py:   os.environ.get("HOME")
来源：http://zcl.c1oappe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iqq.smart0.xyz

JS:   process.env.HOME
来源：http://ffm.andypj.xyz

TS:   process.env.HOME
来源：http://zwz.sxryk.cn

Java: System.getenv("HOME")
来源：http://hff.zhengqikj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://als.epnwcf.com

Ruby: ENV["HOME"]
来源：http://kre.shanyushiyangtech.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lpx.gotoacloud.top

[M03] 执行外部命令
来源：http://odh.c1oappe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vlw.vqdsnc.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wxu.yuanzhike.top

JS:   child_process.execSync("ls -l").toString()
来源：http://nkf.nwbrower.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tqy.yfazqb.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hry.hnxiangtu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://cqd.cashguo.top

Ruby: system("ls -l");  `ls -l`
来源：http://vub.kuanghao11.cn

C#:   Process.Start("ls", "-l");
来源：http://sdg.hywenlv.cn

[M04] 获取当前工作目录
来源：http://xja.xingfuxueyuan.xyz

Py:   os.getcwd()
来源：http://blc.chenjidiqi.icu

PHP:  getcwd();
来源：http://uwo.sjlbkw.cn

JS:   process.cwd()
来源：http://ccf.tian-w.cn

TS:   process.cwd()
来源：http://sre.uphjek.com

Java: Path.of("").toAbsolutePath()
来源：http://apn.zhiwuduotai.top

Go:   os.Getwd()
来源：http://gxu.fehbvm.com

Ruby: Dir.pwd
来源：http://vsi.aibaodan.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zat.zhixingplan.top

[M05] 设置退出码
来源：http://iom.dashuyun.cn

Py:   sys.exit(1)
来源：http://npq.sysykeji.top

PHP:  exit(1);
来源：http://nxb.cqqwz.cn

JS:   process.exit(1)
来源：http://fjn.cqqwz.cn

TS:   process.exit(1)
来源：http://qyo.yj20258.top

Java: System.exit(1)
来源：http://jxl.zhijiandao.cn

Go:   os.Exit(1)
来源：http://std.wangdashe.top

Ruby: exit 1
来源：http://gjc.zhiwuduotai.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eho.tianlin.xyz

[M06] 向标准错误输出
来源：http://bdg.sxryk.cn

Py:   print("err", file=sys.stderr)
来源：http://euq.ctjpmb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://zjs.svipenyu.cn

JS:   console.error("err")
来源：http://dat.nanxuanxn.top

TS:   console.error("err")
来源：http://dtn.andypj.xyz

Java: System.err.println("err")
来源：http://xwr.jqgufenzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fgq.tianlin.xyz

Ruby: warn "err"
来源：http://tyx.hongshengwenyu.top

C#:   Console.Error.WriteLine("err")
来源：http://sbi.xingfuxueyuan.xyz

[M07] 判断是否为主入口
来源：http://ecd.xingfuxueyuan.xyz

Py:   if __name__ == "__main__":
来源：http://ckg.bjfxy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sjh.shanyushiyangtech.top

JS:   require.main === module
来源：http://vbj.cashguo.top

TS:   require.main === module
来源：http://hvz.xuetiantiany.cn

Java: public static void main(String[] args)
来源：http://nem.sxryk.cn

Go:   func main()
来源：http://emj.dianchejie.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://psw.cashguo.top

C#:   static void Main(string[] args)
来源：http://odh.cdnleiting.top

[M08] 获取系统与运行时信息
来源：http://jqu.jqgufenzy.top

Py:   platform.system();  platform.python_version()
来源：http://ugf.jianghu66.top

PHP:  PHP_OS;  phpversion();
来源：http://wjq.tarul.cn

JS:   process.platform;  process.version
来源：http://lcw.yj202588.top

TS:   process.platform;  process.version
来源：http://cyv.hcnkem.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wtw.daria6918.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pkz.shzxlz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cnq.ppjwa.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jph.aibaodan.cn

================================================================================
来源：http://qdu.zdqjudy.top

N. 数据结构与算法
来源：http://xlj.cqqwz.cn

================================================================================
来源：http://ixx.shangyingyoupin.top

[N01] 二分查找（有序数组）
来源：http://ynj.zhixingplan.top

Py:   bisect.bisect_left(arr, x)
来源：http://yst.ybcxt.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ltb.svipenyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://twe.chenlongwang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cxt.c1oappe.top

Java: Arrays.binarySearch(arr, x)
来源：http://sgb.jiagoushi.top

Go:   sort.SearchInts(arr, x)
来源：http://lvc.daria6918.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://brr.guannengcc.top

C#:   Array.BinarySearch(arr, x)
来源：http://oze.yj20258.top

[N02] 排序（工程实践用内置实现）
来源：http://jnn.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://xwx.sysykeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qin.zdbjq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bti.guannengcc.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://uuw.316326.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://itz.fanxiaobao.xyz

Go:   slices.Sort(arr)
来源：http://nwg.meibo888.top

Ruby: arr.sort
来源：http://isd.hesvh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://par.jinyuanbaomall.cn

[N03] 快速排序（分治示例）
来源：http://qdy.ivvv.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lrx.quarkkingdee.top

PHP:  // 递归实现，或用 usort
来源：http://ghp.andypj.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ugy.chenjidiqi.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ddv.shuidangran.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jur.haohaochexian.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qqp.shuidangran.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://exa.hammf.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kuu.ppjwa.cn

[N04] 斐波那契数列
来源：http://ncv.zhaomingkeji.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bll.chenlongwang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mdj.yangfankeji.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jgs.zdqjudy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yle.gotoacloud.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eru.cashguo.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yxa.hesvh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fvf.xylfe.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://erx.epnwcf.com

[N05] 最大公约数
来源：http://iss.fanxiaobao.xyz

Py:   math.gcd(a, b)
来源：http://jbo.guowangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://duo.guannengcc.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cpc.hysaishi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zbx.tanke756.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dmu.cucudq.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lpc.uphjek.com

Ruby: a.gcd(b)
来源：http://sye.yuxming.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bme.sxryk.cn

[N06] 判断回文字符串
来源：http://mcc.xuetiantiany.cn

Py:   s == s[::-1]
来源：http://sec.gotoacloud.top

PHP:  $s === strrev($s);
来源：http://trv.cdnleiting.top

JS:   s === [...s].reverse().join("")
来源：http://tub.bbcook.cn

TS:   s === [...s].reverse().join("")
来源：http://rpi.hesvh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://eya.shzxlz.cn

Go:   // 双指针从两端比较
来源：http://mxn.feifeiyinyue.top

Ruby: s == s.reverse
来源：http://oko.pycfn.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://ahn.zycfv.cn

[N07] 两数之和（返回下标）
来源：http://mgq.smart0.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mmu.kuanghao11.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ifp.feifeiyinyue.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qcx.haohaochexian.top

TS:   // 手写 Map<string, number>
来源：http://kud.hysaishi.cn

Java: // 手写 HashMap
来源：http://tgo.yangfankeji.com

Go:   // 手写 map[int]int
来源：http://tsz.sjlbkw.cn

Ruby: // 手写 Hash
来源：http://ynw.aibaodan.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jvq.shzxlz.cn

[N08] 生成全排列
来源：http://kiu.c1oappe.top

Py:   itertools.permutations(arr)
来源：http://ano.ehwqpu.com

PHP:  // 手写递归交换
来源：http://bth.jianghu66.top

JS:   // 手写回溯递归
来源：http://spi.yuanzhike.top

TS:   // 手写回溯递归
来源：http://oqe.jinqigfzy.top

Java: // 手写回溯递归
来源：http://ppu.tanke756.top

Go:   // 手写回溯递归
来源：http://iib.xingfuxueyuan.xyz

Ruby: arr.permutation.to_a
来源：http://jfl.sjlbkw.cn

C#:   // 手写回溯递归
来源：http://dhf.sjlbkw.cn

[N09] 栈与队列
来源：http://muw.hysaishi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fcy.0kj1m.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ndb.iojbl.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dlt.yj20258.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://uot.birdmap.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xbt.tianlin.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://she.iojbl.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://awg.sjlbkw.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jsr.epnwcf.com

[N10] 链表节点定义
来源：http://lsw.jinqigufen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pnw.redwolf501.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ceu.fengsongda.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vgw.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rjn.ppjwa.cn

Java: class Node { int v; Node next; }
来源：http://qqc.ydzc1.top

Go:   type Node struct { V int; Next *Node }
来源：http://rat.shzxlz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://lxu.jqgfzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tpg.yfazqb.com

[N11] 二叉树中序遍历
来源：http://gbn.shanyushiyangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lxv.cqqwz.cn

PHP:  // 手写递归函数
来源：http://ctx.vqdsnc.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bck.xuetiantiany.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tom.ppjwa.cn

Java: // 手写递归
来源：http://gog.jinqigfzy.top

Go:   // 手写递归
来源：http://wte.sysykeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yls.ybcxt.top

C#:   // 手写递归
来源：http://lzx.ydzc1.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cdb.nanxinkj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://niw.hammf.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://str.xuanzx.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wgk.9152youxi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://egq.yongpay.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mxp.haohaochexian.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://efo.daria6918.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ihh.yfazqb.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ibz.pengpengdd.cyou

================================================================================
来源：http://gnk.hammf.cn

O. 并发与异步
来源：http://trp.yj202588.top

================================================================================
来源：http://bmt.vehdjk.com

[O01] 启动一个线程
来源：http://zeq.daxiang520.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bvf.xingfuxueyuan.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yyz.jqgufenzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tpf.xuetiantiany.cn

TS:   // 同 JS
来源：http://ser.shzxlz.cn

Java: new Thread(() -> f()).start()
来源：http://tzy.hcnkem.com

Go:   go f()
来源：http://owf.aibaodan.cn

Ruby: Thread.new { f }
来源：http://zqd.dashuyun.cn

C#:   Task.Run(() => F());
来源：http://tbb.yj20258888.top

[O02] 使用线程池
来源：http://myt.iojbl.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rbq.yj20258888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://odl.jinqigfzy.top

JS:   // worker_threads 线程池
来源：http://ybp.shanyushiyangkeji.top

TS:   // worker_threads 线程池
来源：http://vpk.yueranfly.top

Java: Executors.newFixedThreadPool(4)
来源：http://mrf.quarkkingdee.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hkh.jyoumei.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ebs.fzhhl.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rid.hysaishi.cn

[O03] 加锁保护共享数据
来源：http://gnn.yj202588.top

Py:   with lock: shared += 1
来源：http://rwa.zdbjq.cn

PHP:  // 用 flock() 做文件锁
来源：http://ugz.tanke756.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hur.wangshuangyany.cn

TS:   // 同 JS
来源：http://dzz.sysykeji.top

Java: synchronized (this) { shared++; }
来源：http://rgp.cheryme.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ygz.yuanzhike.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://hha.nwbrower.top

C#:   lock (gate) { shared++; }
来源：http://bho.birdmap.top

[O04] 定义异步函数并等待
来源：http://aoo.yanxiufei.cn

Py:   async def f():⏎    await g()
来源：http://czb.epnwcf.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yhx.hammf.cn

JS:   async function f() { await g(); }
来源：http://ivq.hnqzz.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jon.bbcook.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ety.zhiwuduotai.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fcp.meibo888.top

Ruby: # 用 Fiber 或 async gem
来源：http://qnr.guowangkeji.top

C#:   async Task F() { await G(); }
来源：http://zok.kuanghao11.cn

[O05] 并发执行并等待全部完成
来源：http://qdp.havefunace.top

Py:   asyncio.gather(*tasks)
来源：http://oow.redwolf501.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vfy.kuanghao11.cn

JS:   await Promise.all(tasks)
来源：http://efm.dianchejie.cn

TS:   await Promise.all(tasks)
来源：http://kzv.bjfxy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yek.daxiang520.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mcb.shuidangran.top

Ruby: threads.map(&:join)
来源：http://yna.nanxinkj.top

C#:   await Task.WhenAll(t1, t2)
来源：http://bqu.fktsv.cn

[O06] 使用进程池
来源：http://imv.cqqwz.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mly.sufxvd.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fth.gzhubu.top

JS:   // child_process / cluster 模块
来源：http://flt.yvedp.cn

TS:   // child_process / cluster 模块
来源：http://oqg.ywan-chungtsiang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://orq.cdnleiting.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nmd.tarul.cn

Ruby: // fork 块
来源：http://lua.feifeiyinyue.top

C#:   Parallel.For
来源：http://jix.yongpay.top

================================================================================
来源：http://yla.hammf.cn

P. 常用工具函数
来源：http://ygk.zhengqikj.top

================================================================================
来源：http://dna.shzxlz.cn

[P01] 生成 UUID
来源：http://ulx.316326.xyz

Py:   str(uuid.uuid4())
来源：http://wkf.dashuyun.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rko.yanxiufei.cn

JS:   crypto.randomUUID()
来源：http://kzx.jinqigfzy.top

TS:   crypto.randomUUID()
来源：http://byb.redwolf501.top

Java: UUID.randomUUID().toString()
来源：http://udo.yanxiufei.cn

Go:   // 用 github.com/google/uuid
来源：http://xtx.shzxlz.cn

Ruby: SecureRandom.uuid
来源：http://zcc.xinyue.icu

C#:   Guid.NewGuid().ToString()
来源：http://pwt.mhx1999.top

[P02] MD5 / SHA256 摘要
来源：http://qvd.wangdashe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://weg.uphjek.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://ski.c1oappe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://npd.zhijiandao.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zxo.cqqwz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tul.gotoacloud.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://voy.shanyushiyangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gpi.shanyushiyangtech.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bpt.andypj.xyz

[P03] 生成短随机字符串
来源：http://tqu.jiagoushi.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cjq.tarul.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qlf.xuetiantiany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://owp.cheryme.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dzv.pengpengdd.cyou

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mjz.ywan-chungtsiang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lvz.gotoacloud.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://kct.cucudq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://efa.jyoumei.cn

[P04] 求长度
来源：http://jly.guowangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wro.hysaishi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://opy.aibaodan.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wme.yj20258888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nhf.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://ajv.ehwqpu.com

Go:   len(arr);  len(m)
来源：http://qwv.fzhhl.top

Ruby: x.length;  x.size
来源：http://dkq.jyoumei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jnn.tarul.cn

[P05] 判断两个对象内容是否相等
来源：http://yli.jinghuilouyu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yvn.xuetiantiany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mgo.hammf.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gox.ybcxt.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jos.zhiwuduotai.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ebv.havefunace.top

Go:   reflect.DeepEqual(a, b)
来源：http://htj.yfazqb.com

Ruby: a == b
来源：http://ujv.ydzc1.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xph.yj202588.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://arf.yongpay.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bjm.andypj.xyz

PHP:  if (empty($x)) {}
来源：http://jyi.xziqi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xhz.tarul.cn

TS:   if (x == null) {}
来源：http://ifz.jinyuanbaomall.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://abd.hywenlv.cn

Go:   if x == nil {}
来源：http://tmy.guowangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dar.tianlin.xyz

C#:   if (x is null) {}
来源：http://axq.xingfuxueyuan.xyz

[P07] 防抖与节流
来源：http://xru.ivvv.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kbd.cheryme.top

PHP:  // 手写时间戳比较
来源：http://xfv.sweek.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hzd.zdbjq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ico.pengpengdd.cyou

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qpm.snrcjt.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ndj.bjfxy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://yqu.52xcode.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xnv.xuanzx.com

[P08] 处理浮点精度问题
来源：http://raf.meibo888.top


<!-- 参考信息 -->