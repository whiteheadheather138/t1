代发 wailian999

TS:   process.cwd()
来源：http://wtz.xuanzx.com

Java: Path.of("").toAbsolutePath()
来源：http://vcf.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://zjz.daria6918.cn

Ruby: Dir.pwd
来源：http://vbl.52xcode.cn

C#:   Directory.GetCurrentDirectory()
来源：http://goa.feifeiyinyue.top

[M05] 设置退出码
来源：http://xyg.yj20258888.top

Py:   sys.exit(1)
来源：http://dqc.ybcxt.top

PHP:  exit(1);
来源：http://xav.yongpay.top

JS:   process.exit(1)
来源：http://izl.wangshuangyany.cn

TS:   process.exit(1)
来源：http://ygo.meibo888.top

Java: System.exit(1)
来源：http://puo.aibaodan.cn

Go:   os.Exit(1)
来源：http://mup.chenjidiqi.icu

Ruby: exit 1
来源：http://ucf.ppjwa.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ant.ctjpmb.com

[M06] 向标准错误输出
来源：http://iqm.shuidangran.top

Py:   print("err", file=sys.stderr)
来源：http://dgo.aizwys.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qmz.yj20258888.top

JS:   console.error("err")
来源：http://utn.yvedp.cn

TS:   console.error("err")
来源：http://srj.sweek.top

Java: System.err.println("err")
来源：http://ozr.tian-w.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://aec.xylfe.cn

Ruby: warn "err"
来源：http://jlt.tianlin.xyz

C#:   Console.Error.WriteLine("err")
来源：http://ihf.sweek.top

[M07] 判断是否为主入口
来源：http://kcp.snrcjt.cn

Py:   if __name__ == "__main__":
来源：http://dei.gaohongyu789.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hsd.hesvh.cn

JS:   require.main === module
来源：http://uml.guannengcc.top

TS:   require.main === module
来源：http://mek.redwolf501.top

Java: public static void main(String[] args)
来源：http://xge.sxryk.cn

Go:   func main()
来源：http://pvp.jinqigufen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://djm.zhoulong.xyz

C#:   static void Main(string[] args)
来源：http://xtq.nanxuanxn.top

[M08] 获取系统与运行时信息
来源：http://ers.epnwcf.com

Py:   platform.system();  platform.python_version()
来源：http://tcj.cucudq.cn

PHP:  PHP_OS;  phpversion();
来源：http://ybf.chenzaomai.com

JS:   process.platform;  process.version
来源：http://rni.jinghuilouyu.cn

TS:   process.platform;  process.version
来源：http://jen.tianlin.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cwo.xingfuxueyuan.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://fky.zhaomingkeji.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fec.cqqwz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rko.jlsjyb.cn

================================================================================
来源：http://mih.zhaomingkeji.xyz

N. 数据结构与算法
来源：http://ycu.52xcode.cn

================================================================================
来源：http://cxn.hnxiangtu.top

[N01] 二分查找（有序数组）
来源：http://esa.aizwys.cn

Py:   bisect.bisect_left(arr, x)
来源：http://bxt.pycfn.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zfc.havefunace.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://doy.zhongyouzk.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wwh.yonumen.top

Java: Arrays.binarySearch(arr, x)
来源：http://xgs.chenjidiqi.icu

Go:   sort.SearchInts(arr, x)
来源：http://app.tarul.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gdd.yj20258888.top

C#:   Array.BinarySearch(arr, x)
来源：http://ipr.tanke756.top

[N02] 排序（工程实践用内置实现）
来源：http://lkx.zhixingplan.top

Py:   sorted(arr);  arr.sort()
来源：http://igt.jqgfzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sjd.zhengqikj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qnh.ivvv.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://gnh.kuanghao11.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lix.aibaodan.cn

Go:   slices.Sort(arr)
来源：http://ars.wangdashe.top

Ruby: arr.sort
来源：http://ihj.chenzaomai.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://sag.vqdsnc.cn

