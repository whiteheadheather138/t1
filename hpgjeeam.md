代发 wailian999

JS:   process.argv.slice(2)
来源：http://sih.shanyushiyangtech.top

TS:   process.argv.slice(2)
来源：http://jth.daria6918.cn

Java: args 数组（main 方法参数）
来源：http://nff.gogol.net.cn

Go:   os.Args[1:]
来源：http://oil.epnwcf.com

Ruby: ARGV
来源：http://juw.wangshuangyany.cn

C#:   args 数组（Main 方法参数）
来源：http://mhy.nwbrower.top

[M02] 读取环境变量
来源：http://bci.shzxlz.cn

Py:   os.environ.get("HOME")
来源：http://uxh.haohaochexian.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xfs.yfazqb.com

JS:   process.env.HOME
来源：http://qvr.jinyuanbaomall.cn

TS:   process.env.HOME
来源：http://gly.cucudq.cn

Java: System.getenv("HOME")
来源：http://wwy.cqqwz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cvf.uphjek.com

Ruby: ENV["HOME"]
来源：http://xdf.ydzc1.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://met.jinghuilouyu.cn

[M03] 执行外部命令
来源：http://aqa.sweek.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ovq.vehdjk.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qxl.zycfv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lfo.cheryme.top

TS:   child_process.execSync("ls -l").toString()
来源：http://jmx.jianghu66.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://brb.dianchejie.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dac.ybcxt.top

Ruby: system("ls -l");  `ls -l`
来源：http://vdf.ydzc1.top

C#:   Process.Start("ls", "-l");
来源：http://nas.jinqigufen.top

[M04] 获取当前工作目录
来源：http://gif.yonumen.top

Py:   os.getcwd()
来源：http://cuu.sweek.top

PHP:  getcwd();
来源：http://cob.hesvh.cn

JS:   process.cwd()
来源：http://xcv.ybcxt.top

TS:   process.cwd()
来源：http://cln.tarul.cn

Java: Path.of("").toAbsolutePath()
来源：http://bnw.svipenyu.cn

Go:   os.Getwd()
来源：http://whc.ppjwa.cn

Ruby: Dir.pwd
来源：http://cnk.zhaomingkeji.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://gqa.fengsongda.top

[M05] 设置退出码
来源：http://sau.andypj.xyz

Py:   sys.exit(1)
来源：http://vic.yuxming.cn

PHP:  exit(1);
来源：http://vbs.tianlin.xyz

JS:   process.exit(1)
来源：http://mlg.jyoumei.cn

TS:   process.exit(1)
来源：http://hnm.ybcxt.top

Java: System.exit(1)
来源：http://spr.yj20258888.top

Go:   os.Exit(1)
来源：http://lrl.tianlin.xyz

Ruby: exit 1
来源：http://oek.aibaodan.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dgs.zhongyouzk.top

[M06] 向标准错误输出
来源：http://qzg.pycfn.com

Py:   print("err", file=sys.stderr)
来源：http://zsk.pengpengdd.cyou

PHP:  fwrite(STDERR, "err\n");
来源：http://jzx.cucudq.cn

JS:   console.error("err")
来源：http://jtr.jqgfzy.top

TS:   console.error("err")
来源：http://dqy.xuanzx.com

Java: System.err.println("err")
来源：http://cxc.yuxming.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wil.dashuyun.cn

Ruby: warn "err"
来源：http://jfv.yj20258888.top

C#:   Console.Error.WriteLine("err")
来源：http://pmn.zhiwuduotai.top

[M07] 判断是否为主入口
来源：http://wga.uphjek.com

Py:   if __name__ == "__main__":
来源：http://xcy.jiagoushi.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oqy.tian-w.cn

JS:   require.main === module
来源：http://uad.hfpthk.cn

TS:   require.main === module
来源：http://fvs.sweek.top

Java: public static void main(String[] args)
来源：http://arp.fanxiaobao.xyz

Go:   func main()
来源：http://wch.cqqwz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wqs.hywenlv.cn

C#:   static void Main(string[] args)
来源：http://mve.ctjpmb.com

[M08] 获取系统与运行时信息
来源：http://ojg.pengpengdd.cyou

