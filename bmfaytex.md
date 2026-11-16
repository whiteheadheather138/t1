代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sbv.kuanghao11.cn

Ruby: warn "err"
来源：http://nbs.cheryme.top

C#:   Console.Error.WriteLine("err")
来源：http://fvm.jianghu66.top

[M07] 判断是否为主入口
来源：http://pqe.0kj1m.cn

Py:   if __name__ == "__main__":
来源：http://ypy.zdbjq.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xfk.xuetiantiany.cn

JS:   require.main === module
来源：http://afn.tarul.cn

TS:   require.main === module
来源：http://bcg.xuanzx.com

Java: public static void main(String[] args)
来源：http://nbk.fengsongda.top

Go:   func main()
来源：http://xxo.nanxinkj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yfr.wangshuangyany.cn

C#:   static void Main(string[] args)
来源：http://fsd.cheryme.top

[M08] 获取系统与运行时信息
来源：http://dpp.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://atp.0kj1m.cn

PHP:  PHP_OS;  phpversion();
来源：http://jzw.shanyushiyangtech.top

JS:   process.platform;  process.version
来源：http://ens.cdnleiting.top

TS:   process.platform;  process.version
来源：http://lrw.meibo888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wxv.shuidangran.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ouj.quarkkingdee.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tdb.zhengqikj.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mwg.zhongyouzk.top

================================================================================
来源：http://ewh.feifeiyinyue.top

N. 数据结构与算法
来源：http://zps.guannengcc.top

================================================================================
来源：http://khi.zhongyouzk.top

[N01] 二分查找（有序数组）
来源：http://tzy.sweek.top

Py:   bisect.bisect_left(arr, x)
来源：http://mwp.yueranfly.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fzb.guannengcc.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bem.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qzv.nanxinkj.top

Java: Arrays.binarySearch(arr, x)
来源：http://fua.fehbvm.com

Go:   sort.SearchInts(arr, x)
来源：http://zfu.vqdsnc.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xdb.zhijiandao.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gkv.gogol.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://xgb.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://xaq.redwolf501.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gjp.cashguo.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://exk.hfpthk.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ppb.cqqwz.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ryk.yonumen.top

Go:   slices.Sort(arr)
来源：http://prm.zdqjudy.top

Ruby: arr.sort
来源：http://fmz.yj202588.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://njb.shanyushiyangkeji.top

[N03] 快速排序（分治示例）
来源：http://qbq.xylfe.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jlb.zhiwuduotai.top

PHP:  // 递归实现，或用 usort
来源：http://san.cashguo.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rhs.sysykeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://znc.gaohongyu789.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sal.cheryme.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kfp.hnxiangtu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ehw.zdbjq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://msd.pycfn.com

[N04] 斐波那契数列
来源：http://uah.ydjk.org.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ssb.tianlin.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zal.jqgufenzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://juo.pengpengdd.cyou

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://plu.dashuyun.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rbu.epnwcf.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nmg.xingfuxueyuan.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zmv.ywan-chungtsiang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kkk.nwbrower.top

[N05] 最大公约数
来源：http://bix.quarkkingdee.top

Py:   math.gcd(a, b)
来源：http://abu.nwbrower.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hra.jinqigfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rvr.zycfv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ypz.redwolf501.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qcq.vehdjk.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uxg.cdnleiting.top

Ruby: a.gcd(b)
来源：http://bxp.yongpay.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kwx.svipenyu.cn

[N06] 判断回文字符串
来源：http://eps.zhijiandao.cn

Py:   s == s[::-1]
来源：http://fle.feifeiyinyue.top

PHP:  $s === strrev($s);
来源：http://rwg.hesvh.cn

JS:   s === [...s].reverse().join("")
来源：http://ept.hongshengwenyu.top

TS:   s === [...s].reverse().join("")
来源：http://flh.hesvh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mmh.andypj.xyz

Go:   // 双指针从两端比较
来源：http://zdv.jinyuanbaomall.cn

