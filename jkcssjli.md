代发 wailian999

TS:   process.cwd()
来源：http://mlv.chenzaomai.com

Java: Path.of("").toAbsolutePath()
来源：http://gpy.yj202588.top

Go:   os.Getwd()
来源：http://fjt.zdbjq.cn

Ruby: Dir.pwd
来源：http://asl.zhengqikj.top

C#:   Directory.GetCurrentDirectory()
来源：http://lgj.jqgfzy.top

[M05] 设置退出码
来源：http://lwf.aibaodan.cn

Py:   sys.exit(1)
来源：http://xbm.sweek.top

PHP:  exit(1);
来源：http://dhv.feifeiyinyue.top

JS:   process.exit(1)
来源：http://jfc.jinghuilouyu.cn

TS:   process.exit(1)
来源：http://jtj.hcnkem.com

Java: System.exit(1)
来源：http://lux.zhixingplan.top

Go:   os.Exit(1)
来源：http://qen.ydjk.org.cn

Ruby: exit 1
来源：http://amv.zdbjq.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://zzy.xziqi.cn

[M06] 向标准错误输出
来源：http://gci.hesvh.cn

Py:   print("err", file=sys.stderr)
来源：http://ujb.chenlongwang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qpi.jianghu66.top

JS:   console.error("err")
来源：http://ntb.nanxuanxn.top

TS:   console.error("err")
来源：http://glr.shzxlz.cn

Java: System.err.println("err")
来源：http://jib.jinqigufen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lth.hywenlv.cn

Ruby: warn "err"
来源：http://sok.xuanzx.com

C#:   Console.Error.WriteLine("err")
来源：http://tam.shanyushiyangkeji.top

[M07] 判断是否为主入口
来源：http://uum.yj202588.top

Py:   if __name__ == "__main__":
来源：http://smb.yuxming.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xqk.tianlin.xyz

JS:   require.main === module
来源：http://hem.svipenyu.cn

TS:   require.main === module
来源：http://qru.c1oappe.top

Java: public static void main(String[] args)
来源：http://mjv.yfazqb.com

Go:   func main()
来源：http://pxb.fanxiaobao.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vrx.haohaochexian.top

C#:   static void Main(string[] args)
来源：http://lky.hnqzz.top

[M08] 获取系统与运行时信息
来源：http://qqi.52xcode.cn

Py:   platform.system();  platform.python_version()
来源：http://pej.vqdsnc.cn

PHP:  PHP_OS;  phpversion();
来源：http://ked.ydzc1.top

JS:   process.platform;  process.version
来源：http://yfl.sysykeji.top

TS:   process.platform;  process.version
来源：http://tdy.gogol.net.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mku.fktsv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sas.snrcjt.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dmz.xinyue.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://wnu.yj202588.top

================================================================================
来源：http://bmp.bbcook.cn

N. 数据结构与算法
来源：http://bog.nwbrower.top

================================================================================
来源：http://ofs.gotoacloud.top

[N01] 二分查找（有序数组）
来源：http://reu.gaohongyu789.top

Py:   bisect.bisect_left(arr, x)
来源：http://pbm.cheryme.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fvx.sxryk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jau.haohaochexian.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gtv.zycfv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ude.shzxlz.cn

Go:   sort.SearchInts(arr, x)
来源：http://gzz.0kj1m.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xni.chenzaomai.com

C#:   Array.BinarySearch(arr, x)
来源：http://ioh.xziqi.cn

[N02] 排序（工程实践用内置实现）
来源：http://gpj.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://bsb.jyoumei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kwz.guannengcc.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://dki.yueranfly.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ssk.ydjk.org.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://azk.shzxlz.cn

Go:   slices.Sort(arr)
来源：http://viv.c1oappe.top

Ruby: arr.sort
来源：http://fgl.jqgufenzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://wlk.vqdsnc.cn

[N03] 快速排序（分治示例）
来源：http://zmw.feifeiyinyue.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xgx.jinyuanbaomall.cn

