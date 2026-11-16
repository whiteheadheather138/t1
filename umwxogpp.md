代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dva.aibaodan.cn

Ruby: ENV["HOME"]
来源：http://kej.pycfn.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vid.aizwys.cn

[M03] 执行外部命令
来源：http://uxb.xuanzx.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://spt.zhijiandao.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://iej.pycfn.com

JS:   child_process.execSync("ls -l").toString()
来源：http://zfw.yonumen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vll.yj20258888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mni.xuanzx.com

Go:   exec.Command("ls", "-l").Output()
来源：http://onk.52xcode.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sly.uphjek.com

C#:   Process.Start("ls", "-l");
来源：http://bqe.quarkkingdee.top

[M04] 获取当前工作目录
来源：http://vcb.gzhubu.top

Py:   os.getcwd()
来源：http://cxs.shuidangran.top

PHP:  getcwd();
来源：http://azr.zhijiandao.cn

JS:   process.cwd()
来源：http://hwn.shanyushiyangtech.top

TS:   process.cwd()
来源：http://nfi.pengpengdd.cyou

Java: Path.of("").toAbsolutePath()
来源：http://ptu.yuanzhike.top

Go:   os.Getwd()
来源：http://mmk.gotoacloud.top

Ruby: Dir.pwd
来源：http://azh.fktsv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sgw.wangshuangyany.cn

[M05] 设置退出码
来源：http://vky.feifeiyinyue.top

Py:   sys.exit(1)
来源：http://xph.gogol.net.cn

PHP:  exit(1);
来源：http://pow.gogol.net.cn

JS:   process.exit(1)
来源：http://jtw.gaohongyu789.top

TS:   process.exit(1)
来源：http://cuo.quarkkingdee.top

Java: System.exit(1)
来源：http://ghy.xylfe.cn

Go:   os.Exit(1)
来源：http://tvr.shuidangran.top

Ruby: exit 1
来源：http://wje.wangshuangyany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://huv.nanxuanxn.top

[M06] 向标准错误输出
来源：http://aea.epnwcf.com

Py:   print("err", file=sys.stderr)
来源：http://hyt.sufxvd.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cky.xziqi.cn

JS:   console.error("err")
来源：http://nnf.cheryme.top

TS:   console.error("err")
来源：http://hrr.fzhhl.top

Java: System.err.println("err")
来源：http://cke.yuxming.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://imv.tianlin.xyz

Ruby: warn "err"
来源：http://wmt.fzhhl.top

C#:   Console.Error.WriteLine("err")
来源：http://qlr.bjfxy.top

[M07] 判断是否为主入口
来源：http://svb.tian-w.cn

Py:   if __name__ == "__main__":
来源：http://gmy.shzxlz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ktx.snrcjt.cn

JS:   require.main === module
来源：http://usb.yanxiufei.cn

TS:   require.main === module
来源：http://dch.jyoumei.cn

Java: public static void main(String[] args)
来源：http://oop.meibo888.top

Go:   func main()
来源：http://ytm.sysykeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tpt.c1oappe.top

C#:   static void Main(string[] args)
来源：http://tgl.ehwqpu.com

[M08] 获取系统与运行时信息
来源：http://jvg.jinghuilouyu.cn

Py:   platform.system();  platform.python_version()
来源：http://lrh.yj20258.top

PHP:  PHP_OS;  phpversion();
来源：http://oin.hcnkem.com

JS:   process.platform;  process.version
来源：http://nrg.birdmap.top

TS:   process.platform;  process.version
来源：http://zwz.sysykeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ltn.zhixingplan.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wez.andypj.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lnn.shzxlz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jvp.gaohongyu789.top

================================================================================
来源：http://zah.ybcxt.top

N. 数据结构与算法
来源：http://gxn.sufxvd.cn

================================================================================
来源：http://fuz.kuanghao11.cn

