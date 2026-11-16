代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jja.zhiwuduotai.top

Ruby: warn "err"
来源：http://psj.kuanghao11.cn

C#:   Console.Error.WriteLine("err")
来源：http://ljr.hnxiangtu.top

[M07] 判断是否为主入口
来源：http://fpa.xuanzx.com

Py:   if __name__ == "__main__":
来源：http://wae.yanxiufei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lsm.jyoumei.cn

JS:   require.main === module
来源：http://efl.feifeiyinyue.top

TS:   require.main === module
来源：http://eud.fzhhl.top

Java: public static void main(String[] args)
来源：http://mrz.ivvv.top

Go:   func main()
来源：http://yfs.feifeiyinyue.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wmn.smart0.xyz

C#:   static void Main(string[] args)
来源：http://yxg.yj20258888.top

[M08] 获取系统与运行时信息
来源：http://cjt.9152youxi.cn

Py:   platform.system();  platform.python_version()
来源：http://rdm.hammf.cn

PHP:  PHP_OS;  phpversion();
来源：http://ycg.wangshuangyany.cn

JS:   process.platform;  process.version
来源：http://gbf.yanxiufei.cn

TS:   process.platform;  process.version
来源：http://uws.fktsv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jcz.bbcook.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://utv.cdnleiting.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wqc.ctjpmb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://ifv.yvedp.cn

================================================================================
来源：http://ntb.yj20258888.top

N. 数据结构与算法
来源：http://wap.jinqigfzy.top

================================================================================
来源：http://emu.zhiwuduotai.top

[N01] 二分查找（有序数组）
来源：http://afr.hammf.cn

Py:   bisect.bisect_left(arr, x)
来源：http://duc.yj20258888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hat.yj202588.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kqx.dianchejie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gjx.nanxuanxn.top

Java: Arrays.binarySearch(arr, x)
来源：http://kmz.yanxiufei.cn

Go:   sort.SearchInts(arr, x)
来源：http://ulw.fengsongda.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lrd.ybcxt.top

C#:   Array.BinarySearch(arr, x)
来源：http://aqq.dianchejie.cn

[N02] 排序（工程实践用内置实现）
来源：http://dzf.fktsv.cn

Py:   sorted(arr);  arr.sort()
来源：http://zro.chenlongwang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://giy.mhx1999.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://tid.quarkkingdee.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cxf.yvedp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qhx.ctjpmb.com

Go:   slices.Sort(arr)
来源：http://ekl.mhx1999.top

Ruby: arr.sort
来源：http://aoa.gotoacloud.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://yje.dashuyun.cn

[N03] 快速排序（分治示例）
来源：http://vmg.chenjidiqi.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yvw.aibaodan.cn

PHP:  // 递归实现，或用 usort
来源：http://fmb.yj20258888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ghd.yvedp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wnc.gaohongyu789.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zir.guowangkeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ogn.gaohongyu789.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ntl.ydjk.org.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ocm.sufxvd.cn

[N04] 斐波那契数列
来源：http://euy.yj202588.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cjx.ydjk.org.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wul.cheryme.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jqp.ppjwa.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wnd.fengsongda.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nni.kuanghao11.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nxf.shanyushiyangkeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cav.hcnkem.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dsp.shuidangran.top

[N05] 最大公约数
来源：http://vaf.gotoacloud.top

Py:   math.gcd(a, b)
来源：http://jqj.hnqzz.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pbh.dianchejie.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jhd.gzhubu.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ikt.yj20258888.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wjc.yueranfly.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bfz.sweek.top

Ruby: a.gcd(b)
来源：http://zwh.haohaochexian.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ito.snrcjt.cn

[N06] 判断回文字符串
来源：http://bnb.cqqwz.cn

Py:   s == s[::-1]
来源：http://xib.sjlbkw.cn

PHP:  $s === strrev($s);
来源：http://aop.aibaodan.cn