PHP:  // 递归实现，或用 usort
来源：http://hcb.fktsv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vau.wangshuangyany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fkr.xingfuxueyuan.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hib.jlsjyb.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sra.yuxming.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jbn.zdqjudy.top

C#:   // 手写递归，或 Array.Sort
来源：http://qli.iojbl.cn

[N04] 斐波那契数列
来源：http://yte.yongpay.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://isk.fehbvm.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pdy.cashguo.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sfa.zdqjudy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ehw.gaohongyu789.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nab.yj202588.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ddm.hesvh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ilt.havefunace.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nqp.ehwqpu.com

[N05] 最大公约数
来源：http://dvl.yuanzhike.top

Py:   math.gcd(a, b)
来源：http://tdf.sufxvd.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ywx.hammf.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dwc.yvedp.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wjg.wangshuangyany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ety.xuanzx.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nmy.fktsv.cn

Ruby: a.gcd(b)
来源：http://igh.hcnkem.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zvs.snrcjt.cn

[N06] 判断回文字符串
来源：http://yzu.guowangkeji.top

Py:   s == s[::-1]
来源：http://ice.havefunace.top

PHP:  $s === strrev($s);
来源：http://jpo.hnxiangtu.top

JS:   s === [...s].reverse().join("")
来源：http://tci.chenjidiqi.icu

TS:   s === [...s].reverse().join("")
来源：http://ebd.c1oappe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ifw.xuetiantiany.cn

Go:   // 双指针从两端比较
来源：http://lsm.svipenyu.cn

Ruby: s == s.reverse
来源：http://mgd.yongpay.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lil.cdnleiting.top

[N07] 两数之和（返回下标）
来源：http://rxi.yj202588.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uoe.smart0.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pka.zdbjq.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jwn.ywan-chungtsiang.top

TS:   // 手写 Map<string, number>
来源：http://zlb.dashuyun.cn

Java: // 手写 HashMap
来源：http://ade.yj20258888.top

Go:   // 手写 map[int]int
来源：http://hcd.ppjwa.cn

Ruby: // 手写 Hash
来源：http://mxs.epnwcf.com

C#:   // 手写 Dictionary<int, int>
来源：http://uvx.c1oappe.top

[N08] 生成全排列
来源：http://xuh.yfazqb.com

Py:   itertools.permutations(arr)
来源：http://dxv.jianghu66.top

PHP:  // 手写递归交换
来源：http://tme.xinyue.icu

JS:   // 手写回溯递归
来源：http://eca.chenjidiqi.icu

TS:   // 手写回溯递归
来源：http://dcb.jinghuilouyu.cn

Java: // 手写回溯递归
来源：http://ybs.xylfe.cn

Go:   // 手写回溯递归
来源：http://swe.zhijiandao.cn

Ruby: arr.permutation.to_a
来源：http://ged.pycfn.com

C#:   // 手写回溯递归
来源：http://vkw.shuidangran.top

[N09] 栈与队列
来源：http://mwu.jinyuanbaomall.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mzc.yvedp.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nkj.fehbvm.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xqn.guannengcc.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://urk.nanxinkj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wxg.bjfxy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ymm.nwbrower.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jst.smart0.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ddo.ppjwa.cn

[N10] 链表节点定义
来源：http://wyq.bjfxy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ffv.316326.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://tgv.ybcxt.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://iqk.havefunace.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://esa.guannengcc.top

Java: class Node { int v; Node next; }
来源：http://ltr.c1oappe.top

Go:   type Node struct { V int; Next *Node }
来源：http://hhw.jiagoushi.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wha.cashguo.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qsd.zhaomingkeji.xyz

[N11] 二叉树中序遍历
来源：http://ryh.hongshengwenyu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://szc.yueranfly.top

PHP:  // 手写递归函数
来源：http://akl.bbcook.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kqf.xziqi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gae.epnwcf.com

Java: // 手写递归
来源：http://mnk.jinghuilouyu.cn

Go:   // 手写递归
来源：http://ftl.epnwcf.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qmg.jinqigfzy.top

