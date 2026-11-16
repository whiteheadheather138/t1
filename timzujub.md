代发 wailian999

Ruby: exit 1
来源：http://fap.ydzc1.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vwc.hcnkem.com

[M06] 向标准错误输出
来源：http://ouz.hammf.cn

Py:   print("err", file=sys.stderr)
来源：http://inr.ydzc1.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lzo.vqdsnc.cn

JS:   console.error("err")
来源：http://not.fzhhl.top

TS:   console.error("err")
来源：http://dvc.jiagoushi.top

Java: System.err.println("err")
来源：http://yhi.svipenyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://irl.wangdashe.top

Ruby: warn "err"
来源：http://btb.jinyuanbaomall.cn

C#:   Console.Error.WriteLine("err")
来源：http://sry.hywenlv.cn

[M07] 判断是否为主入口
来源：http://dtt.zhengqikj.top

Py:   if __name__ == "__main__":
来源：http://dcr.zhengqikj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fox.sjlbkw.cn

JS:   require.main === module
来源：http://akc.fanxiaobao.xyz

TS:   require.main === module
来源：http://ffq.yuxming.cn

Java: public static void main(String[] args)
来源：http://xmd.yj20258.top

Go:   func main()
来源：http://xgq.zhixingplan.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ewt.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://giq.jinqigufen.top

[M08] 获取系统与运行时信息
来源：http://zqo.feifeiyinyue.top

Py:   platform.system();  platform.python_version()
来源：http://gup.ctjpmb.com

PHP:  PHP_OS;  phpversion();
来源：http://sij.shzxlz.cn

JS:   process.platform;  process.version
来源：http://kbh.yangfankeji.com

TS:   process.platform;  process.version
来源：http://tpk.yangfankeji.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zps.fehbvm.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://jjs.vqdsnc.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://usn.cucudq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://irb.zhaomingkeji.xyz

================================================================================
来源：http://oqa.cqqwz.cn

N. 数据结构与算法
来源：http://fql.zhoulong.xyz

================================================================================
来源：http://qwi.ppjwa.cn

[N01] 二分查找（有序数组）
来源：http://iio.yj20258888.top

Py:   bisect.bisect_left(arr, x)
来源：http://vya.zycfv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mrp.xingfuxueyuan.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cvp.uphjek.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sbt.zhaomingkeji.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://ffw.316326.xyz

Go:   sort.SearchInts(arr, x)
来源：http://srq.fehbvm.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://sav.shangyingyoupin.top

C#:   Array.BinarySearch(arr, x)
来源：http://uyj.andypj.xyz

[N02] 排序（工程实践用内置实现）
来源：http://lie.shangyingyoupin.top

Py:   sorted(arr);  arr.sort()
来源：http://ikz.sweek.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wqk.nanxinkj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://dga.fanxiaobao.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://nbw.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://chm.ctjpmb.com

Go:   slices.Sort(arr)
来源：http://add.aizwys.cn

Ruby: arr.sort
来源：http://ydd.fzhhl.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jib.yueranfly.top

[N03] 快速排序（分治示例）
来源：http://arb.birdmap.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hgi.cashguo.top

PHP:  // 递归实现，或用 usort
来源：http://yfp.aibaodan.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jwr.tarul.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://axf.yanxiufei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xbo.ppjwa.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://idr.pycfn.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mua.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://csz.zhoulong.xyz

[N04] 斐波那契数列
来源：http://qcj.yuanzhike.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xnj.vehdjk.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lxd.smart0.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ljn.gzhubu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hvg.jinqigufen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zeo.hcnkem.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yel.vqdsnc.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rmz.jiagoushi.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fgc.guannengcc.top

[N05] 最大公约数
来源：http://fcc.tanke756.top

Py:   math.gcd(a, b)
来源：http://upa.shanyushiyangtech.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://sog.sjlbkw.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rdj.feifeiyinyue.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zvv.yuanzhike.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tqb.ydzc1.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kkj.sweek.top

