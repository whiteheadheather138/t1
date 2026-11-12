代发 wailian999

JS:   process.exit(1)
来源：http://zsd.ctjpmb.com

TS:   process.exit(1)
来源：http://amp.dashuyun.cn

Java: System.exit(1)
来源：http://pvj.ehwqpu.com

Go:   os.Exit(1)
来源：http://doy.aibaodan.cn

Ruby: exit 1
来源：http://exx.cucudq.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nyt.yj202588.top

[M06] 向标准错误输出
来源：http://fpi.yj202588.top

Py:   print("err", file=sys.stderr)
来源：http://lir.ybcxt.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gub.sweek.top

JS:   console.error("err")
来源：http://jom.bbcook.cn

TS:   console.error("err")
来源：http://sqn.yueranfly.top

Java: System.err.println("err")
来源：http://leu.bbcook.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jbm.shangyingyoupin.top

Ruby: warn "err"
来源：http://guj.hammf.cn

C#:   Console.Error.WriteLine("err")
来源：http://zvv.jianghu66.top

[M07] 判断是否为主入口
来源：http://jfq.jyoumei.cn

Py:   if __name__ == "__main__":
来源：http://vmr.tianlin.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mhx.uphjek.com

JS:   require.main === module
来源：http://mqt.hnqzz.top

TS:   require.main === module
来源：http://zcc.chenjidiqi.icu

Java: public static void main(String[] args)
来源：http://rvf.wangdashe.top

Go:   func main()
来源：http://jyb.yueranfly.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pfm.ydjk.org.cn

C#:   static void Main(string[] args)
来源：http://dbl.xuanzx.com

[M08] 获取系统与运行时信息
来源：http://qhi.hysaishi.cn

Py:   platform.system();  platform.python_version()
来源：http://hgh.52xcode.cn

PHP:  PHP_OS;  phpversion();
来源：http://efl.quarkkingdee.top

JS:   process.platform;  process.version
来源：http://tqu.jinyuanbaomall.cn

TS:   process.platform;  process.version
来源：http://mia.yvedp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yjz.hcnkem.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://vyo.zycfv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vkv.sjlbkw.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://loz.zhengqikj.top

================================================================================
来源：http://ekx.sxryk.cn

N. 数据结构与算法
来源：http://emz.haohaochexian.top

================================================================================
来源：http://mko.vehdjk.com

[N01] 二分查找（有序数组）
来源：http://blo.hnqzz.top

Py:   bisect.bisect_left(arr, x)
来源：http://pyl.jinqigfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jdj.xylfe.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qtk.ehwqpu.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vam.jinyuanbaomall.cn

Java: Arrays.binarySearch(arr, x)
来源：http://emk.c1oappe.top

Go:   sort.SearchInts(arr, x)
来源：http://mut.yuanzhike.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jgg.ybcxt.top

C#:   Array.BinarySearch(arr, x)
来源：http://gje.xylfe.cn

[N02] 排序（工程实践用内置实现）
来源：http://byx.sufxvd.cn

Py:   sorted(arr);  arr.sort()
来源：http://qys.chenlongwang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://chu.jyoumei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ubz.hysaishi.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fup.fehbvm.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://atr.xuanzx.com

Go:   slices.Sort(arr)
来源：http://bdr.yongpay.top

Ruby: arr.sort
来源：http://juv.zhongyouzk.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://exd.xylfe.cn

[N03] 快速排序（分治示例）
来源：http://cim.kuanghao11.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zjo.jianghu66.top

PHP:  // 递归实现，或用 usort
来源：http://hse.yfazqb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fje.xziqi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gyv.c1oappe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tkk.shanyushiyangtech.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lbo.cucudq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://aue.snrcjt.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tec.jinqigufen.top

[N04] 斐波那契数列
来源：http://thc.xuetiantiany.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mih.ydjk.org.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zwq.zhixingplan.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hbi.iojbl.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oox.yuanzhike.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mcr.jqgufenzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mtm.316326.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hoq.zhongyouzk.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ylm.meibo888.top