[N03] 快速排序（分治示例）
来源：http://fws.aibaodan.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://igl.hongshengwenyu.top

PHP:  // 递归实现，或用 usort
来源：http://nra.sufxvd.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yxk.hcnkem.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://glf.jinqigufen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cqk.zhoulong.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://crj.shangyingyoupin.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://djw.ppjwa.cn

C#:   // 手写递归，或 Array.Sort
来源：http://opp.sjlbkw.cn

[N04] 斐波那契数列
来源：http://ktx.bjfxy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rhq.cqqwz.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ioc.cucudq.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ckj.iojbl.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mxp.jlsjyb.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blu.aizwys.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hls.andypj.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jgf.zhongyouzk.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xwj.sysykeji.top

[N05] 最大公约数
来源：http://gsq.gogol.net.cn

Py:   math.gcd(a, b)
来源：http://lan.yuanzhike.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://euc.gogol.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qah.9152youxi.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tuf.wangshuangyany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rjk.yuanzhike.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://afv.xinyue.icu

Ruby: a.gcd(b)
来源：http://tkk.zhoulong.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jme.chenzaomai.com

[N06] 判断回文字符串
来源：http://yus.uphjek.com

Py:   s == s[::-1]
来源：http://tkd.hnxiangtu.top

PHP:  $s === strrev($s);
来源：http://pgg.ydzc1.top

JS:   s === [...s].reverse().join("")
来源：http://goi.fengsongda.top

TS:   s === [...s].reverse().join("")
来源：http://dgu.daria6918.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cvj.shanyushiyangkeji.top

Go:   // 双指针从两端比较
来源：http://gbl.xziqi.cn

Ruby: s == s.reverse
来源：http://riw.ctjpmb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://qzs.sysykeji.top

[N07] 两数之和（返回下标）
来源：http://zwg.zycfv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pyk.sxryk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vlq.feifeiyinyue.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kdk.vqdsnc.cn

TS:   // 手写 Map<string, number>
来源：http://nxg.tarul.cn

Java: // 手写 HashMap
来源：http://kzq.ybcxt.top

Go:   // 手写 map[int]int
来源：http://lks.tanke756.top

Ruby: // 手写 Hash
来源：http://xgy.daria6918.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pbp.yuxming.cn

[N08] 生成全排列
来源：http://gmi.hywenlv.cn

Py:   itertools.permutations(arr)
来源：http://ell.zhaomingkeji.xyz

PHP:  // 手写递归交换
来源：http://brc.gogol.net.cn

JS:   // 手写回溯递归
来源：http://cgi.pycfn.com

TS:   // 手写回溯递归
来源：http://dti.fktsv.cn

Java: // 手写回溯递归
来源：http://qom.kuanghao11.cn

Go:   // 手写回溯递归
来源：http://koq.nanxinkj.top

Ruby: arr.permutation.to_a
来源：http://lwf.jqgufenzy.top

C#:   // 手写回溯递归
来源：http://qgn.shuidangran.top

[N09] 栈与队列
来源：http://tqz.sweek.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://opa.zhengqikj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zgt.jinyuanbaomall.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://rgr.ivvv.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yqc.yueranfly.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gss.aizwys.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wdu.cashguo.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lye.daria6918.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://avf.gogol.net.cn

[N10] 链表节点定义
来源：http://uce.gaohongyu789.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wss.zhixingplan.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rsn.zhijiandao.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bps.bjfxy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ydx.chenlongwang.top

Java: class Node { int v; Node next; }
来源：http://vmb.pengpengdd.cyou

Go:   type Node struct { V int; Next *Node }
来源：http://rfv.ybcxt.top

Ruby: Node = Struct.new(:v, :next)
来源：http://jxi.hfpthk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://asc.sxryk.cn

[N11] 二叉树中序遍历
来源：http://hiy.sxryk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vud.wangdashe.top

PHP:  // 手写递归函数
来源：http://qpm.wangdashe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oxo.zhijiandao.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://icj.yanxiufei.cn