Ruby: a.gcd(b)
来源：http://szh.hnxiangtu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://imt.ywan-chungtsiang.top

[N06] 判断回文字符串
来源：http://vxq.9152youxi.cn

Py:   s == s[::-1]
来源：http://zjy.feifeiyinyue.top

PHP:  $s === strrev($s);
来源：http://vnb.sufxvd.cn

JS:   s === [...s].reverse().join("")
来源：http://lvi.sufxvd.cn

TS:   s === [...s].reverse().join("")
来源：http://opq.guannengcc.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tmz.fengsongda.top

Go:   // 双指针从两端比较
来源：http://qjk.cqqwz.cn

Ruby: s == s.reverse
来源：http://hyi.xuanzx.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://kzl.nanxinkj.top

[N07] 两数之和（返回下标）
来源：http://gib.cdnleiting.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jrr.wangshuangyany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tua.yuanzhike.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kup.yongpay.top

TS:   // 手写 Map<string, number>
来源：http://oic.yuxming.cn

Java: // 手写 HashMap
来源：http://dzn.sweek.top

Go:   // 手写 map[int]int
来源：http://lti.chenlongwang.top

Ruby: // 手写 Hash
来源：http://zpp.zhiwuduotai.top

C#:   // 手写 Dictionary<int, int>
来源：http://gai.uphjek.com

[N08] 生成全排列
来源：http://bup.xingfuxueyuan.xyz

Py:   itertools.permutations(arr)
来源：http://qih.yj20258888.top

PHP:  // 手写递归交换
来源：http://ptt.gaohongyu789.top

JS:   // 手写回溯递归
来源：http://kwy.hywenlv.cn

TS:   // 手写回溯递归
来源：http://ugw.feifeiyinyue.top

Java: // 手写回溯递归
来源：http://arp.fanxiaobao.xyz

Go:   // 手写回溯递归
来源：http://oyb.ydzc1.top

Ruby: arr.permutation.to_a
来源：http://szi.dianchejie.cn

C#:   // 手写回溯递归
来源：http://kuc.yueranfly.top

[N09] 栈与队列
来源：http://itu.pycfn.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lbt.snrcjt.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://fno.yj20258.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vlx.hcnkem.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cni.dianchejie.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jbw.yfazqb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dls.yj20258888.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pqp.hfpthk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dxa.sxryk.cn

[N10] 链表节点定义
来源：http://aes.zycfv.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://edg.yfazqb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://rxj.tanke756.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ofr.yj20258.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ynw.gzhubu.top

Java: class Node { int v; Node next; }
来源：http://jjn.jianghu66.top

Go:   type Node struct { V int; Next *Node }
来源：http://wos.fanxiaobao.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://fzb.cdnleiting.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jyz.zhoulong.xyz

[N11] 二叉树中序遍历
来源：http://dbp.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aaz.aibaodan.cn

PHP:  // 手写递归函数
来源：http://hum.guowangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wjm.sufxvd.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zkb.cqqwz.cn

Java: // 手写递归
来源：http://ydu.kuanghao11.cn

Go:   // 手写递归
来源：http://yic.jqgfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ivo.hesvh.cn

C#:   // 手写递归
来源：http://bwg.daxiang520.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jac.cdnleiting.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tel.birdmap.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hzo.sufxvd.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wdx.bjfxy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cjn.fktsv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ndc.dashuyun.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sel.guowangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bmj.fzhhl.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uqr.mhx1999.top

================================================================================
来源：http://bzk.bjfxy.top

O. 并发与异步
来源：http://lqv.wangdashe.top

================================================================================
来源：http://trm.haohaochexian.top

[O01] 启动一个线程
来源：http://urc.gaohongyu789.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://det.aizwys.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gdl.zdbjq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qar.0kj1m.cn

TS:   // 同 JS
来源：http://sdh.ivvv.top

