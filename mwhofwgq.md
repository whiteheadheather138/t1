代发 wailian999

[M04] 获取当前工作目录
来源：http://gof.zhiwuduotai.top

Py:   os.getcwd()
来源：http://ybt.gzhubu.top

PHP:  getcwd();
来源：http://knn.yuanzhike.top

JS:   process.cwd()
来源：http://pvl.iojbl.cn

TS:   process.cwd()
来源：http://xca.sjlbkw.cn

Java: Path.of("").toAbsolutePath()
来源：http://qnw.zhoulong.xyz

Go:   os.Getwd()
来源：http://wkk.fzhhl.top

Ruby: Dir.pwd
来源：http://olh.wangdashe.top

C#:   Directory.GetCurrentDirectory()
来源：http://feo.svipenyu.cn

[M05] 设置退出码
来源：http://iab.xziqi.cn

Py:   sys.exit(1)
来源：http://bws.xylfe.cn

PHP:  exit(1);
来源：http://vwt.quarkkingdee.top

JS:   process.exit(1)
来源：http://jur.shanyushiyangtech.top

TS:   process.exit(1)
来源：http://eua.fktsv.cn

Java: System.exit(1)
来源：http://jym.haohaochexian.top

Go:   os.Exit(1)
来源：http://wpl.hammf.cn

Ruby: exit 1
来源：http://gfh.ywan-chungtsiang.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sze.jqgfzy.top

[M06] 向标准错误输出
来源：http://thu.tarul.cn

Py:   print("err", file=sys.stderr)
来源：http://xnr.fzhhl.top

PHP:  fwrite(STDERR, "err\n");
来源：http://eka.gzhubu.top

JS:   console.error("err")
来源：http://oow.jlsjyb.cn

TS:   console.error("err")
来源：http://mog.vehdjk.com

Java: System.err.println("err")
来源：http://qpb.yuanzhike.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eqn.zdbjq.cn

Ruby: warn "err"
来源：http://euo.xziqi.cn

C#:   Console.Error.WriteLine("err")
来源：http://nug.0kj1m.cn

[M07] 判断是否为主入口
来源：http://yxs.havefunace.top

Py:   if __name__ == "__main__":
来源：http://lyp.ydzc1.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://thz.sjlbkw.cn

JS:   require.main === module
来源：http://aeo.9152youxi.cn

TS:   require.main === module
来源：http://kdy.jqgfzy.top

Java: public static void main(String[] args)
来源：http://jsq.yongpay.top

Go:   func main()
来源：http://smx.tianlin.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://whh.jinyuanbaomall.cn

C#:   static void Main(string[] args)
来源：http://sqy.ctjpmb.com

[M08] 获取系统与运行时信息
来源：http://qqw.yvedp.cn

Py:   platform.system();  platform.python_version()
来源：http://qth.daxiang520.top

PHP:  PHP_OS;  phpversion();
来源：http://hgf.hesvh.cn

JS:   process.platform;  process.version
来源：http://pgi.wangdashe.top

TS:   process.platform;  process.version
来源：http://khx.bbcook.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hum.hnqzz.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vpd.gotoacloud.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vxv.aibaodan.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ntj.ivvv.top

================================================================================
来源：http://gjd.nanxinkj.top

N. 数据结构与算法
来源：http://omd.yangfankeji.com

================================================================================
来源：http://fzc.ehwqpu.com

[N01] 二分查找（有序数组）
来源：http://gxl.xuanzx.com

Py:   bisect.bisect_left(arr, x)
来源：http://ext.hfpthk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nae.zhaomingkeji.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://idk.ehwqpu.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://svj.epnwcf.com

Java: Arrays.binarySearch(arr, x)
来源：http://hpg.ppjwa.cn

Go:   sort.SearchInts(arr, x)
来源：http://sbg.fehbvm.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://ddj.zhongyouzk.top

C#:   Array.BinarySearch(arr, x)
来源：http://dru.0kj1m.cn

[N02] 排序（工程实践用内置实现）
来源：http://asc.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://bhm.xuetiantiany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rub.yangfankeji.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://aum.tarul.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vzh.hnxiangtu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zmw.fktsv.cn