Ruby: s == s.reverse
来源：http://xle.jyoumei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tkj.daxiang520.top

[N07] 两数之和（返回下标）
来源：http://nql.xylfe.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tki.cqqwz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qcl.uphjek.com

JS:   // 手写 Map：map.set(v, i)
来源：http://uyf.tianlin.xyz

TS:   // 手写 Map<string, number>
来源：http://ayz.hammf.cn

Java: // 手写 HashMap
来源：http://qgj.ivvv.top

Go:   // 手写 map[int]int
来源：http://pvt.hcnkem.com

Ruby: // 手写 Hash
来源：http://ina.jinqigfzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://ohy.jlsjyb.cn

[N08] 生成全排列
来源：http://suj.meibo888.top

Py:   itertools.permutations(arr)
来源：http://rpw.yj20258.top

PHP:  // 手写递归交换
来源：http://iqj.ywan-chungtsiang.top

JS:   // 手写回溯递归
来源：http://xxj.ctjpmb.com

TS:   // 手写回溯递归
来源：http://myz.zhongyouzk.top

Java: // 手写回溯递归
来源：http://yze.svipenyu.cn

Go:   // 手写回溯递归
来源：http://nmz.bjfxy.top

Ruby: arr.permutation.to_a
来源：http://tja.xuetiantiany.cn

C#:   // 手写回溯递归
来源：http://fvy.ydzc1.top

[N09] 栈与队列
来源：http://sfp.ydzc1.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pye.uphjek.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vfk.chenzaomai.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zej.uphjek.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ajm.ydzc1.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rpu.hywenlv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fva.sxryk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://txo.wangdashe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mps.gaohongyu789.top

[N10] 链表节点定义
来源：http://iae.birdmap.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ued.guowangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://crg.vqdsnc.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kap.guowangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sjv.yueranfly.top

Java: class Node { int v; Node next; }
来源：http://ifz.yuanzhike.top

Go:   type Node struct { V int; Next *Node }
来源：http://pwm.cheryme.top

Ruby: Node = Struct.new(:v, :next)
来源：http://dfs.epnwcf.com

C#:   class Node { public int V; public Node? Next; }
来源：http://gag.ehwqpu.com

[N11] 二叉树中序遍历
来源：http://cid.hfpthk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dwq.0kj1m.cn

PHP:  // 手写递归函数
来源：http://oqo.daxiang520.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tml.vqdsnc.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lbm.cdnleiting.top

Java: // 手写递归
来源：http://rjg.epnwcf.com

Go:   // 手写递归
来源：http://agp.yj202588.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ivs.yongpay.top

C#:   // 手写递归
来源：http://hyn.yongpay.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://not.vehdjk.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zim.xuanzx.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qqe.vqdsnc.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tni.jlsjyb.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://twi.hfpthk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oel.guowangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sjj.jlsjyb.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://osh.iojbl.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jdy.yj20258888.top

================================================================================
来源：http://ccv.jinghuilouyu.cn

O. 并发与异步
来源：http://rco.jinqigufen.top

================================================================================
来源：http://hzw.nwbrower.top

[O01] 启动一个线程
来源：http://xnk.tanke756.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ekv.0kj1m.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bxz.cucudq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dgn.cqqwz.cn

TS:   // 同 JS
来源：http://jcu.shzxlz.cn

Java: new Thread(() -> f()).start()
来源：http://pmr.jinghuilouyu.cn

Go:   go f()
来源：http://tqi.ydzc1.top

Ruby: Thread.new { f }
来源：http://riz.yangfankeji.com

C#:   Task.Run(() => F());
来源：http://tzx.vqdsnc.cn

[O02] 使用线程池
来源：http://nuc.tarul.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vby.uphjek.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fwu.zdqjudy.top

JS:   // worker_threads 线程池
来源：http://vaz.yongpay.top

TS:   // worker_threads 线程池
来源：http://kvz.birdmap.top

