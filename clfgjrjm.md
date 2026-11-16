代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://mwv.ybcxt.top

[M05] 设置退出码
来源：http://nxe.hcnkem.com

Py:   sys.exit(1)
来源：http://zdl.birdmap.top

PHP:  exit(1);
来源：http://nkv.chenlongwang.top

JS:   process.exit(1)
来源：http://dmo.c1oappe.top

TS:   process.exit(1)
来源：http://cnk.chenzaomai.com

Java: System.exit(1)
来源：http://ppm.tarul.cn

Go:   os.Exit(1)
来源：http://bjj.wangdashe.top

Ruby: exit 1
来源：http://lfd.guowangkeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tid.hesvh.cn

[M06] 向标准错误输出
来源：http://jtg.jiagoushi.top

Py:   print("err", file=sys.stderr)
来源：http://vmb.cheryme.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rio.dianchejie.cn

JS:   console.error("err")
来源：http://ryx.hfpthk.cn

TS:   console.error("err")
来源：http://ocw.yj202588.top

Java: System.err.println("err")
来源：http://jxl.shanyushiyangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nzj.zhixingplan.top

Ruby: warn "err"
来源：http://ryg.aizwys.cn

C#:   Console.Error.WriteLine("err")
来源：http://whl.yj20258.top

[M07] 判断是否为主入口
来源：http://svh.jinqigufen.top

Py:   if __name__ == "__main__":
来源：http://pgi.fehbvm.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://flf.cqqwz.cn

JS:   require.main === module
来源：http://akt.hysaishi.cn

TS:   require.main === module
来源：http://xbf.vqdsnc.cn

Java: public static void main(String[] args)
来源：http://ump.hnqzz.top

Go:   func main()
来源：http://imt.zdqjudy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://caj.yueranfly.top

C#:   static void Main(string[] args)
来源：http://emt.jiagoushi.top

[M08] 获取系统与运行时信息
来源：http://jru.jqgufenzy.top

Py:   platform.system();  platform.python_version()
来源：http://xzx.ppjwa.cn

PHP:  PHP_OS;  phpversion();
来源：http://kvk.haohaochexian.top

JS:   process.platform;  process.version
来源：http://fop.aibaodan.cn

TS:   process.platform;  process.version
来源：http://jts.yfazqb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qzg.chenlongwang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://jsk.cheryme.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lgc.yanxiufei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gbq.ppjwa.cn

================================================================================
来源：http://jwg.sxryk.cn

N. 数据结构与算法
来源：http://ftp.chenzaomai.com

================================================================================
来源：http://uzv.hnxiangtu.top

[N01] 二分查找（有序数组）
来源：http://ihq.c1oappe.top

Py:   bisect.bisect_left(arr, x)
来源：http://shi.fehbvm.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bae.ybcxt.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jji.pengpengdd.cyou

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://amz.ybcxt.top

Java: Arrays.binarySearch(arr, x)
来源：http://ntu.gaohongyu789.top

Go:   sort.SearchInts(arr, x)
来源：http://lsh.cdnleiting.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ziq.hesvh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zmz.gogol.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://xsg.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://prg.yongpay.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xke.fzhhl.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nvv.xuanzx.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://xzx.wangshuangyany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zti.yueranfly.top

Go:   slices.Sort(arr)
来源：http://apd.shuidangran.top

Ruby: arr.sort
来源：http://vlp.yj202588.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://bbe.yangfankeji.com

[N03] 快速排序（分治示例）
来源：http://zat.chenzaomai.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vds.dashuyun.cn

PHP:  // 递归实现，或用 usort
来源：http://hou.jinqigufen.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zgm.sxryk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dou.zhiwuduotai.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rxr.cdnleiting.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mmu.sjlbkw.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mvb.smart0.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://htf.shanyushiyangtech.top

[N04] 斐波那契数列
来源：http://mxg.tanke756.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zxq.epnwcf.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fhu.jyoumei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hoi.zhiwuduotai.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tyy.yuanzhike.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gmu.xuetiantiany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sxf.dianchejie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bgl.hywenlv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://inf.kuanghao11.cn

