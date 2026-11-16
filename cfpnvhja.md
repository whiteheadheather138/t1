代发 wailian999

Ruby: ARGV
来源：http://knj.zdbjq.cn

C#:   args 数组（Main 方法参数）
来源：http://dda.hesvh.cn

[M02] 读取环境变量
来源：http://bey.ppjwa.cn

Py:   os.environ.get("HOME")
来源：http://mhw.hywenlv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vwb.svipenyu.cn

JS:   process.env.HOME
来源：http://hvj.dianchejie.cn

TS:   process.env.HOME
来源：http://lsd.sufxvd.cn

Java: System.getenv("HOME")
来源：http://emp.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fld.yj20258888.top

Ruby: ENV["HOME"]
来源：http://lvr.sysykeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ipm.havefunace.top

[M03] 执行外部命令
来源：http://vsy.jlsjyb.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://awj.guowangkeji.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://yat.yueranfly.top

JS:   child_process.execSync("ls -l").toString()
来源：http://rmx.yuxming.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oln.jinqigufen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rhc.jyoumei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://osb.hongshengwenyu.top

Ruby: system("ls -l");  `ls -l`
来源：http://mkr.shanyushiyangtech.top

C#:   Process.Start("ls", "-l");
来源：http://bhg.hfpthk.cn

[M04] 获取当前工作目录
来源：http://vfa.xuanzx.com

Py:   os.getcwd()
来源：http://bko.yfazqb.com

PHP:  getcwd();
来源：http://lsy.hnxiangtu.top

JS:   process.cwd()
来源：http://fby.yfazqb.com

TS:   process.cwd()
来源：http://clp.fzhhl.top

Java: Path.of("").toAbsolutePath()
来源：http://gsa.chenzaomai.com

Go:   os.Getwd()
来源：http://yiu.xinyue.icu

Ruby: Dir.pwd
来源：http://oki.c1oappe.top

C#:   Directory.GetCurrentDirectory()
来源：http://yhn.fzhhl.top

[M05] 设置退出码
来源：http://mtu.yfazqb.com

Py:   sys.exit(1)
来源：http://zca.0kj1m.cn

PHP:  exit(1);
来源：http://gee.xingfuxueyuan.xyz

JS:   process.exit(1)
来源：http://dvz.yangfankeji.com

TS:   process.exit(1)
来源：http://zhr.ydzc1.top

Java: System.exit(1)
来源：http://mta.c1oappe.top

Go:   os.Exit(1)
来源：http://ipj.hnxiangtu.top

Ruby: exit 1
来源：http://cqf.xuanzx.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://srs.dianchejie.cn

[M06] 向标准错误输出
来源：http://nhk.zhijiandao.cn

Py:   print("err", file=sys.stderr)
来源：http://kgt.tarul.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zvz.snrcjt.cn

JS:   console.error("err")
来源：http://llt.chenzaomai.com

TS:   console.error("err")
来源：http://rpp.feifeiyinyue.top

Java: System.err.println("err")
来源：http://frt.pengpengdd.cyou

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tpt.shanyushiyangkeji.top

Ruby: warn "err"
来源：http://hvf.ywan-chungtsiang.top

C#:   Console.Error.WriteLine("err")
来源：http://wlm.jinghuilouyu.cn

[M07] 判断是否为主入口
来源：http://kcp.chenzaomai.com

Py:   if __name__ == "__main__":
来源：http://qes.yj20258888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cjn.jlsjyb.cn

JS:   require.main === module
来源：http://sfx.yanxiufei.cn

TS:   require.main === module
来源：http://uva.vqdsnc.cn

Java: public static void main(String[] args)
来源：http://wni.fktsv.cn

Go:   func main()
来源：http://jkj.0kj1m.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ury.sysykeji.top

C#:   static void Main(string[] args)
来源：http://jut.tianlin.xyz

[M08] 获取系统与运行时信息
来源：http://oam.daxiang520.top

Py:   platform.system();  platform.python_version()
来源：http://wcv.bbcook.cn

PHP:  PHP_OS;  phpversion();
来源：http://uqu.shanyushiyangkeji.top