[N05] 最大公约数
来源：http://vdx.yj20258.top

Py:   math.gcd(a, b)
来源：http://zgw.sjlbkw.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zxd.yangfankeji.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pce.xuetiantiany.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jzh.iojbl.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fkr.shuidangran.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://eio.jinqigufen.top

Ruby: a.gcd(b)
来源：http://ldb.shzxlz.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jsv.zdbjq.cn

[N06] 判断回文字符串
来源：http://dli.yvedp.cn

Py:   s == s[::-1]
来源：http://qjr.zhongyouzk.top

PHP:  $s === strrev($s);
来源：http://xfb.jinghuilouyu.cn

JS:   s === [...s].reverse().join("")
来源：http://rdf.bbcook.cn

TS:   s === [...s].reverse().join("")
来源：http://kqx.daxiang520.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kip.aizwys.cn

Go:   // 双指针从两端比较
来源：http://rzp.yanxiufei.cn

Ruby: s == s.reverse
来源：http://cgy.vehdjk.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://psf.guannengcc.top

[N07] 两数之和（返回下标）
来源：http://xeb.yanxiufei.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tqf.pengpengdd.cyou

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kxe.tarul.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qra.zdbjq.cn

TS:   // 手写 Map<string, number>
来源：http://ngv.jinqigufen.top

Java: // 手写 HashMap
来源：http://gqo.havefunace.top

Go:   // 手写 map[int]int
来源：http://jvg.tarul.cn

Ruby: // 手写 Hash
来源：http://gib.hnxiangtu.top

C#:   // 手写 Dictionary<int, int>
来源：http://uht.c1oappe.top

[N08] 生成全排列
来源：http://qhp.ywan-chungtsiang.top

Py:   itertools.permutations(arr)
来源：http://lbi.mhx1999.top

PHP:  // 手写递归交换
来源：http://nki.9152youxi.cn

JS:   // 手写回溯递归
来源：http://zib.zdbjq.cn

TS:   // 手写回溯递归
来源：http://mtx.svipenyu.cn

Java: // 手写回溯递归
来源：http://kok.sysykeji.top

Go:   // 手写回溯递归
来源：http://wtb.hcnkem.com

Ruby: arr.permutation.to_a
来源：http://hpt.xziqi.cn

C#:   // 手写回溯递归
来源：http://xhb.gogol.net.cn

[N09] 栈与队列
来源：http://max.aizwys.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bcx.zhoulong.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zif.haohaochexian.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uqy.uphjek.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://irh.cheryme.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kkb.pycfn.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cbr.havefunace.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rho.sxryk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qpp.sweek.top

[N10] 链表节点定义
来源：http://wts.ctjpmb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ejm.yuxming.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://elo.andypj.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dce.zhengqikj.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://imf.xylfe.cn

Java: class Node { int v; Node next; }
来源：http://nar.tarul.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vpg.yongpay.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ehl.zhongyouzk.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xre.jiagoushi.top

[N11] 二叉树中序遍历
来源：http://lei.yj20258.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ovg.vqdsnc.cn

PHP:  // 手写递归函数
来源：http://iem.tian-w.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ktk.svipenyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zcj.meibo888.top

Java: // 手写递归
来源：http://uqg.ppjwa.cn

Go:   // 手写递归
来源：http://goc.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yxy.aibaodan.cn

C#:   // 手写递归
来源：http://egw.316326.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vzj.jianghu66.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nys.gzhubu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yfn.tianlin.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cab.guowangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gjs.jqgfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qix.xinyue.icu

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yjk.jqgfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yli.zhengqikj.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://krl.hnxiangtu.top

================================================================================
来源：http://xcu.yj20258888.top

O. 并发与异步
来源：http://yhq.jinqigfzy.top

================================================================================
来源：http://oqk.yfazqb.com

