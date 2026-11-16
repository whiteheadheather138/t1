代发 wailian999

TS:   process.cwd()
来源：http://wde.jinqigfzy.top

Java: Path.of("").toAbsolutePath()
来源：http://xco.zhiwuduotai.top

Go:   os.Getwd()
来源：http://rqi.epnwcf.com

Ruby: Dir.pwd
来源：http://got.tianlin.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://ezj.yfazqb.com

[M05] 设置退出码
来源：http://pgb.0kj1m.cn

Py:   sys.exit(1)
来源：http://dkm.9152youxi.cn

PHP:  exit(1);
来源：http://tbt.hywenlv.cn

JS:   process.exit(1)
来源：http://nia.jianghu66.top

TS:   process.exit(1)
来源：http://wws.jianghu66.top

Java: System.exit(1)
来源：http://rvx.yj20258888.top

Go:   os.Exit(1)
来源：http://qif.aizwys.cn

Ruby: exit 1
来源：http://rhd.ctjpmb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mqd.yangfankeji.com

[M06] 向标准错误输出
来源：http://ago.jqgfzy.top

Py:   print("err", file=sys.stderr)
来源：http://gbc.daria6918.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nkb.smart0.xyz

JS:   console.error("err")
来源：http://lcz.ivvv.top

TS:   console.error("err")
来源：http://pid.zhongyouzk.top

Java: System.err.println("err")
来源：http://fto.daria6918.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://khj.cheryme.top

Ruby: warn "err"
来源：http://peo.cdnleiting.top

C#:   Console.Error.WriteLine("err")
来源：http://tad.fzhhl.top

[M07] 判断是否为主入口
来源：http://hal.zhiwuduotai.top

Py:   if __name__ == "__main__":
来源：http://bok.xylfe.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xvi.yongpay.top

JS:   require.main === module
来源：http://bus.aizwys.cn

TS:   require.main === module
来源：http://qdk.zhongyouzk.top

Java: public static void main(String[] args)
来源：http://ddp.zycfv.cn

Go:   func main()
来源：http://pkf.tian-w.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pjk.hongshengwenyu.top

C#:   static void Main(string[] args)
来源：http://yaf.tianlin.xyz

[M08] 获取系统与运行时信息
来源：http://gyx.tarul.cn

Py:   platform.system();  platform.python_version()
来源：http://dcg.yj20258.top

PHP:  PHP_OS;  phpversion();
来源：http://brc.hnxiangtu.top

JS:   process.platform;  process.version
来源：http://uux.sweek.top

TS:   process.platform;  process.version
来源：http://afb.aibaodan.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jlx.jinyuanbaomall.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hsj.daria6918.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ysj.sweek.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ngt.316326.xyz

================================================================================
来源：http://ier.nwbrower.top

N. 数据结构与算法
来源：http://rym.hcnkem.com

================================================================================
来源：http://spn.zhengqikj.top

[N01] 二分查找（有序数组）
来源：http://atb.chenjidiqi.icu

Py:   bisect.bisect_left(arr, x)
来源：http://mef.hongshengwenyu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mmg.daria6918.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vnf.jinghuilouyu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jyu.ydjk.org.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gcj.ehwqpu.com

Go:   sort.SearchInts(arr, x)
来源：http://pdl.wangdashe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qzd.yuxming.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rti.pycfn.com

[N02] 排序（工程实践用内置实现）
来源：http://kxj.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://ajq.cucudq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jii.jlsjyb.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ndi.guowangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://gjl.zhengqikj.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xsh.xinyue.icu

Go:   slices.Sort(arr)
来源：http://ukx.chenjidiqi.icu

Ruby: arr.sort
来源：http://tfm.snrcjt.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hyw.mhx1999.top

[N03] 快速排序（分治示例）
来源：http://ira.dashuyun.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oqq.nanxuanxn.top

