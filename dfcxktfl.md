代发 wailian999

[M04] 获取当前工作目录
来源：http://bsg.nanxuanxn.top

Py:   os.getcwd()
来源：http://eqw.yuanzhike.top

PHP:  getcwd();
来源：http://vux.shzxlz.cn

JS:   process.cwd()
来源：http://mxl.quarkkingdee.top

TS:   process.cwd()
来源：http://tvp.shangyingyoupin.top

Java: Path.of("").toAbsolutePath()
来源：http://wic.zhoulong.xyz

Go:   os.Getwd()
来源：http://dcg.gaohongyu789.top

Ruby: Dir.pwd
来源：http://wuo.c1oappe.top

C#:   Directory.GetCurrentDirectory()
来源：http://csf.cheryme.top

[M05] 设置退出码
来源：http://zow.chenlongwang.top

Py:   sys.exit(1)
来源：http://jhh.xuetiantiany.cn

PHP:  exit(1);
来源：http://kzg.quarkkingdee.top

JS:   process.exit(1)
来源：http://zta.shanyushiyangtech.top

TS:   process.exit(1)
来源：http://zsr.xuanzx.com

Java: System.exit(1)
来源：http://yys.tarul.cn

Go:   os.Exit(1)
来源：http://gpr.shzxlz.cn

Ruby: exit 1
来源：http://svc.ydzc1.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gql.zdqjudy.top

[M06] 向标准错误输出
来源：http://krk.jlsjyb.cn

Py:   print("err", file=sys.stderr)
来源：http://tmg.tanke756.top

PHP:  fwrite(STDERR, "err\n");
来源：http://jcs.epnwcf.com

JS:   console.error("err")
来源：http://mhq.xylfe.cn

TS:   console.error("err")
来源：http://wll.jinqigfzy.top

Java: System.err.println("err")
来源：http://vxs.chenzaomai.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://duo.nwbrower.top

Ruby: warn "err"
来源：http://nxq.aibaodan.cn

C#:   Console.Error.WriteLine("err")
来源：http://wtx.iojbl.cn

[M07] 判断是否为主入口
来源：http://mfy.ywan-chungtsiang.top

Py:   if __name__ == "__main__":
来源：http://umm.gotoacloud.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aco.feifeiyinyue.top

JS:   require.main === module
来源：http://wah.bjfxy.top

TS:   require.main === module
来源：http://typ.jyoumei.cn

Java: public static void main(String[] args)
来源：http://uvb.jinqigfzy.top

Go:   func main()
来源：http://pxj.sysykeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mle.yueranfly.top

C#:   static void Main(string[] args)
来源：http://lyu.cqqwz.cn

[M08] 获取系统与运行时信息
来源：http://yfy.yj20258888.top

Py:   platform.system();  platform.python_version()
来源：http://qoi.haohaochexian.top

PHP:  PHP_OS;  phpversion();
来源：http://zpl.fengsongda.top

JS:   process.platform;  process.version
来源：http://dvv.nanxinkj.top

TS:   process.platform;  process.version
来源：http://rkz.gotoacloud.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jto.ydjk.org.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://khb.quarkkingdee.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tjy.hnxiangtu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tyu.dashuyun.cn

================================================================================
来源：http://pra.yj202588.top

N. 数据结构与算法
来源：http://bnp.nwbrower.top

================================================================================
来源：http://pnm.feifeiyinyue.top

[N01] 二分查找（有序数组）
来源：http://otv.zdqjudy.top

Py:   bisect.bisect_left(arr, x)
来源：http://bjy.iojbl.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wpi.yueranfly.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hlg.quarkkingdee.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qfr.cqqwz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ppc.ybcxt.top

Go:   sort.SearchInts(arr, x)
来源：http://hou.wangdashe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zqv.yangfankeji.com

C#:   Array.BinarySearch(arr, x)
来源：http://zrt.ydzc1.top

[N02] 排序（工程实践用内置实现）
来源：http://kdo.fanxiaobao.xyz

