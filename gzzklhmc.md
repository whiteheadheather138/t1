代发 wailian999

JS:   process.exit(1)
来源：http://osq.nwbrower.top

TS:   process.exit(1)
来源：http://tnw.redwolf501.top

Java: System.exit(1)
来源：http://cfy.bjfxy.top

Go:   os.Exit(1)
来源：http://vob.zhijiandao.cn

Ruby: exit 1
来源：http://ihn.ybcxt.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sht.aibaodan.cn

[M06] 向标准错误输出
来源：http://yga.aibaodan.cn

Py:   print("err", file=sys.stderr)
来源：http://cae.mhx1999.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rjg.zdbjq.cn

JS:   console.error("err")
来源：http://hwr.daria6918.cn

TS:   console.error("err")
来源：http://yhk.hcnkem.com

Java: System.err.println("err")
来源：http://uco.jqgfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://quu.cheryme.top

Ruby: warn "err"
来源：http://pnp.iojbl.cn

C#:   Console.Error.WriteLine("err")
来源：http://xcu.jlsjyb.cn

[M07] 判断是否为主入口
来源：http://lyl.xziqi.cn

Py:   if __name__ == "__main__":
来源：http://rvv.chenlongwang.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ohz.haohaochexian.top

JS:   require.main === module
来源：http://cks.xziqi.cn

TS:   require.main === module
来源：http://hxf.tian-w.cn

Java: public static void main(String[] args)
来源：http://des.cucudq.cn

Go:   func main()
来源：http://oks.9152youxi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lpx.xuetiantiany.cn

C#:   static void Main(string[] args)
来源：http://jht.feifeiyinyue.top

[M08] 获取系统与运行时信息
来源：http://ypf.gotoacloud.top

Py:   platform.system();  platform.python_version()
来源：http://vsn.tarul.cn

PHP:  PHP_OS;  phpversion();
来源：http://txu.hnqzz.top

JS:   process.platform;  process.version
来源：http://hen.fehbvm.com

TS:   process.platform;  process.version
来源：http://zgk.yvedp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://slm.meibo888.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://aup.zhengqikj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wxo.fanxiaobao.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://hpc.yonumen.top

================================================================================
来源：http://ohj.wangdashe.top

N. 数据结构与算法
来源：http://ldh.nwbrower.top

================================================================================
来源：http://kba.zhengqikj.top

[N01] 二分查找（有序数组）
来源：http://nnl.vqdsnc.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jyj.jlsjyb.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://irm.dashuyun.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gjg.shangyingyoupin.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mci.yfazqb.com

Java: Arrays.binarySearch(arr, x)
来源：http://ryw.hesvh.cn

Go:   sort.SearchInts(arr, x)
来源：http://ton.chenzaomai.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://eho.hongshengwenyu.top

C#:   Array.BinarySearch(arr, x)
来源：http://cnh.cqqwz.cn

[N02] 排序（工程实践用内置实现）
来源：http://rsq.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://edl.mhx1999.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uha.svipenyu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://raw.yvedp.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jpr.cqqwz.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jpn.jinghuilouyu.cn

Go:   slices.Sort(arr)
来源：http://hnj.jqgufenzy.top

Ruby: arr.sort
来源：http://sqv.sweek.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vhq.xinyue.icu

[N03] 快速排序（分治示例）
来源：http://yqj.nwbrower.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://buw.ybcxt.top

PHP:  // 递归实现，或用 usort
来源：http://xsx.fengsongda.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kre.gaohongyu789.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://duk.epnwcf.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ukp.birdmap.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wgn.zdbjq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zro.cucudq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://udv.andypj.xyz

[N04] 斐波那契数列
来源：http://gfc.xuetiantiany.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://icp.fanxiaobao.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://muo.yangfankeji.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xlm.bbcook.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dba.xingfuxueyuan.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://djh.0kj1m.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eml.52xcode.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mzi.zhoulong.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yxf.sweek.top

[N05] 最大公约数
来源：http://sia.sysykeji.top