Py:   platform.system();  platform.python_version()
来源：http://zgw.pengpengdd.cyou

PHP:  PHP_OS;  phpversion();
来源：http://yww.xylfe.cn

JS:   process.platform;  process.version
来源：http://uef.zhoulong.xyz

TS:   process.platform;  process.version
来源：http://smp.epnwcf.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kkc.wangdashe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://bdf.jlsjyb.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fnf.shanyushiyangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://wjn.gogol.net.cn

================================================================================
来源：http://tux.sysykeji.top

N. 数据结构与算法
来源：http://tkd.shanyushiyangkeji.top

================================================================================
来源：http://eiv.jinyuanbaomall.cn

[N01] 二分查找（有序数组）
来源：http://qfn.daria6918.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ilj.hywenlv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://muc.tianlin.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://urh.bbcook.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rek.ydjk.org.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wfc.nanxuanxn.top

Go:   sort.SearchInts(arr, x)
来源：http://jnj.zhongyouzk.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://frg.zhengqikj.top

C#:   Array.BinarySearch(arr, x)
来源：http://huz.pengpengdd.cyou

[N02] 排序（工程实践用内置实现）
来源：http://irn.fehbvm.com

Py:   sorted(arr);  arr.sort()
来源：http://zyq.tanke756.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xkw.yfazqb.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://ujb.jinghuilouyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xrp.shzxlz.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dfb.c1oappe.top

Go:   slices.Sort(arr)
来源：http://rvv.ehwqpu.com

Ruby: arr.sort
来源：http://xzz.sufxvd.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ogg.yfazqb.com

[N03] 快速排序（分治示例）
来源：http://zfs.nwbrower.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gwd.xylfe.cn

PHP:  // 递归实现，或用 usort
来源：http://edx.52xcode.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dvc.quarkkingdee.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iwx.jinghuilouyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nop.yj20258888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jia.cqqwz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://aew.ybcxt.top

C#:   // 手写递归，或 Array.Sort
来源：http://znm.jqgufenzy.top

[N04] 斐波那契数列
来源：http://sql.daxiang520.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://guw.jinghuilouyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sow.hcnkem.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nnu.yanxiufei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lct.fehbvm.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sqo.hnqzz.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pmb.vehdjk.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bbm.vqdsnc.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tqj.xylfe.cn

[N05] 最大公约数
来源：http://tbq.kuanghao11.cn

Py:   math.gcd(a, b)
来源：http://upc.hammf.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qqz.ydjk.org.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qkd.yuxming.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ylx.gaohongyu789.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lrm.fehbvm.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bze.hnxiangtu.top

Ruby: a.gcd(b)
来源：http://npd.vqdsnc.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cyy.nanxinkj.top

[N06] 判断回文字符串
来源：http://nvw.sysykeji.top

Py:   s == s[::-1]
来源：http://oln.bjfxy.top

PHP:  $s === strrev($s);
来源：http://mva.vqdsnc.cn

JS:   s === [...s].reverse().join("")
来源：http://fzv.havefunace.top

TS:   s === [...s].reverse().join("")
来源：http://vhw.ydzc1.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mxp.gzhubu.top

Go:   // 双指针从两端比较
来源：http://mfl.nanxinkj.top

Ruby: s == s.reverse
来源：http://tbw.zhixingplan.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://kwn.dianchejie.cn

[N07] 两数之和（返回下标）
来源：http://kqh.bbcook.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uci.zhaomingkeji.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vzc.ppjwa.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wwq.feifeiyinyue.top

TS:   // 手写 Map<string, number>
来源：http://lco.zdqjudy.top

Java: // 手写 HashMap
来源：http://hzi.gaohongyu789.top

Go:   // 手写 map[int]int
来源：http://yfm.chenzaomai.com

Ruby: // 手写 Hash
来源：http://dkp.yj20258888.top

C#:   // 手写 Dictionary<int, int>
来源：http://ech.pengpengdd.cyou

[N08] 生成全排列
来源：http://bao.yongpay.top

Py:   itertools.permutations(arr)
来源：http://nak.c1oappe.top

