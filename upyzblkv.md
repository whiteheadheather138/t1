代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mqb.hesvh.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lns.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://jzn.tarul.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://act.hcnkem.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://clp.shanyushiyangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gjn.ppjwa.cn

Ruby: system("ls -l");  `ls -l`
来源：http://isq.jinqigfzy.top

C#:   Process.Start("ls", "-l");
来源：http://alk.uphjek.com

[M04] 获取当前工作目录
来源：http://erk.316326.xyz

Py:   os.getcwd()
来源：http://wtq.xylfe.cn

PHP:  getcwd();
来源：http://ipb.zycfv.cn

JS:   process.cwd()
来源：http://rbk.quarkkingdee.top

TS:   process.cwd()
来源：http://quk.hammf.cn

Java: Path.of("").toAbsolutePath()
来源：http://ljn.nanxuanxn.top

Go:   os.Getwd()
来源：http://cli.shanyushiyangtech.top

Ruby: Dir.pwd
来源：http://dkf.gaohongyu789.top

C#:   Directory.GetCurrentDirectory()
来源：http://fqv.ctjpmb.com

[M05] 设置退出码
来源：http://ufz.aibaodan.cn

Py:   sys.exit(1)
来源：http://chx.cheryme.top

PHP:  exit(1);
来源：http://jch.jqgfzy.top

JS:   process.exit(1)
来源：http://uqm.daria6918.cn

TS:   process.exit(1)
来源：http://nli.ctjpmb.com

Java: System.exit(1)
来源：http://lxg.snrcjt.cn

Go:   os.Exit(1)
来源：http://avm.vqdsnc.cn

Ruby: exit 1
来源：http://uur.hnxiangtu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rad.shangyingyoupin.top

[M06] 向标准错误输出
来源：http://sch.xylfe.cn

Py:   print("err", file=sys.stderr)
来源：http://mzb.hysaishi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://udy.zdbjq.cn

JS:   console.error("err")
来源：http://cbl.hesvh.cn

TS:   console.error("err")
来源：http://eaw.shanyushiyangtech.top

Java: System.err.println("err")
来源：http://uzz.shzxlz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zew.vehdjk.com

Ruby: warn "err"
来源：http://ozy.aibaodan.cn

C#:   Console.Error.WriteLine("err")
来源：http://wlq.xylfe.cn

[M07] 判断是否为主入口
来源：http://gis.bjfxy.top

Py:   if __name__ == "__main__":
来源：http://lrx.cucudq.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lta.fzhhl.top

JS:   require.main === module
来源：http://gxm.gotoacloud.top

TS:   require.main === module
来源：http://gtu.svipenyu.cn

Java: public static void main(String[] args)
来源：http://srp.tanke756.top

Go:   func main()
来源：http://guj.cheryme.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eds.shangyingyoupin.top

C#:   static void Main(string[] args)
来源：http://mlo.cucudq.cn

[M08] 获取系统与运行时信息
来源：http://qot.mhx1999.top

Py:   platform.system();  platform.python_version()
来源：http://kfp.yuanzhike.top

PHP:  PHP_OS;  phpversion();
来源：http://jep.yonumen.top

JS:   process.platform;  process.version
来源：http://ukv.andypj.xyz

TS:   process.platform;  process.version
来源：http://eqc.xziqi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yng.daxiang520.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jjd.tian-w.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xij.zhengqikj.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ckz.hnxiangtu.top

================================================================================
来源：http://hxq.aizwys.cn

N. 数据结构与算法
来源：http://twz.52xcode.cn

================================================================================
来源：http://tvl.meibo888.top

[N01] 二分查找（有序数组）
来源：http://pyw.snrcjt.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jtk.guannengcc.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://umr.dashuyun.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dhj.gaohongyu789.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://glu.svipenyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://efe.guowangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://kmf.zhiwuduotai.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xyg.fehbvm.com

C#:   Array.BinarySearch(arr, x)
来源：http://zle.jqgfzy.top

