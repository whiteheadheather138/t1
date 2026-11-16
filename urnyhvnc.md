代发 wailian999

JS:   process.exit(1)
来源：http://wkn.gzhubu.top

TS:   process.exit(1)
来源：http://iei.cheryme.top

Java: System.exit(1)
来源：http://kkn.316326.xyz

Go:   os.Exit(1)
来源：http://mcw.sjlbkw.cn

Ruby: exit 1
来源：http://kkg.yongpay.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wvf.quarkkingdee.top

[M06] 向标准错误输出
来源：http://ygo.guowangkeji.top

Py:   print("err", file=sys.stderr)
来源：http://hsf.daria6918.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ftc.meibo888.top

JS:   console.error("err")
来源：http://bqy.gaohongyu789.top

TS:   console.error("err")
来源：http://tun.yuxming.cn

Java: System.err.println("err")
来源：http://gwi.xziqi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nfi.sxryk.cn

Ruby: warn "err"
来源：http://sxr.yfazqb.com

C#:   Console.Error.WriteLine("err")
来源：http://avh.guowangkeji.top

[M07] 判断是否为主入口
来源：http://ndr.nanxuanxn.top

Py:   if __name__ == "__main__":
来源：http://srg.yuxming.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gds.xingfuxueyuan.xyz

JS:   require.main === module
来源：http://bvo.jiagoushi.top

TS:   require.main === module
来源：http://qez.andypj.xyz

Java: public static void main(String[] args)
来源：http://rln.nanxuanxn.top

Go:   func main()
来源：http://qgx.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nhu.hnxiangtu.top

C#:   static void Main(string[] args)
来源：http://phh.ydjk.org.cn

[M08] 获取系统与运行时信息
来源：http://huz.cucudq.cn

Py:   platform.system();  platform.python_version()
来源：http://usm.vqdsnc.cn

PHP:  PHP_OS;  phpversion();
来源：http://uvb.yanxiufei.cn

JS:   process.platform;  process.version
来源：http://rtt.ydzc1.top

TS:   process.platform;  process.version
来源：http://bvo.guannengcc.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kgy.jqgfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://qbf.yfazqb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://suu.zdqjudy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://pyz.cdnleiting.top

================================================================================
来源：http://qwk.fzhhl.top

N. 数据结构与算法
来源：http://wzs.jiagoushi.top

================================================================================
来源：http://mmk.hysaishi.cn

[N01] 二分查找（有序数组）
来源：http://azk.smart0.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://pat.pycfn.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ssw.haohaochexian.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yxf.havefunace.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hkx.pengpengdd.cyou

Java: Arrays.binarySearch(arr, x)
来源：http://iuj.hcnkem.com

Go:   sort.SearchInts(arr, x)
来源：http://uzv.yuanzhike.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://swk.aizwys.cn

C#:   Array.BinarySearch(arr, x)
来源：http://itv.uphjek.com

[N02] 排序（工程实践用内置实现）
来源：http://nis.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://yjf.kuanghao11.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mtt.snrcjt.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qcb.nanxuanxn.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://txr.jinyuanbaomall.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ijr.sysykeji.top

Go:   slices.Sort(arr)
来源：http://oyz.yanxiufei.cn

Ruby: arr.sort
来源：http://rls.fktsv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vcw.hysaishi.cn

[N03] 快速排序（分治示例）
来源：http://gtb.shuidangran.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xak.jinyuanbaomall.cn

PHP:  // 递归实现，或用 usort
来源：http://fsq.daxiang520.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lig.cucudq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qrq.hammf.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uyq.shanyushiyangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mqq.hfpthk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://csr.birdmap.top

C#:   // 手写递归，或 Array.Sort
来源：http://cgx.hnqzz.top

[N04] 斐波那契数列
来源：http://nam.yfazqb.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vfu.gogol.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://amm.sufxvd.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ooo.yonumen.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nhw.ivvv.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://umw.yj202588.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rae.yueranfly.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yay.aizwys.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://chp.xinyue.icu

