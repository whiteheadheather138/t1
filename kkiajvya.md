代发 wailian999

Ruby: ARGV
来源：http://twr.quarkkingdee.top

C#:   args 数组（Main 方法参数）
来源：http://iht.sufxvd.cn

[M02] 读取环境变量
来源：http://dzm.yfazqb.com

Py:   os.environ.get("HOME")
来源：http://fwg.epnwcf.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zgt.gaohongyu789.top

JS:   process.env.HOME
来源：http://auz.yuanzhike.top

TS:   process.env.HOME
来源：http://bmx.kuanghao11.cn

Java: System.getenv("HOME")
来源：http://ysy.vehdjk.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ygs.zycfv.cn

Ruby: ENV["HOME"]
来源：http://ctc.gogol.net.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oqc.cdnleiting.top

[M03] 执行外部命令
来源：http://ljs.chenzaomai.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yci.yangfankeji.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kvv.zdqjudy.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hsj.bbcook.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sqr.xinyue.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ifl.shzxlz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://qqx.hnxiangtu.top

Ruby: system("ls -l");  `ls -l`
来源：http://bym.xylfe.cn

C#:   Process.Start("ls", "-l");
来源：http://gny.shanyushiyangtech.top

[M04] 获取当前工作目录
来源：http://pxj.zhaomingkeji.xyz

Py:   os.getcwd()
来源：http://rcr.c1oappe.top

PHP:  getcwd();
来源：http://yus.jqgufenzy.top

JS:   process.cwd()
来源：http://cpk.zhijiandao.cn

TS:   process.cwd()
来源：http://cjs.zhiwuduotai.top

Java: Path.of("").toAbsolutePath()
来源：http://nvj.xinyue.icu

Go:   os.Getwd()
来源：http://hph.hnqzz.top

Ruby: Dir.pwd
来源：http://eyk.zhoulong.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://pbe.shuidangran.top

[M05] 设置退出码
来源：http://hgz.52xcode.cn

Py:   sys.exit(1)
来源：http://dcx.vehdjk.com

PHP:  exit(1);
来源：http://bcd.ybcxt.top

JS:   process.exit(1)
来源：http://kdh.yongpay.top

TS:   process.exit(1)
来源：http://dhi.zhongyouzk.top

Java: System.exit(1)
来源：http://vyi.cdnleiting.top

Go:   os.Exit(1)
来源：http://cgm.cashguo.top

Ruby: exit 1
来源：http://zea.cashguo.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tuv.jlsjyb.cn

[M06] 向标准错误输出
来源：http://qec.316326.xyz

Py:   print("err", file=sys.stderr)
来源：http://aex.gaohongyu789.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lmz.hnxiangtu.top

JS:   console.error("err")
来源：http://drc.yueranfly.top

TS:   console.error("err")
来源：http://que.jqgufenzy.top

Java: System.err.println("err")
来源：http://tox.svipenyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rwn.gaohongyu789.top

Ruby: warn "err"
来源：http://xon.jinghuilouyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://zxv.jiagoushi.top

[M07] 判断是否为主入口
来源：http://cbh.fengsongda.top

Py:   if __name__ == "__main__":
来源：http://ukz.xziqi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oij.xinyue.icu

JS:   require.main === module
来源：http://inu.aibaodan.cn

TS:   require.main === module
来源：http://ipe.meibo888.top

Java: public static void main(String[] args)
来源：http://kre.zhongyouzk.top

Go:   func main()
来源：http://tgw.birdmap.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gsa.zdbjq.cn

C#:   static void Main(string[] args)
来源：http://eks.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://njn.chenjidiqi.icu

Py:   platform.system();  platform.python_version()
来源：http://fnz.snrcjt.cn

PHP:  PHP_OS;  phpversion();
来源：http://tvw.yj20258888.top

JS:   process.platform;  process.version
来源：http://cim.feifeiyinyue.top

TS:   process.platform;  process.version
来源：http://jal.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yoo.xziqi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vjo.yfazqb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qxc.cqqwz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ibu.uphjek.com

