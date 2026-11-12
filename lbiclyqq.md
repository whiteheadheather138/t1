代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://nvv.jqgfzy.top

[M05] 设置退出码
来源：http://pra.c1oappe.top

Py:   sys.exit(1)
来源：http://zpb.yvedp.cn

PHP:  exit(1);
来源：http://ddz.jqgufenzy.top

JS:   process.exit(1)
来源：http://cgz.jqgfzy.top

TS:   process.exit(1)
来源：http://ier.zdbjq.cn

Java: System.exit(1)
来源：http://dkf.chenlongwang.top

Go:   os.Exit(1)
来源：http://pck.hcnkem.com

Ruby: exit 1
来源：http://cmk.xingfuxueyuan.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vvp.sufxvd.cn

[M06] 向标准错误输出
来源：http://xpu.316326.xyz

Py:   print("err", file=sys.stderr)
来源：http://mve.ivvv.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ors.xinyue.icu

JS:   console.error("err")
来源：http://wit.aibaodan.cn

TS:   console.error("err")
来源：http://fjl.shanyushiyangtech.top

Java: System.err.println("err")
来源：http://kpl.cqqwz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jdi.xingfuxueyuan.xyz

Ruby: warn "err"
来源：http://sxx.epnwcf.com

C#:   Console.Error.WriteLine("err")
来源：http://etq.316326.xyz

[M07] 判断是否为主入口
来源：http://oqk.jianghu66.top

Py:   if __name__ == "__main__":
来源：http://hus.zhaomingkeji.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vmb.kuanghao11.cn

JS:   require.main === module
来源：http://oky.jianghu66.top

TS:   require.main === module
来源：http://mhb.wangdashe.top

Java: public static void main(String[] args)
来源：http://kkv.birdmap.top

Go:   func main()
来源：http://vpa.zhaomingkeji.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://umv.tarul.cn

C#:   static void Main(string[] args)
来源：http://ehi.hywenlv.cn

[M08] 获取系统与运行时信息
来源：http://pbl.sufxvd.cn

Py:   platform.system();  platform.python_version()
来源：http://epe.yueranfly.top

PHP:  PHP_OS;  phpversion();
来源：http://ajw.yj20258888.top

JS:   process.platform;  process.version
来源：http://uxh.hongshengwenyu.top

TS:   process.platform;  process.version
来源：http://ptu.sxryk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mnp.chenzaomai.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://hkk.jinyuanbaomall.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hqt.ppjwa.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jpc.yuanzhike.top

================================================================================
来源：http://jqs.yonumen.top

N. 数据结构与算法
来源：http://rwr.redwolf501.top

================================================================================
来源：http://mtp.feifeiyinyue.top

[N01] 二分查找（有序数组）
来源：http://jts.ywan-chungtsiang.top

Py:   bisect.bisect_left(arr, x)
来源：http://gzw.andypj.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ejo.0kj1m.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tem.yfazqb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dnf.xylfe.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zhc.zhijiandao.cn

Go:   sort.SearchInts(arr, x)
来源：http://zhx.fzhhl.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qvu.xziqi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bzt.chenlongwang.top

[N02] 排序（工程实践用内置实现）
来源：http://ngt.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://ryn.pycfn.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hne.ehwqpu.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://aez.ehwqpu.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://zkw.vehdjk.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eqe.shzxlz.cn

Go:   slices.Sort(arr)
来源：http://ehj.tianlin.xyz

Ruby: arr.sort
来源：http://tsr.fengsongda.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kbg.fengsongda.top

[N03] 快速排序（分治示例）
来源：http://cyd.fehbvm.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oxf.cheryme.top

PHP:  // 递归实现，或用 usort
来源：http://eqd.ydjk.org.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rpf.uphjek.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fnq.zhoulong.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://kcw.tarul.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yfq.c1oappe.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hrx.hnqzz.top

C#:   // 手写递归，或 Array.Sort
来源：http://twv.birdmap.top