[N05] 最大公约数
来源：http://ktm.birdmap.top

Py:   math.gcd(a, b)
来源：http://tfc.shzxlz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bab.redwolf501.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fxg.tian-w.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dwv.gotoacloud.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tfl.xuanzx.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dgk.mhx1999.top

Ruby: a.gcd(b)
来源：http://gjw.fehbvm.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eua.bbcook.cn

[N06] 判断回文字符串
来源：http://ehf.jinqigufen.top

Py:   s == s[::-1]
来源：http://rhg.xingfuxueyuan.xyz

PHP:  $s === strrev($s);
来源：http://hda.hcnkem.com

JS:   s === [...s].reverse().join("")
来源：http://yue.vqdsnc.cn

TS:   s === [...s].reverse().join("")
来源：http://xml.yj20258888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://aqn.ehwqpu.com

Go:   // 双指针从两端比较
来源：http://pir.guowangkeji.top

Ruby: s == s.reverse
来源：http://bns.mhx1999.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xkp.hesvh.cn

[N07] 两数之和（返回下标）
来源：http://xde.cdnleiting.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rfe.xylfe.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://acm.andypj.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://dzv.ybcxt.top

TS:   // 手写 Map<string, number>
来源：http://kuq.yfazqb.com

Java: // 手写 HashMap
来源：http://rut.52xcode.cn

Go:   // 手写 map[int]int
来源：http://wqy.yueranfly.top

Ruby: // 手写 Hash
来源：http://cot.jqgfzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://hzr.andypj.xyz

[N08] 生成全排列
来源：http://ret.xylfe.cn

Py:   itertools.permutations(arr)
来源：http://beh.jinyuanbaomall.cn

PHP:  // 手写递归交换
来源：http://qks.ctjpmb.com

JS:   // 手写回溯递归
来源：http://njl.c1oappe.top

TS:   // 手写回溯递归
来源：http://rbm.smart0.xyz

Java: // 手写回溯递归
来源：http://ipq.xziqi.cn

Go:   // 手写回溯递归
来源：http://vgt.hywenlv.cn

Ruby: arr.permutation.to_a
来源：http://gyw.yangfankeji.com

C#:   // 手写回溯递归
来源：http://nfi.zdbjq.cn

[N09] 栈与队列
来源：http://zhv.hfpthk.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://thf.9152youxi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://znf.xylfe.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ixe.uphjek.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hzv.shanyushiyangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qft.jinqigufen.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rvm.chenjidiqi.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tad.zhijiandao.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uot.zhongyouzk.top

[N10] 链表节点定义
来源：http://qit.hesvh.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pde.havefunace.top

PHP:  class Node { public $v; public $next = null; }
来源：http://etw.tarul.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qwz.wangshuangyany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yjh.epnwcf.com

Java: class Node { int v; Node next; }
来源：http://pxn.yfazqb.com

Go:   type Node struct { V int; Next *Node }
来源：http://xoc.cucudq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xbh.dianchejie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uzt.sjlbkw.cn

[N11] 二叉树中序遍历
来源：http://kal.ydzc1.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tkv.nwbrower.top

PHP:  // 手写递归函数
来源：http://nhj.sxryk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://plg.nanxinkj.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nwx.zhijiandao.cn

Java: // 手写递归
来源：http://lqw.hnqzz.top

Go:   // 手写递归
来源：http://tid.yj20258888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qpb.smart0.xyz

C#:   // 手写递归
来源：http://dmx.pycfn.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ayf.tanke756.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dsh.jinqigufen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://clb.yj202588.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tdz.yuxming.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://one.tanke756.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vhf.jinghuilouyu.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ygr.birdmap.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xca.andypj.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vdw.yj20258888.top

================================================================================
来源：http://njm.snrcjt.cn

O. 并发与异步
来源：http://tdy.nanxuanxn.top

================================================================================
来源：http://kbq.daria6918.cn