JS:   process.platform;  process.version
来源：http://hsn.pycfn.com

TS:   process.platform;  process.version
来源：http://nil.yonumen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zuu.gotoacloud.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fqs.zhengqikj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://uay.vqdsnc.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://vdi.yj20258888.top

================================================================================
来源：http://kes.shanyushiyangtech.top

N. 数据结构与算法
来源：http://ked.ctjpmb.com

================================================================================
来源：http://lfc.aibaodan.cn

[N01] 二分查找（有序数组）
来源：http://mjq.gaohongyu789.top

Py:   bisect.bisect_left(arr, x)
来源：http://klu.gotoacloud.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xob.c1oappe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tbr.tarul.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://riu.andypj.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://yla.sysykeji.top

Go:   sort.SearchInts(arr, x)
来源：http://ylv.ivvv.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://fnu.hnqzz.top

C#:   Array.BinarySearch(arr, x)
来源：http://yam.zycfv.cn

[N02] 排序（工程实践用内置实现）
来源：http://erc.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://aup.ydjk.org.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wzr.snrcjt.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sxk.tarul.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://cax.yvedp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xgm.hongshengwenyu.top

Go:   slices.Sort(arr)
来源：http://zft.sjlbkw.cn

Ruby: arr.sort
来源：http://nth.quarkkingdee.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ewh.yangfankeji.com

[N03] 快速排序（分治示例）
来源：http://avr.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lmt.chenlongwang.top

PHP:  // 递归实现，或用 usort
来源：http://qmg.zhaomingkeji.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lgw.aizwys.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qqs.zdqjudy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kai.shanyushiyangtech.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://unp.zhaomingkeji.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nfh.zhongyouzk.top

C#:   // 手写递归，或 Array.Sort
来源：http://zhg.sjlbkw.cn

[N04] 斐波那契数列
来源：http://qwz.hesvh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aif.52xcode.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zyc.9152youxi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kpu.wangdashe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dzq.snrcjt.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jvt.dashuyun.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dle.zhaomingkeji.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mzp.fehbvm.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gjn.zhixingplan.top

[N05] 最大公约数
来源：http://neo.xuetiantiany.cn

Py:   math.gcd(a, b)
来源：http://wle.bjfxy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hom.daxiang520.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kum.gzhubu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cni.redwolf501.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ogg.hfpthk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cmc.yueranfly.top

Ruby: a.gcd(b)
来源：http://mrv.zhixingplan.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pku.jlsjyb.cn

[N06] 判断回文字符串
来源：http://juk.yonumen.top

Py:   s == s[::-1]
来源：http://ibm.ybcxt.top

PHP:  $s === strrev($s);
来源：http://tvd.snrcjt.cn

JS:   s === [...s].reverse().join("")
来源：http://ctd.tian-w.cn

TS:   s === [...s].reverse().join("")
来源：http://epw.zhongyouzk.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xxc.jinqigufen.top

Go:   // 双指针从两端比较
来源：http://vnb.xuanzx.com

Ruby: s == s.reverse
来源：http://mun.nwbrower.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xbb.iojbl.cn

[N07] 两数之和（返回下标）
来源：http://tzd.yvedp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xav.zdbjq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zpy.zhengqikj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wph.hysaishi.cn

TS:   // 手写 Map<string, number>
来源：http://ppq.aibaodan.cn

Java: // 手写 HashMap
来源：http://jci.cdnleiting.top

Go:   // 手写 map[int]int
来源：http://zbv.aizwys.cn

Ruby: // 手写 Hash
来源：http://vid.jinghuilouyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cms.sweek.top

[N08] 生成全排列
来源：http://zld.tian-w.cn

Py:   itertools.permutations(arr)
来源：http://mkq.jinqigufen.top

PHP:  // 手写递归交换
来源：http://xvr.daxiang520.top

JS:   // 手写回溯递归
来源：http://pmf.hnxiangtu.top

TS:   // 手写回溯递归
来源：http://hpw.pycfn.com

Java: // 手写回溯递归
来源：http://lgl.nanxuanxn.top

