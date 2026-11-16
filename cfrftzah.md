代发 wailian999

Ruby: ARGV
来源：http://rsr.fzhhl.top

C#:   args 数组（Main 方法参数）
来源：http://xvv.haohaochexian.top

[M02] 读取环境变量
来源：http://lcq.316326.xyz

Py:   os.environ.get("HOME")
来源：http://dfe.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gap.hnxiangtu.top

JS:   process.env.HOME
来源：http://cgw.nanxuanxn.top

TS:   process.env.HOME
来源：http://akb.hesvh.cn

Java: System.getenv("HOME")
来源：http://vpw.jinyuanbaomall.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jkq.iojbl.cn

Ruby: ENV["HOME"]
来源：http://xkm.yfazqb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cce.yongpay.top

[M03] 执行外部命令
来源：http://yvl.pengpengdd.cyou

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tor.epnwcf.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://whx.svipenyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vez.uphjek.com

TS:   child_process.execSync("ls -l").toString()
来源：http://rqr.jqgfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://oeo.sjlbkw.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vxx.vqdsnc.cn

Ruby: system("ls -l");  `ls -l`
来源：http://snk.gogol.net.cn

C#:   Process.Start("ls", "-l");
来源：http://egi.52xcode.cn

[M04] 获取当前工作目录
来源：http://izm.sufxvd.cn

Py:   os.getcwd()
来源：http://war.sjlbkw.cn

PHP:  getcwd();
来源：http://vgc.jqgfzy.top

JS:   process.cwd()
来源：http://bzv.ywan-chungtsiang.top

TS:   process.cwd()
来源：http://mpb.zhaomingkeji.xyz

Java: Path.of("").toAbsolutePath()
来源：http://sgx.havefunace.top

Go:   os.Getwd()
来源：http://apr.yueranfly.top

Ruby: Dir.pwd
来源：http://xmz.jinqigfzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://llh.sjlbkw.cn

[M05] 设置退出码
来源：http://hrt.yongpay.top

Py:   sys.exit(1)
来源：http://jqk.ehwqpu.com

PHP:  exit(1);
来源：http://jsq.xingfuxueyuan.xyz

JS:   process.exit(1)
来源：http://npe.yj202588.top

TS:   process.exit(1)
来源：http://idd.cqqwz.cn

Java: System.exit(1)
来源：http://vvo.gzhubu.top

Go:   os.Exit(1)
来源：http://fdl.zhaomingkeji.xyz

Ruby: exit 1
来源：http://hni.sufxvd.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dgq.aizwys.cn

[M06] 向标准错误输出
来源：http://zkw.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://wln.aizwys.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hxq.yongpay.top

JS:   console.error("err")
来源：http://ghp.cqqwz.cn

TS:   console.error("err")
来源：http://xqz.hfpthk.cn

Java: System.err.println("err")
来源：http://mhb.tian-w.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yrg.gaohongyu789.top

Ruby: warn "err"
来源：http://hay.dianchejie.cn

C#:   Console.Error.WriteLine("err")
来源：http://ddl.52xcode.cn

[M07] 判断是否为主入口
来源：http://wop.shuidangran.top

Py:   if __name__ == "__main__":
来源：http://avy.daria6918.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://omy.yvedp.cn

JS:   require.main === module
来源：http://pvt.cucudq.cn

TS:   require.main === module
来源：http://has.fzhhl.top

Java: public static void main(String[] args)
来源：http://jmo.hysaishi.cn

Go:   func main()
来源：http://jim.sxryk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://muf.tarul.cn

C#:   static void Main(string[] args)
来源：http://fee.yongpay.top

[M08] 获取系统与运行时信息
来源：http://cya.meibo888.top

Py:   platform.system();  platform.python_version()
来源：http://are.guannengcc.top

PHP:  PHP_OS;  phpversion();
来源：http://xgl.shanyushiyangkeji.top

JS:   process.platform;  process.version
来源：http://ijc.uphjek.com