[O01] 启动一个线程
来源：http://oxu.zdqjudy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://avv.zhoulong.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bpu.316326.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hbn.xziqi.cn

TS:   // 同 JS
来源：http://xlo.gotoacloud.top

Java: new Thread(() -> f()).start()
来源：http://fmx.gzhubu.top

Go:   go f()
来源：http://jbg.shzxlz.cn

Ruby: Thread.new { f }
来源：http://axy.jinqigufen.top

C#:   Task.Run(() => F());
来源：http://vvu.fengsongda.top

[O02] 使用线程池
来源：http://uxs.vqdsnc.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://abn.cdnleiting.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tvs.fengsongda.top

JS:   // worker_threads 线程池
来源：http://myh.vehdjk.com

TS:   // worker_threads 线程池
来源：http://hzt.vqdsnc.cn

Java: Executors.newFixedThreadPool(4)
来源：http://irb.chenlongwang.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wzc.yj202588.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oej.tianlin.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://guq.bbcook.cn

[O03] 加锁保护共享数据
来源：http://qfb.svipenyu.cn

Py:   with lock: shared += 1
来源：http://tsz.yfazqb.com

PHP:  // 用 flock() 做文件锁
来源：http://hlg.bjfxy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://crv.xylfe.cn

TS:   // 同 JS
来源：http://rad.kuanghao11.cn

Java: synchronized (this) { shared++; }
来源：http://lcf.yangfankeji.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fvu.zdbjq.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zqn.shanyushiyangtech.top

C#:   lock (gate) { shared++; }
来源：http://bjb.aizwys.cn

[O04] 定义异步函数并等待
来源：http://pxf.sweek.top

Py:   async def f():⏎    await g()
来源：http://xvm.zhoulong.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wol.tarul.cn

JS:   async function f() { await g(); }
来源：http://gfr.havefunace.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wdx.yueranfly.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lbg.dashuyun.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sjj.tarul.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hjl.cucudq.cn

C#:   async Task F() { await G(); }
来源：http://bvr.shangyingyoupin.top

[O05] 并发执行并等待全部完成
来源：http://wwk.cqqwz.cn

Py:   asyncio.gather(*tasks)
来源：http://hzu.gogol.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mib.tarul.cn

JS:   await Promise.all(tasks)
来源：http://wvs.jlsjyb.cn

TS:   await Promise.all(tasks)
来源：http://jvu.yanxiufei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yys.fanxiaobao.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://goa.sysykeji.top

Ruby: threads.map(&:join)
来源：http://xol.fktsv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zgi.yanxiufei.cn

[O06] 使用进程池
来源：http://wse.dianchejie.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://aug.zhijiandao.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tkr.quarkkingdee.top

JS:   // child_process / cluster 模块
来源：http://zis.vehdjk.com

TS:   // child_process / cluster 模块
来源：http://nmd.jqgufenzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jmu.yvedp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tae.hongshengwenyu.top

Ruby: // fork 块
来源：http://vop.hywenlv.cn

C#:   Parallel.For
来源：http://wek.yj202588.top

================================================================================
来源：http://mjq.shuidangran.top

P. 常用工具函数
来源：http://fjp.jqgfzy.top

================================================================================
来源：http://zyu.redwolf501.top

[P01] 生成 UUID
来源：http://yry.nanxinkj.top

Py:   str(uuid.uuid4())
来源：http://xwp.xylfe.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wxv.jqgfzy.top

JS:   crypto.randomUUID()
来源：http://woa.shzxlz.cn

TS:   crypto.randomUUID()
来源：http://ota.jinyuanbaomall.cn

Java: UUID.randomUUID().toString()
来源：http://wmm.zhengqikj.top

Go:   // 用 github.com/google/uuid
来源：http://kth.tianlin.xyz

Ruby: SecureRandom.uuid
来源：http://scm.jyoumei.cn

C#:   Guid.NewGuid().ToString()
来源：http://inm.xingfuxueyuan.xyz