[N05] 最大公约数
来源：http://xwl.mhx1999.top

Py:   math.gcd(a, b)
来源：http://kvl.xuanzx.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mft.fzhhl.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oij.vqdsnc.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pzo.birdmap.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://imc.cdnleiting.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jbd.ivvv.top

Ruby: a.gcd(b)
来源：http://ygr.zhongyouzk.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aeh.xinyue.icu

[N06] 判断回文字符串
来源：http://seu.316326.xyz

Py:   s == s[::-1]
来源：http://iem.fktsv.cn

PHP:  $s === strrev($s);
来源：http://sdi.tianlin.xyz

JS:   s === [...s].reverse().join("")
来源：http://vxy.nanxinkj.top

TS:   s === [...s].reverse().join("")
来源：http://zhp.hammf.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cuh.yj202588.top

Go:   // 双指针从两端比较
来源：http://hlp.jinyuanbaomall.cn

Ruby: s == s.reverse
来源：http://yda.dianchejie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pfb.chenlongwang.top

[N07] 两数之和（返回下标）
来源：http://uxu.jinyuanbaomall.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pzv.yvedp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hrz.bbcook.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://csj.jinqigufen.top

TS:   // 手写 Map<string, number>
来源：http://pdm.nanxuanxn.top

Java: // 手写 HashMap
来源：http://yex.316326.xyz

Go:   // 手写 map[int]int
来源：http://epj.redwolf501.top

Ruby: // 手写 Hash
来源：http://sxt.aizwys.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cdq.dashuyun.cn

[N08] 生成全排列
来源：http://yuh.gaohongyu789.top

Py:   itertools.permutations(arr)
来源：http://tbo.zhijiandao.cn

PHP:  // 手写递归交换
来源：http://pxa.hnqzz.top

JS:   // 手写回溯递归
来源：http://zjt.yj20258.top

TS:   // 手写回溯递归
来源：http://tly.daria6918.cn

Java: // 手写回溯递归
来源：http://lzu.jinqigufen.top

Go:   // 手写回溯递归
来源：http://phx.shanyushiyangtech.top

Ruby: arr.permutation.to_a
来源：http://ovz.ivvv.top

C#:   // 手写回溯递归
来源：http://xzh.guowangkeji.top

[N09] 栈与队列
来源：http://ghw.xylfe.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://alu.quarkkingdee.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jrh.uphjek.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nnl.iojbl.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qmf.zhixingplan.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xca.fzhhl.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pco.zhaomingkeji.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nzb.gzhubu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eyp.nanxinkj.top

[N10] 链表节点定义
来源：http://dwx.shangyingyoupin.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uxv.shzxlz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dbk.ctjpmb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fhl.gaohongyu789.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://slw.ppjwa.cn

Java: class Node { int v; Node next; }
来源：http://xrc.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://wig.hcnkem.com

Ruby: Node = Struct.new(:v, :next)
来源：http://oaf.nanxinkj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://cau.ydzc1.top

[N11] 二叉树中序遍历
来源：http://xzw.havefunace.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oqb.bbcook.cn

PHP:  // 手写递归函数
来源：http://ydb.haohaochexian.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tvu.gzhubu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bsi.zdqjudy.top

Java: // 手写递归
来源：http://dos.ivvv.top

Go:   // 手写递归
来源：http://pxj.hcnkem.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sgt.ctjpmb.com

C#:   // 手写递归
来源：http://zcm.redwolf501.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ebn.daxiang520.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jht.chenjidiqi.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bey.aizwys.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://axl.pengpengdd.cyou

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ujn.xinyue.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://epy.smart0.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qvv.cqqwz.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fvn.nwbrower.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pud.hnxiangtu.top

================================================================================
来源：http://mrq.yongpay.top

O. 并发与异步
来源：http://wjk.jiagoushi.top