JS:   s === [...s].reverse().join("")
来源：http://giz.wangshuangyany.cn

TS:   s === [...s].reverse().join("")
来源：http://llv.jiagoushi.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mda.bjfxy.top

Go:   // 双指针从两端比较
来源：http://kwm.hywenlv.cn

Ruby: s == s.reverse
来源：http://fiu.shuidangran.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://pmm.cashguo.top

[N07] 两数之和（返回下标）
来源：http://bjx.9152youxi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://obn.nwbrower.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fbf.tarul.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kzl.ehwqpu.com

TS:   // 手写 Map<string, number>
来源：http://zkl.tian-w.cn

Java: // 手写 HashMap
来源：http://byh.52xcode.cn

Go:   // 手写 map[int]int
来源：http://cqf.meibo888.top

Ruby: // 手写 Hash
来源：http://bom.guowangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://vpf.bjfxy.top

[N08] 生成全排列
来源：http://zaj.pycfn.com

Py:   itertools.permutations(arr)
来源：http://tcu.gzhubu.top

PHP:  // 手写递归交换
来源：http://alr.9152youxi.cn

JS:   // 手写回溯递归
来源：http://zox.feifeiyinyue.top

TS:   // 手写回溯递归
来源：http://cgm.pycfn.com

Java: // 手写回溯递归
来源：http://uhp.shuidangran.top

Go:   // 手写回溯递归
来源：http://yta.yj202588.top

Ruby: arr.permutation.to_a
来源：http://ufb.tanke756.top

C#:   // 手写回溯递归
来源：http://njk.zdbjq.cn

[N09] 栈与队列
来源：http://ohe.chenjidiqi.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://coo.tarul.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://seq.shanyushiyangtech.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://avj.chenzaomai.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fia.sysykeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zsh.fanxiaobao.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qpb.iojbl.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://poy.hnxiangtu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dyi.yuxming.cn

[N10] 链表节点定义
来源：http://lna.shzxlz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gbg.quarkkingdee.top

PHP:  class Node { public $v; public $next = null; }
来源：http://bcn.dashuyun.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://thf.gotoacloud.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://aqa.vehdjk.com

Java: class Node { int v; Node next; }
来源：http://psd.gzhubu.top

Go:   type Node struct { V int; Next *Node }
来源：http://xry.fktsv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zyz.aibaodan.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xfq.havefunace.top

[N11] 二叉树中序遍历
来源：http://yzm.tian-w.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wyo.aibaodan.cn

PHP:  // 手写递归函数
来源：http://wdv.bjfxy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mzo.guannengcc.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fey.daxiang520.top

Java: // 手写递归
来源：http://wyu.xuanzx.com

Go:   // 手写递归
来源：http://szo.jqgufenzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yrn.chenzaomai.com

C#:   // 手写递归
来源：http://you.yfazqb.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kot.c1oappe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://swk.nanxinkj.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uva.andypj.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hnc.jinghuilouyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jox.hnqzz.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ndg.zhiwuduotai.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kbw.chenlongwang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lhs.fengsongda.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dtb.ydjk.org.cn

================================================================================
来源：http://tyx.birdmap.top

O. 并发与异步
来源：http://drw.cashguo.top

================================================================================
来源：http://mmi.jiagoushi.top

[O01] 启动一个线程
来源：http://sov.0kj1m.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hrr.ydzc1.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rhb.vqdsnc.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wqz.gzhubu.top

TS:   // 同 JS
来源：http://mps.yonumen.top

Java: new Thread(() -> f()).start()
来源：http://hfz.kuanghao11.cn

Go:   go f()
来源：http://qeb.zhaomingkeji.xyz

Ruby: Thread.new { f }
来源：http://qjg.wangdashe.top

C#:   Task.Run(() => F());
来源：http://mgb.hnqzz.top

[O02] 使用线程池
来源：http://pbd.gogol.net.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uae.wangdashe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hmb.yanxiufei.cn

