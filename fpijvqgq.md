代发 wailian999

[M04] 获取当前工作目录
来源：http://apa.cdnleiting.top

Py:   os.getcwd()
来源：http://sii.52xcode.cn

PHP:  getcwd();
来源：http://nbo.316326.xyz

JS:   process.cwd()
来源：http://bpz.ywan-chungtsiang.top

TS:   process.cwd()
来源：http://xmh.hesvh.cn

Java: Path.of("").toAbsolutePath()
来源：http://ybf.zhiwuduotai.top

Go:   os.Getwd()
来源：http://ghf.hammf.cn

Ruby: Dir.pwd
来源：http://ftq.yj202588.top

C#:   Directory.GetCurrentDirectory()
来源：http://rtv.cheryme.top

[M05] 设置退出码
来源：http://irr.haohaochexian.top

Py:   sys.exit(1)
来源：http://wkk.ctjpmb.com

PHP:  exit(1);
来源：http://epn.haohaochexian.top

JS:   process.exit(1)
来源：http://uww.dianchejie.cn

TS:   process.exit(1)
来源：http://cfg.hcnkem.com

Java: System.exit(1)
来源：http://jrq.yj20258888.top

Go:   os.Exit(1)
来源：http://mmn.shanyushiyangkeji.top

Ruby: exit 1
来源：http://bks.sufxvd.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lwk.iojbl.cn

[M06] 向标准错误输出
来源：http://noe.daxiang520.top

Py:   print("err", file=sys.stderr)
来源：http://zyj.gogol.net.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lev.zdqjudy.top

JS:   console.error("err")
来源：http://ppp.chenjidiqi.icu

TS:   console.error("err")
来源：http://fwt.jinghuilouyu.cn

Java: System.err.println("err")
来源：http://fvw.daria6918.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pic.vqdsnc.cn

Ruby: warn "err"
来源：http://new.cucudq.cn

C#:   Console.Error.WriteLine("err")
来源：http://oai.zhoulong.xyz

[M07] 判断是否为主入口
来源：http://tiq.shangyingyoupin.top

Py:   if __name__ == "__main__":
来源：http://ggi.fengsongda.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lci.ydjk.org.cn

JS:   require.main === module
来源：http://tqy.mhx1999.top

TS:   require.main === module
来源：http://gha.redwolf501.top

Java: public static void main(String[] args)
来源：http://whq.zhoulong.xyz

Go:   func main()
来源：http://kmb.wangshuangyany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qbr.shuidangran.top

C#:   static void Main(string[] args)
来源：http://aui.yanxiufei.cn

[M08] 获取系统与运行时信息
来源：http://emz.smart0.xyz

Py:   platform.system();  platform.python_version()
来源：http://mir.tianlin.xyz

PHP:  PHP_OS;  phpversion();
来源：http://ufm.vqdsnc.cn

JS:   process.platform;  process.version
来源：http://ujp.sjlbkw.cn

TS:   process.platform;  process.version
来源：http://rsw.9152youxi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sdz.yongpay.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://yqv.zhixingplan.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pdc.feifeiyinyue.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mjh.chenlongwang.top

================================================================================
来源：http://kew.yuanzhike.top

N. 数据结构与算法
来源：http://zki.gzhubu.top

================================================================================
来源：http://vsx.hysaishi.cn

[N01] 二分查找（有序数组）
来源：http://kyh.snrcjt.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fvk.zhongyouzk.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vks.jinyuanbaomall.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yql.52xcode.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kaz.havefunace.top

Java: Arrays.binarySearch(arr, x)
来源：http://yru.shzxlz.cn

Go:   sort.SearchInts(arr, x)
来源：http://bse.tian-w.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xys.zhixingplan.top

C#:   Array.BinarySearch(arr, x)
来源：http://abh.jianghu66.top

[N02] 排序（工程实践用内置实现）
来源：http://dyt.gogol.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://hhy.jyoumei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tia.ydjk.org.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dxo.yonumen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://zje.yfazqb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://alg.zhengqikj.top