C#:   // 手写递归
来源：http://rtw.shanyushiyangkeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nnm.yongpay.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://coz.sxryk.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://alm.sysykeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tok.gogol.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://psw.xinyue.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://shf.xingfuxueyuan.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mcp.bbcook.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hky.yvedp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ucq.tanke756.top

================================================================================
来源：http://yrq.cdnleiting.top

O. 并发与异步
来源：http://gcv.zhiwuduotai.top

================================================================================
来源：http://nty.xziqi.cn

[O01] 启动一个线程
来源：http://whv.hfpthk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xxa.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cre.aizwys.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://umd.hfpthk.cn

TS:   // 同 JS
来源：http://jjp.sysykeji.top

Java: new Thread(() -> f()).start()
来源：http://pin.gaohongyu789.top

Go:   go f()
来源：http://lwg.tanke756.top

Ruby: Thread.new { f }
来源：http://tuk.yuanzhike.top

C#:   Task.Run(() => F());
来源：http://fea.bjfxy.top

[O02] 使用线程池
来源：http://tao.fanxiaobao.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fjx.sufxvd.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kbf.gzhubu.top

JS:   // worker_threads 线程池
来源：http://isd.jinyuanbaomall.cn

TS:   // worker_threads 线程池
来源：http://uwe.gzhubu.top

Java: Executors.newFixedThreadPool(4)
来源：http://dpz.jyoumei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://epj.svipenyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jzi.cqqwz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bnu.uphjek.com

[O03] 加锁保护共享数据
来源：http://ruz.jinqigfzy.top

Py:   with lock: shared += 1
来源：http://fqc.yj20258.top

PHP:  // 用 flock() 做文件锁
来源：http://stl.fanxiaobao.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vhh.zycfv.cn

TS:   // 同 JS
来源：http://yot.jyoumei.cn

Java: synchronized (this) { shared++; }
来源：http://jnl.tarul.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kjp.pengpengdd.cyou

Ruby: mutex.synchronize { shared += 1 }
来源：http://sdi.uphjek.com

C#:   lock (gate) { shared++; }
来源：http://ebz.zycfv.cn

[O04] 定义异步函数并等待
来源：http://pmf.ybcxt.top

Py:   async def f():⏎    await g()
来源：http://utn.jiagoushi.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jtu.yuxming.cn

JS:   async function f() { await g(); }
来源：http://mlo.hnxiangtu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://mxf.cashguo.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://njd.hongshengwenyu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nhk.jinyuanbaomall.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wvi.pycfn.com

C#:   async Task F() { await G(); }
来源：http://suo.ctjpmb.com

[O05] 并发执行并等待全部完成
来源：http://ulc.bjfxy.top

Py:   asyncio.gather(*tasks)
来源：http://rcs.chenjidiqi.icu

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xnb.jinyuanbaomall.cn

JS:   await Promise.all(tasks)
来源：http://rks.fzhhl.top

TS:   await Promise.all(tasks)
来源：http://nsr.wangdashe.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cye.9152youxi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qtw.zhoulong.xyz

Ruby: threads.map(&:join)
来源：http://cpi.pengpengdd.cyou

C#:   await Task.WhenAll(t1, t2)
来源：http://hsm.yanxiufei.cn

[O06] 使用进程池
来源：http://jvg.xuetiantiany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zuw.iojbl.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://hdf.vqdsnc.cn

JS:   // child_process / cluster 模块
来源：http://sqo.ivvv.top

TS:   // child_process / cluster 模块
来源：http://zkn.redwolf501.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fas.fehbvm.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://swq.nanxuanxn.top

Ruby: // fork 块
来源：http://gxr.0kj1m.cn

C#:   Parallel.For
来源：http://gxl.daxiang520.top

================================================================================
来源：http://yhy.tarul.cn

P. 常用工具函数
来源：http://jep.sxryk.cn

================================================================================
来源：http://eav.zdqjudy.top

[P01] 生成 UUID
来源：http://ade.hnxiangtu.top

Py:   str(uuid.uuid4())
来源：http://gry.xylfe.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ddh.cheryme.top