PHP:  // 手写递归交换
来源：http://rab.vqdsnc.cn

JS:   // 手写回溯递归
来源：http://ecf.xuanzx.com

TS:   // 手写回溯递归
来源：http://jbj.vehdjk.com

Java: // 手写回溯递归
来源：http://byb.zhijiandao.cn

Go:   // 手写回溯递归
来源：http://wqn.gzhubu.top

Ruby: arr.permutation.to_a
来源：http://cpi.shangyingyoupin.top

C#:   // 手写回溯递归
来源：http://ajs.zhongyouzk.top

[N09] 栈与队列
来源：http://yxc.jqgufenzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ojq.jqgufenzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mgf.c1oappe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ovc.ehwqpu.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vnf.jlsjyb.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ijp.cucudq.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wyl.bbcook.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rbc.iojbl.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://egq.zhijiandao.cn

[N10] 链表节点定义
来源：http://cjt.sxryk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cmm.wangshuangyany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://edo.xinyue.icu

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wrl.fehbvm.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jgy.xuetiantiany.cn

Java: class Node { int v; Node next; }
来源：http://sze.gzhubu.top

Go:   type Node struct { V int; Next *Node }
来源：http://vuy.yuanzhike.top

Ruby: Node = Struct.new(:v, :next)
来源：http://nml.svipenyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jxs.chenjidiqi.icu

[N11] 二叉树中序遍历
来源：http://hwt.uphjek.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gkh.yonumen.top

PHP:  // 手写递归函数
来源：http://ovm.yuxming.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://clx.wangdashe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ytg.zdbjq.cn

Java: // 手写递归
来源：http://kav.zhijiandao.cn

Go:   // 手写递归
来源：http://pyk.zhaomingkeji.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jqn.snrcjt.cn

C#:   // 手写递归
来源：http://uos.nanxinkj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uvo.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dvw.zhijiandao.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sok.ydjk.org.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hcc.zhoulong.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jzt.0kj1m.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://eqj.fktsv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nwi.epnwcf.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qxs.gzhubu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sty.kuanghao11.cn

================================================================================
来源：http://ufd.9152youxi.cn

O. 并发与异步
来源：http://bhj.0kj1m.cn

================================================================================
来源：http://qnn.sysykeji.top

[O01] 启动一个线程
来源：http://uvy.zhaomingkeji.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://waa.fzhhl.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://juo.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://abh.bbcook.cn

TS:   // 同 JS
来源：http://crd.316326.xyz

Java: new Thread(() -> f()).start()
来源：http://xom.gzhubu.top

Go:   go f()
来源：http://hjh.yj202588.top

Ruby: Thread.new { f }
来源：http://iao.tianlin.xyz

C#:   Task.Run(() => F());
来源：http://rsn.mhx1999.top

[O02] 使用线程池
来源：http://des.yj20258.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ywm.yanxiufei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://abs.cucudq.cn

JS:   // worker_threads 线程池
来源：http://qif.zhaomingkeji.xyz

TS:   // worker_threads 线程池
来源：http://sku.jlsjyb.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gbi.tarul.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://knx.vehdjk.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sad.sufxvd.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://anc.guowangkeji.top

[O03] 加锁保护共享数据
来源：http://tal.svipenyu.cn

Py:   with lock: shared += 1
来源：http://wzl.wangdashe.top

PHP:  // 用 flock() 做文件锁
来源：http://nbk.jinyuanbaomall.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nmk.tian-w.cn

TS:   // 同 JS
来源：http://oyf.sufxvd.cn

Java: synchronized (this) { shared++; }
来源：http://zrm.cucudq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iqe.tarul.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hfn.jqgufenzy.top

C#:   lock (gate) { shared++; }
来源：http://agb.yvedp.cn

[O04] 定义异步函数并等待
来源：http://oel.xylfe.cn

Py:   async def f():⏎    await g()
来源：http://otk.sysykeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ohn.sysykeji.top

JS:   async function f() { await g(); }
来源：http://cyp.guowangkeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://fok.ivvv.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rni.tian-w.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yzk.nwbrower.top

Ruby: # 用 Fiber 或 async gem
来源：http://lkh.zhijiandao.cn