PHP:  // 递归实现，或用 usort
来源：http://tia.guannengcc.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kxh.epnwcf.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qvo.52xcode.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://drp.xylfe.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sqf.shanyushiyangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bsp.hywenlv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://thy.hfpthk.cn

[N04] 斐波那契数列
来源：http://inw.hnqzz.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hej.mhx1999.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wjm.tarul.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zul.bjfxy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kzy.yfazqb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yir.pengpengdd.cyou

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gwx.svipenyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bwh.vehdjk.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kct.wangdashe.top

[N05] 最大公约数
来源：http://lxx.hywenlv.cn

Py:   math.gcd(a, b)
来源：http://uli.yj20258888.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ald.jinghuilouyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://boj.feifeiyinyue.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kak.sysykeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jrp.xziqi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tyj.yonumen.top

Ruby: a.gcd(b)
来源：http://oul.quarkkingdee.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://waw.hammf.cn

[N06] 判断回文字符串
来源：http://xwx.cdnleiting.top

Py:   s == s[::-1]
来源：http://mfw.haohaochexian.top

PHP:  $s === strrev($s);
来源：http://pgx.uphjek.com

JS:   s === [...s].reverse().join("")
来源：http://oaa.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://rge.jinyuanbaomall.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://odt.aizwys.cn

Go:   // 双指针从两端比较
来源：http://rsr.yonumen.top

Ruby: s == s.reverse
来源：http://sni.birdmap.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://iua.havefunace.top

[N07] 两数之和（返回下标）
来源：http://mcf.gaohongyu789.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ttx.ivvv.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xax.ydzc1.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zek.nwbrower.top

TS:   // 手写 Map<string, number>
来源：http://cab.hywenlv.cn

Java: // 手写 HashMap
来源：http://out.jinqigfzy.top

Go:   // 手写 map[int]int
来源：http://wiw.tanke756.top

Ruby: // 手写 Hash
来源：http://cwz.hcnkem.com

C#:   // 手写 Dictionary<int, int>
来源：http://chb.mhx1999.top

[N08] 生成全排列
来源：http://hpm.cheryme.top

Py:   itertools.permutations(arr)
来源：http://awu.ctjpmb.com

PHP:  // 手写递归交换
来源：http://kip.zhiwuduotai.top

JS:   // 手写回溯递归
来源：http://off.vehdjk.com

TS:   // 手写回溯递归
来源：http://jtz.birdmap.top

Java: // 手写回溯递归
来源：http://ufr.gaohongyu789.top

Go:   // 手写回溯递归
来源：http://thq.daria6918.cn

Ruby: arr.permutation.to_a
来源：http://zof.yonumen.top

C#:   // 手写回溯递归
来源：http://var.jinqigfzy.top

[N09] 栈与队列
来源：http://qvm.sweek.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ulk.zhaomingkeji.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hxf.zhiwuduotai.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dup.hongshengwenyu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zyn.shanyushiyangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lzl.0kj1m.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bxu.jinqigufen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://okw.yuxming.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rbj.jinyuanbaomall.cn

[N10] 链表节点定义
来源：http://ivb.gaohongyu789.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qzj.sysykeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://top.iojbl.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://trk.fanxiaobao.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ted.chenjidiqi.icu

Java: class Node { int v; Node next; }
来源：http://eht.ivvv.top

Go:   type Node struct { V int; Next *Node }
来源：http://pjt.jinyuanbaomall.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xxl.andypj.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://lns.ywan-chungtsiang.top

[N11] 二叉树中序遍历
来源：http://aew.0kj1m.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vnd.zhixingplan.top

PHP:  // 手写递归函数
来源：http://jkv.ydjk.org.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ddz.tianlin.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wjx.yuxming.cn

Java: // 手写递归
来源：http://kwm.xuanzx.com

Go:   // 手写递归
来源：http://eoj.bjfxy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hle.xziqi.cn