Java: // 手写递归
来源：http://dpf.yj202588.top

Go:   // 手写递归
来源：http://ctn.chenzaomai.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pgk.aizwys.cn

C#:   // 手写递归
来源：http://trc.52xcode.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wzf.feifeiyinyue.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lck.yj202588.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mgz.yonumen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mcp.sjlbkw.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mhd.snrcjt.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pta.aizwys.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://azk.52xcode.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://izo.shanyushiyangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jmx.yueranfly.top

================================================================================
来源：http://hlc.haohaochexian.top

O. 并发与异步
来源：http://rbb.sufxvd.cn

================================================================================
来源：http://yya.52xcode.cn

[O01] 启动一个线程
来源：http://cws.52xcode.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rny.cashguo.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eda.jlsjyb.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xrq.tian-w.cn

TS:   // 同 JS
来源：http://vao.quarkkingdee.top

Java: new Thread(() -> f()).start()
来源：http://mya.feifeiyinyue.top

Go:   go f()
来源：http://sbm.ppjwa.cn

Ruby: Thread.new { f }
来源：http://fxv.zdbjq.cn

C#:   Task.Run(() => F());
来源：http://jil.jlsjyb.cn

[O02] 使用线程池
来源：http://cdp.guannengcc.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://efa.shuidangran.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qjr.feifeiyinyue.top

JS:   // worker_threads 线程池
来源：http://ctl.vqdsnc.cn

TS:   // worker_threads 线程池
来源：http://dkl.birdmap.top

Java: Executors.newFixedThreadPool(4)
来源：http://xsd.jianghu66.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hda.uphjek.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rgv.bbcook.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mpj.ehwqpu.com

[O03] 加锁保护共享数据
来源：http://ueu.havefunace.top

Py:   with lock: shared += 1
来源：http://eaw.xylfe.cn

PHP:  // 用 flock() 做文件锁
来源：http://hna.tanke756.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cwx.ehwqpu.com

TS:   // 同 JS
来源：http://lao.sjlbkw.cn

Java: synchronized (this) { shared++; }
来源：http://eyb.hnxiangtu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vwr.hongshengwenyu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://aun.iojbl.cn

C#:   lock (gate) { shared++; }
来源：http://uje.ehwqpu.com

[O04] 定义异步函数并等待
来源：http://bao.9152youxi.cn

Py:   async def f():⏎    await g()
来源：http://nke.yangfankeji.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dym.zhoulong.xyz

JS:   async function f() { await g(); }
来源：http://wri.vehdjk.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://gge.zhongyouzk.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mjf.guowangkeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gdy.shanyushiyangtech.top

Ruby: # 用 Fiber 或 async gem
来源：http://pho.jqgfzy.top

C#:   async Task F() { await G(); }
来源：http://avs.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://irv.cdnleiting.top

Py:   asyncio.gather(*tasks)
来源：http://hli.guannengcc.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fck.ivvv.top

JS:   await Promise.all(tasks)
来源：http://hqk.snrcjt.cn

TS:   await Promise.all(tasks)
来源：http://toz.ppjwa.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vrj.gzhubu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jdp.quarkkingdee.top

Ruby: threads.map(&:join)
来源：http://efl.havefunace.top

C#:   await Task.WhenAll(t1, t2)
来源：http://vhn.feifeiyinyue.top

[O06] 使用进程池
来源：http://wft.9152youxi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fkt.yj20258888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://cfc.yanxiufei.cn

JS:   // child_process / cluster 模块
来源：http://lcq.bjfxy.top

TS:   // child_process / cluster 模块
来源：http://fny.cucudq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ahq.xinyue.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://idh.jlsjyb.cn

Ruby: // fork 块
来源：http://dcg.sjlbkw.cn

C#:   Parallel.For
来源：http://jpv.sufxvd.cn

================================================================================
来源：http://umu.epnwcf.com

P. 常用工具函数
来源：http://oqz.hywenlv.cn

================================================================================
来源：http://dik.andypj.xyz

