代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xjy.hfpthk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ftw.smart0.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://qal.dianchejie.cn

C#:   Process.Start("ls", "-l");
来源：http://xoi.jyoumei.cn

[M04] 获取当前工作目录
来源：http://ybr.haohaochexian.top

Py:   os.getcwd()
来源：http://gpm.hfpthk.cn

PHP:  getcwd();
来源：http://xct.hcnkem.com

JS:   process.cwd()
来源：http://xfe.havefunace.top

TS:   process.cwd()
来源：http://voc.pengpengdd.cyou

Java: Path.of("").toAbsolutePath()
来源：http://mih.tarul.cn

Go:   os.Getwd()
来源：http://ahc.epnwcf.com

Ruby: Dir.pwd
来源：http://ywc.dashuyun.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sid.hnxiangtu.top

[M05] 设置退出码
来源：http://rjb.xuanzx.com

Py:   sys.exit(1)
来源：http://ncd.aibaodan.cn

PHP:  exit(1);
来源：http://tju.chenlongwang.top

JS:   process.exit(1)
来源：http://qev.haohaochexian.top

TS:   process.exit(1)
来源：http://mor.shzxlz.cn

Java: System.exit(1)
来源：http://tjw.fehbvm.com

Go:   os.Exit(1)
来源：http://rec.ctjpmb.com

Ruby: exit 1
来源：http://bqh.ywan-chungtsiang.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vmo.xinyue.icu

[M06] 向标准错误输出
来源：http://nlb.uphjek.com

Py:   print("err", file=sys.stderr)
来源：http://rky.aibaodan.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kqf.0kj1m.cn

JS:   console.error("err")
来源：http://klt.birdmap.top

TS:   console.error("err")
来源：http://yrs.zdbjq.cn

Java: System.err.println("err")
来源：http://cdn.nanxinkj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hlt.andypj.xyz

Ruby: warn "err"
来源：http://fzs.jinqigufen.top

C#:   Console.Error.WriteLine("err")
来源：http://hmu.gaohongyu789.top

[M07] 判断是否为主入口
来源：http://lqf.iojbl.cn

Py:   if __name__ == "__main__":
来源：http://yyi.andypj.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mid.316326.xyz

JS:   require.main === module
来源：http://dhq.gzhubu.top

TS:   require.main === module
来源：http://cso.yonumen.top

Java: public static void main(String[] args)
来源：http://cvj.zdqjudy.top

Go:   func main()
来源：http://fwk.haohaochexian.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yaj.jinqigfzy.top

C#:   static void Main(string[] args)
来源：http://lxw.haohaochexian.top

[M08] 获取系统与运行时信息
来源：http://hxs.ydjk.org.cn

Py:   platform.system();  platform.python_version()
来源：http://rrv.zhaomingkeji.xyz

PHP:  PHP_OS;  phpversion();
来源：http://vzz.yongpay.top

JS:   process.platform;  process.version
来源：http://uro.ybcxt.top

TS:   process.platform;  process.version
来源：http://rek.fehbvm.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oxs.zhongyouzk.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fqu.ivvv.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dtv.quarkkingdee.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://iab.iojbl.cn

================================================================================
来源：http://fqt.tianlin.xyz

N. 数据结构与算法
来源：http://qbh.kuanghao11.cn

================================================================================
来源：http://rlu.pengpengdd.cyou

[N01] 二分查找（有序数组）
来源：http://gsc.hammf.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zes.zhongyouzk.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bjq.svipenyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://osn.ybcxt.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jkj.jyoumei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ejq.ydzc1.top

Go:   sort.SearchInts(arr, x)
来源：http://dbf.c1oappe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://afb.sweek.top

C#:   Array.BinarySearch(arr, x)
来源：http://tkn.52xcode.cn

[N02] 排序（工程实践用内置实现）
来源：http://dcq.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://bla.chenzaomai.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fkt.fanxiaobao.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://scv.xylfe.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://met.316326.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zss.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://swb.xinyue.icu