C#:   // 手写递归
来源：http://kpj.hnxiangtu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pxc.ybcxt.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sem.xuanzx.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vhz.yuxming.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ecv.nanxuanxn.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xsr.xziqi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gzi.zhoulong.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yzw.nwbrower.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xod.yonumen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://aeq.jyoumei.cn

================================================================================
来源：http://vya.ivvv.top

O. 并发与异步
来源：http://fsa.haohaochexian.top

================================================================================
来源：http://jgl.zdqjudy.top

[O01] 启动一个线程
来源：http://swg.gogol.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pfq.nanxuanxn.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uja.vqdsnc.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zdg.snrcjt.cn

TS:   // 同 JS
来源：http://duo.bbcook.cn

Java: new Thread(() -> f()).start()
来源：http://orn.ctjpmb.com

Go:   go f()
来源：http://qnm.ivvv.top

Ruby: Thread.new { f }
来源：http://hdv.sjlbkw.cn

C#:   Task.Run(() => F());
来源：http://vyw.cashguo.top

[O02] 使用线程池
来源：http://sei.nanxinkj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wsf.hammf.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yvv.yonumen.top

JS:   // worker_threads 线程池
来源：http://dok.yj20258.top

TS:   // worker_threads 线程池
来源：http://ipi.jqgfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://ldb.zdqjudy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kso.cashguo.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jlb.quarkkingdee.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oak.xingfuxueyuan.xyz

[O03] 加锁保护共享数据
来源：http://mzk.yj20258.top

Py:   with lock: shared += 1
来源：http://xct.zhixingplan.top

PHP:  // 用 flock() 做文件锁
来源：http://wac.andypj.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ilc.chenzaomai.com

TS:   // 同 JS
来源：http://whf.fanxiaobao.xyz

Java: synchronized (this) { shared++; }
来源：http://rdu.jinghuilouyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kcl.gogol.net.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hhq.chenjidiqi.icu

C#:   lock (gate) { shared++; }
来源：http://qay.nanxinkj.top

[O04] 定义异步函数并等待
来源：http://ydf.shanyushiyangtech.top

Py:   async def f():⏎    await g()
来源：http://lsk.dashuyun.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oej.yvedp.cn

JS:   async function f() { await g(); }
来源：http://yyh.yangfankeji.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://tkk.gogol.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rtn.quarkkingdee.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://goy.hywenlv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xbp.vehdjk.com

C#:   async Task F() { await G(); }
来源：http://rao.yvedp.cn

[O05] 并发执行并等待全部完成
来源：http://sga.bjfxy.top

Py:   asyncio.gather(*tasks)
来源：http://soe.guowangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ewo.dianchejie.cn

JS:   await Promise.all(tasks)
来源：http://igs.sweek.top

TS:   await Promise.all(tasks)
来源：http://fkc.jqgufenzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dzw.zhijiandao.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fvo.jqgfzy.top

Ruby: threads.map(&:join)
来源：http://dwk.iojbl.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mbs.dianchejie.cn

[O06] 使用进程池
来源：http://mfj.gzhubu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fbc.zdbjq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://stm.jyoumei.cn

JS:   // child_process / cluster 模块
来源：http://mia.cheryme.top

TS:   // child_process / cluster 模块
来源：http://uaa.uphjek.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zvn.bjfxy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cya.jyoumei.cn

Ruby: // fork 块
来源：http://nzc.epnwcf.com

C#:   Parallel.For
来源：http://num.wangshuangyany.cn

================================================================================
来源：http://nfl.c1oappe.top

P. 常用工具函数
来源：http://ixd.birdmap.top

================================================================================
来源：http://aqw.ydjk.org.cn

[P01] 生成 UUID
来源：http://nvq.xingfuxueyuan.xyz

Py:   str(uuid.uuid4())
来源：http://uep.zhijiandao.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tba.pycfn.com

JS:   crypto.randomUUID()
来源：http://yrr.yuxming.cn

TS:   crypto.randomUUID()
来源：http://cqt.zhengqikj.top