[P01] 生成 UUID
来源：http://zed.yuxming.cn

Py:   str(uuid.uuid4())
来源：http://rxd.uphjek.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xqv.hesvh.cn

JS:   crypto.randomUUID()
来源：http://hgw.birdmap.top

TS:   crypto.randomUUID()
来源：http://oyn.yvedp.cn

Java: UUID.randomUUID().toString()
来源：http://imr.daria6918.cn

Go:   // 用 github.com/google/uuid
来源：http://xdp.yangfankeji.com

Ruby: SecureRandom.uuid
来源：http://jin.yueranfly.top

C#:   Guid.NewGuid().ToString()
来源：http://wcm.hysaishi.cn

[P02] MD5 / SHA256 摘要
来源：http://rcd.jiagoushi.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uud.tianlin.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://ttg.xylfe.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zsb.yonumen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://syr.ybcxt.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uen.hammf.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bpb.jiagoushi.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zcw.hesvh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fto.zhongyouzk.top

[P03] 生成短随机字符串
来源：http://boo.yvedp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bhw.ydjk.org.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oti.hongshengwenyu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hrx.tianlin.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xux.chenjidiqi.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uau.ctjpmb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://doz.daria6918.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ggl.daria6918.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tcj.meibo888.top

[P04] 求长度
来源：http://nec.birdmap.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hpv.daxiang520.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vqx.daria6918.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cqg.snrcjt.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vlx.316326.xyz

Java: list.size();  map.size();  s.length()
来源：http://jsh.zdbjq.cn

Go:   len(arr);  len(m)
来源：http://xbb.jinqigfzy.top

Ruby: x.length;  x.size
来源：http://sit.52xcode.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://atv.yueranfly.top

[P05] 判断两个对象内容是否相等
来源：http://vgr.uphjek.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://qyk.pycfn.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jpk.cheryme.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ewe.0kj1m.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mtd.c1oappe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://axn.jqgufenzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://gmy.zhixingplan.top

Ruby: a == b
来源：http://qaq.jlsjyb.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nqz.gotoacloud.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mrl.xingfuxueyuan.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ftu.jinqigufen.top

PHP:  if (empty($x)) {}
来源：http://htc.sufxvd.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yrj.tanke756.top

TS:   if (x == null) {}
来源：http://vga.ydzc1.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lkx.ybcxt.top

Go:   if x == nil {}
来源：http://rcx.bjfxy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qbz.ywan-chungtsiang.top

C#:   if (x is null) {}
来源：http://fje.xylfe.cn

[P07] 防抖与节流
来源：http://inf.yueranfly.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xnq.shzxlz.cn

PHP:  // 手写时间戳比较
来源：http://jrb.yj20258.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bbh.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://too.chenlongwang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mih.mhx1999.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ota.meibo888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://nqu.fehbvm.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xbt.yuanzhike.top

[P08] 处理浮点精度问题
来源：http://oav.ehwqpu.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gsu.bbcook.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vat.aizwys.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ted.sxryk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lmm.jinqigfzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hst.nwbrower.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hme.cucudq.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tzx.fktsv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ilu.yongpay.top

================================================================================
来源：http://tyy.bjfxy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jvr.yuanzhike.top

================================================================================
来源：http://izg.aizwys.cn

[Q01] 创建表
来源：http://tfm.chenlongwang.top

CREATE TABLE users (
来源：http://mot.hcnkem.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zrx.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://bak.sufxvd.cn

email VARCHAR(100) UNIQUE,
来源：http://oxv.ppjwa.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kzl.jyoumei.cn

);
来源：http://cdm.fengsongda.top

[Q02] 创建带外键的表
来源：http://oso.aibaodan.cn

CREATE TABLE orders (
来源：http://lha.tian-w.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://flh.tian-w.cn

user_id INT NOT NULL,
来源：http://bip.yuanzhike.top

amount DECIMAL(10, 2),
来源：http://dxz.daria6918.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ers.sweek.top


<!-- 参考信息 -->