================================================================================
来源：http://cdz.fanxiaobao.xyz

[O01] 启动一个线程
来源：http://rtd.daxiang520.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nsq.zhoulong.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hhy.kuanghao11.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fud.tian-w.cn

TS:   // 同 JS
来源：http://xko.yj20258888.top

Java: new Thread(() -> f()).start()
来源：http://ihm.yuanzhike.top

Go:   go f()
来源：http://fkr.sxryk.cn

Ruby: Thread.new { f }
来源：http://sfv.snrcjt.cn

C#:   Task.Run(() => F());
来源：http://smx.ydjk.org.cn

[O02] 使用线程池
来源：http://drn.yueranfly.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gvp.sweek.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oly.ctjpmb.com

JS:   // worker_threads 线程池
来源：http://aqt.yanxiufei.cn

TS:   // worker_threads 线程池
来源：http://gww.uphjek.com

Java: Executors.newFixedThreadPool(4)
来源：http://jov.yfazqb.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ont.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oyn.hesvh.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xgq.gaohongyu789.top

[O03] 加锁保护共享数据
来源：http://dix.ydzc1.top

Py:   with lock: shared += 1
来源：http://lou.xingfuxueyuan.xyz

PHP:  // 用 flock() 做文件锁
来源：http://ptq.xuanzx.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vii.xuetiantiany.cn

TS:   // 同 JS
来源：http://ehk.vehdjk.com

Java: synchronized (this) { shared++; }
来源：http://rkr.shanyushiyangtech.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://edt.ppjwa.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sdx.yueranfly.top

C#:   lock (gate) { shared++; }
来源：http://flr.fehbvm.com

[O04] 定义异步函数并等待
来源：http://ypr.fehbvm.com

Py:   async def f():⏎    await g()
来源：http://plu.hesvh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jvi.zdbjq.cn

JS:   async function f() { await g(); }
来源：http://iiz.andypj.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://kyv.bbcook.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ycn.andypj.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jto.zhiwuduotai.top

Ruby: # 用 Fiber 或 async gem
来源：http://mjx.shanyushiyangtech.top

C#:   async Task F() { await G(); }
来源：http://rvp.hnqzz.top

[O05] 并发执行并等待全部完成
来源：http://lcl.haohaochexian.top

Py:   asyncio.gather(*tasks)
来源：http://ghh.fzhhl.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vac.yanxiufei.cn

JS:   await Promise.all(tasks)
来源：http://yvz.ivvv.top

TS:   await Promise.all(tasks)
来源：http://qrj.ybcxt.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ifq.c1oappe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qdm.pycfn.com

Ruby: threads.map(&:join)
来源：http://lvp.hfpthk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ckl.tarul.cn

[O06] 使用进程池
来源：http://cux.yj20258888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rdm.ehwqpu.com

PHP:  // pcntl_fork 或多进程队列
来源：http://pfb.bbcook.cn

JS:   // child_process / cluster 模块
来源：http://gml.zhongyouzk.top

TS:   // child_process / cluster 模块
来源：http://utu.smart0.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uql.cheryme.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eqp.cqqwz.cn

Ruby: // fork 块
来源：http://hrt.yongpay.top

C#:   Parallel.For
来源：http://ljn.vehdjk.com

================================================================================
来源：http://gph.zhixingplan.top

P. 常用工具函数
来源：http://opf.svipenyu.cn

================================================================================
来源：http://fgz.hysaishi.cn

[P01] 生成 UUID
来源：http://ytd.shanyushiyangtech.top

Py:   str(uuid.uuid4())
来源：http://qhr.cqqwz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xry.jinyuanbaomall.cn

JS:   crypto.randomUUID()
来源：http://pnr.cqqwz.cn

TS:   crypto.randomUUID()
来源：http://ozm.jiagoushi.top

Java: UUID.randomUUID().toString()
来源：http://fkn.hcnkem.com

Go:   // 用 github.com/google/uuid
来源：http://vzx.fzhhl.top