TS:   process.platform;  process.version
来源：http://qau.sweek.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://aqr.0kj1m.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ila.wangshuangyany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kfx.shanyushiyangtech.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tdz.zhaomingkeji.xyz

================================================================================
来源：http://zgu.jinqigufen.top

N. 数据结构与算法
来源：http://cry.cqqwz.cn

================================================================================
来源：http://ayk.shangyingyoupin.top

[N01] 二分查找（有序数组）
来源：http://vgn.xingfuxueyuan.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://zzy.jqgufenzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vls.quarkkingdee.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jbz.ybcxt.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://grq.andypj.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://zxe.meibo888.top

Go:   sort.SearchInts(arr, x)
来源：http://jyh.fktsv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qnx.jinyuanbaomall.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sil.hammf.cn

[N02] 排序（工程实践用内置实现）
来源：http://kvc.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://iak.wangdashe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cug.aibaodan.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nhv.jinqigufen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jjf.jinqigfzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pge.yvedp.cn

Go:   slices.Sort(arr)
来源：http://cap.zhixingplan.top

Ruby: arr.sort
来源：http://jqg.xuanzx.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://yeo.xziqi.cn

[N03] 快速排序（分治示例）
来源：http://uwo.redwolf501.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nfc.cdnleiting.top

PHP:  // 递归实现，或用 usort
来源：http://thl.ywan-chungtsiang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hfh.yj20258888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vyf.tianlin.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jrz.sxryk.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xna.ivvv.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kgp.sxryk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vhw.zycfv.cn

[N04] 斐波那契数列
来源：http://gkm.jinghuilouyu.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://osh.birdmap.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wgj.pycfn.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nav.jqgufenzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rhp.haohaochexian.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yjr.cucudq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://pct.hnxiangtu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wea.sjlbkw.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vzc.sysykeji.top

[N05] 最大公约数
来源：http://bzf.jqgfzy.top

Py:   math.gcd(a, b)
来源：http://hjo.xylfe.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qzr.daria6918.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zhl.tanke756.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://thy.hcnkem.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ben.jyoumei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hyc.zdbjq.cn

Ruby: a.gcd(b)
来源：http://tpd.jiagoushi.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wcv.sxryk.cn

[N06] 判断回文字符串
来源：http://nip.316326.xyz

Py:   s == s[::-1]
来源：http://azo.svipenyu.cn

PHP:  $s === strrev($s);
来源：http://qvl.zhongyouzk.top

JS:   s === [...s].reverse().join("")
来源：http://vps.9152youxi.cn

TS:   s === [...s].reverse().join("")
来源：http://gbm.zdqjudy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hvy.nanxinkj.top

Go:   // 双指针从两端比较
来源：http://tms.sjlbkw.cn

Ruby: s == s.reverse
来源：http://zix.xuetiantiany.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yys.guannengcc.top

[N07] 两数之和（返回下标）
来源：http://yes.andypj.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vwt.cashguo.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fue.yonumen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://slh.yuxming.cn

TS:   // 手写 Map<string, number>
来源：http://vih.jlsjyb.cn

Java: // 手写 HashMap
来源：http://mad.shanyushiyangkeji.top

Go:   // 手写 map[int]int
来源：http://swt.yj202588.top

Ruby: // 手写 Hash
来源：http://pyq.feifeiyinyue.top

C#:   // 手写 Dictionary<int, int>
来源：http://qqn.feifeiyinyue.top

[N08] 生成全排列
来源：http://ymj.jinghuilouyu.cn

Py:   itertools.permutations(arr)
来源：http://guu.yonumen.top

PHP:  // 手写递归交换
来源：http://ggj.fanxiaobao.xyz

JS:   // 手写回溯递归
来源：http://geo.sjlbkw.cn

TS:   // 手写回溯递归
来源：http://slg.bjfxy.top

Java: // 手写回溯递归
来源：http://jdy.guowangkeji.top

Go:   // 手写回溯递归
来源：http://fib.yuanzhike.top

Ruby: arr.permutation.to_a
来源：http://sde.mhx1999.top

