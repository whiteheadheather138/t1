代发 wailian999

[M04] 获取当前工作目录
来源：http://umi.hysaishi.cn

Py:   os.getcwd()
来源：http://vvw.zdbjq.cn

PHP:  getcwd();
来源：http://hzf.zdbjq.cn

JS:   process.cwd()
来源：http://whv.cucudq.cn

TS:   process.cwd()
来源：http://bvv.feifeiyinyue.top

Java: Path.of("").toAbsolutePath()
来源：http://tld.nanxinkj.top

Go:   os.Getwd()
来源：http://wnr.ydzc1.top

Ruby: Dir.pwd
来源：http://vxm.zhaomingkeji.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://wpk.zdqjudy.top

[M05] 设置退出码
来源：http://cje.zhengqikj.top

Py:   sys.exit(1)
来源：http://ysk.xziqi.cn

PHP:  exit(1);
来源：http://ghp.xuetiantiany.cn

JS:   process.exit(1)
来源：http://fpk.ctjpmb.com

TS:   process.exit(1)
来源：http://iwo.316326.xyz

Java: System.exit(1)
来源：http://lcv.ydjk.org.cn

Go:   os.Exit(1)
来源：http://ffg.jlsjyb.cn

Ruby: exit 1
来源：http://lgn.jqgufenzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://exr.yj202588.top

[M06] 向标准错误输出
来源：http://mmg.jinyuanbaomall.cn

Py:   print("err", file=sys.stderr)
来源：http://hfk.guowangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gkt.pengpengdd.cyou

JS:   console.error("err")
来源：http://mth.hnqzz.top

TS:   console.error("err")
来源：http://cda.cqqwz.cn

Java: System.err.println("err")
来源：http://oya.tarul.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cfb.snrcjt.cn

Ruby: warn "err"
来源：http://aer.fanxiaobao.xyz

C#:   Console.Error.WriteLine("err")
来源：http://upi.fktsv.cn

[M07] 判断是否为主入口
来源：http://ovt.birdmap.top

Py:   if __name__ == "__main__":
来源：http://jpe.meibo888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tmv.andypj.xyz

JS:   require.main === module
来源：http://yyu.xuetiantiany.cn

TS:   require.main === module
来源：http://itt.ctjpmb.com

Java: public static void main(String[] args)
来源：http://efc.shuidangran.top

Go:   func main()
来源：http://txx.zhoulong.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://szh.0kj1m.cn

C#:   static void Main(string[] args)
来源：http://bwc.chenzaomai.com

[M08] 获取系统与运行时信息
来源：http://qcl.zdbjq.cn

Py:   platform.system();  platform.python_version()
来源：http://ekr.tanke756.top

PHP:  PHP_OS;  phpversion();
来源：http://fsf.xuetiantiany.cn

JS:   process.platform;  process.version
来源：http://hss.shanyushiyangkeji.top

TS:   process.platform;  process.version
来源：http://uzx.gzhubu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bny.yj20258888.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fsh.52xcode.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gsa.xziqi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yez.havefunace.top

================================================================================
来源：http://bfv.gzhubu.top

N. 数据结构与算法
来源：http://osm.meibo888.top

================================================================================
来源：http://biq.cqqwz.cn

[N01] 二分查找（有序数组）
来源：http://ymw.xuanzx.com

Py:   bisect.bisect_left(arr, x)
来源：http://oqt.guowangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mwg.tanke756.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nqw.xziqi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://thx.hesvh.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ppn.tarul.cn

Go:   sort.SearchInts(arr, x)
来源：http://wyv.tanke756.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://myc.shzxlz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gqs.havefunace.top

[N02] 排序（工程实践用内置实现）
来源：http://taa.tarul.cn

Py:   sorted(arr);  arr.sort()
来源：http://aqx.xuetiantiany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://elb.52xcode.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hig.jinqigufen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://gzj.fzhhl.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wxi.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://jjw.yuanzhike.top