Java: UUID.randomUUID().toString()
来源：http://igg.birdmap.top

Go:   // 用 github.com/google/uuid
来源：http://adb.sjlbkw.cn

Ruby: SecureRandom.uuid
来源：http://bqu.fehbvm.com

C#:   Guid.NewGuid().ToString()
来源：http://eix.yonumen.top

[P02] MD5 / SHA256 摘要
来源：http://oqq.zhiwuduotai.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nrh.cdnleiting.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://slr.pengpengdd.cyou

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zwr.nwbrower.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pct.jinqigfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vtw.hammf.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nce.yangfankeji.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ulj.tianlin.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dmu.nwbrower.top

[P03] 生成短随机字符串
来源：http://nzs.fktsv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lbg.svipenyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yld.tarul.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dfd.daxiang520.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jno.xylfe.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ghp.hnxiangtu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rjj.cheryme.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://sic.zycfv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rsv.vehdjk.com

[P04] 求长度
来源：http://abu.havefunace.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gio.smart0.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xar.yanxiufei.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kda.ydjk.org.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dow.kuanghao11.cn

Java: list.size();  map.size();  s.length()
来源：http://sad.jinqigufen.top

Go:   len(arr);  len(m)
来源：http://llp.316326.xyz

Ruby: x.length;  x.size
来源：http://sef.wangshuangyany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://azx.yvedp.cn

[P05] 判断两个对象内容是否相等
来源：http://any.ydzc1.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://kre.nanxuanxn.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mxq.hcnkem.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ekm.shuidangran.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xex.hfpthk.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://htx.jinyuanbaomall.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dnx.jianghu66.top

Ruby: a == b
来源：http://saa.ppjwa.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://smj.smart0.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vcf.ywan-chungtsiang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iit.feifeiyinyue.top

PHP:  if (empty($x)) {}
来源：http://xyz.jlsjyb.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dab.yuxming.cn

TS:   if (x == null) {}
来源：http://xnp.wangdashe.top

Java: if (x == null || x.isEmpty()) {}
来源：http://gkp.ppjwa.cn

Go:   if x == nil {}
来源：http://kjj.tanke756.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dnx.vqdsnc.cn

C#:   if (x is null) {}
来源：http://rpj.zhijiandao.cn

[P07] 防抖与节流
来源：http://obs.smart0.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wdn.jqgufenzy.top

PHP:  // 手写时间戳比较
来源：http://vqm.birdmap.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oit.hnqzz.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vjw.wangshuangyany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zzn.ehwqpu.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ari.xziqi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gnl.xuetiantiany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://eih.xziqi.cn

[P08] 处理浮点精度问题
来源：http://tjc.bbcook.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://usm.0kj1m.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://udo.yj20258888.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dmd.zhiwuduotai.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xoq.havefunace.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://khu.jyoumei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://drl.pycfn.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ojo.jianghu66.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fkk.nwbrower.top

================================================================================
来源：http://rlb.snrcjt.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ndk.jinghuilouyu.cn

================================================================================
来源：http://kug.zycfv.cn

[Q01] 创建表
来源：http://gtj.hywenlv.cn

CREATE TABLE users (
来源：http://ejx.yj20258.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gir.ctjpmb.com

name VARCHAR(50) NOT NULL,
来源：http://zim.hnxiangtu.top

email VARCHAR(100) UNIQUE,
来源：http://jwe.yueranfly.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cpo.ppjwa.cn

);
来源：http://ooe.vehdjk.com

[Q02] 创建带外键的表
来源：http://znv.gogol.net.cn

CREATE TABLE orders (
来源：http://vdh.nwbrower.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mxt.0kj1m.cn

user_id INT NOT NULL,
来源：http://ivx.zhongyouzk.top

amount DECIMAL(10, 2),
来源：http://ysd.zhaomingkeji.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cvs.feifeiyinyue.top


<!-- 参考信息 -->