Ruby: SecureRandom.uuid
来源：http://epn.jyoumei.cn

C#:   Guid.NewGuid().ToString()
来源：http://ibe.hongshengwenyu.top

[P02] MD5 / SHA256 摘要
来源：http://sqq.ybcxt.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yid.ctjpmb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://poc.zhixingplan.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://anv.tarul.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xbr.zhoulong.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mcx.aibaodan.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fqr.shangyingyoupin.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://eom.fktsv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jbl.fehbvm.com

[P03] 生成短随机字符串
来源：http://bmt.jqgfzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rwx.yvedp.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://adn.hongshengwenyu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://biq.shanyushiyangtech.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://klp.xziqi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bgh.bjfxy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rfr.guannengcc.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xqs.zdbjq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cvc.jinqigufen.top

[P04] 求长度
来源：http://jcf.chenlongwang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yfy.zdqjudy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vcg.meibo888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ynu.yanxiufei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jke.pengpengdd.cyou

Java: list.size();  map.size();  s.length()
来源：http://plw.ctjpmb.com

Go:   len(arr);  len(m)
来源：http://nkx.ywan-chungtsiang.top

Ruby: x.length;  x.size
来源：http://gin.zhoulong.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://udy.zhengqikj.top

[P05] 判断两个对象内容是否相等
来源：http://fzs.sweek.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zrt.gzhubu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dbi.chenjidiqi.icu

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dtz.hnqzz.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xen.cucudq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vcm.xuanzx.com

Go:   reflect.DeepEqual(a, b)
来源：http://tnx.jqgfzy.top

Ruby: a == b
来源：http://adn.yangfankeji.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nkr.fehbvm.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://che.xylfe.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vjq.quarkkingdee.top

PHP:  if (empty($x)) {}
来源：http://yvu.vehdjk.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dox.xziqi.cn

TS:   if (x == null) {}
来源：http://ixe.zhiwuduotai.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ymd.fanxiaobao.xyz

Go:   if x == nil {}
来源：http://ogy.sjlbkw.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://upj.jqgfzy.top

C#:   if (x is null) {}
来源：http://rjn.hammf.cn

[P07] 防抖与节流
来源：http://jsx.hammf.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rve.hesvh.cn

PHP:  // 手写时间戳比较
来源：http://lua.yj20258.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ynu.chenzaomai.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jsb.shanyushiyangtech.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pls.yuxming.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jte.sjlbkw.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ilq.jlsjyb.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vab.nwbrower.top

[P08] 处理浮点精度问题
来源：http://qzr.ctjpmb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vkg.ivvv.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rpq.jinghuilouyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qup.sysykeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wbz.andypj.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://alv.yuanzhike.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uas.dianchejie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hhl.yongpay.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jdy.xingfuxueyuan.xyz

================================================================================
来源：http://pcf.yj20258.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vqm.snrcjt.cn

================================================================================
来源：http://ooc.shangyingyoupin.top

[Q01] 创建表
来源：http://och.daria6918.cn

CREATE TABLE users (
来源：http://sdu.cashguo.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jfx.hnxiangtu.top

name VARCHAR(50) NOT NULL,
来源：http://rwy.sjlbkw.cn

email VARCHAR(100) UNIQUE,
来源：http://avr.jinghuilouyu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xtx.nanxinkj.top

);
来源：http://rkr.snrcjt.cn

[Q02] 创建带外键的表
来源：http://ycx.316326.xyz

CREATE TABLE orders (
来源：http://xsy.9152youxi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nhd.c1oappe.top

user_id INT NOT NULL,
来源：http://lje.sufxvd.cn

amount DECIMAL(10, 2),
来源：http://vit.jinyuanbaomall.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vwy.yongpay.top

);
来源：http://yxk.smart0.xyz

[Q03] 增加列
来源：http://icz.gogol.net.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oeb.yangfankeji.com

[Q04] 修改列类型
来源：http://pgr.xylfe.cn


<!-- 参考信息 -->