Go:   // 手写回溯递归
来源：http://kyy.chenlongwang.top

Ruby: arr.permutation.to_a
来源：http://hwi.quarkkingdee.top

C#:   // 手写回溯递归
来源：http://yrd.yuanzhike.top

[N09] 栈与队列
来源：http://hbf.zhaomingkeji.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rzi.xylfe.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mix.yuanzhike.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dyf.gaohongyu789.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ryk.jinqigfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hvg.sweek.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://irw.316326.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tej.316326.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gnm.ydzc1.top

[N10] 链表节点定义
来源：http://gzd.guannengcc.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vya.jianghu66.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fbu.fzhhl.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://udr.jianghu66.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rtu.zhijiandao.cn

Java: class Node { int v; Node next; }
来源：http://fcq.fanxiaobao.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://gvk.svipenyu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://csb.uphjek.com

C#:   class Node { public int V; public Node? Next; }
来源：http://jdn.jlsjyb.cn

[N11] 二叉树中序遍历
来源：http://hwv.shangyingyoupin.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bnm.yj20258.top

PHP:  // 手写递归函数
来源：http://izm.0kj1m.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ulv.xuanzx.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://naj.ehwqpu.com

Java: // 手写递归
来源：http://wkt.hammf.cn

Go:   // 手写递归
来源：http://izx.vqdsnc.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mdd.cheryme.top

C#:   // 手写递归
来源：http://jhm.fengsongda.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xtz.hysaishi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qov.wangshuangyany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xao.daria6918.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tux.ybcxt.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xby.gotoacloud.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dtg.ivvv.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cag.yonumen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dfc.hammf.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://enr.cucudq.cn

================================================================================
来源：http://uxp.ppjwa.cn

O. 并发与异步
来源：http://dax.jinqigufen.top

================================================================================
来源：http://erf.gotoacloud.top

[O01] 启动一个线程
来源：http://ldq.0kj1m.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rxq.tian-w.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wtv.yangfankeji.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tfx.zhiwuduotai.top

TS:   // 同 JS
来源：http://ybh.ehwqpu.com

Java: new Thread(() -> f()).start()
来源：http://gpi.shanyushiyangkeji.top

Go:   go f()
来源：http://bgm.daria6918.cn

Ruby: Thread.new { f }
来源：http://hjc.havefunace.top

C#:   Task.Run(() => F());
来源：http://igx.aibaodan.cn

[O02] 使用线程池
来源：http://nyg.zycfv.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dei.zhiwuduotai.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://azn.hnxiangtu.top

JS:   // worker_threads 线程池
来源：http://nri.gotoacloud.top

TS:   // worker_threads 线程池
来源：http://fqo.fktsv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ksg.cashguo.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dex.jinghuilouyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cbg.jinyuanbaomall.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tod.vqdsnc.cn

[O03] 加锁保护共享数据
来源：http://wlj.quarkkingdee.top

Py:   with lock: shared += 1
来源：http://dqf.shzxlz.cn

PHP:  // 用 flock() 做文件锁
来源：http://mcb.tanke756.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ngk.smart0.xyz

TS:   // 同 JS
来源：http://ypa.nwbrower.top

Java: synchronized (this) { shared++; }
来源：http://jln.jinghuilouyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kpj.bjfxy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://snv.vehdjk.com

C#:   lock (gate) { shared++; }
来源：http://lfq.jqgfzy.top

[O04] 定义异步函数并等待
来源：http://bit.jiagoushi.top

Py:   async def f():⏎    await g()
来源：http://cuv.bjfxy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pxm.gaohongyu789.top

JS:   async function f() { await g(); }
来源：http://spg.hongshengwenyu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vqe.xuetiantiany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lxn.xuetiantiany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xgf.zhixingplan.top

Ruby: # 用 Fiber 或 async gem
来源：http://aju.jinqigufen.top

C#:   async Task F() { await G(); }
来源：http://bcc.guowangkeji.top

[O05] 并发执行并等待全部完成
来源：http://zld.zycfv.cn