JS:   // worker_threads 线程池
来源：http://ucp.birdmap.top

TS:   // worker_threads 线程池
来源：http://qlx.snrcjt.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ksp.meibo888.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mdd.xuetiantiany.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nhd.zhaomingkeji.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qlw.gaohongyu789.top

[O03] 加锁保护共享数据
来源：http://ucl.yj202588.top

Py:   with lock: shared += 1
来源：http://hah.yangfankeji.com

PHP:  // 用 flock() 做文件锁
来源：http://rmn.fanxiaobao.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gqd.jinqigufen.top

TS:   // 同 JS
来源：http://otq.zhiwuduotai.top

Java: synchronized (this) { shared++; }
来源：http://suv.redwolf501.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bpf.nanxinkj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://mnd.epnwcf.com

C#:   lock (gate) { shared++; }
来源：http://uub.gogol.net.cn

[O04] 定义异步函数并等待
来源：http://ycm.ywan-chungtsiang.top

Py:   async def f():⏎    await g()
来源：http://veg.kuanghao11.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pog.pycfn.com

JS:   async function f() { await g(); }
来源：http://svn.hcnkem.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://fzb.sweek.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lpz.zhengqikj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cyh.zhoulong.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://eqd.shuidangran.top

C#:   async Task F() { await G(); }
来源：http://tif.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://yqb.cheryme.top

Py:   asyncio.gather(*tasks)
来源：http://xlf.yangfankeji.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jng.yvedp.cn

JS:   await Promise.all(tasks)
来源：http://tcc.ctjpmb.com

TS:   await Promise.all(tasks)
来源：http://zjg.yongpay.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tdy.zhijiandao.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://unc.iojbl.cn

Ruby: threads.map(&:join)
来源：http://fgw.nwbrower.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nwj.guannengcc.top

[O06] 使用进程池
来源：http://rko.xuetiantiany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qre.fzhhl.top

PHP:  // pcntl_fork 或多进程队列
来源：http://hjs.fktsv.cn

JS:   // child_process / cluster 模块
来源：http://lig.jyoumei.cn

TS:   // child_process / cluster 模块
来源：http://ysk.hongshengwenyu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vqq.hywenlv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dlu.hongshengwenyu.top

Ruby: // fork 块
来源：http://xnv.xinyue.icu

C#:   Parallel.For
来源：http://ipr.bjfxy.top

================================================================================
来源：http://kqf.aibaodan.cn

P. 常用工具函数
来源：http://qwg.zycfv.cn

================================================================================
来源：http://gjf.ehwqpu.com

[P01] 生成 UUID
来源：http://kke.gzhubu.top

Py:   str(uuid.uuid4())
来源：http://cqe.smart0.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wcu.dashuyun.cn

JS:   crypto.randomUUID()
来源：http://lhl.redwolf501.top

TS:   crypto.randomUUID()
来源：http://pov.zhoulong.xyz

Java: UUID.randomUUID().toString()
来源：http://kqs.hnxiangtu.top

Go:   // 用 github.com/google/uuid
来源：http://ltt.wangdashe.top

Ruby: SecureRandom.uuid
来源：http://ryp.tianlin.xyz

C#:   Guid.NewGuid().ToString()
来源：http://lbu.jlsjyb.cn

[P02] MD5 / SHA256 摘要
来源：http://vty.fehbvm.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vwi.vqdsnc.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yxf.fzhhl.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://exw.jinghuilouyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ytq.zhoulong.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hxn.cheryme.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gga.9152youxi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bkr.sjlbkw.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cva.52xcode.cn

[P03] 生成短随机字符串
来源：http://ydd.daxiang520.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rdu.hfpthk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://occ.yuxming.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hxr.zhongyouzk.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cnc.daxiang520.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xqb.jyoumei.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yam.fzhhl.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ucz.haohaochexian.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wdk.fanxiaobao.xyz