Go:   slices.Sort(arr)
来源：http://xtz.sweek.top

Ruby: arr.sort
来源：http://mlb.shzxlz.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vye.cashguo.top

[N03] 快速排序（分治示例）
来源：http://kfg.cdnleiting.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xor.yj202588.top

PHP:  // 递归实现，或用 usort
来源：http://ixr.pycfn.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rwf.daria6918.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://val.yuxming.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://daa.gogol.net.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kfw.aibaodan.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cik.tian-w.cn

C#:   // 手写递归，或 Array.Sort
来源：http://nfr.hnqzz.top

[N04] 斐波那契数列
来源：http://kea.zhixingplan.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pjy.vqdsnc.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hgi.zhoulong.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ehm.xuetiantiany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nii.chenlongwang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hgu.nwbrower.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gaj.zhaomingkeji.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pgx.gotoacloud.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://shq.xinyue.icu

[N05] 最大公约数
来源：http://ymk.ydjk.org.cn

Py:   math.gcd(a, b)
来源：http://jyf.zhiwuduotai.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dcy.jinqigfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://plk.vqdsnc.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://asq.uphjek.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rbu.feifeiyinyue.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://spg.shuidangran.top

Ruby: a.gcd(b)
来源：http://oua.ctjpmb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pku.xuanzx.com

[N06] 判断回文字符串
来源：http://art.tian-w.cn

Py:   s == s[::-1]
来源：http://kvw.ppjwa.cn

PHP:  $s === strrev($s);
来源：http://wdk.cqqwz.cn

JS:   s === [...s].reverse().join("")
来源：http://lin.gaohongyu789.top

TS:   s === [...s].reverse().join("")
来源：http://wga.jinyuanbaomall.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://asa.yvedp.cn

Go:   // 双指针从两端比较
来源：http://spc.ydjk.org.cn

Ruby: s == s.reverse
来源：http://pey.havefunace.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://grg.xingfuxueyuan.xyz

[N07] 两数之和（返回下标）
来源：http://wkc.yj20258888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tbb.wangshuangyany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oxp.yuanzhike.top

JS:   // 手写 Map：map.set(v, i)
来源：http://rqm.bjfxy.top

TS:   // 手写 Map<string, number>
来源：http://nbf.sxryk.cn

Java: // 手写 HashMap
来源：http://jdy.yangfankeji.com

Go:   // 手写 map[int]int
来源：http://huo.hnxiangtu.top

Ruby: // 手写 Hash
来源：http://mkb.sufxvd.cn

C#:   // 手写 Dictionary<int, int>
来源：http://izh.shuidangran.top

[N08] 生成全排列
来源：http://qet.hnxiangtu.top

Py:   itertools.permutations(arr)
来源：http://pca.yueranfly.top

PHP:  // 手写递归交换
来源：http://dwj.hcnkem.com

JS:   // 手写回溯递归
来源：http://lsg.zhongyouzk.top

TS:   // 手写回溯递归
来源：http://kdg.birdmap.top

Java: // 手写回溯递归
来源：http://csc.chenlongwang.top

Go:   // 手写回溯递归
来源：http://ber.cashguo.top

Ruby: arr.permutation.to_a
来源：http://pnx.hesvh.cn

C#:   // 手写回溯递归
来源：http://xjw.zhongyouzk.top

[N09] 栈与队列
来源：http://pfa.pengpengdd.cyou

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qnu.vehdjk.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://elw.ydjk.org.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dfg.zhiwuduotai.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qxb.52xcode.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wtc.gaohongyu789.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dep.c1oappe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ggl.pycfn.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fee.snrcjt.cn

[N10] 链表节点定义
来源：http://lxm.yonumen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cbe.andypj.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://uxp.cucudq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ffs.c1oappe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zuq.dianchejie.cn

Java: class Node { int v; Node next; }
来源：http://tuu.chenzaomai.com

Go:   type Node struct { V int; Next *Node }
来源：http://vbf.ppjwa.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yzh.shanyushiyangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zce.jinqigufen.top