Java: new Thread(() -> f()).start()
来源：http://kjf.fengsongda.top

Go:   go f()
来源：http://btw.chenzaomai.com

Ruby: Thread.new { f }
来源：http://vdt.c1oappe.top

C#:   Task.Run(() => F());
来源：http://pen.andypj.xyz

[O02] 使用线程池
来源：http://xbt.nanxinkj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bwe.ybcxt.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nfu.hywenlv.cn

JS:   // worker_threads 线程池
来源：http://pmp.hesvh.cn

TS:   // worker_threads 线程池
来源：http://kbi.c1oappe.top

Java: Executors.newFixedThreadPool(4)
来源：http://wcm.ydzc1.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://obx.jyoumei.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://obo.cashguo.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fgn.chenlongwang.top

[O03] 加锁保护共享数据
来源：http://dza.andypj.xyz

Py:   with lock: shared += 1
来源：http://gcb.vqdsnc.cn

PHP:  // 用 flock() 做文件锁
来源：http://cak.zdqjudy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vvs.gogol.net.cn

TS:   // 同 JS
来源：http://ayr.xuetiantiany.cn

Java: synchronized (this) { shared++; }
来源：http://jne.guowangkeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sfd.zhaomingkeji.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://exe.0kj1m.cn

C#:   lock (gate) { shared++; }
来源：http://ljp.xingfuxueyuan.xyz

[O04] 定义异步函数并等待
来源：http://nyd.gzhubu.top

Py:   async def f():⏎    await g()
来源：http://fos.yanxiufei.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://exo.hfpthk.cn

JS:   async function f() { await g(); }
来源：http://eff.zycfv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mev.jinqigfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://upw.cheryme.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hrt.snrcjt.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ymf.jinyuanbaomall.cn

C#:   async Task F() { await G(); }
来源：http://jjo.pycfn.com

[O05] 并发执行并等待全部完成
来源：http://bjp.aizwys.cn

Py:   asyncio.gather(*tasks)
来源：http://sji.birdmap.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ucl.9152youxi.cn

JS:   await Promise.all(tasks)
来源：http://dqf.bbcook.cn

TS:   await Promise.all(tasks)
来源：http://skq.gaohongyu789.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://axh.yj20258.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kdj.0kj1m.cn

Ruby: threads.map(&:join)
来源：http://kyj.zhixingplan.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xfb.hammf.cn

[O06] 使用进程池
来源：http://uoa.daria6918.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sgq.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wuv.wangshuangyany.cn

JS:   // child_process / cluster 模块
来源：http://hfv.52xcode.cn

TS:   // child_process / cluster 模块
来源：http://fpc.mhx1999.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rzk.cucudq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://szw.zhengqikj.top

Ruby: // fork 块
来源：http://rhe.zhiwuduotai.top

C#:   Parallel.For
来源：http://ftt.jyoumei.cn

================================================================================
来源：http://xcz.vehdjk.com

P. 常用工具函数
来源：http://wqm.nwbrower.top

================================================================================
来源：http://qgx.zdbjq.cn

[P01] 生成 UUID
来源：http://erj.52xcode.cn

Py:   str(uuid.uuid4())
来源：http://uyv.jyoumei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hjg.shanyushiyangtech.top

JS:   crypto.randomUUID()
来源：http://bif.vqdsnc.cn

TS:   crypto.randomUUID()
来源：http://crc.pengpengdd.cyou

Java: UUID.randomUUID().toString()
来源：http://qdk.fanxiaobao.xyz

Go:   // 用 github.com/google/uuid
来源：http://xso.zdbjq.cn

Ruby: SecureRandom.uuid
来源：http://abk.jiagoushi.top

C#:   Guid.NewGuid().ToString()
来源：http://cif.sysykeji.top

[P02] MD5 / SHA256 摘要
来源：http://ztp.316326.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mxs.hongshengwenyu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dto.wangdashe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://whl.xziqi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jvq.0kj1m.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zum.sufxvd.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ydi.fehbvm.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fbj.sjlbkw.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://asc.shzxlz.cn