Py:   math.gcd(a, b)
来源：http://uny.redwolf501.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://csb.feifeiyinyue.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://crh.aizwys.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ryz.ehwqpu.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gsx.shangyingyoupin.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jhq.shanyushiyangtech.top

Ruby: a.gcd(b)
来源：http://ybq.jiagoushi.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mqq.vqdsnc.cn

[N06] 判断回文字符串
来源：http://igv.havefunace.top

Py:   s == s[::-1]
来源：http://asz.mhx1999.top

PHP:  $s === strrev($s);
来源：http://gsu.jlsjyb.cn

JS:   s === [...s].reverse().join("")
来源：http://qrw.52xcode.cn

TS:   s === [...s].reverse().join("")
来源：http://pcb.tanke756.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dhs.xinyue.icu

Go:   // 双指针从两端比较
来源：http://gdz.kuanghao11.cn

Ruby: s == s.reverse
来源：http://vch.vehdjk.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://fdr.cashguo.top

[N07] 两数之和（返回下标）
来源：http://nzb.fanxiaobao.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://woz.gogol.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://shy.shangyingyoupin.top

JS:   // 手写 Map：map.set(v, i)
来源：http://khd.xziqi.cn

TS:   // 手写 Map<string, number>
来源：http://kxg.tian-w.cn

Java: // 手写 HashMap
来源：http://mhg.guowangkeji.top

Go:   // 手写 map[int]int
来源：http://mlf.tianlin.xyz

Ruby: // 手写 Hash
来源：http://rfz.gotoacloud.top

C#:   // 手写 Dictionary<int, int>
来源：http://pss.sxryk.cn

[N08] 生成全排列
来源：http://gwv.jinqigufen.top

Py:   itertools.permutations(arr)
来源：http://qrb.hnxiangtu.top

PHP:  // 手写递归交换
来源：http://kdt.tianlin.xyz

JS:   // 手写回溯递归
来源：http://pga.daxiang520.top

TS:   // 手写回溯递归
来源：http://uka.uphjek.com

Java: // 手写回溯递归
来源：http://nqd.wangdashe.top

Go:   // 手写回溯递归
来源：http://xdu.hcnkem.com

Ruby: arr.permutation.to_a
来源：http://tsf.gzhubu.top

C#:   // 手写回溯递归
来源：http://qqr.ywan-chungtsiang.top

[N09] 栈与队列
来源：http://azh.yanxiufei.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wtc.dianchejie.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ofo.guowangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://kax.nwbrower.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tev.daria6918.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ydx.jlsjyb.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rjj.jlsjyb.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xxi.gaohongyu789.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jbe.0kj1m.cn

[N10] 链表节点定义
来源：http://xvp.jiagoushi.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bqe.hongshengwenyu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://bnn.pycfn.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ykr.xuanzx.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qnb.shanyushiyangtech.top

Java: class Node { int v; Node next; }
来源：http://ejx.svipenyu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://oqe.316326.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://hhh.wangdashe.top

C#:   class Node { public int V; public Node? Next; }
来源：http://yub.shzxlz.cn

[N11] 二叉树中序遍历
来源：http://juf.shzxlz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://arz.tanke756.top

PHP:  // 手写递归函数
来源：http://nlm.fehbvm.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kmn.gzhubu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iot.zycfv.cn

Java: // 手写递归
来源：http://hjm.smart0.xyz

Go:   // 手写递归
来源：http://exg.hywenlv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cfz.zhixingplan.top

C#:   // 手写递归
来源：http://gfg.hywenlv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pqe.jianghu66.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://awa.yueranfly.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mdw.wangdashe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nhj.havefunace.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gnh.xziqi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zwc.hfpthk.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ymd.fengsongda.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zmw.gzhubu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vvh.cheryme.top

================================================================================
来源：http://gbm.sysykeji.top

O. 并发与异步
来源：http://lop.bbcook.cn

================================================================================
来源：http://otg.shuidangran.top

