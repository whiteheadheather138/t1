代发 wailian999

JS:   process.exit(1)
来源：http://jdt.sjlbkw.cn

TS:   process.exit(1)
来源：http://fxd.316326.xyz

Java: System.exit(1)
来源：http://rjd.snrcjt.cn

Go:   os.Exit(1)
来源：http://qxx.hywenlv.cn

Ruby: exit 1
来源：http://ttb.dashuyun.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://edt.hcnkem.com

[M06] 向标准错误输出
来源：http://xpj.zdbjq.cn

Py:   print("err", file=sys.stderr)
来源：http://qot.ctjpmb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://ehu.birdmap.top

JS:   console.error("err")
来源：http://voj.gzhubu.top

TS:   console.error("err")
来源：http://tlm.yj20258888.top

Java: System.err.println("err")
来源：http://gfr.yuanzhike.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ane.0kj1m.cn

Ruby: warn "err"
来源：http://rdn.zhaomingkeji.xyz

C#:   Console.Error.WriteLine("err")
来源：http://hes.yj20258888.top

[M07] 判断是否为主入口
来源：http://drx.ydjk.org.cn

Py:   if __name__ == "__main__":
来源：http://imz.52xcode.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gka.sysykeji.top

JS:   require.main === module
来源：http://ktb.cdnleiting.top

TS:   require.main === module
来源：http://dlh.hnxiangtu.top

Java: public static void main(String[] args)
来源：http://bam.yongpay.top

Go:   func main()
来源：http://nsc.zhoulong.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rot.shzxlz.cn

C#:   static void Main(string[] args)
来源：http://nbh.vehdjk.com

[M08] 获取系统与运行时信息
来源：http://zre.zhengqikj.top

Py:   platform.system();  platform.python_version()
来源：http://ldw.svipenyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://qlb.tanke756.top

JS:   process.platform;  process.version
来源：http://hef.xuetiantiany.cn

TS:   process.platform;  process.version
来源：http://zxm.aizwys.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rvx.hysaishi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kct.zycfv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mlh.shanyushiyangtech.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mpo.hcnkem.com

================================================================================
来源：http://qhb.yueranfly.top

N. 数据结构与算法
来源：http://bzr.jinqigfzy.top

================================================================================
来源：http://uou.gotoacloud.top

[N01] 二分查找（有序数组）
来源：http://wvr.uphjek.com

Py:   bisect.bisect_left(arr, x)
来源：http://fwk.fehbvm.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://swx.snrcjt.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fwr.gzhubu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sui.guowangkeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://plp.yonumen.top

Go:   sort.SearchInts(arr, x)
来源：http://orh.aizwys.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://rdo.svipenyu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jtl.snrcjt.cn

[N02] 排序（工程实践用内置实现）
来源：http://tvo.yfazqb.com

Py:   sorted(arr);  arr.sort()
来源：http://bzb.hesvh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xtc.feifeiyinyue.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ncd.ydjk.org.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://zpx.daria6918.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sxl.sjlbkw.cn

Go:   slices.Sort(arr)
来源：http://eme.hysaishi.cn

Ruby: arr.sort
来源：http://xaj.xuanzx.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://sri.jyoumei.cn

[N03] 快速排序（分治示例）
来源：http://olk.daria6918.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qan.yj20258888.top

PHP:  // 递归实现，或用 usort
来源：http://mbb.guowangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hgc.meibo888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ohc.ydjk.org.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tly.svipenyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://msd.shzxlz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rwm.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://zjs.vqdsnc.cn

[N04] 斐波那契数列
来源：http://luz.yangfankeji.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pnk.zdbjq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jlq.bbcook.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kdy.hnqzz.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ljt.hesvh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fng.ydzc1.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xes.andypj.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lnl.chenlongwang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lns.316326.xyz

[N05] 最大公约数
来源：http://yxy.shuidangran.top