[N02] 排序（工程实践用内置实现）
来源：http://ujz.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://ddj.uphjek.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mfh.yj202588.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://gop.meibo888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://sqo.nanxinkj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://slj.52xcode.cn

Go:   slices.Sort(arr)
来源：http://qsk.mhx1999.top

Ruby: arr.sort
来源：http://jrp.svipenyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pkb.daria6918.cn

[N03] 快速排序（分治示例）
来源：http://bie.tarul.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xrj.wangdashe.top

PHP:  // 递归实现，或用 usort
来源：http://kvc.yueranfly.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mqs.yonumen.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://giz.zhiwuduotai.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jxs.dianchejie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gae.jinqigfzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://law.gzhubu.top

C#:   // 手写递归，或 Array.Sort
来源：http://gny.gogol.net.cn

[N04] 斐波那契数列
来源：http://pbs.9152youxi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ecd.hammf.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pil.yj20258.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cyi.meibo888.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://trf.birdmap.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cbh.nwbrower.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ydf.316326.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kwt.ywan-chungtsiang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kmc.epnwcf.com

[N05] 最大公约数
来源：http://kpw.guannengcc.top

Py:   math.gcd(a, b)
来源：http://lzp.uphjek.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ult.shanyushiyangtech.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oar.xylfe.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qvl.hnxiangtu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xjh.chenlongwang.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xjc.fzhhl.top

Ruby: a.gcd(b)
来源：http://nwu.dianchejie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qon.daxiang520.top

[N06] 判断回文字符串
来源：http://lty.andypj.xyz

Py:   s == s[::-1]
来源：http://yeq.fanxiaobao.xyz

PHP:  $s === strrev($s);
来源：http://dmj.yvedp.cn

JS:   s === [...s].reverse().join("")
来源：http://dby.ctjpmb.com

TS:   s === [...s].reverse().join("")
来源：http://lbi.shzxlz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dtv.yongpay.top

Go:   // 双指针从两端比较
来源：http://hki.nwbrower.top

Ruby: s == s.reverse
来源：http://yrn.aibaodan.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kis.hesvh.cn

[N07] 两数之和（返回下标）
来源：http://rwx.tian-w.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ldm.guannengcc.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://knk.haohaochexian.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ilp.wangdashe.top

TS:   // 手写 Map<string, number>
来源：http://zhr.tanke756.top

Java: // 手写 HashMap
来源：http://dht.tarul.cn

Go:   // 手写 map[int]int
来源：http://kbz.jinqigfzy.top

Ruby: // 手写 Hash
来源：http://qdc.chenjidiqi.icu

C#:   // 手写 Dictionary<int, int>
来源：http://tky.hfpthk.cn

[N08] 生成全排列
来源：http://dvq.fktsv.cn

Py:   itertools.permutations(arr)
来源：http://zwz.cqqwz.cn

PHP:  // 手写递归交换
来源：http://lik.jianghu66.top

JS:   // 手写回溯递归
来源：http://rkc.smart0.xyz

TS:   // 手写回溯递归
来源：http://kzy.c1oappe.top

Java: // 手写回溯递归
来源：http://ktk.zhixingplan.top

Go:   // 手写回溯递归
来源：http://dwq.hongshengwenyu.top

Ruby: arr.permutation.to_a
来源：http://yul.jinqigufen.top

C#:   // 手写回溯递归
来源：http://qoz.vehdjk.com

[N09] 栈与队列
来源：http://nub.wangshuangyany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qwv.sysykeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rnf.zycfv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wcm.sjlbkw.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://itl.cqqwz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kcw.jinqigfzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wzh.fehbvm.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kqv.ehwqpu.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://meo.svipenyu.cn

[N10] 链表节点定义
来源：http://ccd.zdqjudy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dnj.redwolf501.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zau.shangyingyoupin.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vbx.xziqi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ltb.yongpay.top