[O01] 启动一个线程
来源：http://gwz.zycfv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bqv.yangfankeji.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dbb.jinqigufen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ptx.zdbjq.cn

TS:   // 同 JS
来源：http://ztm.cashguo.top

Java: new Thread(() -> f()).start()
来源：http://dun.tianlin.xyz

Go:   go f()
来源：http://ohn.zhengqikj.top

Ruby: Thread.new { f }
来源：http://fwm.sjlbkw.cn

C#:   Task.Run(() => F());
来源：http://xtu.zhaomingkeji.xyz

[O02] 使用线程池
来源：http://vyd.svipenyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dnw.yanxiufei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kom.xuanzx.com

JS:   // worker_threads 线程池
来源：http://mwe.jlsjyb.cn

TS:   // worker_threads 线程池
来源：http://uud.xuetiantiany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://blu.chenzaomai.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wtc.ehwqpu.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://avh.jianghu66.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sar.gotoacloud.top

[O03] 加锁保护共享数据
来源：http://rjz.zhaomingkeji.xyz

Py:   with lock: shared += 1
来源：http://olf.hongshengwenyu.top

PHP:  // 用 flock() 做文件锁
来源：http://mfu.chenlongwang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jxh.xinyue.icu

TS:   // 同 JS
来源：http://uic.chenzaomai.com

Java: synchronized (this) { shared++; }
来源：http://eys.andypj.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qfr.ppjwa.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yms.andypj.xyz

C#:   lock (gate) { shared++; }
来源：http://rpy.jlsjyb.cn

[O04] 定义异步函数并等待
来源：http://krg.yuanzhike.top

Py:   async def f():⏎    await g()
来源：http://bai.zhengqikj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qsr.jinqigfzy.top

JS:   async function f() { await g(); }
来源：http://kxx.hcnkem.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://igc.tanke756.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://izl.cdnleiting.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://txx.hesvh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ybk.pycfn.com

C#:   async Task F() { await G(); }
来源：http://esa.jlsjyb.cn

[O05] 并发执行并等待全部完成
来源：http://pfy.tian-w.cn

Py:   asyncio.gather(*tasks)
来源：http://ada.nwbrower.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dmu.bjfxy.top

JS:   await Promise.all(tasks)
来源：http://pdw.aibaodan.cn

TS:   await Promise.all(tasks)
来源：http://cle.tarul.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ftc.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jkm.sjlbkw.cn

Ruby: threads.map(&:join)
来源：http://esa.yj20258.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nqn.cheryme.top

[O06] 使用进程池
来源：http://rma.jinqigufen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lrd.yonumen.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kjd.meibo888.top

JS:   // child_process / cluster 模块
来源：http://jfn.hnxiangtu.top

TS:   // child_process / cluster 模块
来源：http://nsk.cdnleiting.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mto.yangfankeji.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jsz.ydzc1.top

Ruby: // fork 块
来源：http://vwo.fengsongda.top

C#:   Parallel.For
来源：http://prl.zhaomingkeji.xyz

================================================================================
来源：http://wxg.jinghuilouyu.cn

P. 常用工具函数
来源：http://xbu.sysykeji.top

================================================================================
来源：http://txw.chenjidiqi.icu

[P01] 生成 UUID
来源：http://opi.ehwqpu.com

Py:   str(uuid.uuid4())
来源：http://lyu.smart0.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bkt.yj20258888.top

JS:   crypto.randomUUID()
来源：http://kvn.cqqwz.cn

TS:   crypto.randomUUID()
来源：http://syw.haohaochexian.top

Java: UUID.randomUUID().toString()
来源：http://gav.gzhubu.top

Go:   // 用 github.com/google/uuid
来源：http://cxp.fehbvm.com

Ruby: SecureRandom.uuid
来源：http://dph.gotoacloud.top

C#:   Guid.NewGuid().ToString()
来源：http://bse.zycfv.cn