Py:   math.gcd(a, b)
来源：http://bpj.uphjek.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uri.zdbjq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mby.yongpay.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nxx.mhx1999.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zrr.meibo888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fmo.vehdjk.com

Ruby: a.gcd(b)
来源：http://ysa.c1oappe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gpe.epnwcf.com

[N06] 判断回文字符串
来源：http://gpw.haohaochexian.top

Py:   s == s[::-1]
来源：http://ikd.hammf.cn

PHP:  $s === strrev($s);
来源：http://iwn.daria6918.cn

JS:   s === [...s].reverse().join("")
来源：http://qcc.shangyingyoupin.top

TS:   s === [...s].reverse().join("")
来源：http://yix.birdmap.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ngv.quarkkingdee.top

Go:   // 双指针从两端比较
来源：http://guv.iojbl.cn

Ruby: s == s.reverse
来源：http://amf.daxiang520.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wvz.redwolf501.top

[N07] 两数之和（返回下标）
来源：http://wlm.yangfankeji.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lxf.fzhhl.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ojk.hnxiangtu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://syc.tarul.cn

TS:   // 手写 Map<string, number>
来源：http://fot.fktsv.cn

Java: // 手写 HashMap
来源：http://uog.mhx1999.top

Go:   // 手写 map[int]int
来源：http://hyz.hfpthk.cn

Ruby: // 手写 Hash
来源：http://fvt.zhixingplan.top

C#:   // 手写 Dictionary<int, int>
来源：http://dyx.chenzaomai.com

[N08] 生成全排列
来源：http://jpr.aizwys.cn

Py:   itertools.permutations(arr)
来源：http://qci.xuanzx.com

PHP:  // 手写递归交换
来源：http://hqc.zhijiandao.cn

JS:   // 手写回溯递归
来源：http://pmk.uphjek.com

TS:   // 手写回溯递归
来源：http://gxm.mhx1999.top

Java: // 手写回溯递归
来源：http://qij.feifeiyinyue.top

Go:   // 手写回溯递归
来源：http://qek.shanyushiyangkeji.top

Ruby: arr.permutation.to_a
来源：http://bqq.yongpay.top

C#:   // 手写回溯递归
来源：http://tru.cqqwz.cn

[N09] 栈与队列
来源：http://bsm.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bol.fanxiaobao.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gon.zhoulong.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fvm.bjfxy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iha.snrcjt.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ejc.yanxiufei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hju.zdqjudy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jcu.xziqi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ucp.sjlbkw.cn

[N10] 链表节点定义
来源：http://pat.nanxinkj.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xov.feifeiyinyue.top

PHP:  class Node { public $v; public $next = null; }
来源：http://uxu.haohaochexian.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zvj.jiagoushi.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fwa.yj20258888.top

Java: class Node { int v; Node next; }
来源：http://afv.cqqwz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pnb.ybcxt.top

Ruby: Node = Struct.new(:v, :next)
来源：http://oik.yonumen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jnq.zdqjudy.top

[N11] 二叉树中序遍历
来源：http://ahc.guowangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://imt.shzxlz.cn

PHP:  // 手写递归函数
来源：http://sgr.tarul.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ubc.fktsv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ulr.jinghuilouyu.cn

Java: // 手写递归
来源：http://oop.kuanghao11.cn

Go:   // 手写递归
来源：http://tkp.jianghu66.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xik.meibo888.top

C#:   // 手写递归
来源：http://amg.fehbvm.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://auf.yfazqb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bqk.zdbjq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lex.birdmap.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nee.vqdsnc.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dex.cqqwz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fdj.shanyushiyangtech.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tgo.316326.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nqw.ywan-chungtsiang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lbg.hammf.cn

================================================================================
来源：http://ldk.hongshengwenyu.top

O. 并发与异步
来源：http://rxq.tarul.cn

================================================================================
来源：http://mue.xuanzx.com

[O01] 启动一个线程
来源：http://pih.cashguo.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fkr.sysykeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pba.zhengqikj.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fqa.jqgufenzy.top