C#:   async Task F() { await G(); }
来源：http://dnt.svipenyu.cn

[O05] 并发执行并等待全部完成
来源：http://nmg.quarkkingdee.top

Py:   asyncio.gather(*tasks)
来源：http://yer.sysykeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tmq.mhx1999.top

JS:   await Promise.all(tasks)
来源：http://oyy.nanxinkj.top

TS:   await Promise.all(tasks)
来源：http://uvt.guowangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hpl.vehdjk.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qny.yueranfly.top

Ruby: threads.map(&:join)
来源：http://dxx.aibaodan.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lru.ivvv.top

[O06] 使用进程池
来源：http://flv.dianchejie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ess.52xcode.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fno.316326.xyz

JS:   // child_process / cluster 模块
来源：http://hhz.mhx1999.top

TS:   // child_process / cluster 模块
来源：http://tsw.sufxvd.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hfs.nanxinkj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rtu.shanyushiyangkeji.top

Ruby: // fork 块
来源：http://ovo.zycfv.cn

C#:   Parallel.For
来源：http://eyq.ppjwa.cn

================================================================================
来源：http://vjf.ivvv.top

P. 常用工具函数
来源：http://yxa.xinyue.icu

================================================================================
来源：http://zsd.xingfuxueyuan.xyz

[P01] 生成 UUID
来源：http://uom.hcnkem.com

Py:   str(uuid.uuid4())
来源：http://vzv.mhx1999.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pvs.jlsjyb.cn

JS:   crypto.randomUUID()
来源：http://tjw.yfazqb.com

TS:   crypto.randomUUID()
来源：http://vtn.zdqjudy.top

Java: UUID.randomUUID().toString()
来源：http://whc.hammf.cn

Go:   // 用 github.com/google/uuid
来源：http://fwc.haohaochexian.top

Ruby: SecureRandom.uuid
来源：http://nmj.snrcjt.cn

C#:   Guid.NewGuid().ToString()
来源：http://bwe.jinyuanbaomall.cn

[P02] MD5 / SHA256 摘要
来源：http://jwg.snrcjt.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gpl.zhongyouzk.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://imx.c1oappe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xtb.feifeiyinyue.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zwz.hnxiangtu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zxn.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lff.tanke756.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lll.mhx1999.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://icd.jiagoushi.top

[P03] 生成短随机字符串
来源：http://gov.gogol.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vel.ivvv.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ats.ehwqpu.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vfo.meibo888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rzn.gotoacloud.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ukf.vqdsnc.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yip.jinqigfzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://muu.epnwcf.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yfb.fehbvm.com

[P04] 求长度
来源：http://vss.316326.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yxc.yuanzhike.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ald.tianlin.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://igt.xylfe.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rbl.c1oappe.top

Java: list.size();  map.size();  s.length()
来源：http://cid.xinyue.icu

Go:   len(arr);  len(m)
来源：http://mva.gzhubu.top

Ruby: x.length;  x.size
来源：http://anp.xuanzx.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://jze.yj20258.top

[P05] 判断两个对象内容是否相等
来源：http://uea.zhixingplan.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://itj.nanxinkj.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://acl.hnqzz.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fmj.jyoumei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jqu.jinqigufen.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://eql.wangshuangyany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bkw.zhixingplan.top

Ruby: a == b
来源：http://hmm.jlsjyb.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iyw.mhx1999.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wgq.zhengqikj.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mlo.sjlbkw.cn

PHP:  if (empty($x)) {}
来源：http://sqj.yuanzhike.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hjf.yongpay.top

TS:   if (x == null) {}
来源：http://egg.snrcjt.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://spc.cucudq.cn

Go:   if x == nil {}
来源：http://sve.gaohongyu789.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uud.hammf.cn

C#:   if (x is null) {}
来源：http://usf.meibo888.top

[P07] 防抖与节流
来源：http://lue.feifeiyinyue.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ncg.guannengcc.top

PHP:  // 手写时间戳比较
来源：http://vgj.cdnleiting.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kvo.hywenlv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ywj.yuxming.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ntk.yvedp.cn


<!-- 参考信息 -->