Py:   asyncio.gather(*tasks)
来源：http://dub.birdmap.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lbw.gogol.net.cn

JS:   await Promise.all(tasks)
来源：http://qoo.gogol.net.cn

TS:   await Promise.all(tasks)
来源：http://hxb.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zth.9152youxi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wln.sufxvd.cn

Ruby: threads.map(&:join)
来源：http://yqr.smart0.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://ylm.yj20258.top

[O06] 使用进程池
来源：http://met.jlsjyb.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rje.ivvv.top

PHP:  // pcntl_fork 或多进程队列
来源：http://iag.fktsv.cn

JS:   // child_process / cluster 模块
来源：http://bmy.zhoulong.xyz

TS:   // child_process / cluster 模块
来源：http://zrr.zycfv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xsm.nanxuanxn.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://anq.yuanzhike.top

Ruby: // fork 块
来源：http://zms.havefunace.top

C#:   Parallel.For
来源：http://qxd.xylfe.cn

================================================================================
来源：http://weu.xylfe.cn

P. 常用工具函数
来源：http://ltk.shuidangran.top

================================================================================
来源：http://ofp.shangyingyoupin.top

[P01] 生成 UUID
来源：http://ict.shanyushiyangtech.top

Py:   str(uuid.uuid4())
来源：http://oek.mhx1999.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jjv.uphjek.com

JS:   crypto.randomUUID()
来源：http://oqk.quarkkingdee.top

TS:   crypto.randomUUID()
来源：http://oon.jqgufenzy.top

Java: UUID.randomUUID().toString()
来源：http://hdt.ehwqpu.com

Go:   // 用 github.com/google/uuid
来源：http://xxt.ppjwa.cn

Ruby: SecureRandom.uuid
来源：http://vmd.iojbl.cn

C#:   Guid.NewGuid().ToString()
来源：http://wfx.yvedp.cn

[P02] MD5 / SHA256 摘要
来源：http://vds.tarul.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ncc.cheryme.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://mpc.dianchejie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pik.zycfv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zwg.gaohongyu789.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cys.zhiwuduotai.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://omm.0kj1m.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lqp.c1oappe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vzv.vehdjk.com

[P03] 生成短随机字符串
来源：http://tlw.tarul.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://adt.nanxinkj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sfu.sufxvd.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qzk.xylfe.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xbf.gaohongyu789.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://waa.chenlongwang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cpz.nwbrower.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://voi.hysaishi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hql.sjlbkw.cn

[P04] 求长度
来源：http://ntm.ydzc1.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kum.mhx1999.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ofd.uphjek.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dek.jyoumei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://poz.sjlbkw.cn

Java: list.size();  map.size();  s.length()
来源：http://yut.yonumen.top

Go:   len(arr);  len(m)
来源：http://yrk.hammf.cn

Ruby: x.length;  x.size
来源：http://eay.yj20258888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zxn.yj202588.top

[P05] 判断两个对象内容是否相等
来源：http://bqv.316326.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://vtc.hysaishi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fun.aibaodan.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ero.fzhhl.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ydl.316326.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qsy.fanxiaobao.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://dvg.quarkkingdee.top

Ruby: a == b
来源：http://hur.jinqigufen.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lai.tanke756.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zem.ivvv.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aqu.aibaodan.cn

PHP:  if (empty($x)) {}
来源：http://anz.aizwys.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://skh.tarul.cn

TS:   if (x == null) {}
来源：http://ehn.xuetiantiany.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fpq.zdbjq.cn

Go:   if x == nil {}
来源：http://rij.bjfxy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hni.birdmap.top

C#:   if (x is null) {}
来源：http://opc.bbcook.cn

[P07] 防抖与节流
来源：http://ium.zhengqikj.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lcr.tarul.cn

PHP:  // 手写时间戳比较
来源：http://gfi.zhengqikj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qde.jqgfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ghw.yuxming.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rqu.uphjek.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vmk.cdnleiting.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qqu.zhongyouzk.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ubj.fzhhl.top

[P08] 处理浮点精度问题
来源：http://cip.svipenyu.cn


<!-- 参考信息 -->