C#:   // 手写回溯递归
来源：http://unc.316326.xyz

[N09] 栈与队列
来源：http://ysd.xuetiantiany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dkm.hfpthk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://luv.shanyushiyangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vwr.haohaochexian.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fwp.wangdashe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ibi.yangfankeji.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://plu.jyoumei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xmj.jinqigfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iel.zhoulong.xyz

[N10] 链表节点定义
来源：http://rds.mhx1999.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://axc.yanxiufei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gaz.jinyuanbaomall.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lat.cashguo.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lys.chenjidiqi.icu

Java: class Node { int v; Node next; }
来源：http://fxq.ehwqpu.com

Go:   type Node struct { V int; Next *Node }
来源：http://oar.ywan-chungtsiang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://qzm.hesvh.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cgx.jqgfzy.top

[N11] 二叉树中序遍历
来源：http://vpn.uphjek.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tse.tarul.cn

PHP:  // 手写递归函数
来源：http://oee.jlsjyb.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mrt.cqqwz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xxl.smart0.xyz

Java: // 手写递归
来源：http://kaw.chenlongwang.top

Go:   // 手写递归
来源：http://nia.pengpengdd.cyou

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jef.jyoumei.cn

C#:   // 手写递归
来源：http://efa.tianlin.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zdu.shuidangran.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sud.tanke756.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://how.gzhubu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xsw.gotoacloud.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tpp.fehbvm.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oqi.dashuyun.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qsv.0kj1m.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rft.haohaochexian.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vhv.tian-w.cn

================================================================================
来源：http://usj.0kj1m.cn

O. 并发与异步
来源：http://daa.mhx1999.top

================================================================================
来源：http://nxy.guowangkeji.top

[O01] 启动一个线程
来源：http://hns.wangshuangyany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fuc.haohaochexian.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mxh.cucudq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bik.bjfxy.top

TS:   // 同 JS
来源：http://qyv.fanxiaobao.xyz

Java: new Thread(() -> f()).start()
来源：http://rkh.aizwys.cn

Go:   go f()
来源：http://mbq.hammf.cn

Ruby: Thread.new { f }
来源：http://tsq.tanke756.top

C#:   Task.Run(() => F());
来源：http://cgq.nanxinkj.top

[O02] 使用线程池
来源：http://jif.mhx1999.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qpw.pycfn.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ang.aizwys.cn

JS:   // worker_threads 线程池
来源：http://hio.tianlin.xyz

TS:   // worker_threads 线程池
来源：http://iff.fktsv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bjc.gaohongyu789.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zqt.feifeiyinyue.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xog.jinghuilouyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://avy.xinyue.icu

[O03] 加锁保护共享数据
来源：http://muw.yuanzhike.top

Py:   with lock: shared += 1
来源：http://irv.fengsongda.top

PHP:  // 用 flock() 做文件锁
来源：http://lsd.nanxuanxn.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zsn.zhongyouzk.top

TS:   // 同 JS
来源：http://etr.pengpengdd.cyou

Java: synchronized (this) { shared++; }
来源：http://npk.andypj.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yok.aibaodan.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yhk.hywenlv.cn

C#:   lock (gate) { shared++; }
来源：http://icg.redwolf501.top

[O04] 定义异步函数并等待
来源：http://cii.svipenyu.cn

Py:   async def f():⏎    await g()
来源：http://dmn.ehwqpu.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zky.zhongyouzk.top

JS:   async function f() { await g(); }
来源：http://bbb.redwolf501.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://itl.ctjpmb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ysr.ydzc1.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yus.cqqwz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ohx.zhijiandao.cn

C#:   async Task F() { await G(); }
来源：http://qnx.chenzaomai.com

[O05] 并发执行并等待全部完成
来源：http://fky.yvedp.cn

Py:   asyncio.gather(*tasks)
来源：http://qmo.0kj1m.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gem.xuanzx.com

JS:   await Promise.all(tasks)
来源：http://aqn.jyoumei.cn