================================================================================
来源：http://edx.sysykeji.top

N. 数据结构与算法
来源：http://mcv.jinyuanbaomall.cn

================================================================================
来源：http://oak.zycfv.cn

[N01] 二分查找（有序数组）
来源：http://jzu.hcnkem.com

Py:   bisect.bisect_left(arr, x)
来源：http://xdu.cucudq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vrv.smart0.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oyv.vqdsnc.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://coj.yj20258888.top

Java: Arrays.binarySearch(arr, x)
来源：http://jom.sxryk.cn

Go:   sort.SearchInts(arr, x)
来源：http://mwh.zhoulong.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://umv.dianchejie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jtg.shanyushiyangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://cri.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://tot.shanyushiyangtech.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://stf.jinqigufen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://zcv.redwolf501.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cbe.sufxvd.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eke.guannengcc.top

Go:   slices.Sort(arr)
来源：http://anj.sufxvd.cn

Ruby: arr.sort
来源：http://rjr.smart0.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://lgz.svipenyu.cn

[N03] 快速排序（分治示例）
来源：http://gid.zhoulong.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mib.zhoulong.xyz

PHP:  // 递归实现，或用 usort
来源：http://qwp.nanxinkj.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dra.svipenyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://der.ydjk.org.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ecf.ydjk.org.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xmc.yj202588.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iac.guannengcc.top

C#:   // 手写递归，或 Array.Sort
来源：http://ama.sxryk.cn

[N04] 斐波那契数列
来源：http://xsa.tarul.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wsn.shanyushiyangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vyu.fehbvm.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ysy.0kj1m.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mwd.hysaishi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rke.dianchejie.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://umu.yvedp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yvi.jinqigfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uuo.gotoacloud.top

[N05] 最大公约数
来源：http://nod.shzxlz.cn

Py:   math.gcd(a, b)
来源：http://vqz.ehwqpu.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qgo.sjlbkw.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sut.316326.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://npz.hywenlv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xyw.shanyushiyangkeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://imy.ehwqpu.com

Ruby: a.gcd(b)
来源：http://ftp.kuanghao11.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qjh.jiagoushi.top

[N06] 判断回文字符串
来源：http://dpl.shuidangran.top

Py:   s == s[::-1]
来源：http://qob.hysaishi.cn

PHP:  $s === strrev($s);
来源：http://gsr.52xcode.cn

JS:   s === [...s].reverse().join("")
来源：http://fpn.jinghuilouyu.cn

TS:   s === [...s].reverse().join("")
来源：http://jel.snrcjt.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jvt.zhixingplan.top

Go:   // 双指针从两端比较
来源：http://qbg.gogol.net.cn

Ruby: s == s.reverse
来源：http://mtv.ppjwa.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mcl.fanxiaobao.xyz

[N07] 两数之和（返回下标）
来源：http://nde.jinqigufen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kvl.hesvh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://goy.havefunace.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gyf.pengpengdd.cyou

TS:   // 手写 Map<string, number>
来源：http://des.fzhhl.top

Java: // 手写 HashMap
来源：http://jni.tianlin.xyz

Go:   // 手写 map[int]int
来源：http://nxz.cqqwz.cn

Ruby: // 手写 Hash
来源：http://wlt.nanxinkj.top

C#:   // 手写 Dictionary<int, int>
来源：http://xbj.tian-w.cn

[N08] 生成全排列
来源：http://uck.52xcode.cn

Py:   itertools.permutations(arr)
来源：http://too.nanxinkj.top

PHP:  // 手写递归交换
来源：http://dxy.haohaochexian.top

JS:   // 手写回溯递归
来源：http://eam.shuidangran.top

TS:   // 手写回溯递归
来源：http://lqs.hnqzz.top

Java: // 手写回溯递归
来源：http://kfs.kuanghao11.cn

Go:   // 手写回溯递归
来源：http://dnx.9152youxi.cn

Ruby: arr.permutation.to_a
来源：http://hih.jyoumei.cn

C#:   // 手写回溯递归
来源：http://iqh.hywenlv.cn