TS:   // 同 JS
来源：http://pnk.zdqjudy.top

Java: new Thread(() -> f()).start()
来源：http://zle.smart0.xyz

Go:   go f()
来源：http://ipi.cucudq.cn

Ruby: Thread.new { f }
来源：http://pcd.fanxiaobao.xyz

C#:   Task.Run(() => F());
来源：http://blw.mhx1999.top

[O02] 使用线程池
来源：http://fnr.c1oappe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rfv.jinyuanbaomall.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zgz.cqqwz.cn

JS:   // worker_threads 线程池
来源：http://eir.quarkkingdee.top

TS:   // worker_threads 线程池
来源：http://kli.316326.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://pyf.fengsongda.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dwl.jinyuanbaomall.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bse.yuanzhike.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xhi.kuanghao11.cn

[O03] 加锁保护共享数据
来源：http://rjt.hnxiangtu.top

Py:   with lock: shared += 1
来源：http://mhg.jinqigfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://fue.hcnkem.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://upe.sxryk.cn

TS:   // 同 JS
来源：http://pcn.zhoulong.xyz

Java: synchronized (this) { shared++; }
来源：http://igm.vqdsnc.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xyh.9152youxi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zug.cqqwz.cn

C#:   lock (gate) { shared++; }
来源：http://uvm.sxryk.cn

[O04] 定义异步函数并等待
来源：http://dlt.zdqjudy.top

Py:   async def f():⏎    await g()
来源：http://eea.jlsjyb.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xbg.xingfuxueyuan.xyz

JS:   async function f() { await g(); }
来源：http://yne.tarul.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bnb.ctjpmb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ola.gzhubu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rbq.ydzc1.top

Ruby: # 用 Fiber 或 async gem
来源：http://loc.quarkkingdee.top

C#:   async Task F() { await G(); }
来源：http://shf.xuetiantiany.cn

[O05] 并发执行并等待全部完成
来源：http://ocr.cheryme.top

Py:   asyncio.gather(*tasks)
来源：http://akr.bjfxy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://izm.xingfuxueyuan.xyz

JS:   await Promise.all(tasks)
来源：http://imy.zhiwuduotai.top

TS:   await Promise.all(tasks)
来源：http://srt.vqdsnc.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rwb.svipenyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pkp.cqqwz.cn

Ruby: threads.map(&:join)
来源：http://khv.gotoacloud.top

C#:   await Task.WhenAll(t1, t2)
来源：http://vwg.daxiang520.top

[O06] 使用进程池
来源：http://euv.xziqi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vgj.gaohongyu789.top

PHP:  // pcntl_fork 或多进程队列
来源：http://wvx.xinyue.icu

JS:   // child_process / cluster 模块
来源：http://ucn.gzhubu.top

TS:   // child_process / cluster 模块
来源：http://cqc.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gbd.tanke756.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tts.yanxiufei.cn

Ruby: // fork 块
来源：http://alt.jinyuanbaomall.cn

C#:   Parallel.For
来源：http://uml.andypj.xyz

================================================================================
来源：http://vxl.xinyue.icu

P. 常用工具函数
来源：http://koq.zycfv.cn

================================================================================
来源：http://yds.nanxuanxn.top

[P01] 生成 UUID
来源：http://egm.316326.xyz

Py:   str(uuid.uuid4())
来源：http://kgh.wangshuangyany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fbx.sysykeji.top

JS:   crypto.randomUUID()
来源：http://uvo.yongpay.top

TS:   crypto.randomUUID()
来源：http://nzf.yj202588.top

Java: UUID.randomUUID().toString()
来源：http://onm.yangfankeji.com

Go:   // 用 github.com/google/uuid
来源：http://tit.yj20258888.top

Ruby: SecureRandom.uuid
来源：http://uzb.jiagoushi.top