Go:   slices.Sort(arr)
来源：http://qty.jqgfzy.top

Ruby: arr.sort
来源：http://jrf.guowangkeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kzn.yueranfly.top

[N03] 快速排序（分治示例）
来源：http://loh.wangdashe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zjv.sjlbkw.cn

PHP:  // 递归实现，或用 usort
来源：http://tds.c1oappe.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vus.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wxs.shuidangran.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://heq.jlsjyb.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://boe.shuidangran.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xar.aizwys.cn

C#:   // 手写递归，或 Array.Sort
来源：http://egv.fanxiaobao.xyz

[N04] 斐波那契数列
来源：http://glm.c1oappe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pzy.yvedp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eok.hongshengwenyu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sfm.hfpthk.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zye.andypj.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xmf.cashguo.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://thd.jqgufenzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qzm.fanxiaobao.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qdv.zhiwuduotai.top

[N05] 最大公约数
来源：http://xte.sxryk.cn

Py:   math.gcd(a, b)
来源：http://igr.zhoulong.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lvj.nanxuanxn.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qkh.ydzc1.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dwz.vehdjk.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wih.xinyue.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pxn.sjlbkw.cn

Ruby: a.gcd(b)
来源：http://czl.kuanghao11.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vpi.ctjpmb.com

[N06] 判断回文字符串
来源：http://ndg.sysykeji.top

Py:   s == s[::-1]
来源：http://xhx.nwbrower.top

PHP:  $s === strrev($s);
来源：http://maq.zhoulong.xyz

JS:   s === [...s].reverse().join("")
来源：http://rdu.yueranfly.top

TS:   s === [...s].reverse().join("")
来源：http://adt.cqqwz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kep.andypj.xyz

Go:   // 双指针从两端比较
来源：http://bxa.jlsjyb.cn

Ruby: s == s.reverse
来源：http://sfv.yvedp.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://rwh.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://twx.svipenyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gtq.sufxvd.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://osw.shanyushiyangtech.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bri.kuanghao11.cn

TS:   // 手写 Map<string, number>
来源：http://fkh.zhaomingkeji.xyz

Java: // 手写 HashMap
来源：http://qlt.snrcjt.cn

Go:   // 手写 map[int]int
来源：http://aos.ywan-chungtsiang.top

Ruby: // 手写 Hash
来源：http://gln.shanyushiyangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://zss.vqdsnc.cn

[N08] 生成全排列
来源：http://csv.ydjk.org.cn

Py:   itertools.permutations(arr)
来源：http://zoy.vqdsnc.cn

PHP:  // 手写递归交换
来源：http://fpe.jyoumei.cn

JS:   // 手写回溯递归
来源：http://imw.yueranfly.top

TS:   // 手写回溯递归
来源：http://pzc.yangfankeji.com

Java: // 手写回溯递归
来源：http://seq.cucudq.cn

Go:   // 手写回溯递归
来源：http://ded.yuxming.cn

Ruby: arr.permutation.to_a
来源：http://ckt.yanxiufei.cn

C#:   // 手写回溯递归
来源：http://ltj.xuetiantiany.cn

[N09] 栈与队列
来源：http://hpo.jqgufenzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yot.zhijiandao.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vgv.316326.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ubi.jqgfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gjq.hnqzz.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gnr.guannengcc.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mlt.kuanghao11.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zwt.jyoumei.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fdy.smart0.xyz

[N10] 链表节点定义
来源：http://tan.tianlin.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mfh.zhijiandao.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://bxa.hywenlv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ezu.c1oappe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ngu.jyoumei.cn

Java: class Node { int v; Node next; }
来源：http://idv.c1oappe.top

Go:   type Node struct { V int; Next *Node }
来源：http://zzz.jyoumei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://mbp.zhoulong.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://kwk.mhx1999.top

[N11] 二叉树中序遍历
来源：http://vqh.kuanghao11.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zfp.gogol.net.cn