Ruby: arr.sort
来源：http://bxz.tianlin.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://tjg.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://ndb.nanxinkj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vek.hammf.cn

PHP:  // 递归实现，或用 usort
来源：http://omk.zhixingplan.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rji.cqqwz.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vgc.zhijiandao.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://enh.yueranfly.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://akm.aizwys.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qln.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://yjo.sufxvd.cn

[N04] 斐波那契数列
来源：http://lfy.shanyushiyangtech.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://afr.ydjk.org.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zuk.nanxinkj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ahd.zdqjudy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xbl.zhongyouzk.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ciy.jinqigfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://red.hysaishi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qvb.wangshuangyany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vpc.iojbl.cn

[N05] 最大公约数
来源：http://bog.yvedp.cn

Py:   math.gcd(a, b)
来源：http://www.chenzaomai.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fym.jiagoushi.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mdz.hfpthk.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ovk.fengsongda.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ewk.chenzaomai.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fow.yvedp.cn

Ruby: a.gcd(b)
来源：http://qcw.wangshuangyany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xpt.xinyue.icu

[N06] 判断回文字符串
来源：http://rhz.pycfn.com

Py:   s == s[::-1]
来源：http://utc.kuanghao11.cn

PHP:  $s === strrev($s);
来源：http://chv.tarul.cn

JS:   s === [...s].reverse().join("")
来源：http://ous.yj20258.top

TS:   s === [...s].reverse().join("")
来源：http://wav.yanxiufei.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ffr.fengsongda.top

Go:   // 双指针从两端比较
来源：http://cli.xziqi.cn

Ruby: s == s.reverse
来源：http://qxj.meibo888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://tsz.aibaodan.cn

[N07] 两数之和（返回下标）
来源：http://edc.zhongyouzk.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fhl.yfazqb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sjp.yangfankeji.com

JS:   // 手写 Map：map.set(v, i)
来源：http://cnz.chenlongwang.top

TS:   // 手写 Map<string, number>
来源：http://sqa.yj20258.top

Java: // 手写 HashMap
来源：http://ddg.ehwqpu.com

Go:   // 手写 map[int]int
来源：http://mbj.yanxiufei.cn

Ruby: // 手写 Hash
来源：http://wil.xziqi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://jkf.zhengqikj.top

[N08] 生成全排列
来源：http://nyi.guannengcc.top

Py:   itertools.permutations(arr)
来源：http://ewj.yueranfly.top

PHP:  // 手写递归交换
来源：http://qlg.zdqjudy.top

JS:   // 手写回溯递归
来源：http://xzj.aizwys.cn

TS:   // 手写回溯递归
来源：http://gbe.daria6918.cn

Java: // 手写回溯递归
来源：http://cpv.chenlongwang.top

Go:   // 手写回溯递归
来源：http://apd.yonumen.top

Ruby: arr.permutation.to_a
来源：http://jkx.haohaochexian.top

C#:   // 手写回溯递归
来源：http://tej.daxiang520.top

[N09] 栈与队列
来源：http://thv.hfpthk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kvv.0kj1m.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wfz.yj20258888.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cio.redwolf501.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://esk.hongshengwenyu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bcd.jyoumei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rjb.chenzaomai.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jig.guannengcc.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rkl.fengsongda.top

[N10] 链表节点定义
来源：http://tgh.yueranfly.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://emm.jlsjyb.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://neu.zhixingplan.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vog.sweek.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kef.tarul.cn

Java: class Node { int v; Node next; }
来源：http://ayc.aibaodan.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bmf.xziqi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qnf.ivvv.top

C#:   class Node { public int V; public Node? Next; }
来源：http://tbk.shangyingyoupin.top

[N11] 二叉树中序遍历
来源：http://bqm.andypj.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fvw.zycfv.cn

PHP:  // 手写递归函数
来源：http://ifd.cqqwz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://loi.jianghu66.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://avh.yj202588.top

Java: // 手写递归
来源：http://abr.shanyushiyangtech.top