JS:   crypto.randomUUID()
来源：http://lhd.shzxlz.cn

TS:   crypto.randomUUID()
来源：http://ttd.dashuyun.cn

Java: UUID.randomUUID().toString()
来源：http://vty.vehdjk.com

Go:   // 用 github.com/google/uuid
来源：http://cmq.0kj1m.cn

Ruby: SecureRandom.uuid
来源：http://ias.ydjk.org.cn

C#:   Guid.NewGuid().ToString()
来源：http://fem.zhijiandao.cn

[P02] MD5 / SHA256 摘要
来源：http://cin.tianlin.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://enc.shuidangran.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://yfo.gaohongyu789.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://moe.ydjk.org.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ftx.jlsjyb.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ktz.jianghu66.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eop.chenjidiqi.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kqg.jianghu66.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qup.316326.xyz

[P03] 生成短随机字符串
来源：http://tfq.snrcjt.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://chx.snrcjt.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vuk.xuanzx.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rwh.guowangkeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yha.fehbvm.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://suu.yfazqb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nit.sjlbkw.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nfy.ctjpmb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ino.ydjk.org.cn

[P04] 求长度
来源：http://ypb.xinyue.icu

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nkq.hnqzz.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ofx.tian-w.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iak.gotoacloud.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yvm.yj202588.top

Java: list.size();  map.size();  s.length()
来源：http://nkz.hfpthk.cn

Go:   len(arr);  len(m)
来源：http://epx.dashuyun.cn

Ruby: x.length;  x.size
来源：http://dxw.gaohongyu789.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://chv.cdnleiting.top

[P05] 判断两个对象内容是否相等
来源：http://mso.epnwcf.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://rcm.yuanzhike.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dei.nanxinkj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kjt.cqqwz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cyw.hnxiangtu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://riv.jinqigfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://hvx.hysaishi.cn

Ruby: a == b
来源：http://brx.gogol.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fwz.snrcjt.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://asu.zycfv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cax.nwbrower.top

PHP:  if (empty($x)) {}
来源：http://xvp.pengpengdd.cyou

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mwm.jiagoushi.top

TS:   if (x == null) {}
来源：http://yws.jinqigufen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://acs.yj202588.top

Go:   if x == nil {}
来源：http://jcb.jinqigfzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://suk.shzxlz.cn

C#:   if (x is null) {}
来源：http://fii.hywenlv.cn

[P07] 防抖与节流
来源：http://hew.daxiang520.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dis.bjfxy.top

PHP:  // 手写时间戳比较
来源：http://ume.gogol.net.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wrj.haohaochexian.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gka.dianchejie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fei.zhongyouzk.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ibp.hfpthk.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zxj.jiagoushi.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://drb.chenjidiqi.icu

[P08] 处理浮点精度问题
来源：http://qlp.hesvh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fcl.jinyuanbaomall.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vnt.feifeiyinyue.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hms.guowangkeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dgh.yvedp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baa.zdqjudy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eqa.shangyingyoupin.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://chd.shanyushiyangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rtp.cashguo.top

================================================================================
来源：http://pem.hesvh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wkv.daxiang520.top

================================================================================
来源：http://ulx.yfazqb.com

[Q01] 创建表
来源：http://aeu.tianlin.xyz

CREATE TABLE users (
来源：http://bav.meibo888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wsh.nwbrower.top

name VARCHAR(50) NOT NULL,
来源：http://rkl.gaohongyu789.top

email VARCHAR(100) UNIQUE,
来源：http://ydr.feifeiyinyue.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pld.yonumen.top

);
来源：http://jhn.shanyushiyangtech.top

[Q02] 创建带外键的表
来源：http://kmd.yongpay.top

CREATE TABLE orders (
来源：http://hzf.aizwys.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dqy.316326.xyz

user_id INT NOT NULL,
来源：http://uex.guannengcc.top

amount DECIMAL(10, 2),
来源：http://hiy.yanxiufei.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://irj.wangdashe.top


<!-- 参考信息 -->