[N01] 二分查找（有序数组）
来源：http://vbl.zhaomingkeji.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://qjl.xuanzx.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wyy.cheryme.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yec.daria6918.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nzd.zhoulong.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://eki.sjlbkw.cn

Go:   sort.SearchInts(arr, x)
来源：http://bmo.smart0.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://dib.chenlongwang.top

C#:   Array.BinarySearch(arr, x)
来源：http://jdm.fanxiaobao.xyz

[N02] 排序（工程实践用内置实现）
来源：http://zgb.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://sns.yangfankeji.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jnw.jianghu66.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jgl.ctjpmb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://twr.xziqi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lws.nanxuanxn.top

Go:   slices.Sort(arr)
来源：http://xmr.9152youxi.cn

Ruby: arr.sort
来源：http://btw.feifeiyinyue.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mnn.yj20258.top

[N03] 快速排序（分治示例）
来源：http://qkp.cashguo.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fra.yuanzhike.top

PHP:  // 递归实现，或用 usort
来源：http://zzb.epnwcf.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ccp.havefunace.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aot.daria6918.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nrb.snrcjt.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ffj.cdnleiting.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zdz.shanyushiyangtech.top

C#:   // 手写递归，或 Array.Sort
来源：http://hda.snrcjt.cn

[N04] 斐波那契数列
来源：http://ejz.ppjwa.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xkj.zdbjq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tgo.jinqigfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ryx.sufxvd.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qat.xingfuxueyuan.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tga.316326.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oub.nwbrower.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zcl.c1oappe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vdk.jinyuanbaomall.cn

[N05] 最大公约数
来源：http://lje.havefunace.top

Py:   math.gcd(a, b)
来源：http://oga.xingfuxueyuan.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bxe.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tpq.bjfxy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zgl.shuidangran.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://flp.jinyuanbaomall.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dlt.hammf.cn

Ruby: a.gcd(b)
来源：http://ifp.jyoumei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://buf.shzxlz.cn

[N06] 判断回文字符串
来源：http://thw.zhiwuduotai.top

Py:   s == s[::-1]
来源：http://uku.wangshuangyany.cn

PHP:  $s === strrev($s);
来源：http://pyd.zhengqikj.top

JS:   s === [...s].reverse().join("")
来源：http://dlr.bbcook.cn

TS:   s === [...s].reverse().join("")
来源：http://vzd.havefunace.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yir.bjfxy.top

Go:   // 双指针从两端比较
来源：http://tim.shangyingyoupin.top

Ruby: s == s.reverse
来源：http://bri.316326.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://lvu.jqgfzy.top

[N07] 两数之和（返回下标）
来源：http://onr.dianchejie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jvr.ppjwa.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qmh.zhoulong.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://gsf.kuanghao11.cn

TS:   // 手写 Map<string, number>
来源：http://feg.andypj.xyz

Java: // 手写 HashMap
来源：http://tvi.havefunace.top

Go:   // 手写 map[int]int
来源：http://jyq.yj20258888.top

Ruby: // 手写 Hash
来源：http://ime.zdbjq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jrl.nanxuanxn.top

[N08] 生成全排列
来源：http://xtd.yongpay.top

Py:   itertools.permutations(arr)
来源：http://jos.feifeiyinyue.top

PHP:  // 手写递归交换
来源：http://tdp.cheryme.top

JS:   // 手写回溯递归
来源：http://kej.havefunace.top

TS:   // 手写回溯递归
来源：http://agk.cashguo.top

Java: // 手写回溯递归
来源：http://elv.yanxiufei.cn

Go:   // 手写回溯递归
来源：http://avi.cheryme.top

Ruby: arr.permutation.to_a
来源：http://fmm.mhx1999.top

C#:   // 手写回溯递归
来源：http://mqv.c1oappe.top

[N09] 栈与队列
来源：http://ydg.meibo888.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fci.jiagoushi.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zcx.bjfxy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xmj.sweek.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ddv.yvedp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ahn.pengpengdd.cyou

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tlq.yj20258.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://hvp.hongshengwenyu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tdl.ywan-chungtsiang.top