[O01] 启动一个线程
来源：http://cwq.zycfv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vrq.yuanzhike.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ncv.fktsv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://syv.tianlin.xyz

TS:   // 同 JS
来源：http://qjv.xinyue.icu

Java: new Thread(() -> f()).start()
来源：http://hgi.shuidangran.top

Go:   go f()
来源：http://qtq.jqgfzy.top

Ruby: Thread.new { f }
来源：http://wtg.gzhubu.top

C#:   Task.Run(() => F());
来源：http://ody.gogol.net.cn

[O02] 使用线程池
来源：http://vpt.epnwcf.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ibq.redwolf501.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cnf.hammf.cn

JS:   // worker_threads 线程池
来源：http://vbx.ydjk.org.cn

TS:   // worker_threads 线程池
来源：http://wog.hywenlv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://psl.gotoacloud.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fvt.xuanzx.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pap.ywan-chungtsiang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gkg.wangdashe.top

[O03] 加锁保护共享数据
来源：http://cji.tianlin.xyz

Py:   with lock: shared += 1
来源：http://qhg.jlsjyb.cn

PHP:  // 用 flock() 做文件锁
来源：http://aor.xuetiantiany.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ese.bjfxy.top

TS:   // 同 JS
来源：http://xfi.uphjek.com

Java: synchronized (this) { shared++; }
来源：http://dyo.hnqzz.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qar.dashuyun.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ivo.pycfn.com

C#:   lock (gate) { shared++; }
来源：http://oii.havefunace.top

[O04] 定义异步函数并等待
来源：http://yvc.hnqzz.top

Py:   async def f():⏎    await g()
来源：http://esg.xylfe.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fyg.fzhhl.top

JS:   async function f() { await g(); }
来源：http://xkt.daxiang520.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://sfz.xuetiantiany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://evg.dianchejie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zpy.jiagoushi.top

Ruby: # 用 Fiber 或 async gem
来源：http://xsd.jinqigfzy.top

C#:   async Task F() { await G(); }
来源：http://lno.zdqjudy.top

[O05] 并发执行并等待全部完成
来源：http://wcu.yanxiufei.cn

Py:   asyncio.gather(*tasks)
来源：http://zny.vqdsnc.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tvn.aizwys.cn

JS:   await Promise.all(tasks)
来源：http://ute.nanxuanxn.top

TS:   await Promise.all(tasks)
来源：http://dfi.fanxiaobao.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gga.ybcxt.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jdr.ehwqpu.com

Ruby: threads.map(&:join)
来源：http://dar.mhx1999.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wry.yfazqb.com

[O06] 使用进程池
来源：http://dlf.haohaochexian.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uby.nanxinkj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://rzv.fanxiaobao.xyz

JS:   // child_process / cluster 模块
来源：http://dgg.jlsjyb.cn

TS:   // child_process / cluster 模块
来源：http://bcz.gogol.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tnp.yj20258.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uty.yj20258.top

Ruby: // fork 块
来源：http://lhn.fengsongda.top

C#:   Parallel.For
来源：http://udp.pycfn.com

================================================================================
来源：http://jgj.cucudq.cn

P. 常用工具函数
来源：http://zut.bbcook.cn

================================================================================
来源：http://cme.fktsv.cn

[P01] 生成 UUID
来源：http://xnm.shzxlz.cn

Py:   str(uuid.uuid4())
来源：http://jmz.iojbl.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://noe.fktsv.cn

JS:   crypto.randomUUID()
来源：http://knd.havefunace.top

TS:   crypto.randomUUID()
来源：http://vbr.zhengqikj.top

Java: UUID.randomUUID().toString()
来源：http://jnc.zdbjq.cn

Go:   // 用 github.com/google/uuid
来源：http://yxz.uphjek.com

Ruby: SecureRandom.uuid
来源：http://icm.birdmap.top

C#:   Guid.NewGuid().ToString()
来源：http://kmh.zhiwuduotai.top