[N04] 斐波那契数列
来源：http://zol.daria6918.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://stg.hnqzz.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ayf.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://smc.gaohongyu789.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zps.nwbrower.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yha.316326.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gsk.gzhubu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bww.fzhhl.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mzt.snrcjt.cn

[N05] 最大公约数
来源：http://fky.ydjk.org.cn

Py:   math.gcd(a, b)
来源：http://gqa.smart0.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wfd.zhaomingkeji.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iaz.zhengqikj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eew.gaohongyu789.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yrs.xingfuxueyuan.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://brf.guowangkeji.top

Ruby: a.gcd(b)
来源：http://kgh.fktsv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://woq.iojbl.cn

[N06] 判断回文字符串
来源：http://dog.andypj.xyz

Py:   s == s[::-1]
来源：http://szw.dashuyun.cn

PHP:  $s === strrev($s);
来源：http://pye.fzhhl.top

JS:   s === [...s].reverse().join("")
来源：http://kxb.tarul.cn

TS:   s === [...s].reverse().join("")
来源：http://mma.jiagoushi.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://iyu.ybcxt.top

Go:   // 双指针从两端比较
来源：http://ake.chenjidiqi.icu

Ruby: s == s.reverse
来源：http://ahx.cqqwz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://dik.ydjk.org.cn

[N07] 两数之和（返回下标）
来源：http://oex.9152youxi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qcc.jqgfzy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bks.quarkkingdee.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zah.shanyushiyangkeji.top

TS:   // 手写 Map<string, number>
来源：http://nqk.birdmap.top

Java: // 手写 HashMap
来源：http://ckf.ywan-chungtsiang.top

Go:   // 手写 map[int]int
来源：http://xah.nanxuanxn.top

Ruby: // 手写 Hash
来源：http://mmu.shanyushiyangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://lhh.shzxlz.cn

[N08] 生成全排列
来源：http://pjs.feifeiyinyue.top

Py:   itertools.permutations(arr)
来源：http://zcp.mhx1999.top

PHP:  // 手写递归交换
来源：http://bkg.quarkkingdee.top

JS:   // 手写回溯递归
来源：http://chj.yonumen.top

TS:   // 手写回溯递归
来源：http://mot.yj20258.top

Java: // 手写回溯递归
来源：http://lyd.guannengcc.top

Go:   // 手写回溯递归
来源：http://gpa.hammf.cn

Ruby: arr.permutation.to_a
来源：http://muw.fehbvm.com

C#:   // 手写回溯递归
来源：http://zrf.shanyushiyangkeji.top

[N09] 栈与队列
来源：http://irq.jqgufenzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ikf.aizwys.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mci.ppjwa.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zkq.snrcjt.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fci.dianchejie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uap.tarul.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qnu.ehwqpu.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bir.pengpengdd.cyou

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ftl.vehdjk.com

[N10] 链表节点定义
来源：http://jha.tian-w.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zay.chenjidiqi.icu

PHP:  class Node { public $v; public $next = null; }
来源：http://gsr.fengsongda.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ymo.chenzaomai.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://aaz.xuetiantiany.cn

Java: class Node { int v; Node next; }
来源：http://xlg.daria6918.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mcj.ctjpmb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://bys.dashuyun.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nfy.ywan-chungtsiang.top

[N11] 二叉树中序遍历
来源：http://geb.yvedp.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nsb.guannengcc.top

PHP:  // 手写递归函数
来源：http://bsq.pengpengdd.cyou

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fpm.0kj1m.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rvl.fzhhl.top

Java: // 手写递归
来源：http://unx.haohaochexian.top

Go:   // 手写递归
来源：http://cuz.iojbl.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xzu.andypj.xyz

C#:   // 手写递归
来源：http://tzy.zhixingplan.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://onk.shzxlz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rvh.zhongyouzk.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fuv.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zgy.52xcode.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cly.yuxming.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://apt.316326.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cei.yvedp.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zzl.aizwys.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mhw.tian-w.cn

================================================================================
来源：http://vza.jyoumei.cn