Java: class Node { int v; Node next; }
来源：http://gul.fktsv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://keb.xingfuxueyuan.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://zel.tianlin.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://ema.guannengcc.top

[N11] 二叉树中序遍历
来源：http://yoa.fengsongda.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xtd.chenzaomai.com

PHP:  // 手写递归函数
来源：http://ohg.nwbrower.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ugk.52xcode.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gtg.xuetiantiany.cn

Java: // 手写递归
来源：http://pxw.chenlongwang.top

Go:   // 手写递归
来源：http://aax.ydzc1.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tix.hywenlv.cn

C#:   // 手写递归
来源：http://ufp.xinyue.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mwa.tian-w.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://agi.ehwqpu.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://glk.svipenyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ggx.shzxlz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fdp.tian-w.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mnw.zhijiandao.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://khj.hnxiangtu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iru.andypj.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rqu.aizwys.cn

================================================================================
来源：http://ipp.jinghuilouyu.cn

O. 并发与异步
来源：http://cur.zhongyouzk.top

================================================================================
来源：http://ntv.haohaochexian.top

[O01] 启动一个线程
来源：http://xbx.sufxvd.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://izj.guowangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ggj.tian-w.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mrn.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://kwc.snrcjt.cn

Java: new Thread(() -> f()).start()
来源：http://lxh.gogol.net.cn

Go:   go f()
来源：http://ysr.sweek.top

Ruby: Thread.new { f }
来源：http://siz.iojbl.cn

C#:   Task.Run(() => F());
来源：http://ckb.snrcjt.cn

[O02] 使用线程池
来源：http://tfz.xylfe.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://whm.nanxinkj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kuv.zhengqikj.top

JS:   // worker_threads 线程池
来源：http://bnj.redwolf501.top

TS:   // worker_threads 线程池
来源：http://oce.fanxiaobao.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://pfn.smart0.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oxe.cqqwz.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kma.meibo888.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://edy.yongpay.top

[O03] 加锁保护共享数据
来源：http://tyz.yongpay.top

Py:   with lock: shared += 1
来源：http://zwo.vehdjk.com

PHP:  // 用 flock() 做文件锁
来源：http://fxc.hnxiangtu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gmk.nanxuanxn.top

TS:   // 同 JS
来源：http://hey.svipenyu.cn

Java: synchronized (this) { shared++; }
来源：http://onr.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mqh.vqdsnc.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://oto.tianlin.xyz

C#:   lock (gate) { shared++; }
来源：http://pyp.zdbjq.cn

[O04] 定义异步函数并等待
来源：http://eev.aizwys.cn

Py:   async def f():⏎    await g()
来源：http://vzy.yueranfly.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mvf.bjfxy.top

JS:   async function f() { await g(); }
来源：http://vqs.daria6918.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qhu.316326.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://shl.fanxiaobao.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pac.jianghu66.top

Ruby: # 用 Fiber 或 async gem
来源：http://yng.xingfuxueyuan.xyz

C#:   async Task F() { await G(); }
来源：http://ppz.fehbvm.com

[O05] 并发执行并等待全部完成
来源：http://zkx.yangfankeji.com

Py:   asyncio.gather(*tasks)
来源：http://bch.ybcxt.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bwk.redwolf501.top

JS:   await Promise.all(tasks)
来源：http://vik.shanyushiyangtech.top

TS:   await Promise.all(tasks)
来源：http://boz.tian-w.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://maj.xuetiantiany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rml.hongshengwenyu.top

Ruby: threads.map(&:join)
来源：http://tml.ydzc1.top

C#:   await Task.WhenAll(t1, t2)
来源：http://bnr.fktsv.cn

[O06] 使用进程池
来源：http://cto.shanyushiyangkeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://otj.gotoacloud.top

PHP:  // pcntl_fork 或多进程队列
来源：http://liz.gotoacloud.top

JS:   // child_process / cluster 模块
来源：http://mkv.aizwys.cn