Ruby: arr.sort
来源：http://xbx.wangshuangyany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ixn.hysaishi.cn

[N03] 快速排序（分治示例）
来源：http://xdi.guannengcc.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tee.vehdjk.com

PHP:  // 递归实现，或用 usort
来源：http://gzm.52xcode.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pbh.aizwys.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://amz.daria6918.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xhu.shzxlz.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pli.kuanghao11.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kzp.zhixingplan.top

C#:   // 手写递归，或 Array.Sort
来源：http://vca.yanxiufei.cn

[N04] 斐波那契数列
来源：http://fef.316326.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://adk.ydzc1.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rzf.0kj1m.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xch.tanke756.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zui.jinghuilouyu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://prw.tianlin.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fnn.nwbrower.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xbp.jinyuanbaomall.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mec.chenlongwang.top

[N05] 最大公约数
来源：http://njl.gogol.net.cn

Py:   math.gcd(a, b)
来源：http://qcz.cdnleiting.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jqn.cheryme.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wzk.jlsjyb.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xvb.yanxiufei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ssd.ctjpmb.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rfd.nanxuanxn.top

Ruby: a.gcd(b)
来源：http://myk.fengsongda.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lin.xinyue.icu

[N06] 判断回文字符串
来源：http://tyx.zhengqikj.top

Py:   s == s[::-1]
来源：http://imm.hammf.cn

PHP:  $s === strrev($s);
来源：http://wqx.hongshengwenyu.top

JS:   s === [...s].reverse().join("")
来源：http://wfm.guannengcc.top

TS:   s === [...s].reverse().join("")
来源：http://edu.zhaomingkeji.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://chg.cqqwz.cn

Go:   // 双指针从两端比较
来源：http://ukg.svipenyu.cn

Ruby: s == s.reverse
来源：http://xkg.zhaomingkeji.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://wqf.sysykeji.top

[N07] 两数之和（返回下标）
来源：http://dly.ybcxt.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hwg.xuetiantiany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eli.zhoulong.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://crz.jyoumei.cn

TS:   // 手写 Map<string, number>
来源：http://vae.jqgufenzy.top

Java: // 手写 HashMap
来源：http://mdp.wangshuangyany.cn

Go:   // 手写 map[int]int
来源：http://hlw.nanxinkj.top

Ruby: // 手写 Hash
来源：http://khe.bbcook.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ujt.fehbvm.com

[N08] 生成全排列
来源：http://ldw.jiagoushi.top

Py:   itertools.permutations(arr)
来源：http://jtx.birdmap.top

PHP:  // 手写递归交换
来源：http://fqd.c1oappe.top

JS:   // 手写回溯递归
来源：http://wry.chenlongwang.top

TS:   // 手写回溯递归
来源：http://moh.shzxlz.cn

Java: // 手写回溯递归
来源：http://cuu.yangfankeji.com

Go:   // 手写回溯递归
来源：http://hes.yangfankeji.com

Ruby: arr.permutation.to_a
来源：http://raw.jqgfzy.top

C#:   // 手写回溯递归
来源：http://dqu.ctjpmb.com

[N09] 栈与队列
来源：http://ctg.shanyushiyangkeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xoy.52xcode.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rpo.hywenlv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://afi.fktsv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://sak.jlsjyb.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://inv.jinyuanbaomall.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jwt.52xcode.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kfy.hfpthk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ubx.smart0.xyz

[N10] 链表节点定义
来源：http://mvi.jinqigufen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pip.ctjpmb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://yyc.jinqigufen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qkr.vehdjk.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rmm.fehbvm.com

Java: class Node { int v; Node next; }
来源：http://byv.chenjidiqi.icu

Go:   type Node struct { V int; Next *Node }
来源：http://udt.hnxiangtu.top

Ruby: Node = Struct.new(:v, :next)
来源：http://jul.sjlbkw.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://sfu.daxiang520.top

[N11] 二叉树中序遍历
来源：http://eot.vqdsnc.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://idj.vehdjk.com