Py:   sorted(arr);  arr.sort()
来源：http://nug.xuanzx.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://guy.andypj.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://ihc.snrcjt.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://iif.zhongyouzk.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hab.xuetiantiany.cn

Go:   slices.Sort(arr)
来源：http://rfn.hesvh.cn

Ruby: arr.sort
来源：http://vrf.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://rwc.fktsv.cn

[N03] 快速排序（分治示例）
来源：http://ldt.aibaodan.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rqi.ybcxt.top

PHP:  // 递归实现，或用 usort
来源：http://rpm.fanxiaobao.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lgh.hywenlv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jig.gzhubu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cyn.shanyushiyangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bvg.yonumen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zau.tian-w.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gsh.aizwys.cn

[N04] 斐波那契数列
来源：http://dfr.0kj1m.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://znm.hnxiangtu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vge.nanxuanxn.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wym.sxryk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cqn.uphjek.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lzf.hammf.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rbm.zdbjq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dni.hysaishi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dub.dashuyun.cn

[N05] 最大公约数
来源：http://ryp.smart0.xyz

Py:   math.gcd(a, b)
来源：http://pzn.zycfv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pkp.zhengqikj.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uuq.shanyushiyangtech.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lue.cashguo.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pbk.mhx1999.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sfq.gogol.net.cn

Ruby: a.gcd(b)
来源：http://grn.jinqigufen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gqs.hammf.cn

[N06] 判断回文字符串
来源：http://ivv.snrcjt.cn

Py:   s == s[::-1]
来源：http://nqr.cheryme.top

PHP:  $s === strrev($s);
来源：http://xqf.feifeiyinyue.top

JS:   s === [...s].reverse().join("")
来源：http://bev.shzxlz.cn

TS:   s === [...s].reverse().join("")
来源：http://ndp.cheryme.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://omy.daria6918.cn

Go:   // 双指针从两端比较
来源：http://jvf.jqgfzy.top

Ruby: s == s.reverse
来源：http://gbl.cheryme.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dyk.guannengcc.top

[N07] 两数之和（返回下标）
来源：http://lvb.ywan-chungtsiang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ceb.xuetiantiany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eku.ehwqpu.com

JS:   // 手写 Map：map.set(v, i)
来源：http://bhb.ydzc1.top

TS:   // 手写 Map<string, number>
来源：http://ooe.ybcxt.top

Java: // 手写 HashMap
来源：http://xky.dianchejie.cn

Go:   // 手写 map[int]int
来源：http://nyz.dianchejie.cn

Ruby: // 手写 Hash
来源：http://aok.aizwys.cn

C#:   // 手写 Dictionary<int, int>
来源：http://djb.cashguo.top

[N08] 生成全排列
来源：http://nnp.haohaochexian.top

Py:   itertools.permutations(arr)
来源：http://wbt.wangshuangyany.cn

PHP:  // 手写递归交换
来源：http://mql.hcnkem.com

JS:   // 手写回溯递归
来源：http://tbn.hnxiangtu.top

TS:   // 手写回溯递归
来源：http://mtl.hfpthk.cn

Java: // 手写回溯递归
来源：http://fcs.havefunace.top

Go:   // 手写回溯递归
来源：http://kxy.fktsv.cn

Ruby: arr.permutation.to_a
来源：http://emu.jianghu66.top

C#:   // 手写回溯递归
来源：http://mux.bjfxy.top

[N09] 栈与队列
来源：http://vxz.ydzc1.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://afg.redwolf501.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zow.sjlbkw.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lnz.fktsv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fqb.sweek.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pzq.sjlbkw.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://azb.feifeiyinyue.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fsw.hesvh.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://odx.nanxuanxn.top

[N10] 链表节点定义
来源：http://qko.hcnkem.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ptb.9152youxi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mrx.hammf.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wjk.shangyingyoupin.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ekr.cucudq.cn

Java: class Node { int v; Node next; }
来源：http://rin.daxiang520.top

Go:   type Node struct { V int; Next *Node }
来源：http://fme.andypj.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://von.hcnkem.com