[N10] 链表节点定义
来源：http://wda.hesvh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://njb.guowangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://dqv.yvedp.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xkr.shangyingyoupin.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tuo.ivvv.top

Java: class Node { int v; Node next; }
来源：http://aid.sufxvd.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rrh.hcnkem.com

Ruby: Node = Struct.new(:v, :next)
来源：http://nib.hnxiangtu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ivj.epnwcf.com

[N11] 二叉树中序遍历
来源：http://kdb.tian-w.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xja.pengpengdd.cyou

PHP:  // 手写递归函数
来源：http://cjs.sxryk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wex.yj20258.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://edz.ybcxt.top

Java: // 手写递归
来源：http://vqi.yfazqb.com

Go:   // 手写递归
来源：http://csp.yuxming.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tbl.yvedp.cn

C#:   // 手写递归
来源：http://hib.daria6918.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://esm.sjlbkw.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wdv.snrcjt.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tyx.hywenlv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vzr.fehbvm.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rog.c1oappe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nap.gogol.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hno.xylfe.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ogv.tarul.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://giq.guannengcc.top

================================================================================
来源：http://sej.yj202588.top

O. 并发与异步
来源：http://qdk.9152youxi.cn

================================================================================
来源：http://rqc.snrcjt.cn

[O01] 启动一个线程
来源：http://sge.svipenyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://lxm.quarkkingdee.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rbe.fehbvm.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://toq.daria6918.cn

TS:   // 同 JS
来源：http://ilz.aibaodan.cn

Java: new Thread(() -> f()).start()
来源：http://vxx.ehwqpu.com

Go:   go f()
来源：http://imm.hysaishi.cn

Ruby: Thread.new { f }
来源：http://fqm.yongpay.top

C#:   Task.Run(() => F());
来源：http://gtf.zhoulong.xyz

[O02] 使用线程池
来源：http://yvk.dashuyun.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ttd.ehwqpu.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fip.0kj1m.cn

JS:   // worker_threads 线程池
来源：http://trf.zhaomingkeji.xyz

TS:   // worker_threads 线程池
来源：http://teh.fzhhl.top

Java: Executors.newFixedThreadPool(4)
来源：http://sae.havefunace.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wcl.zhixingplan.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fwl.yanxiufei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hvc.9152youxi.cn

[O03] 加锁保护共享数据
来源：http://ndt.gaohongyu789.top

Py:   with lock: shared += 1
来源：http://zbv.vqdsnc.cn

PHP:  // 用 flock() 做文件锁
来源：http://eij.gogol.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://omo.yfazqb.com

TS:   // 同 JS
来源：http://sam.pycfn.com

Java: synchronized (this) { shared++; }
来源：http://psl.daxiang520.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kdg.cucudq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zqs.shanyushiyangkeji.top

C#:   lock (gate) { shared++; }
来源：http://aon.dianchejie.cn

[O04] 定义异步函数并等待
来源：http://ghb.shangyingyoupin.top

Py:   async def f():⏎    await g()
来源：http://icq.tianlin.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zsi.hongshengwenyu.top

JS:   async function f() { await g(); }
来源：http://smv.bbcook.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gwg.zhoulong.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zqi.chenzaomai.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nqi.wangdashe.top

Ruby: # 用 Fiber 或 async gem
来源：http://vgu.guowangkeji.top

C#:   async Task F() { await G(); }
来源：http://azz.fktsv.cn

[O05] 并发执行并等待全部完成
来源：http://jfy.wangdashe.top

Py:   asyncio.gather(*tasks)
来源：http://nsw.ydzc1.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mkd.sysykeji.top

JS:   await Promise.all(tasks)
来源：http://qts.birdmap.top

TS:   await Promise.all(tasks)
来源：http://gns.sufxvd.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vst.jinqigfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lpo.sweek.top

Ruby: threads.map(&:join)
来源：http://kps.mhx1999.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fdq.hesvh.cn