[P02] MD5 / SHA256 摘要
来源：http://ewz.hywenlv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://srv.kuanghao11.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rix.yj202588.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://igf.feifeiyinyue.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cdd.feifeiyinyue.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nms.birdmap.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kmy.andypj.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xyh.wangdashe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zbc.jinqigfzy.top

[P03] 生成短随机字符串
来源：http://jzg.sufxvd.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rsc.cucudq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wgh.jinghuilouyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hyu.pengpengdd.cyou

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lxk.cqqwz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vwe.nwbrower.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oiq.shanyushiyangtech.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wij.birdmap.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mxn.shzxlz.cn

[P04] 求长度
来源：http://nmc.shangyingyoupin.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yem.shzxlz.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ytw.havefunace.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lis.yfazqb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cmq.gogol.net.cn

Java: list.size();  map.size();  s.length()
来源：http://afx.hnqzz.top

Go:   len(arr);  len(m)
来源：http://lkl.zhixingplan.top

Ruby: x.length;  x.size
来源：http://syy.shanyushiyangtech.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://iyu.aizwys.cn

[P05] 判断两个对象内容是否相等
来源：http://sxb.kuanghao11.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wko.shanyushiyangtech.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ehe.shanyushiyangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://evo.0kj1m.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vip.shangyingyoupin.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wun.52xcode.cn

Go:   reflect.DeepEqual(a, b)
来源：http://owq.jinyuanbaomall.cn

Ruby: a == b
来源：http://nsk.xylfe.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jmf.zhiwuduotai.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vep.yongpay.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lpd.jqgfzy.top

PHP:  if (empty($x)) {}
来源：http://kdw.zdbjq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lmx.hcnkem.com

TS:   if (x == null) {}
来源：http://buk.ivvv.top

Java: if (x == null || x.isEmpty()) {}
来源：http://eha.havefunace.top

Go:   if x == nil {}
来源：http://lqd.yongpay.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blp.yfazqb.com

C#:   if (x is null) {}
来源：http://mhd.yuxming.cn

[P07] 防抖与节流
来源：http://nnd.hesvh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sda.yueranfly.top

PHP:  // 手写时间戳比较
来源：http://xqm.yonumen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ttp.dashuyun.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://joy.9152youxi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vgp.sjlbkw.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://muw.cashguo.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qvq.jyoumei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://suv.feifeiyinyue.top

[P08] 处理浮点精度问题
来源：http://stt.chenjidiqi.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gkh.fktsv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pij.shangyingyoupin.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jdu.yuxming.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jmk.zdbjq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qpg.zdqjudy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jhw.gogol.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lze.meibo888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oys.316326.xyz

================================================================================
来源：http://sjl.cashguo.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bsw.hnxiangtu.top

================================================================================
来源：http://abc.fengsongda.top

[Q01] 创建表
来源：http://jbd.yonumen.top

CREATE TABLE users (
来源：http://vdf.jqgfzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://chk.smart0.xyz

name VARCHAR(50) NOT NULL,
来源：http://jjy.ivvv.top

email VARCHAR(100) UNIQUE,
来源：http://elg.pengpengdd.cyou

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ghg.jqgfzy.top

);
来源：http://box.gogol.net.cn

[Q02] 创建带外键的表
来源：http://jrx.hesvh.cn

CREATE TABLE orders (
来源：http://qei.zhiwuduotai.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rgm.sxryk.cn

user_id INT NOT NULL,
来源：http://ujp.pycfn.com

amount DECIMAL(10, 2),
来源：http://yqp.guowangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zbx.daria6918.cn

);
来源：http://xeg.zhengqikj.top

[Q03] 增加列
来源：http://hce.gotoacloud.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dgh.yangfankeji.com

[Q04] 修改列类型
来源：http://fnj.haohaochexian.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gib.jiagoushi.top

[Q05] 重命名列
来源：http://pkk.guowangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pqa.0kj1m.cn

[Q06] 删除列
来源：http://nkr.vehdjk.com


<!-- 参考信息 -->