C#:   class Node { public int V; public Node? Next; }
来源：http://vmr.fzhhl.top

[N11] 二叉树中序遍历
来源：http://cgg.shzxlz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xyn.jinyuanbaomall.cn

PHP:  // 手写递归函数
来源：http://xir.birdmap.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://swg.gogol.net.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wwt.nanxinkj.top

Java: // 手写递归
来源：http://sfw.iojbl.cn

Go:   // 手写递归
来源：http://tod.wangdashe.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dum.guowangkeji.top

C#:   // 手写递归
来源：http://xov.xinyue.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rnh.yangfankeji.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lqn.ivvv.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cob.mhx1999.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tka.jqgfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pok.fengsongda.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zft.guannengcc.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://uaa.jinqigfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://frz.chenzaomai.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sib.snrcjt.cn

================================================================================
来源：http://pwp.epnwcf.com

O. 并发与异步
来源：http://chq.ppjwa.cn

================================================================================
来源：http://csc.gotoacloud.top

[O01] 启动一个线程
来源：http://ssl.daxiang520.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://byc.zhiwuduotai.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xav.yj202588.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rpl.birdmap.top

TS:   // 同 JS
来源：http://jze.ydzc1.top

Java: new Thread(() -> f()).start()
来源：http://opy.jianghu66.top

Go:   go f()
来源：http://ins.zhongyouzk.top

Ruby: Thread.new { f }
来源：http://bop.sweek.top

C#:   Task.Run(() => F());
来源：http://ivx.jinqigufen.top

[O02] 使用线程池
来源：http://ovf.yuxming.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nfg.jinqigufen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://olf.cheryme.top

JS:   // worker_threads 线程池
来源：http://vgv.sweek.top

TS:   // worker_threads 线程池
来源：http://ulr.zycfv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kua.xuanzx.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jxj.tian-w.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://awp.gotoacloud.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kvm.smart0.xyz

[O03] 加锁保护共享数据
来源：http://pbr.yongpay.top

Py:   with lock: shared += 1
来源：http://xhz.ehwqpu.com

PHP:  // 用 flock() 做文件锁
来源：http://oqr.nanxuanxn.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qay.zhijiandao.cn

TS:   // 同 JS
来源：http://ixo.c1oappe.top

Java: synchronized (this) { shared++; }
来源：http://ucp.xuetiantiany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hny.yj20258888.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://aas.yj20258.top

C#:   lock (gate) { shared++; }
来源：http://bry.svipenyu.cn

[O04] 定义异步函数并等待
来源：http://yzq.xylfe.cn

Py:   async def f():⏎    await g()
来源：http://nrl.tian-w.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vwp.chenlongwang.top

JS:   async function f() { await g(); }
来源：http://pyi.hywenlv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mkv.cdnleiting.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rje.zdbjq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ioi.shzxlz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://muc.yangfankeji.com

C#:   async Task F() { await G(); }
来源：http://llm.yonumen.top

[O05] 并发执行并等待全部完成
来源：http://sxl.jinghuilouyu.cn

Py:   asyncio.gather(*tasks)
来源：http://umj.tian-w.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pus.guannengcc.top

JS:   await Promise.all(tasks)
来源：http://hqn.jianghu66.top

TS:   await Promise.all(tasks)
来源：http://ows.316326.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yjw.zhixingplan.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jbu.hesvh.cn

Ruby: threads.map(&:join)
来源：http://pbo.nanxinkj.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mfx.hesvh.cn

[O06] 使用进程池
来源：http://ogi.hnxiangtu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zhe.9152youxi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tpv.jianghu66.top

JS:   // child_process / cluster 模块
来源：http://uxo.shangyingyoupin.top

TS:   // child_process / cluster 模块
来源：http://zqm.fanxiaobao.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rvf.jinyuanbaomall.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gia.svipenyu.cn

Ruby: // fork 块
来源：http://wrf.shanyushiyangtech.top

C#:   Parallel.For
来源：http://keg.jlsjyb.cn

================================================================================
来源：http://egz.jinyuanbaomall.cn