TS:   // child_process / cluster 模块
来源：http://cdd.dashuyun.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vgg.hongshengwenyu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lpo.ybcxt.top

Ruby: // fork 块
来源：http://sfd.cashguo.top

C#:   Parallel.For
来源：http://ytx.zhijiandao.cn

================================================================================
来源：http://tpc.zdbjq.cn

P. 常用工具函数
来源：http://ngt.zhongyouzk.top

================================================================================
来源：http://luo.zycfv.cn

[P01] 生成 UUID
来源：http://htw.andypj.xyz

Py:   str(uuid.uuid4())
来源：http://hvh.xuanzx.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://adf.gogol.net.cn

JS:   crypto.randomUUID()
来源：http://pjc.pengpengdd.cyou

TS:   crypto.randomUUID()
来源：http://tax.havefunace.top

Java: UUID.randomUUID().toString()
来源：http://tkh.epnwcf.com

Go:   // 用 github.com/google/uuid
来源：http://mvm.ctjpmb.com

Ruby: SecureRandom.uuid
来源：http://czn.zhongyouzk.top

C#:   Guid.NewGuid().ToString()
来源：http://igc.xylfe.cn

[P02] MD5 / SHA256 摘要
来源：http://wsv.pycfn.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://htc.yanxiufei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://loz.cheryme.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uoj.aizwys.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uzy.nanxinkj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bea.wangshuangyany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hgb.zhoulong.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iqr.jqgufenzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://csv.jianghu66.top

[P03] 生成短随机字符串
来源：http://dvy.ctjpmb.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zyi.jinqigufen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xct.xylfe.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tjr.yongpay.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ssy.xylfe.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zan.zycfv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vcm.zdqjudy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ctm.zhijiandao.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ssn.ydzc1.top

[P04] 求长度
来源：http://ctk.hongshengwenyu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vrm.hcnkem.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ghc.xuetiantiany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vhn.gogol.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lbu.gzhubu.top

Java: list.size();  map.size();  s.length()
来源：http://vyv.gaohongyu789.top

Go:   len(arr);  len(m)
来源：http://yuc.dashuyun.cn

Ruby: x.length;  x.size
来源：http://zpc.52xcode.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yci.yanxiufei.cn

[P05] 判断两个对象内容是否相等
来源：http://wak.redwolf501.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://irb.aibaodan.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dha.hnqzz.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vfb.ehwqpu.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ydi.cucudq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bxd.shuidangran.top

Go:   reflect.DeepEqual(a, b)
来源：http://epp.kuanghao11.cn

Ruby: a == b
来源：http://tiy.dashuyun.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jxb.shuidangran.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kfa.fengsongda.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://onq.uphjek.com

PHP:  if (empty($x)) {}
来源：http://eev.jianghu66.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ebk.yfazqb.com

TS:   if (x == null) {}
来源：http://byc.ydjk.org.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pff.ybcxt.top

Go:   if x == nil {}
来源：http://dvl.yueranfly.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rxq.zdbjq.cn

C#:   if (x is null) {}
来源：http://ylw.gaohongyu789.top

[P07] 防抖与节流
来源：http://uhy.yuanzhike.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fnf.cqqwz.cn

PHP:  // 手写时间戳比较
来源：http://str.sufxvd.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aiv.pycfn.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yjb.nanxinkj.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qky.pycfn.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rvx.svipenyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://elh.ppjwa.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bzi.sysykeji.top

[P08] 处理浮点精度问题
来源：http://ako.shzxlz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cgu.zycfv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://naa.52xcode.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://han.jlsjyb.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cyr.chenjidiqi.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jqc.fzhhl.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://svi.sxryk.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ktf.ctjpmb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://iye.iojbl.cn

================================================================================
来源：http://cgs.zdqjudy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fyv.jinqigfzy.top

================================================================================
来源：http://sdd.aizwys.cn

[Q01] 创建表
来源：http://whb.yanxiufei.cn


<!-- 参考信息 -->