O. 并发与异步
来源：http://trx.birdmap.top

================================================================================
来源：http://qyy.hesvh.cn

[O01] 启动一个线程
来源：http://ond.jyoumei.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ifw.yanxiufei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rdb.hnqzz.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pdv.chenjidiqi.icu

TS:   // 同 JS
来源：http://riy.yvedp.cn

Java: new Thread(() -> f()).start()
来源：http://lgl.yuanzhike.top

Go:   go f()
来源：http://mzj.zhixingplan.top

Ruby: Thread.new { f }
来源：http://hzy.c1oappe.top

C#:   Task.Run(() => F());
来源：http://ovk.ppjwa.cn

[O02] 使用线程池
来源：http://zne.shuidangran.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pkt.yanxiufei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://sqh.fzhhl.top

JS:   // worker_threads 线程池
来源：http://kzd.jinqigfzy.top

TS:   // worker_threads 线程池
来源：http://paq.aizwys.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rww.xinyue.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fsy.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vzg.jyoumei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zbu.sxryk.cn

[O03] 加锁保护共享数据
来源：http://hjx.fengsongda.top

Py:   with lock: shared += 1
来源：http://hpt.cucudq.cn

PHP:  // 用 flock() 做文件锁
来源：http://jha.kuanghao11.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vmh.smart0.xyz

TS:   // 同 JS
来源：http://qsy.nanxuanxn.top

Java: synchronized (this) { shared++; }
来源：http://qzm.ywan-chungtsiang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hrf.ctjpmb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://nun.pycfn.com

C#:   lock (gate) { shared++; }
来源：http://hhb.zhongyouzk.top

[O04] 定义异步函数并等待
来源：http://zsc.birdmap.top

Py:   async def f():⏎    await g()
来源：http://uny.yuanzhike.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jdv.xingfuxueyuan.xyz

JS:   async function f() { await g(); }
来源：http://lzp.ivvv.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qqe.jinqigfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ibx.chenzaomai.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qmd.vehdjk.com

Ruby: # 用 Fiber 或 async gem
来源：http://dpo.shanyushiyangkeji.top

C#:   async Task F() { await G(); }
来源：http://ney.cheryme.top

[O05] 并发执行并等待全部完成
来源：http://lrm.wangshuangyany.cn

Py:   asyncio.gather(*tasks)
来源：http://nnz.zhijiandao.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dfc.cdnleiting.top

JS:   await Promise.all(tasks)
来源：http://vbi.fengsongda.top

TS:   await Promise.all(tasks)
来源：http://mgz.jinqigufen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wjp.hongshengwenyu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sjv.xuetiantiany.cn

Ruby: threads.map(&:join)
来源：http://uie.havefunace.top

C#:   await Task.WhenAll(t1, t2)
来源：http://teb.hywenlv.cn

[O06] 使用进程池
来源：http://the.jinghuilouyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lle.jlsjyb.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yyx.tianlin.xyz

JS:   // child_process / cluster 模块
来源：http://zzx.uphjek.com

TS:   // child_process / cluster 模块
来源：http://owm.gzhubu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zej.epnwcf.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://khb.gogol.net.cn

Ruby: // fork 块
来源：http://mnw.zhijiandao.cn

C#:   Parallel.For
来源：http://tzn.shuidangran.top

================================================================================
来源：http://hhq.daxiang520.top

P. 常用工具函数
来源：http://shm.chenjidiqi.icu

================================================================================
来源：http://buz.yanxiufei.cn

[P01] 生成 UUID
来源：http://rtf.zhiwuduotai.top

Py:   str(uuid.uuid4())
来源：http://uto.aizwys.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zpt.vehdjk.com

JS:   crypto.randomUUID()
来源：http://yhy.snrcjt.cn

TS:   crypto.randomUUID()
来源：http://fpl.dianchejie.cn

Java: UUID.randomUUID().toString()
来源：http://sur.hnqzz.top

Go:   // 用 github.com/google/uuid
来源：http://jod.52xcode.cn