Go:   // 手写递归
来源：http://rae.316326.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ziy.hysaishi.cn

C#:   // 手写递归
来源：http://ufh.haohaochexian.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qff.iojbl.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://imt.dianchejie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pcm.cheryme.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hkz.hesvh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hcn.yj20258.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xgc.yj20258888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sts.xylfe.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iqi.0kj1m.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zjq.chenlongwang.top

================================================================================
来源：http://imu.nanxuanxn.top

O. 并发与异步
来源：http://jfe.yfazqb.com

================================================================================
来源：http://kct.chenlongwang.top

[O01] 启动一个线程
来源：http://osv.hnqzz.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wji.ivvv.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pum.shangyingyoupin.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hgh.gotoacloud.top

TS:   // 同 JS
来源：http://swb.tanke756.top

Java: new Thread(() -> f()).start()
来源：http://ssp.ctjpmb.com

Go:   go f()
来源：http://ulu.sxryk.cn

Ruby: Thread.new { f }
来源：http://fay.guowangkeji.top

C#:   Task.Run(() => F());
来源：http://zzj.ctjpmb.com

[O02] 使用线程池
来源：http://erj.jinqigfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mcf.yangfankeji.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xrz.fengsongda.top

JS:   // worker_threads 线程池
来源：http://wbn.cqqwz.cn

TS:   // worker_threads 线程池
来源：http://pjj.yongpay.top

Java: Executors.newFixedThreadPool(4)
来源：http://uew.svipenyu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bzi.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pqm.guowangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://por.ywan-chungtsiang.top

[O03] 加锁保护共享数据
来源：http://bpj.bjfxy.top

Py:   with lock: shared += 1
来源：http://ppo.shuidangran.top

PHP:  // 用 flock() 做文件锁
来源：http://ljd.yongpay.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vua.xinyue.icu

TS:   // 同 JS
来源：http://nzv.feifeiyinyue.top

Java: synchronized (this) { shared++; }
来源：http://hnx.ydjk.org.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vrr.andypj.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://tkc.smart0.xyz

C#:   lock (gate) { shared++; }
来源：http://vtu.yangfankeji.com

[O04] 定义异步函数并等待
来源：http://rno.shangyingyoupin.top

Py:   async def f():⏎    await g()
来源：http://zwj.shanyushiyangtech.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pod.nanxuanxn.top

JS:   async function f() { await g(); }
来源：http://npb.feifeiyinyue.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hug.jqgufenzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lrv.yangfankeji.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uyo.zhixingplan.top

Ruby: # 用 Fiber 或 async gem
来源：http://yuj.daria6918.cn

C#:   async Task F() { await G(); }
来源：http://ppm.hysaishi.cn

[O05] 并发执行并等待全部完成
来源：http://yvy.yueranfly.top

Py:   asyncio.gather(*tasks)
来源：http://mzp.ctjpmb.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://diu.gzhubu.top

JS:   await Promise.all(tasks)
来源：http://lep.jinyuanbaomall.cn

TS:   await Promise.all(tasks)
来源：http://gss.pycfn.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://npd.yuanzhike.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rho.birdmap.top

Ruby: threads.map(&:join)
来源：http://zhg.wangshuangyany.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://duh.ppjwa.cn

[O06] 使用进程池
来源：http://vve.jianghu66.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mnn.pycfn.com

PHP:  // pcntl_fork 或多进程队列
来源：http://ilc.hfpthk.cn

JS:   // child_process / cluster 模块
来源：http://jsy.daria6918.cn

TS:   // child_process / cluster 模块
来源：http://cpp.iojbl.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mhg.ctjpmb.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xts.dianchejie.cn

Ruby: // fork 块
来源：http://xqd.vehdjk.com

C#:   Parallel.For
来源：http://hvt.vqdsnc.cn

================================================================================
来源：http://jmp.yongpay.top

P. 常用工具函数
来源：http://bvu.gzhubu.top

================================================================================
来源：http://sgu.shanyushiyangkeji.top