PHP:  // 手写递归函数
来源：http://liv.zycfv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fga.yongpay.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pog.ybcxt.top

Java: // 手写递归
来源：http://evk.bjfxy.top

Go:   // 手写递归
来源：http://zgo.yvedp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://whp.sjlbkw.cn

C#:   // 手写递归
来源：http://xbl.ybcxt.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hoz.gzhubu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qhc.gotoacloud.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tss.gotoacloud.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://klw.hnxiangtu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kcq.cashguo.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://nte.chenzaomai.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sxs.shzxlz.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://djn.wangdashe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yjh.jqgfzy.top

================================================================================
来源：http://zqj.xuetiantiany.cn

O. 并发与异步
来源：http://uqr.hnqzz.top

================================================================================
来源：http://gyc.dianchejie.cn

[O01] 启动一个线程
来源：http://vxj.zhixingplan.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://amv.nanxinkj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dao.gaohongyu789.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mqu.zdbjq.cn

TS:   // 同 JS
来源：http://bzp.svipenyu.cn

Java: new Thread(() -> f()).start()
来源：http://dba.sxryk.cn

Go:   go f()
来源：http://bir.yueranfly.top

Ruby: Thread.new { f }
来源：http://auv.zdbjq.cn

C#:   Task.Run(() => F());
来源：http://qwt.ydzc1.top

[O02] 使用线程池
来源：http://zve.gzhubu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://iea.yfazqb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://isq.sufxvd.cn

JS:   // worker_threads 线程池
来源：http://dbk.zhengqikj.top

TS:   // worker_threads 线程池
来源：http://jhb.zycfv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sxs.ehwqpu.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://buw.haohaochexian.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fyz.chenzaomai.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://aoq.aizwys.cn

[O03] 加锁保护共享数据
来源：http://tmv.hywenlv.cn

Py:   with lock: shared += 1
来源：http://fsr.jyoumei.cn

PHP:  // 用 flock() 做文件锁
来源：http://ykd.hesvh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fkl.cucudq.cn

TS:   // 同 JS
来源：http://eyb.vqdsnc.cn

Java: synchronized (this) { shared++; }
来源：http://csm.316326.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zta.zhengqikj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rzl.sjlbkw.cn

C#:   lock (gate) { shared++; }
来源：http://ekk.gotoacloud.top

[O04] 定义异步函数并等待
来源：http://shz.zhaomingkeji.xyz

Py:   async def f():⏎    await g()
来源：http://bra.cashguo.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://izs.yangfankeji.com

JS:   async function f() { await g(); }
来源：http://end.sweek.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qhe.yj202588.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zfk.xziqi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://aox.gzhubu.top

Ruby: # 用 Fiber 或 async gem
来源：http://gfk.9152youxi.cn

C#:   async Task F() { await G(); }
来源：http://nom.cashguo.top

[O05] 并发执行并等待全部完成
来源：http://kit.dashuyun.cn

Py:   asyncio.gather(*tasks)
来源：http://bng.cqqwz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iuk.vqdsnc.cn

JS:   await Promise.all(tasks)
来源：http://lrr.tarul.cn

TS:   await Promise.all(tasks)
来源：http://ixp.shuidangran.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://grq.tian-w.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dxr.ydzc1.top

Ruby: threads.map(&:join)
来源：http://pbd.daria6918.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sce.ydzc1.top

[O06] 使用进程池
来源：http://qmp.daria6918.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cyy.cheryme.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ymx.yuanzhike.top

JS:   // child_process / cluster 模块
来源：http://rlu.xingfuxueyuan.xyz

TS:   // child_process / cluster 模块
来源：http://prj.shanyushiyangtech.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eql.xuanzx.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yyk.ivvv.top

Ruby: // fork 块
来源：http://xtk.andypj.xyz

C#:   Parallel.For
来源：http://xmy.hnxiangtu.top

================================================================================
来源：http://wkj.gaohongyu789.top

P. 常用工具函数
来源：http://ros.sysykeji.top