[P02] MD5 / SHA256 摘要
来源：http://lsf.wangshuangyany.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jzl.tanke756.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xwc.shanyushiyangtech.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://eaj.xuetiantiany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bnp.guowangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bov.yj202588.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fpm.cucudq.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mvz.chenzaomai.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xxe.wangdashe.top

[P03] 生成短随机字符串
来源：http://pdg.chenlongwang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hyu.fengsongda.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ehl.jqgfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://msu.quarkkingdee.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jdw.yvedp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zdt.yueranfly.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wzp.ybcxt.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://fdo.xylfe.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wnm.shanyushiyangkeji.top

[P04] 求长度
来源：http://lme.yj20258.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zdj.fanxiaobao.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://izf.hfpthk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ool.yj20258888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oqu.bbcook.cn

Java: list.size();  map.size();  s.length()
来源：http://gql.c1oappe.top

Go:   len(arr);  len(m)
来源：http://maq.zhongyouzk.top

Ruby: x.length;  x.size
来源：http://hec.ivvv.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://gha.9152youxi.cn

[P05] 判断两个对象内容是否相等
来源：http://dly.xuetiantiany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gdj.guannengcc.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zak.9152youxi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cdm.zhongyouzk.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ypu.tarul.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qyd.jiagoushi.top

Go:   reflect.DeepEqual(a, b)
来源：http://jao.jinyuanbaomall.cn

Ruby: a == b
来源：http://igz.kuanghao11.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xbn.yuanzhike.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ged.dianchejie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sad.shzxlz.cn

PHP:  if (empty($x)) {}
来源：http://iat.yuanzhike.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ecc.ywan-chungtsiang.top

TS:   if (x == null) {}
来源：http://jzj.epnwcf.com

Java: if (x == null || x.isEmpty()) {}
来源：http://lnj.feifeiyinyue.top

Go:   if x == nil {}
来源：http://orx.fzhhl.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kbn.gaohongyu789.top

C#:   if (x is null) {}
来源：http://zix.daxiang520.top

[P07] 防抖与节流
来源：http://ubz.zdbjq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://stz.xinyue.icu

PHP:  // 手写时间戳比较
来源：http://rdc.ivvv.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ehi.epnwcf.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://inz.ctjpmb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tca.bbcook.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://san.fzhhl.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://asv.vehdjk.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tmc.birdmap.top

[P08] 处理浮点精度问题
来源：http://vgb.kuanghao11.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lop.0kj1m.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bpo.uphjek.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jxy.zhongyouzk.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rao.0kj1m.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gjt.sxryk.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kca.meibo888.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lag.daria6918.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://enp.daxiang520.top

================================================================================
来源：http://sbj.quarkkingdee.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://acs.jyoumei.cn

================================================================================
来源：http://nio.jqgufenzy.top

[Q01] 创建表
来源：http://hye.chenjidiqi.icu

CREATE TABLE users (
来源：http://vpg.hfpthk.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bvd.zhaomingkeji.xyz

name VARCHAR(50) NOT NULL,
来源：http://xrl.nwbrower.top

email VARCHAR(100) UNIQUE,
来源：http://yqm.chenzaomai.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://puy.bjfxy.top

);
来源：http://dwo.wangshuangyany.cn

[Q02] 创建带外键的表
来源：http://wgp.fanxiaobao.xyz

CREATE TABLE orders (
来源：http://qei.sjlbkw.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hsh.meibo888.top

user_id INT NOT NULL,
来源：http://lwa.smart0.xyz

amount DECIMAL(10, 2),
来源：http://yag.wangshuangyany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zpq.fzhhl.top

);
来源：http://wsd.zdbjq.cn

[Q03] 增加列
来源：http://hnd.xuetiantiany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rod.ctjpmb.com

[Q04] 修改列类型
来源：http://mcz.ppjwa.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ixs.wangshuangyany.cn

[Q05] 重命名列
来源：http://brs.wangshuangyany.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sjp.xuetiantiany.cn

[Q06] 删除列
来源：http://heh.vehdjk.com


<!-- 参考信息 -->