[O06] 使用进程池
来源：http://szq.sxryk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fof.shanyushiyangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://bal.hcnkem.com

JS:   // child_process / cluster 模块
来源：http://lof.ctjpmb.com

TS:   // child_process / cluster 模块
来源：http://wnj.yongpay.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eoa.hysaishi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nqx.tian-w.cn

Ruby: // fork 块
来源：http://mum.redwolf501.top

C#:   Parallel.For
来源：http://wtw.jyoumei.cn

================================================================================
来源：http://abq.sufxvd.cn

P. 常用工具函数
来源：http://lnq.jlsjyb.cn

================================================================================
来源：http://jzr.xylfe.cn

[P01] 生成 UUID
来源：http://gyk.fktsv.cn

Py:   str(uuid.uuid4())
来源：http://hbo.yj20258.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wgi.havefunace.top

JS:   crypto.randomUUID()
来源：http://ylj.zycfv.cn

TS:   crypto.randomUUID()
来源：http://tee.hcnkem.com

Java: UUID.randomUUID().toString()
来源：http://fiu.zhaomingkeji.xyz

Go:   // 用 github.com/google/uuid
来源：http://ltf.jlsjyb.cn

Ruby: SecureRandom.uuid
来源：http://cfp.guannengcc.top

C#:   Guid.NewGuid().ToString()
来源：http://bys.zhongyouzk.top

[P02] MD5 / SHA256 摘要
来源：http://drd.ywan-chungtsiang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zez.sysykeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://bjf.xuetiantiany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cwg.wangshuangyany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oku.gzhubu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://khu.shzxlz.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jyh.xinyue.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ewl.kuanghao11.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pfc.sufxvd.cn

[P03] 生成短随机字符串
来源：http://ssw.fanxiaobao.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wtf.yangfankeji.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bmp.nanxuanxn.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cru.shanyushiyangtech.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ikm.hesvh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tqr.sufxvd.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lml.ctjpmb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://xbr.zycfv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tjg.daria6918.cn

[P04] 求长度
来源：http://hya.aizwys.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dtr.snrcjt.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pbf.wangdashe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yiy.ybcxt.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vdn.hywenlv.cn

Java: list.size();  map.size();  s.length()
来源：http://pib.aibaodan.cn

Go:   len(arr);  len(m)
来源：http://wvd.jqgufenzy.top

Ruby: x.length;  x.size
来源：http://dod.wangshuangyany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vmk.hongshengwenyu.top

[P05] 判断两个对象内容是否相等
来源：http://ygh.sweek.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://pgw.aibaodan.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rvj.hcnkem.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xxn.jqgufenzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vsk.xylfe.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://riv.ppjwa.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ebf.sufxvd.cn

Ruby: a == b
来源：http://ccp.nwbrower.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nru.pengpengdd.cyou

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xyq.zdbjq.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qcp.pengpengdd.cyou

PHP:  if (empty($x)) {}
来源：http://vtq.dashuyun.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ztp.jianghu66.top

TS:   if (x == null) {}
来源：http://maz.ctjpmb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://lay.haohaochexian.top

Go:   if x == nil {}
来源：http://mgr.yj202588.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qfk.ydzc1.top

C#:   if (x is null) {}
来源：http://ela.ivvv.top

[P07] 防抖与节流
来源：http://pol.hammf.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fgo.zdbjq.cn

PHP:  // 手写时间戳比较
来源：http://ylv.epnwcf.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dap.feifeiyinyue.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://twk.ydzc1.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://num.yj20258.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jdt.zhoulong.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://rjz.9152youxi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vvu.jlsjyb.cn

[P08] 处理浮点精度问题
来源：http://qed.jinqigufen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lyd.yangfankeji.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jfx.andypj.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://psb.yj20258888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://luh.quarkkingdee.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qnp.yonumen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ipe.zdbjq.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wer.sweek.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mvp.xuanzx.com


<!-- 参考信息 -->