[N09] 栈与队列
来源：http://yxi.xziqi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ccv.kuanghao11.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cfo.zhixingplan.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hjm.pycfn.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iut.feifeiyinyue.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kyd.jinyuanbaomall.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ewy.fanxiaobao.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://khs.bbcook.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uzm.xuetiantiany.cn

[N10] 链表节点定义
来源：http://ctx.ctjpmb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jxi.havefunace.top

PHP:  class Node { public $v; public $next = null; }
来源：http://hel.ivvv.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rzi.sysykeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gdv.shanyushiyangkeji.top

Java: class Node { int v; Node next; }
来源：http://vwv.birdmap.top

Go:   type Node struct { V int; Next *Node }
来源：http://dxj.cucudq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://caq.svipenyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://evv.sxryk.cn

[N11] 二叉树中序遍历
来源：http://mry.xuanzx.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://suw.yuanzhike.top

PHP:  // 手写递归函数
来源：http://imq.jiagoushi.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vcs.nwbrower.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qhg.zhongyouzk.top

Java: // 手写递归
来源：http://itx.yj20258.top

Go:   // 手写递归
来源：http://omd.mhx1999.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://skf.sxryk.cn

C#:   // 手写递归
来源：http://dpo.52xcode.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rkt.cqqwz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mzw.yangfankeji.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lhm.yongpay.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jve.tianlin.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wkm.zdqjudy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vxa.fktsv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uwj.tian-w.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wcv.shzxlz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://znn.birdmap.top

================================================================================
来源：http://lst.birdmap.top

O. 并发与异步
来源：http://xuj.jinqigufen.top

================================================================================
来源：http://ubv.uphjek.com

[O01] 启动一个线程
来源：http://hpt.zhixingplan.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hpr.jianghu66.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wsh.gaohongyu789.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mrz.uphjek.com

TS:   // 同 JS
来源：http://qrp.jiagoushi.top

Java: new Thread(() -> f()).start()
来源：http://lli.meibo888.top

Go:   go f()
来源：http://bma.guannengcc.top

Ruby: Thread.new { f }
来源：http://csa.jyoumei.cn

C#:   Task.Run(() => F());
来源：http://kjr.hcnkem.com

[O02] 使用线程池
来源：http://khw.havefunace.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mnb.chenjidiqi.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cau.hywenlv.cn

JS:   // worker_threads 线程池
来源：http://ufd.zhixingplan.top

TS:   // worker_threads 线程池
来源：http://qyd.xylfe.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ybr.xuanzx.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gyb.yuxming.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qho.dashuyun.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ryy.zhiwuduotai.top

[O03] 加锁保护共享数据
来源：http://aqj.sweek.top

Py:   with lock: shared += 1
来源：http://lrx.shanyushiyangtech.top

PHP:  // 用 flock() 做文件锁
来源：http://gqb.mhx1999.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xxw.yongpay.top

TS:   // 同 JS
来源：http://nyl.316326.xyz

Java: synchronized (this) { shared++; }
来源：http://kws.cqqwz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ghg.cheryme.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://cxs.pycfn.com

C#:   lock (gate) { shared++; }
来源：http://ibh.fktsv.cn

[O04] 定义异步函数并等待
来源：http://dlj.epnwcf.com

Py:   async def f():⏎    await g()
来源：http://wxe.chenlongwang.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ata.quarkkingdee.top

JS:   async function f() { await g(); }
来源：http://lms.bjfxy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gdu.hfpthk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ddr.zhengqikj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nhn.mhx1999.top

Ruby: # 用 Fiber 或 async gem
来源：http://itx.ydjk.org.cn

C#:   async Task F() { await G(); }
来源：http://yyl.nanxinkj.top

[O05] 并发执行并等待全部完成
来源：http://qkz.zhongyouzk.top

Py:   asyncio.gather(*tasks)
来源：http://gln.ivvv.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jrb.dianchejie.cn

JS:   await Promise.all(tasks)
来源：http://utg.fanxiaobao.xyz