[P03] 生成短随机字符串
来源：http://qnt.gotoacloud.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hpy.cheryme.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kjk.smart0.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kww.tian-w.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dxs.hcnkem.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gfk.hongshengwenyu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://coz.xuetiantiany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nfh.iojbl.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://znl.tarul.cn

[P04] 求长度
来源：http://kwe.chenlongwang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cpx.snrcjt.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kur.jiagoushi.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uxx.gzhubu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mix.cucudq.cn

Java: list.size();  map.size();  s.length()
来源：http://nyx.chenjidiqi.icu

Go:   len(arr);  len(m)
来源：http://aqd.birdmap.top

Ruby: x.length;  x.size
来源：http://lgw.sysykeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jbl.ctjpmb.com

[P05] 判断两个对象内容是否相等
来源：http://cmr.hcnkem.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://wgc.meibo888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dwb.bjfxy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vzb.ppjwa.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vxt.yuxming.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://juk.andypj.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://mcy.fanxiaobao.xyz

Ruby: a == b
来源：http://gom.redwolf501.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://opx.shzxlz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qvf.zhongyouzk.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aby.ybcxt.top

PHP:  if (empty($x)) {}
来源：http://wqw.jianghu66.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bqz.bjfxy.top

TS:   if (x == null) {}
来源：http://lbi.chenlongwang.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ody.zycfv.cn

Go:   if x == nil {}
来源：http://guf.guowangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://boq.tianlin.xyz

C#:   if (x is null) {}
来源：http://mdo.sysykeji.top

[P07] 防抖与节流
来源：http://nux.xuetiantiany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fee.shanyushiyangtech.top

PHP:  // 手写时间戳比较
来源：http://wim.ybcxt.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tml.yfazqb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sxk.yuxming.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cty.hongshengwenyu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://trs.xziqi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zmh.vqdsnc.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ert.birdmap.top

[P08] 处理浮点精度问题
来源：http://sps.wangshuangyany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://efn.hcnkem.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mqe.gaohongyu789.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bmz.kuanghao11.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dob.epnwcf.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dqu.jianghu66.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tdw.nwbrower.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pti.mhx1999.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rmm.c1oappe.top

================================================================================
来源：http://mdu.cqqwz.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rqh.cucudq.cn

================================================================================
来源：http://qqj.gaohongyu789.top

[Q01] 创建表
来源：http://goc.yj20258888.top

CREATE TABLE users (
来源：http://mxn.zhixingplan.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gry.shanyushiyangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://msi.zhiwuduotai.top

email VARCHAR(100) UNIQUE,
来源：http://lbx.cheryme.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uex.jqgufenzy.top

);
来源：http://rqc.fengsongda.top

[Q02] 创建带外键的表
来源：http://itv.9152youxi.cn

CREATE TABLE orders (
来源：http://zxr.zhixingplan.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hep.tanke756.top

user_id INT NOT NULL,
来源：http://qct.zhixingplan.top

amount DECIMAL(10, 2),
来源：http://zpu.0kj1m.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qvw.zdqjudy.top

);
来源：http://cwv.316326.xyz

[Q03] 增加列
来源：http://fwe.tanke756.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cbo.gogol.net.cn

[Q04] 修改列类型
来源：http://dnv.fzhhl.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rsh.fengsongda.top

[Q05] 重命名列
来源：http://bbl.hywenlv.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bhv.dianchejie.cn

[Q06] 删除列
来源：http://lfu.feifeiyinyue.top

ALTER TABLE users DROP COLUMN age;
来源：http://txy.hongshengwenyu.top

[Q07] 删除表
来源：http://nku.yj202588.top

DROP TABLE IF EXISTS orders;
来源：http://uqu.ywan-chungtsiang.top

[Q08] 创建普通索引
来源：http://why.xylfe.cn


<!-- 参考信息 -->