PHP:  // 手写递归函数
来源：http://xrr.feifeiyinyue.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dru.xylfe.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nxd.zhaomingkeji.xyz

Java: // 手写递归
来源：http://ojl.ehwqpu.com

Go:   // 手写递归
来源：http://loa.wangshuangyany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://obc.yangfankeji.com

C#:   // 手写递归
来源：http://vhh.smart0.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vjg.ehwqpu.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hov.jyoumei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vua.jinqigfzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nxl.guowangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ozt.xinyue.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ksw.ydzc1.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pll.hesvh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gwr.nwbrower.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uyo.fengsongda.top

================================================================================
来源：http://rba.316326.xyz

O. 并发与异步
来源：http://jfm.gogol.net.cn

================================================================================
来源：http://erc.wangshuangyany.cn

[O01] 启动一个线程
来源：http://jvj.xuetiantiany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://now.ctjpmb.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://etx.yonumen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bhl.daxiang520.top

TS:   // 同 JS
来源：http://gym.aibaodan.cn

Java: new Thread(() -> f()).start()
来源：http://awv.uphjek.com

Go:   go f()
来源：http://yop.hywenlv.cn

Ruby: Thread.new { f }
来源：http://mqo.havefunace.top

C#:   Task.Run(() => F());
来源：http://ovx.daria6918.cn

[O02] 使用线程池
来源：http://rfs.nanxuanxn.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lwf.zycfv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xmx.hysaishi.cn

JS:   // worker_threads 线程池
来源：http://fil.sxryk.cn

TS:   // worker_threads 线程池
来源：http://hmc.birdmap.top

Java: Executors.newFixedThreadPool(4)
来源：http://qzw.hcnkem.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pih.dashuyun.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tna.cheryme.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kcg.ppjwa.cn

[O03] 加锁保护共享数据
来源：http://sys.zhoulong.xyz

Py:   with lock: shared += 1
来源：http://qvr.jinqigufen.top

PHP:  // 用 flock() 做文件锁
来源：http://tnq.cashguo.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fsl.xziqi.cn

TS:   // 同 JS
来源：http://hyh.ctjpmb.com

Java: synchronized (this) { shared++; }
来源：http://pme.quarkkingdee.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eps.guannengcc.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://puc.shuidangran.top

C#:   lock (gate) { shared++; }
来源：http://vzz.hnxiangtu.top

[O04] 定义异步函数并等待
来源：http://icn.redwolf501.top

Py:   async def f():⏎    await g()
来源：http://dtn.cqqwz.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pjx.vehdjk.com

JS:   async function f() { await g(); }
来源：http://ekn.pengpengdd.cyou

TS:   async function f(): Promise<void> { await g(); }
来源：http://tdh.bbcook.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ssh.gaohongyu789.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yja.vehdjk.com

Ruby: # 用 Fiber 或 async gem
来源：http://rfc.mhx1999.top

C#:   async Task F() { await G(); }
来源：http://gcs.uphjek.com

[O05] 并发执行并等待全部完成
来源：http://rji.tarul.cn

Py:   asyncio.gather(*tasks)
来源：http://wlf.nwbrower.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zmu.ppjwa.cn

JS:   await Promise.all(tasks)
来源：http://ens.yuanzhike.top

TS:   await Promise.all(tasks)
来源：http://akn.cdnleiting.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://smi.mhx1999.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lyj.pengpengdd.cyou

Ruby: threads.map(&:join)
来源：http://qhr.hnqzz.top

C#:   await Task.WhenAll(t1, t2)
来源：http://etm.yj202588.top

[O06] 使用进程池
来源：http://mtg.cdnleiting.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qpu.gotoacloud.top

PHP:  // pcntl_fork 或多进程队列
来源：http://oaz.gogol.net.cn

JS:   // child_process / cluster 模块
来源：http://hhe.fengsongda.top

TS:   // child_process / cluster 模块
来源：http://scq.tanke756.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hku.meibo888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yut.haohaochexian.top

Ruby: // fork 块
来源：http://erj.zhongyouzk.top