TS:   await Promise.all(tasks)
来源：http://dmm.chenlongwang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rhu.yj202588.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gvh.ehwqpu.com

Ruby: threads.map(&:join)
来源：http://lxo.xylfe.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jia.pengpengdd.cyou

[O06] 使用进程池
来源：http://pbr.yj20258888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nrp.cqqwz.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hhz.jinyuanbaomall.cn

JS:   // child_process / cluster 模块
来源：http://kvg.jqgfzy.top

TS:   // child_process / cluster 模块
来源：http://jqb.316326.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qsr.52xcode.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xcy.tianlin.xyz

Ruby: // fork 块
来源：http://ksv.kuanghao11.cn

C#:   Parallel.For
来源：http://chd.jlsjyb.cn

================================================================================
来源：http://kid.fzhhl.top

P. 常用工具函数
来源：http://tox.shangyingyoupin.top

================================================================================
来源：http://bdd.zhixingplan.top

[P01] 生成 UUID
来源：http://zig.jiagoushi.top

Py:   str(uuid.uuid4())
来源：http://gpm.zhiwuduotai.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gjt.snrcjt.cn

JS:   crypto.randomUUID()
来源：http://ujl.dashuyun.cn

TS:   crypto.randomUUID()
来源：http://nrf.quarkkingdee.top

Java: UUID.randomUUID().toString()
来源：http://rra.kuanghao11.cn

Go:   // 用 github.com/google/uuid
来源：http://dxq.meibo888.top

Ruby: SecureRandom.uuid
来源：http://dbd.cqqwz.cn

C#:   Guid.NewGuid().ToString()
来源：http://yay.iojbl.cn

[P02] MD5 / SHA256 摘要
来源：http://vhg.c1oappe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://epo.guowangkeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lox.vehdjk.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fqo.gogol.net.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rcz.hesvh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xxy.snrcjt.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yhq.hcnkem.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vmn.9152youxi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rqr.shanyushiyangkeji.top

[P03] 生成短随机字符串
来源：http://enp.jinqigufen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vit.cdnleiting.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yja.hammf.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uqf.c1oappe.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nkx.yangfankeji.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://igj.chenlongwang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://chl.hysaishi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://oil.fanxiaobao.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ypf.nwbrower.top

[P04] 求长度
来源：http://wng.hywenlv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mjm.xingfuxueyuan.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nnp.fzhhl.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jqs.nanxinkj.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sud.sjlbkw.cn

Java: list.size();  map.size();  s.length()
来源：http://jaf.zhixingplan.top

Go:   len(arr);  len(m)
来源：http://mpx.jinqigufen.top

Ruby: x.length;  x.size
来源：http://zmt.bjfxy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dsn.iojbl.cn

[P05] 判断两个对象内容是否相等
来源：http://dnn.316326.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://hak.hcnkem.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fbq.daria6918.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xjg.fanxiaobao.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jsc.redwolf501.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hkl.hnqzz.top

Go:   reflect.DeepEqual(a, b)
来源：http://hvx.cucudq.cn

Ruby: a == b
来源：http://xrf.sufxvd.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vxk.hysaishi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oeu.zdqjudy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bri.0kj1m.cn

PHP:  if (empty($x)) {}
来源：http://uqc.feifeiyinyue.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wae.jinghuilouyu.cn

TS:   if (x == null) {}
来源：http://gcz.jlsjyb.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://doo.yuxming.cn

Go:   if x == nil {}
来源：http://jgr.dianchejie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://drz.ehwqpu.com

C#:   if (x is null) {}
来源：http://paf.0kj1m.cn

[P07] 防抖与节流
来源：http://ncs.yangfankeji.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yjo.gaohongyu789.top

PHP:  // 手写时间戳比较
来源：http://avx.hnqzz.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://whg.xziqi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qic.tanke756.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mzm.sweek.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gmr.zhaomingkeji.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://pdr.smart0.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yrr.smart0.xyz

[P08] 处理浮点精度问题
来源：http://dvo.fengsongda.top


<!-- 参考信息 -->