Java: Executors.newFixedThreadPool(4)
来源：http://flt.yuanzhike.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rhg.xingfuxueyuan.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ioi.jinyuanbaomall.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mem.hnxiangtu.top

[O03] 加锁保护共享数据
来源：http://frm.shanyushiyangtech.top

Py:   with lock: shared += 1
来源：http://cyj.jqgfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://jwz.jiagoushi.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://erk.jinqigfzy.top

TS:   // 同 JS
来源：http://tzr.gaohongyu789.top

Java: synchronized (this) { shared++; }
来源：http://kek.tarul.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qss.yj202588.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://btj.zhongyouzk.top

C#:   lock (gate) { shared++; }
来源：http://ufr.zycfv.cn

[O04] 定义异步函数并等待
来源：http://sxo.dashuyun.cn

Py:   async def f():⏎    await g()
来源：http://zep.jlsjyb.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ekv.haohaochexian.top

JS:   async function f() { await g(); }
来源：http://kfb.uphjek.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://iii.zhengqikj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yik.ydjk.org.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oso.quarkkingdee.top

Ruby: # 用 Fiber 或 async gem
来源：http://qkc.andypj.xyz

C#:   async Task F() { await G(); }
来源：http://hma.316326.xyz

[O05] 并发执行并等待全部完成
来源：http://cfd.pengpengdd.cyou

Py:   asyncio.gather(*tasks)
来源：http://gyl.shanyushiyangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://crx.zdqjudy.top

JS:   await Promise.all(tasks)
来源：http://mzm.fehbvm.com

TS:   await Promise.all(tasks)
来源：http://jwa.kuanghao11.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kgs.xingfuxueyuan.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ktd.52xcode.cn

Ruby: threads.map(&:join)
来源：http://vhz.quarkkingdee.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jrr.snrcjt.cn

[O06] 使用进程池
来源：http://eck.jqgfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://llx.nanxuanxn.top

PHP:  // pcntl_fork 或多进程队列
来源：http://yje.tianlin.xyz

JS:   // child_process / cluster 模块
来源：http://zrd.jinghuilouyu.cn

TS:   // child_process / cluster 模块
来源：http://zyq.hysaishi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gra.9152youxi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xox.yj20258.top

Ruby: // fork 块
来源：http://ngb.gotoacloud.top

C#:   Parallel.For
来源：http://vdr.yvedp.cn

================================================================================
来源：http://wgw.zhoulong.xyz

P. 常用工具函数
来源：http://gem.yuxming.cn

================================================================================
来源：http://swm.zdbjq.cn

[P01] 生成 UUID
来源：http://wfd.wangshuangyany.cn

Py:   str(uuid.uuid4())
来源：http://jlr.ivvv.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ycb.uphjek.com

JS:   crypto.randomUUID()
来源：http://rkv.haohaochexian.top

TS:   crypto.randomUUID()
来源：http://gov.0kj1m.cn

Java: UUID.randomUUID().toString()
来源：http://pkz.chenzaomai.com

Go:   // 用 github.com/google/uuid
来源：http://sgp.nwbrower.top

Ruby: SecureRandom.uuid
来源：http://hdw.9152youxi.cn

C#:   Guid.NewGuid().ToString()
来源：http://wsm.yvedp.cn

[P02] MD5 / SHA256 摘要
来源：http://jui.fzhhl.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zkn.yueranfly.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zxt.jianghu66.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ico.jqgfzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ljk.xuetiantiany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ayk.mhx1999.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://urm.hcnkem.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wlp.andypj.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qzk.dashuyun.cn

[P03] 生成短随机字符串
来源：http://nvx.andypj.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ymb.quarkkingdee.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cxl.ydjk.org.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fiz.yj202588.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jgm.quarkkingdee.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fui.jianghu66.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uld.yonumen.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vnz.guowangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rpb.shanyushiyangtech.top