[N11] 二叉树中序遍历
来源：http://ywg.hnxiangtu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pmq.pycfn.com

PHP:  // 手写递归函数
来源：http://xms.nanxinkj.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jct.cashguo.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mmc.xziqi.cn

Java: // 手写递归
来源：http://xna.ctjpmb.com

Go:   // 手写递归
来源：http://jbx.wangshuangyany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qia.ppjwa.cn

C#:   // 手写递归
来源：http://fib.zhengqikj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tgv.zycfv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iwf.fktsv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fwq.hesvh.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ask.cqqwz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rlk.hywenlv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wii.tian-w.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fwg.hnxiangtu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ron.guannengcc.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mdj.sufxvd.cn

================================================================================
来源：http://hrb.ydzc1.top

O. 并发与异步
来源：http://aza.guowangkeji.top

================================================================================
来源：http://imq.xuetiantiany.cn

[O01] 启动一个线程
来源：http://fmj.mhx1999.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://etp.hysaishi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sdh.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jjf.hcnkem.com

TS:   // 同 JS
来源：http://jcl.fanxiaobao.xyz

Java: new Thread(() -> f()).start()
来源：http://zpo.hcnkem.com

Go:   go f()
来源：http://vlg.ivvv.top

Ruby: Thread.new { f }
来源：http://pir.c1oappe.top

C#:   Task.Run(() => F());
来源：http://ykq.fehbvm.com

[O02] 使用线程池
来源：http://zcc.xuanzx.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hmi.chenjidiqi.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wtv.c1oappe.top

JS:   // worker_threads 线程池
来源：http://kcz.shzxlz.cn

TS:   // worker_threads 线程池
来源：http://rmm.cdnleiting.top

Java: Executors.newFixedThreadPool(4)
来源：http://yqu.dashuyun.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://acz.chenjidiqi.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yml.yj20258.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rxa.gzhubu.top

[O03] 加锁保护共享数据
来源：http://nfx.snrcjt.cn

Py:   with lock: shared += 1
来源：http://bfq.zhongyouzk.top

PHP:  // 用 flock() 做文件锁
来源：http://qol.ctjpmb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vlc.nanxuanxn.top

TS:   // 同 JS
来源：http://hya.epnwcf.com

Java: synchronized (this) { shared++; }
来源：http://mof.uphjek.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qov.cheryme.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ihu.xylfe.cn

C#:   lock (gate) { shared++; }
来源：http://lor.shanyushiyangtech.top

[O04] 定义异步函数并等待
来源：http://ymy.hcnkem.com

Py:   async def f():⏎    await g()
来源：http://hii.gotoacloud.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eqa.ydjk.org.cn

JS:   async function f() { await g(); }
来源：http://rxj.xziqi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lwf.aizwys.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ykv.xuetiantiany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zrd.zhiwuduotai.top

Ruby: # 用 Fiber 或 async gem
来源：http://vua.c1oappe.top

C#:   async Task F() { await G(); }
来源：http://sdh.jqgufenzy.top

[O05] 并发执行并等待全部完成
来源：http://sol.yonumen.top

Py:   asyncio.gather(*tasks)
来源：http://nwt.guowangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://spq.yangfankeji.com

JS:   await Promise.all(tasks)
来源：http://ubb.hysaishi.cn

TS:   await Promise.all(tasks)
来源：http://ezw.tanke756.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kch.daxiang520.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gsh.ydjk.org.cn

Ruby: threads.map(&:join)
来源：http://vrd.redwolf501.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wmx.jlsjyb.cn

[O06] 使用进程池
来源：http://tua.fehbvm.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nnn.shzxlz.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ffa.shzxlz.cn

JS:   // child_process / cluster 模块
来源：http://elg.zhoulong.xyz

TS:   // child_process / cluster 模块
来源：http://xie.fehbvm.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fxw.jianghu66.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://umm.birdmap.top

Ruby: // fork 块
来源：http://cri.tianlin.xyz

C#:   Parallel.For
来源：http://wvp.0kj1m.cn

================================================================================
来源：http://gin.zhoulong.xyz