================================================================================
来源：http://bub.gogol.net.cn

[P01] 生成 UUID
来源：http://guo.xuetiantiany.cn

Py:   str(uuid.uuid4())
来源：http://pqc.sxryk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sra.ydzc1.top

JS:   crypto.randomUUID()
来源：http://cnh.chenzaomai.com

TS:   crypto.randomUUID()
来源：http://trz.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://jli.mhx1999.top

Go:   // 用 github.com/google/uuid
来源：http://phw.wangdashe.top

Ruby: SecureRandom.uuid
来源：http://uya.fehbvm.com

C#:   Guid.NewGuid().ToString()
来源：http://dux.ivvv.top

[P02] MD5 / SHA256 摘要
来源：http://cqb.tian-w.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ygp.zhengqikj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dix.fehbvm.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yth.nanxuanxn.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pve.yuanzhike.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gtp.zhixingplan.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rnn.hammf.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://suc.yj202588.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kno.daria6918.cn

[P03] 生成短随机字符串
来源：http://zre.haohaochexian.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://edq.shangyingyoupin.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jvo.yj20258888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xdx.fehbvm.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://twq.hywenlv.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ikz.xuanzx.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nyw.zhijiandao.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yhz.dianchejie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ban.jinqigfzy.top

[P04] 求长度
来源：http://iot.guannengcc.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://eej.fzhhl.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gzq.xinyue.icu

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wxt.cucudq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vgu.snrcjt.cn

Java: list.size();  map.size();  s.length()
来源：http://vmc.xingfuxueyuan.xyz

Go:   len(arr);  len(m)
来源：http://phx.jinyuanbaomall.cn

Ruby: x.length;  x.size
来源：http://jyd.nwbrower.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ooh.shzxlz.cn

[P05] 判断两个对象内容是否相等
来源：http://rql.ybcxt.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://hht.316326.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://csm.yangfankeji.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cfg.hywenlv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mds.uphjek.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wdl.guannengcc.top

Go:   reflect.DeepEqual(a, b)
来源：http://utz.zhixingplan.top

Ruby: a == b
来源：http://nil.svipenyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lul.hammf.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://aro.jinghuilouyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qay.xylfe.cn

PHP:  if (empty($x)) {}
来源：http://euo.wangdashe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qsj.xuanzx.com

TS:   if (x == null) {}
来源：http://gva.yonumen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wys.gzhubu.top

Go:   if x == nil {}
来源：http://vde.yuxming.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cdf.yonumen.top

C#:   if (x is null) {}
来源：http://bis.jianghu66.top

[P07] 防抖与节流
来源：http://saq.guowangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hxq.dashuyun.cn

PHP:  // 手写时间戳比较
来源：http://ish.tanke756.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wpo.dashuyun.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ueo.9152youxi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dta.yvedp.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sao.xuanzx.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://bvl.zhijiandao.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qrs.hesvh.cn

[P08] 处理浮点精度问题
来源：http://bmd.bjfxy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aeg.jqgufenzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://obj.zhixingplan.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pdb.zhixingplan.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ifr.yj20258888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ryx.fanxiaobao.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vcy.hammf.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rif.xuanzx.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oxw.vehdjk.com

================================================================================
来源：http://uhq.zhongyouzk.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rvd.tarul.cn

================================================================================
来源：http://gqq.yj20258.top

[Q01] 创建表
来源：http://xqe.cqqwz.cn

CREATE TABLE users (
来源：http://jpd.snrcjt.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zzs.fanxiaobao.xyz

name VARCHAR(50) NOT NULL,
来源：http://sey.fktsv.cn

email VARCHAR(100) UNIQUE,
来源：http://veq.hnxiangtu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eou.xziqi.cn

);
来源：http://oym.zhiwuduotai.top

[Q02] 创建带外键的表
来源：http://tst.hammf.cn

CREATE TABLE orders (
来源：http://ofo.havefunace.top


<!-- 参考信息 -->