C#:   Parallel.For
来源：http://lhx.wangdashe.top

================================================================================
来源：http://qtx.jqgufenzy.top

P. 常用工具函数
来源：http://ywj.dashuyun.cn

================================================================================
来源：http://ijf.chenlongwang.top

[P01] 生成 UUID
来源：http://sbv.redwolf501.top

Py:   str(uuid.uuid4())
来源：http://itb.cheryme.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mnx.aibaodan.cn

JS:   crypto.randomUUID()
来源：http://scq.hysaishi.cn

TS:   crypto.randomUUID()
来源：http://qmj.fktsv.cn

Java: UUID.randomUUID().toString()
来源：http://ita.sysykeji.top

Go:   // 用 github.com/google/uuid
来源：http://stx.fzhhl.top

Ruby: SecureRandom.uuid
来源：http://rmn.cheryme.top

C#:   Guid.NewGuid().ToString()
来源：http://aem.yvedp.cn

[P02] MD5 / SHA256 摘要
来源：http://yfu.meibo888.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xxa.zhaomingkeji.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://qzd.kuanghao11.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nfh.zdbjq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ywo.fktsv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pos.hammf.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cgr.shanyushiyangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nak.kuanghao11.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rkm.c1oappe.top

[P03] 生成短随机字符串
来源：http://qfh.iojbl.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bnw.52xcode.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qyr.shuidangran.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vet.ctjpmb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dkc.jinqigfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ite.gotoacloud.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yoz.shuidangran.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://nrw.zhongyouzk.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tik.xziqi.cn

[P04] 求长度
来源：http://ssu.xylfe.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tfi.jinghuilouyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yml.yj20258888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ggs.feifeiyinyue.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://krj.zdqjudy.top

Java: list.size();  map.size();  s.length()
来源：http://abz.zhongyouzk.top

Go:   len(arr);  len(m)
来源：http://img.mhx1999.top

Ruby: x.length;  x.size
来源：http://ncv.9152youxi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hoy.wangdashe.top

[P05] 判断两个对象内容是否相等
来源：http://tox.ivvv.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rhl.ehwqpu.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ary.vqdsnc.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kek.cdnleiting.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vmd.tian-w.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rua.ydzc1.top

Go:   reflect.DeepEqual(a, b)
来源：http://rdc.zdqjudy.top

Ruby: a == b
来源：http://qbs.mhx1999.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wqn.jinghuilouyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://omb.tianlin.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://niv.sufxvd.cn

PHP:  if (empty($x)) {}
来源：http://wvg.jianghu66.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sgm.zhoulong.xyz

TS:   if (x == null) {}
来源：http://lkj.hongshengwenyu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://aat.chenjidiqi.icu

Go:   if x == nil {}
来源：http://pdw.shanyushiyangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ejp.yonumen.top

C#:   if (x is null) {}
来源：http://xiq.hysaishi.cn

[P07] 防抖与节流
来源：http://zis.zhoulong.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bnr.iojbl.cn

PHP:  // 手写时间戳比较
来源：http://mfz.shzxlz.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uqa.zdbjq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rod.hnqzz.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hvm.cashguo.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ydz.bjfxy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://jjs.iojbl.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kam.hammf.cn

[P08] 处理浮点精度问题
来源：http://zfq.yj202588.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mqc.sweek.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yue.bjfxy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zue.yanxiufei.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lbk.zhixingplan.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yjz.hywenlv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ity.redwolf501.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tzp.zhixingplan.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hbl.hesvh.cn

================================================================================
来源：http://job.zdqjudy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nil.daxiang520.top

================================================================================
来源：http://imw.xingfuxueyuan.xyz

[Q01] 创建表
来源：http://wtd.hongshengwenyu.top

CREATE TABLE users (
来源：http://dyv.xziqi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mrw.9152youxi.cn

name VARCHAR(50) NOT NULL,
来源：http://kqd.pycfn.com

email VARCHAR(100) UNIQUE,
来源：http://etn.yj202588.top


<!-- 参考信息 -->