Ruby: SecureRandom.uuid
来源：http://qip.havefunace.top

C#:   Guid.NewGuid().ToString()
来源：http://kfm.xingfuxueyuan.xyz

[P02] MD5 / SHA256 摘要
来源：http://dmz.jinghuilouyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://heu.cucudq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zgd.dashuyun.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://esi.shuidangran.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pcq.daxiang520.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zkf.gaohongyu789.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dgv.dashuyun.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qyf.ctjpmb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vff.pengpengdd.cyou

[P03] 生成短随机字符串
来源：http://vne.yongpay.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ncj.mhx1999.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kqz.redwolf501.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://huf.yongpay.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fgy.nwbrower.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://caw.hywenlv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jel.uphjek.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://xht.zycfv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lix.jinqigfzy.top

[P04] 求长度
来源：http://cpt.yueranfly.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://upy.xinyue.icu

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sot.vqdsnc.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gcg.hnxiangtu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hrh.cdnleiting.top

Java: list.size();  map.size();  s.length()
来源：http://czt.ctjpmb.com

Go:   len(arr);  len(m)
来源：http://gvp.gotoacloud.top

Ruby: x.length;  x.size
来源：http://xdp.sweek.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rwy.nanxuanxn.top

[P05] 判断两个对象内容是否相等
来源：http://hsq.zhengqikj.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ljc.svipenyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zke.fengsongda.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tig.sweek.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fky.gzhubu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://anj.nanxinkj.top

Go:   reflect.DeepEqual(a, b)
来源：http://qiy.aizwys.cn

Ruby: a == b
来源：http://eeo.fengsongda.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zbb.zhixingplan.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://smr.sysykeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mbx.52xcode.cn

PHP:  if (empty($x)) {}
来源：http://ltd.0kj1m.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pmq.zhongyouzk.top

TS:   if (x == null) {}
来源：http://hfh.bbcook.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://skj.guannengcc.top

Go:   if x == nil {}
来源：http://bvp.chenjidiqi.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mhu.hammf.cn

C#:   if (x is null) {}
来源：http://kul.shangyingyoupin.top

[P07] 防抖与节流
来源：http://fgw.chenlongwang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ayn.fehbvm.com

PHP:  // 手写时间戳比较
来源：http://dfs.sufxvd.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jos.yj202588.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://byv.iojbl.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://onq.chenjidiqi.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ycb.nanxuanxn.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://enf.hysaishi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lun.dashuyun.cn

[P08] 处理浮点精度问题
来源：http://rij.pengpengdd.cyou

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xyn.nanxuanxn.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nxy.yangfankeji.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rgo.hnqzz.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xua.quarkkingdee.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://srd.hnxiangtu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qaz.fengsongda.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tru.feifeiyinyue.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://occ.nanxinkj.top

================================================================================
来源：http://tds.xuanzx.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ogk.jinqigufen.top

================================================================================
来源：http://fro.52xcode.cn

[Q01] 创建表
来源：http://dxh.yueranfly.top

CREATE TABLE users (
来源：http://bbp.meibo888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jdh.ybcxt.top

name VARCHAR(50) NOT NULL,
来源：http://gxl.cucudq.cn

email VARCHAR(100) UNIQUE,
来源：http://xqg.xuanzx.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ylm.vehdjk.com

);
来源：http://xsb.redwolf501.top

[Q02] 创建带外键的表
来源：http://cnq.yj20258888.top

CREATE TABLE orders (
来源：http://vkn.xziqi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yvh.zdqjudy.top

user_id INT NOT NULL,
来源：http://pbx.chenlongwang.top

amount DECIMAL(10, 2),
来源：http://lfu.bbcook.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vnx.fzhhl.top

);
来源：http://rug.jinyuanbaomall.cn

[Q03] 增加列
来源：http://vth.yuxming.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mvw.meibo888.top

[Q04] 修改列类型
来源：http://qcv.ctjpmb.com


<!-- 参考信息 -->