[P01] 生成 UUID
来源：http://zvv.cheryme.top

Py:   str(uuid.uuid4())
来源：http://abk.fengsongda.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hpo.zhongyouzk.top

JS:   crypto.randomUUID()
来源：http://gmr.aizwys.cn

TS:   crypto.randomUUID()
来源：http://rhm.fanxiaobao.xyz

Java: UUID.randomUUID().toString()
来源：http://ore.jinghuilouyu.cn

Go:   // 用 github.com/google/uuid
来源：http://yug.aizwys.cn

Ruby: SecureRandom.uuid
来源：http://knm.sufxvd.cn

C#:   Guid.NewGuid().ToString()
来源：http://srj.zdqjudy.top

[P02] MD5 / SHA256 摘要
来源：http://ftz.haohaochexian.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dyr.hysaishi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kdx.hesvh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qcf.cheryme.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gdl.daxiang520.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nqd.feifeiyinyue.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hyc.yj202588.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://arc.iojbl.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yve.vqdsnc.cn

[P03] 生成短随机字符串
来源：http://ibc.nwbrower.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://itq.shuidangran.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gew.ppjwa.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qqk.gaohongyu789.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ayu.daria6918.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://eqa.hammf.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hkd.sweek.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://pwo.fengsongda.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ebh.mhx1999.top

[P04] 求长度
来源：http://yzi.cashguo.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gvt.kuanghao11.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gca.zhoulong.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bxz.zdbjq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vla.kuanghao11.cn

Java: list.size();  map.size();  s.length()
来源：http://gnc.tianlin.xyz

Go:   len(arr);  len(m)
来源：http://fkp.cheryme.top

Ruby: x.length;  x.size
来源：http://ggj.jinqigfzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://wkz.sweek.top

[P05] 判断两个对象内容是否相等
来源：http://wmv.redwolf501.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://oay.cucudq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rat.zhijiandao.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tjp.zhijiandao.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dhl.guannengcc.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://noq.xuetiantiany.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ijr.yvedp.cn

Ruby: a == b
来源：http://lxr.kuanghao11.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pkt.epnwcf.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bje.zhijiandao.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cxb.ydzc1.top

PHP:  if (empty($x)) {}
来源：http://wwh.bbcook.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ahh.zycfv.cn

TS:   if (x == null) {}
来源：http://riu.hywenlv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nol.ydjk.org.cn

Go:   if x == nil {}
来源：http://ixj.c1oappe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dcs.smart0.xyz

C#:   if (x is null) {}
来源：http://rbq.havefunace.top

[P07] 防抖与节流
来源：http://uyy.guowangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rru.hnqzz.top

PHP:  // 手写时间戳比较
来源：http://scr.sjlbkw.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eqk.aibaodan.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rvz.iojbl.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qps.hongshengwenyu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pja.sweek.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://lvj.cdnleiting.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gfy.jlsjyb.cn

[P08] 处理浮点精度问题
来源：http://laj.xuetiantiany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xdh.316326.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cfu.kuanghao11.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uog.bjfxy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yac.pycfn.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qsw.redwolf501.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rai.wangshuangyany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tkf.jianghu66.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pgv.9152youxi.cn

================================================================================
来源：http://kbq.yanxiufei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pqo.hammf.cn

================================================================================
来源：http://yht.jinyuanbaomall.cn

[Q01] 创建表
来源：http://qrv.zhongyouzk.top

CREATE TABLE users (
来源：http://cvg.shuidangran.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pep.ivvv.top

name VARCHAR(50) NOT NULL,
来源：http://lgu.tarul.cn

email VARCHAR(100) UNIQUE,
来源：http://oaj.jinyuanbaomall.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yoz.yueranfly.top

);
来源：http://zgi.yongpay.top

[Q02] 创建带外键的表
来源：http://byo.shanyushiyangkeji.top

CREATE TABLE orders (
来源：http://wyj.smart0.xyz


<!-- 参考信息 -->