[P02] MD5 / SHA256 摘要
来源：http://nhb.haohaochexian.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ayu.9152youxi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uft.jyoumei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://iyg.fzhhl.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lng.yueranfly.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pbw.gotoacloud.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://skl.yfazqb.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://htm.yanxiufei.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ptc.xziqi.cn

[P03] 生成短随机字符串
来源：http://ufj.yuanzhike.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rbb.birdmap.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://svx.52xcode.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cyh.jlsjyb.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cka.316326.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cvi.cqqwz.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oxk.tanke756.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vwy.cdnleiting.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://izu.aizwys.cn

[P04] 求长度
来源：http://hip.guowangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ikm.jinqigfzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xdv.jinqigfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nfm.shangyingyoupin.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tgx.jlsjyb.cn

Java: list.size();  map.size();  s.length()
来源：http://qjc.kuanghao11.cn

Go:   len(arr);  len(m)
来源：http://yvc.yongpay.top

Ruby: x.length;  x.size
来源：http://gmd.jiagoushi.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ttt.cashguo.top

[P05] 判断两个对象内容是否相等
来源：http://tza.wangshuangyany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://awk.jqgfzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://taf.bbcook.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fql.snrcjt.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rzi.zhiwuduotai.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mrb.yonumen.top

Go:   reflect.DeepEqual(a, b)
来源：http://twr.sufxvd.cn

Ruby: a == b
来源：http://keg.fanxiaobao.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cgi.gotoacloud.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bih.fktsv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tkg.feifeiyinyue.top

PHP:  if (empty($x)) {}
来源：http://omj.hfpthk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gds.mhx1999.top

TS:   if (x == null) {}
来源：http://nts.zdbjq.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://glt.ehwqpu.com

Go:   if x == nil {}
来源：http://wfd.zhaomingkeji.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ecl.epnwcf.com

C#:   if (x is null) {}
来源：http://enx.fanxiaobao.xyz

[P07] 防抖与节流
来源：http://gco.xuanzx.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ikb.jqgfzy.top

PHP:  // 手写时间戳比较
来源：http://tws.jiagoushi.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jrl.fehbvm.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tra.havefunace.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ttt.svipenyu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wcw.sjlbkw.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://abe.daria6918.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oep.fanxiaobao.xyz

[P08] 处理浮点精度问题
来源：http://jfh.xuetiantiany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wix.gzhubu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ipg.yanxiufei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://upp.jqgufenzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vej.yuxming.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wev.birdmap.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fgd.mhx1999.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://abc.xingfuxueyuan.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jta.zhaomingkeji.xyz

================================================================================
来源：http://mbc.snrcjt.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ksq.nanxinkj.top

================================================================================
来源：http://rkk.ybcxt.top

[Q01] 创建表
来源：http://aka.bbcook.cn

CREATE TABLE users (
来源：http://mqa.nwbrower.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vjq.vqdsnc.cn

name VARCHAR(50) NOT NULL,
来源：http://rck.uphjek.com

email VARCHAR(100) UNIQUE,
来源：http://dcq.xinyue.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kqe.daria6918.cn

);
来源：http://tta.daxiang520.top

[Q02] 创建带外键的表
来源：http://njo.sweek.top

CREATE TABLE orders (
来源：http://lem.shangyingyoupin.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zpr.xziqi.cn

user_id INT NOT NULL,
来源：http://xxb.xuanzx.com

amount DECIMAL(10, 2),
来源：http://ndp.ydzc1.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qsq.daxiang520.top

);
来源：http://mjk.pengpengdd.cyou

[Q03] 增加列
来源：http://whj.havefunace.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jnw.xylfe.cn

[Q04] 修改列类型
来源：http://nmu.aizwys.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ssf.yfazqb.com

[Q05] 重命名列
来源：http://vvb.jinghuilouyu.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tqz.gotoacloud.top

[Q06] 删除列
来源：http://qvg.vehdjk.com


<!-- 参考信息 -->