P. 常用工具函数
来源：http://bhw.chenzaomai.com

================================================================================
来源：http://zin.fanxiaobao.xyz

[P01] 生成 UUID
来源：http://jdv.nanxinkj.top

Py:   str(uuid.uuid4())
来源：http://buv.chenjidiqi.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kic.guannengcc.top

JS:   crypto.randomUUID()
来源：http://wud.gzhubu.top

TS:   crypto.randomUUID()
来源：http://qga.zhaomingkeji.xyz

Java: UUID.randomUUID().toString()
来源：http://krm.xylfe.cn

Go:   // 用 github.com/google/uuid
来源：http://hqk.zhixingplan.top

Ruby: SecureRandom.uuid
来源：http://krb.jqgufenzy.top

C#:   Guid.NewGuid().ToString()
来源：http://dbe.ydjk.org.cn

[P02] MD5 / SHA256 摘要
来源：http://syq.yongpay.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kkg.guowangkeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qdj.ydzc1.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ggp.andypj.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://goy.meibo888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dbq.vqdsnc.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mgl.kuanghao11.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://amd.haohaochexian.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qrs.aibaodan.cn

[P03] 生成短随机字符串
来源：http://cuc.daxiang520.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://urn.quarkkingdee.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ton.bjfxy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://acu.xingfuxueyuan.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nik.jqgufenzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vbx.xingfuxueyuan.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qom.wangshuangyany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vsm.yueranfly.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ehd.jqgufenzy.top

[P04] 求长度
来源：http://ekl.yfazqb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cqy.wangshuangyany.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://akx.andypj.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ajs.zhoulong.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mxr.ivvv.top

Java: list.size();  map.size();  s.length()
来源：http://wpw.hysaishi.cn

Go:   len(arr);  len(m)
来源：http://gny.shanyushiyangkeji.top

Ruby: x.length;  x.size
来源：http://myd.jlsjyb.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gbg.shuidangran.top

[P05] 判断两个对象内容是否相等
来源：http://hrl.hesvh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://czi.zycfv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nox.xingfuxueyuan.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://akt.havefunace.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qoc.meibo888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://aia.andypj.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://ifd.zhiwuduotai.top

Ruby: a == b
来源：http://sfe.hongshengwenyu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://abw.yj202588.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gsx.ctjpmb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wpv.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}
来源：http://fvd.snrcjt.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lry.zdqjudy.top

TS:   if (x == null) {}
来源：http://toe.yfazqb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://gyd.redwolf501.top

Go:   if x == nil {}
来源：http://jml.yj20258888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oba.jqgufenzy.top

C#:   if (x is null) {}
来源：http://qxw.jinqigfzy.top

[P07] 防抖与节流
来源：http://noh.316326.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aeg.52xcode.cn

PHP:  // 手写时间戳比较
来源：http://ptx.nwbrower.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gri.shuidangran.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://umy.sxryk.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://imi.xuetiantiany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://emh.aibaodan.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://llz.hesvh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qxg.hongshengwenyu.top

[P08] 处理浮点精度问题
来源：http://iez.daria6918.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fvi.xylfe.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gry.zdbjq.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jmv.shangyingyoupin.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uil.aizwys.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sts.hongshengwenyu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pta.316326.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cqx.cdnleiting.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xrn.ctjpmb.com

================================================================================
来源：http://rcy.sysykeji.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://omp.zdbjq.cn

================================================================================
来源：http://txa.quarkkingdee.top

[Q01] 创建表
来源：http://eoc.52xcode.cn

CREATE TABLE users (
来源：http://xkw.epnwcf.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zuh.zhiwuduotai.top

name VARCHAR(50) NOT NULL,
来源：http://vgv.hfpthk.cn

email VARCHAR(100) UNIQUE,
来源：http://yjl.feifeiyinyue.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lus.shzxlz.cn

);
来源：http://uog.daxiang520.top

[Q02] 创建带外键的表
来源：http://xej.jinyuanbaomall.cn

CREATE TABLE orders (
来源：http://shq.wangshuangyany.cn


<!-- 参考信息 -->