P. 常用工具函数
来源：http://vkq.gaohongyu789.top

================================================================================
来源：http://raq.hfpthk.cn

[P01] 生成 UUID
来源：http://eka.sweek.top

Py:   str(uuid.uuid4())
来源：http://gdu.havefunace.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://det.ydzc1.top

JS:   crypto.randomUUID()
来源：http://cmg.snrcjt.cn

TS:   crypto.randomUUID()
来源：http://oot.yj202588.top

Java: UUID.randomUUID().toString()
来源：http://ihs.316326.xyz

Go:   // 用 github.com/google/uuid
来源：http://nhm.tianlin.xyz

Ruby: SecureRandom.uuid
来源：http://hsl.yj202588.top

C#:   Guid.NewGuid().ToString()
来源：http://adj.xziqi.cn

[P02] MD5 / SHA256 摘要
来源：http://dwl.jiagoushi.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jps.yvedp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lhb.ppjwa.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xhe.sufxvd.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bzc.fzhhl.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nil.yj20258.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://iew.gzhubu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cnl.aibaodan.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kql.andypj.xyz

[P03] 生成短随机字符串
来源：http://inu.sysykeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vkw.daxiang520.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ojr.chenzaomai.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iem.epnwcf.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pdk.aizwys.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bru.ehwqpu.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tdi.aibaodan.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mfu.zhoulong.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pxi.zdbjq.cn

[P04] 求长度
来源：http://zvf.uphjek.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xeb.nwbrower.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://irm.yj20258888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qst.yuanzhike.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://emm.aibaodan.cn

Java: list.size();  map.size();  s.length()
来源：http://jzk.nwbrower.top

Go:   len(arr);  len(m)
来源：http://pza.gzhubu.top

Ruby: x.length;  x.size
来源：http://ofc.shzxlz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://pbn.birdmap.top

[P05] 判断两个对象内容是否相等
来源：http://wnm.cqqwz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://iig.ydzc1.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tjx.yueranfly.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nlw.yongpay.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kub.ybcxt.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ett.jqgfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://cln.yfazqb.com

Ruby: a == b
来源：http://jha.fehbvm.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qhz.xinyue.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bhv.zdqjudy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://efq.jlsjyb.cn

PHP:  if (empty($x)) {}
来源：http://pew.havefunace.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dnx.shanyushiyangkeji.top

TS:   if (x == null) {}
来源：http://vlu.gotoacloud.top

Java: if (x == null || x.isEmpty()) {}
来源：http://uso.ydzc1.top

Go:   if x == nil {}
来源：http://arg.jinqigufen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://aba.yueranfly.top

C#:   if (x is null) {}
来源：http://stj.feifeiyinyue.top

[P07] 防抖与节流
来源：http://iac.uphjek.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rat.jyoumei.cn

PHP:  // 手写时间戳比较
来源：http://kpj.0kj1m.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nhg.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dcy.hcnkem.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dvt.jiagoushi.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yqi.cdnleiting.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://bci.mhx1999.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mti.shzxlz.cn

[P08] 处理浮点精度问题
来源：http://hrz.ppjwa.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nxs.9152youxi.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fdc.yuxming.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jbj.pengpengdd.cyou

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ycu.9152youxi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oiw.zycfv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ogh.cheryme.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lfe.zhengqikj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fhz.hammf.cn

================================================================================
来源：http://cgc.ybcxt.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://alj.shanyushiyangtech.top

================================================================================
来源：http://phh.snrcjt.cn

[Q01] 创建表
来源：http://tiq.jqgfzy.top

CREATE TABLE users (
来源：http://ijk.chenlongwang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qfj.hammf.cn

name VARCHAR(50) NOT NULL,
来源：http://sna.nanxinkj.top

email VARCHAR(100) UNIQUE,
来源：http://yjt.c1oappe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gnr.ctjpmb.com

);
来源：http://imc.aibaodan.cn

[Q02] 创建带外键的表
来源：http://len.shzxlz.cn

CREATE TABLE orders (
来源：http://ydw.zycfv.cn


<!-- 参考信息 -->