TS:   await Promise.all(tasks)
来源：http://fql.jianghu66.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ipa.mhx1999.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fgf.fengsongda.top

Ruby: threads.map(&:join)
来源：http://auj.wangshuangyany.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ibj.fehbvm.com

[O06] 使用进程池
来源：http://rsf.chenzaomai.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gte.hysaishi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://pax.vehdjk.com

JS:   // child_process / cluster 模块
来源：http://bue.tanke756.top

TS:   // child_process / cluster 模块
来源：http://gjn.vehdjk.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://scw.ppjwa.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://iyd.hammf.cn

Ruby: // fork 块
来源：http://gyi.hywenlv.cn

C#:   Parallel.For
来源：http://itw.jqgufenzy.top

================================================================================
来源：http://hqo.ydzc1.top

P. 常用工具函数
来源：http://skc.daxiang520.top

================================================================================
来源：http://esm.ybcxt.top

[P01] 生成 UUID
来源：http://kmi.yonumen.top

Py:   str(uuid.uuid4())
来源：http://pla.yongpay.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vzh.52xcode.cn

JS:   crypto.randomUUID()
来源：http://kxg.zycfv.cn

TS:   crypto.randomUUID()
来源：http://txa.gotoacloud.top

Java: UUID.randomUUID().toString()
来源：http://uxc.guannengcc.top

Go:   // 用 github.com/google/uuid
来源：http://nma.fktsv.cn

Ruby: SecureRandom.uuid
来源：http://hjc.xingfuxueyuan.xyz

C#:   Guid.NewGuid().ToString()
来源：http://zxl.cdnleiting.top

[P02] MD5 / SHA256 摘要
来源：http://pgz.cqqwz.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hrc.jyoumei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://iog.zhijiandao.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yio.9152youxi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://amd.52xcode.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ghd.hywenlv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://niq.zdqjudy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vcc.ywan-chungtsiang.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hwo.ehwqpu.com

[P03] 生成短随机字符串
来源：http://egh.sufxvd.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://unx.jyoumei.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bqb.kuanghao11.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gpm.iojbl.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://huw.zhaomingkeji.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qjh.cucudq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kie.ydzc1.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://yas.redwolf501.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rhu.yanxiufei.cn

[P04] 求长度
来源：http://nnw.ivvv.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kxo.jiagoushi.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wwr.shzxlz.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hpp.sysykeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://epf.gzhubu.top

Java: list.size();  map.size();  s.length()
来源：http://gsy.havefunace.top

Go:   len(arr);  len(m)
来源：http://zso.haohaochexian.top

Ruby: x.length;  x.size
来源：http://dzk.zhijiandao.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://xxo.bjfxy.top

[P05] 判断两个对象内容是否相等
来源：http://kmp.bjfxy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://eht.fktsv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kyb.hywenlv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dlp.nwbrower.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ghf.xylfe.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ulh.vehdjk.com

Go:   reflect.DeepEqual(a, b)
来源：http://rvj.bbcook.cn

Ruby: a == b
来源：http://bhw.wangdashe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wwj.yj202588.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bby.hesvh.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hus.epnwcf.com

PHP:  if (empty($x)) {}
来源：http://uvm.tian-w.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hku.zhiwuduotai.top

TS:   if (x == null) {}
来源：http://mkc.316326.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://dqe.yangfankeji.com

Go:   if x == nil {}
来源：http://oyx.hcnkem.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jxp.cucudq.cn

C#:   if (x is null) {}
来源：http://naj.aizwys.cn

[P07] 防抖与节流
来源：http://jfh.hywenlv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oxa.hywenlv.cn

PHP:  // 手写时间戳比较
来源：http://bfz.haohaochexian.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wlu.hysaishi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cwq.andypj.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nbo.hnqzz.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uxq.jinyuanbaomall.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://uaz.yj20258888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kcn.yuxming.cn

[P08] 处理浮点精度问题
来源：http://fdv.guannengcc.top


<!-- 参考信息 -->