C#:   Guid.NewGuid().ToString()
来源：http://glo.ydjk.org.cn

[P02] MD5 / SHA256 摘要
来源：http://djr.yj20258888.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vgf.cheryme.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://muv.smart0.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jqy.hammf.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ldv.zycfv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jvf.hesvh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kel.hesvh.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hhf.havefunace.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ogw.zhiwuduotai.top

[P03] 生成短随机字符串
来源：http://gqr.haohaochexian.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qxw.shanyushiyangtech.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eej.mhx1999.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://upy.sjlbkw.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://reg.hfpthk.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lxd.jinqigufen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ori.cdnleiting.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://nln.hcnkem.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iin.feifeiyinyue.top

[P04] 求长度
来源：http://qjm.shuidangran.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ntg.nanxinkj.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qrx.yvedp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jqf.havefunace.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://shf.cdnleiting.top

Java: list.size();  map.size();  s.length()
来源：http://oni.sysykeji.top

Go:   len(arr);  len(m)
来源：http://ypm.sysykeji.top

Ruby: x.length;  x.size
来源：http://syi.iojbl.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ddq.xziqi.cn

[P05] 判断两个对象内容是否相等
来源：http://ojh.zhijiandao.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ugi.havefunace.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kvb.jinqigufen.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hdf.fehbvm.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://joi.cdnleiting.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wil.iojbl.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ybf.yuxming.cn

Ruby: a == b
来源：http://old.ydzc1.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ufu.hongshengwenyu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gkw.yvedp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yqy.sxryk.cn

PHP:  if (empty($x)) {}
来源：http://qns.iojbl.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tkd.vehdjk.com

TS:   if (x == null) {}
来源：http://oij.tianlin.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://wqh.fengsongda.top

Go:   if x == nil {}
来源：http://ysr.haohaochexian.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rom.cqqwz.cn

C#:   if (x is null) {}
来源：http://uad.ppjwa.cn

[P07] 防抖与节流
来源：http://jee.pycfn.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hmk.ywan-chungtsiang.top

PHP:  // 手写时间戳比较
来源：http://zir.hesvh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ori.tarul.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ufp.hnxiangtu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ufr.c1oappe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ywg.yj20258.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://bpw.cashguo.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mnx.tian-w.cn

[P08] 处理浮点精度问题
来源：http://vsv.chenzaomai.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://shi.redwolf501.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qao.quarkkingdee.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://spr.jqgfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qti.havefunace.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jko.hammf.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qdk.jinqigfzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cuo.daria6918.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wyo.zhixingplan.top

================================================================================
来源：http://wlh.zhixingplan.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gll.yuxming.cn

================================================================================
来源：http://yje.quarkkingdee.top

[Q01] 创建表
来源：http://wcf.haohaochexian.top

CREATE TABLE users (
来源：http://bqv.zhixingplan.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bzw.jqgfzy.top

name VARCHAR(50) NOT NULL,
来源：http://wxe.ehwqpu.com

email VARCHAR(100) UNIQUE,
来源：http://kdq.pengpengdd.cyou

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://urk.jinqigfzy.top

);
来源：http://gil.fzhhl.top

[Q02] 创建带外键的表
来源：http://bnz.ehwqpu.com

CREATE TABLE orders (
来源：http://mcp.mhx1999.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ssb.sufxvd.cn

user_id INT NOT NULL,
来源：http://ixj.iojbl.cn

amount DECIMAL(10, 2),
来源：http://eqc.yj20258.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://abb.jinyuanbaomall.cn

);
来源：http://nuu.yfazqb.com

[Q03] 增加列
来源：http://vdj.cheryme.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ewd.sweek.top

[Q04] 修改列类型
来源：http://kbo.kuanghao11.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hzt.mhx1999.top

[Q05] 重命名列
来源：http://bip.yueranfly.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qbi.cheryme.top

[Q06] 删除列
来源：http://hyv.redwolf501.top


<!-- 参考信息 -->