[P04] 求长度
来源：http://iaa.tianlin.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://opz.yfazqb.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wkn.nanxuanxn.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xii.sweek.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://irh.guowangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://uiq.hcnkem.com

Go:   len(arr);  len(m)
来源：http://dlp.zhoulong.xyz

Ruby: x.length;  x.size
来源：http://vyq.daria6918.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tjc.jinyuanbaomall.cn

[P05] 判断两个对象内容是否相等
来源：http://edr.havefunace.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jsn.xinyue.icu

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wry.shuidangran.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://twv.ctjpmb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blp.0kj1m.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xup.jinqigfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://gzs.jianghu66.top

Ruby: a == b
来源：http://wwc.wangshuangyany.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ryb.nanxinkj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yok.xuanzx.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://prq.ppjwa.cn

PHP:  if (empty($x)) {}
来源：http://pci.c1oappe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://twd.jinqigfzy.top

TS:   if (x == null) {}
来源：http://tvd.9152youxi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uvt.cashguo.top

Go:   if x == nil {}
来源：http://bjc.aibaodan.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rom.yanxiufei.cn

C#:   if (x is null) {}
来源：http://ghr.jianghu66.top

[P07] 防抖与节流
来源：http://oim.pycfn.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bie.yongpay.top

PHP:  // 手写时间戳比较
来源：http://vgr.ctjpmb.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cyr.gotoacloud.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ycr.fehbvm.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lqq.yj202588.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lse.jiagoushi.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://tla.cdnleiting.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://efc.chenzaomai.com

[P08] 处理浮点精度问题
来源：http://nff.sweek.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dai.hywenlv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yzt.pycfn.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://egk.hfpthk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wea.jinghuilouyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mrl.sjlbkw.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://keo.shangyingyoupin.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vcw.pengpengdd.cyou

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mdt.zhixingplan.top

================================================================================
来源：http://lhx.vehdjk.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://enu.aibaodan.cn

================================================================================
来源：http://dht.tianlin.xyz

[Q01] 创建表
来源：http://ypf.c1oappe.top

CREATE TABLE users (
来源：http://fgl.xuanzx.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://puu.9152youxi.cn

name VARCHAR(50) NOT NULL,
来源：http://rbr.havefunace.top

email VARCHAR(100) UNIQUE,
来源：http://tfy.redwolf501.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kcw.hfpthk.cn

);
来源：http://wbh.jqgfzy.top

[Q02] 创建带外键的表
来源：http://agv.meibo888.top

CREATE TABLE orders (
来源：http://bij.meibo888.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://onk.hongshengwenyu.top

user_id INT NOT NULL,
来源：http://zkt.gotoacloud.top

amount DECIMAL(10, 2),
来源：http://rac.jinyuanbaomall.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tit.jinqigufen.top

);
来源：http://eou.pycfn.com

[Q03] 增加列
来源：http://rpe.jinqigufen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fya.ivvv.top

[Q04] 修改列类型
来源：http://cbv.shuidangran.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nou.guannengcc.top

[Q05] 重命名列
来源：http://pzp.52xcode.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lku.yvedp.cn

[Q06] 删除列
来源：http://xsn.tianlin.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://xpz.aizwys.cn

[Q07] 删除表
来源：http://vid.sufxvd.cn

DROP TABLE IF EXISTS orders;
来源：http://sno.ctjpmb.com

[Q08] 创建普通索引
来源：http://wlq.chenzaomai.com

CREATE INDEX idx_users_email ON users(email);
来源：http://pay.yueranfly.top

[Q09] 创建唯一索引
来源：http://oaq.nwbrower.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kfy.xuetiantiany.cn

[Q10] 插入单行
来源：http://uja.snrcjt.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vzu.zhijiandao.cn

[Q11] 一次插入多行
来源：http://jqq.sxryk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mha.shangyingyoupin.top

[Q12] 插入后取自增 ID
来源：http://bmh.sjlbkw.cn


<!-- 参考信息 -->