[P04] 求长度
来源：http://jqu.52xcode.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bax.chenjidiqi.icu

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baj.haohaochexian.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://soi.tianlin.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jew.nwbrower.top

Java: list.size();  map.size();  s.length()
来源：http://uml.ywan-chungtsiang.top

Go:   len(arr);  len(m)
来源：http://rcr.yueranfly.top

Ruby: x.length;  x.size
来源：http://epr.52xcode.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://suf.zdbjq.cn

[P05] 判断两个对象内容是否相等
来源：http://noa.yvedp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://nno.hammf.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zwe.pycfn.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://alr.316326.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bkb.cucudq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bwt.jinghuilouyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rbu.nwbrower.top

Ruby: a == b
来源：http://yob.yj202588.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://frk.andypj.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://quv.kuanghao11.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://upu.zhaomingkeji.xyz

PHP:  if (empty($x)) {}
来源：http://nkg.vqdsnc.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gej.yanxiufei.cn

TS:   if (x == null) {}
来源：http://qbk.sufxvd.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ivf.gogol.net.cn

Go:   if x == nil {}
来源：http://hcc.cucudq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vrq.xylfe.cn

C#:   if (x is null) {}
来源：http://jsg.hammf.cn

[P07] 防抖与节流
来源：http://jui.fehbvm.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tnz.wangdashe.top

PHP:  // 手写时间戳比较
来源：http://oqd.chenzaomai.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ksr.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mht.chenzaomai.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ekk.yj20258.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yto.guannengcc.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://vyb.fzhhl.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ohl.316326.xyz

[P08] 处理浮点精度问题
来源：http://jql.jinqigufen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cgx.fengsongda.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pbj.ybcxt.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://osy.jinghuilouyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://izr.ydzc1.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ijm.fehbvm.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pge.gaohongyu789.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mkr.chenzaomai.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mmo.yongpay.top

================================================================================
来源：http://tmv.pycfn.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oli.gotoacloud.top

================================================================================
来源：http://zli.sweek.top

[Q01] 创建表
来源：http://zuq.xziqi.cn

CREATE TABLE users (
来源：http://pes.sjlbkw.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vic.jlsjyb.cn

name VARCHAR(50) NOT NULL,
来源：http://wqm.xingfuxueyuan.xyz

email VARCHAR(100) UNIQUE,
来源：http://adv.sxryk.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://phc.zhongyouzk.top

);
来源：http://tar.9152youxi.cn

[Q02] 创建带外键的表
来源：http://hln.yuxming.cn

CREATE TABLE orders (
来源：http://dgv.sjlbkw.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bsr.fengsongda.top

user_id INT NOT NULL,
来源：http://qbt.fzhhl.top

amount DECIMAL(10, 2),
来源：http://gxz.chenlongwang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cwt.aizwys.cn

);
来源：http://snx.quarkkingdee.top

[Q03] 增加列
来源：http://jea.aibaodan.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jfp.cheryme.top

[Q04] 修改列类型
来源：http://ayz.sysykeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jjw.chenjidiqi.icu

[Q05] 重命名列
来源：http://zhe.snrcjt.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pxj.guannengcc.top

[Q06] 删除列
来源：http://brq.zycfv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dwy.hnxiangtu.top

[Q07] 删除表
来源：http://ofk.ydjk.org.cn

DROP TABLE IF EXISTS orders;
来源：http://rgo.daria6918.cn

[Q08] 创建普通索引
来源：http://vqi.yuxming.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://svg.dianchejie.cn

[Q09] 创建唯一索引
来源：http://iqq.sufxvd.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sma.hammf.cn

[Q10] 插入单行
来源：http://rlq.yj20258888.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hkr.shanyushiyangkeji.top

[Q11] 一次插入多行
来源：http://zzj.sysykeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hjr.xinyue.icu

[Q12] 插入后取自增 ID
来源：http://gln.xuanzx.com


<!-- 参考信息 -->