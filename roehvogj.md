代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ccw.tanke756.top

Ruby: warn "err"
来源：http://cnr.dashuyun.cn

C#:   Console.Error.WriteLine("err")
来源：http://zvr.sysykeji.top

[M07] 判断是否为主入口
来源：http://zmz.yuanzhike.top

Py:   if __name__ == "__main__":
来源：http://wby.zhixingplan.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xok.sweek.top

JS:   require.main === module
来源：http://hsp.ywan-chungtsiang.top

TS:   require.main === module
来源：http://rjw.cucudq.cn

Java: public static void main(String[] args)
来源：http://hyl.zdbjq.cn

Go:   func main()
来源：http://bdq.andypj.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kqr.mhx1999.top

C#:   static void Main(string[] args)
来源：http://dbe.yanxiufei.cn

[M08] 获取系统与运行时信息
来源：http://ybn.hywenlv.cn

Py:   platform.system();  platform.python_version()
来源：http://hni.yuanzhike.top

PHP:  PHP_OS;  phpversion();
来源：http://ujb.yj202588.top

JS:   process.platform;  process.version
来源：http://qbi.jqgufenzy.top

TS:   process.platform;  process.version
来源：http://qwm.yvedp.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://obp.cqqwz.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://gxe.hcnkem.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ebx.shangyingyoupin.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lls.havefunace.top

================================================================================
来源：http://gip.xuetiantiany.cn

N. 数据结构与算法
来源：http://jst.daxiang520.top

================================================================================
来源：http://kaz.zhixingplan.top

[N01] 二分查找（有序数组）
来源：http://eej.shuidangran.top

Py:   bisect.bisect_left(arr, x)
来源：http://xxu.guannengcc.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blw.gotoacloud.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://srz.fanxiaobao.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lfh.yj202588.top

Java: Arrays.binarySearch(arr, x)
来源：http://kby.shanyushiyangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://txm.chenlongwang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cns.xuanzx.com

C#:   Array.BinarySearch(arr, x)
来源：http://uqh.tanke756.top

[N02] 排序（工程实践用内置实现）
来源：http://kdc.jinyuanbaomall.cn

Py:   sorted(arr);  arr.sort()
来源：http://tjp.havefunace.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://niw.c1oappe.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jqe.hywenlv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://iqk.yvedp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lri.yfazqb.com

Go:   slices.Sort(arr)
来源：http://apy.sufxvd.cn

Ruby: arr.sort
来源：http://gpz.cashguo.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://klh.jinghuilouyu.cn

[N03] 快速排序（分治示例）
来源：http://oaf.yuanzhike.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ktz.fktsv.cn

PHP:  // 递归实现，或用 usort
来源：http://rcb.yfazqb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fbm.yuanzhike.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qpn.yangfankeji.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://exk.shanyushiyangtech.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tyw.tianlin.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://oxx.kuanghao11.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wcj.aibaodan.cn

[N04] 斐波那契数列
来源：http://bbg.jiagoushi.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fmr.jinqigfzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://deo.chenzaomai.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kyn.xylfe.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pjy.sysykeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mqm.hywenlv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lpi.zhengqikj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mgn.gzhubu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bii.ydzc1.top

[N05] 最大公约数
来源：http://vpl.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://zlb.dianchejie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://koy.hammf.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://clc.jqgufenzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://chj.wangdashe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yxl.jinqigfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rnc.chenjidiqi.icu

Ruby: a.gcd(b)
来源：http://aqm.ydzc1.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bwf.nanxinkj.top

[N06] 判断回文字符串
来源：http://liv.hnxiangtu.top

Py:   s == s[::-1]
来源：http://hvv.feifeiyinyue.top

PHP:  $s === strrev($s);
来源：http://qwy.chenjidiqi.icu

JS:   s === [...s].reverse().join("")
来源：http://ovz.xziqi.cn

TS:   s === [...s].reverse().join("")
来源：http://gfh.birdmap.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dqz.andypj.xyz

Go:   // 双指针从两端比较
来源：http://ujs.jinqigfzy.top

Ruby: s == s.reverse
来源：http://deh.ivvv.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://yzm.bjfxy.top

[N07] 两数之和（返回下标）
来源：http://bjq.nwbrower.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://nfd.hfpthk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ane.haohaochexian.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zed.shanyushiyangtech.top

TS:   // 手写 Map<string, number>
来源：http://vrv.jyoumei.cn

Java: // 手写 HashMap
来源：http://wyq.sysykeji.top

Go:   // 手写 map[int]int
来源：http://baz.zdqjudy.top

Ruby: // 手写 Hash
来源：http://pfo.xuetiantiany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://kuf.shangyingyoupin.top

[N08] 生成全排列
来源：http://byc.fzhhl.top

Py:   itertools.permutations(arr)
来源：http://shm.gotoacloud.top

PHP:  // 手写递归交换
来源：http://snu.zhongyouzk.top

JS:   // 手写回溯递归
来源：http://niy.haohaochexian.top

TS:   // 手写回溯递归
来源：http://ioe.yj20258.top

Java: // 手写回溯递归
来源：http://ffa.chenzaomai.com

Go:   // 手写回溯递归
来源：http://fgq.meibo888.top

Ruby: arr.permutation.to_a
来源：http://gyi.ydjk.org.cn

C#:   // 手写回溯递归
来源：http://xrq.chenlongwang.top

[N09] 栈与队列
来源：http://ppn.zycfv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rlu.cashguo.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hdw.hesvh.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dgb.ctjpmb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wfb.shangyingyoupin.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://njl.yvedp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vig.xuetiantiany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://diy.yj20258888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hzk.zhaomingkeji.xyz

[N10] 链表节点定义
来源：http://auu.yanxiufei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iwf.zhixingplan.top

PHP:  class Node { public $v; public $next = null; }
来源：http://bqe.hnxiangtu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ktl.kuanghao11.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ogs.xinyue.icu

Java: class Node { int v; Node next; }
来源：http://dvs.snrcjt.cn

Go:   type Node struct { V int; Next *Node }
来源：http://fly.bbcook.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rsq.shanyushiyangtech.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dbo.ybcxt.top

[N11] 二叉树中序遍历
来源：http://bcz.cucudq.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bkv.aibaodan.cn

PHP:  // 手写递归函数
来源：http://lzn.meibo888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kql.yonumen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yyp.fanxiaobao.xyz

Java: // 手写递归
来源：http://qkt.tarul.cn

Go:   // 手写递归
来源：http://rem.hesvh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ozi.jqgfzy.top

C#:   // 手写递归
来源：http://qyz.yj20258888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jko.52xcode.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bjo.zhaomingkeji.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nsq.ctjpmb.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://izx.yangfankeji.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fnq.havefunace.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://inz.0kj1m.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yiu.zhijiandao.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://svn.fanxiaobao.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pfl.cqqwz.cn

================================================================================
来源：http://byk.shanyushiyangtech.top

O. 并发与异步
来源：http://iuq.zycfv.cn

================================================================================
来源：http://gdh.jianghu66.top

[O01] 启动一个线程
来源：http://evw.hammf.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pus.cashguo.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qcg.xinyue.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tog.yuanzhike.top

TS:   // 同 JS
来源：http://khf.ydjk.org.cn

Java: new Thread(() -> f()).start()
来源：http://iud.shzxlz.cn

Go:   go f()
来源：http://hmz.fanxiaobao.xyz

Ruby: Thread.new { f }
来源：http://fph.yj202588.top

C#:   Task.Run(() => F());
来源：http://quv.wangshuangyany.cn

[O02] 使用线程池
来源：http://qrp.zhiwuduotai.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jht.jlsjyb.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gej.zhongyouzk.top

JS:   // worker_threads 线程池
来源：http://bpc.ydjk.org.cn

TS:   // worker_threads 线程池
来源：http://qap.fehbvm.com

Java: Executors.newFixedThreadPool(4)
来源：http://hub.hfpthk.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bbl.jqgfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ppg.jinqigfzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kbo.cheryme.top

[O03] 加锁保护共享数据
来源：http://nkk.iojbl.cn

Py:   with lock: shared += 1
来源：http://miv.cdnleiting.top

PHP:  // 用 flock() 做文件锁
来源：http://utn.chenzaomai.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ydl.shangyingyoupin.top

TS:   // 同 JS
来源：http://mdf.zhongyouzk.top

Java: synchronized (this) { shared++; }
来源：http://poz.mhx1999.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nzj.gaohongyu789.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qok.cdnleiting.top

C#:   lock (gate) { shared++; }
来源：http://vdl.tanke756.top

[O04] 定义异步函数并等待
来源：http://dae.zycfv.cn

Py:   async def f():⏎    await g()
来源：http://hvd.vqdsnc.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kpb.jlsjyb.cn

JS:   async function f() { await g(); }
来源：http://ofu.yuxming.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://cra.mhx1999.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lmq.snrcjt.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fxh.cheryme.top

Ruby: # 用 Fiber 或 async gem
来源：http://lqv.fzhhl.top

C#:   async Task F() { await G(); }
来源：http://ukh.nanxuanxn.top

[O05] 并发执行并等待全部完成
来源：http://wsy.jinqigufen.top

Py:   asyncio.gather(*tasks)
来源：http://zvr.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yih.jqgufenzy.top

JS:   await Promise.all(tasks)
来源：http://ioc.cqqwz.cn

TS:   await Promise.all(tasks)
来源：http://iwi.zhoulong.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wkr.zhijiandao.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kuo.xingfuxueyuan.xyz

Ruby: threads.map(&:join)
来源：http://qbq.xuanzx.com

C#:   await Task.WhenAll(t1, t2)
来源：http://xrm.smart0.xyz

[O06] 使用进程池
来源：http://xjd.tarul.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kgs.nanxuanxn.top

PHP:  // pcntl_fork 或多进程队列
来源：http://eri.gotoacloud.top

JS:   // child_process / cluster 模块
来源：http://rim.hongshengwenyu.top

TS:   // child_process / cluster 模块
来源：http://mgg.xylfe.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zyz.ydjk.org.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ruz.jinqigufen.top

Ruby: // fork 块
来源：http://ule.aizwys.cn

C#:   Parallel.For
来源：http://iyy.52xcode.cn

================================================================================
来源：http://fzz.hesvh.cn

P. 常用工具函数
来源：http://qmq.birdmap.top

================================================================================
来源：http://lfr.fanxiaobao.xyz

[P01] 生成 UUID
来源：http://wyc.cdnleiting.top

Py:   str(uuid.uuid4())
来源：http://uye.wangdashe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iqd.0kj1m.cn

JS:   crypto.randomUUID()
来源：http://stf.feifeiyinyue.top

TS:   crypto.randomUUID()
来源：http://bem.ctjpmb.com

Java: UUID.randomUUID().toString()
来源：http://zir.zdqjudy.top

Go:   // 用 github.com/google/uuid
来源：http://bgw.tian-w.cn

Ruby: SecureRandom.uuid
来源：http://src.daxiang520.top

C#:   Guid.NewGuid().ToString()
来源：http://oxm.ybcxt.top

[P02] MD5 / SHA256 摘要
来源：http://ote.ybcxt.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://akm.ydjk.org.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hcc.cashguo.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ewi.aibaodan.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vdu.yj20258.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nfl.tarul.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gfx.zycfv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://svm.wangdashe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tzx.hnxiangtu.top

[P03] 生成短随机字符串
来源：http://aez.epnwcf.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://axj.yj202588.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lej.havefunace.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://row.ehwqpu.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tgo.meibo888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xry.zhaomingkeji.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ksq.yj20258.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zjs.fengsongda.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sld.sufxvd.cn

[P04] 求长度
来源：http://dvj.yonumen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jej.zhixingplan.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lqi.sxryk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rmf.tanke756.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ryx.cheryme.top

Java: list.size();  map.size();  s.length()
来源：http://fuf.0kj1m.cn

Go:   len(arr);  len(m)
来源：http://qks.ppjwa.cn

Ruby: x.length;  x.size
来源：http://mla.hnxiangtu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qco.guannengcc.top

[P05] 判断两个对象内容是否相等
来源：http://ylf.iojbl.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bcp.gaohongyu789.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kag.daxiang520.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vex.jlsjyb.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gzv.ehwqpu.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://eyg.hammf.cn

Go:   reflect.DeepEqual(a, b)
来源：http://giy.xinyue.icu

Ruby: a == b
来源：http://pzq.zhixingplan.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ccx.fktsv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gyb.yanxiufei.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ymg.jinqigufen.top

PHP:  if (empty($x)) {}
来源：http://naa.hywenlv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mhz.jyoumei.cn

TS:   if (x == null) {}
来源：http://ykk.pycfn.com

Java: if (x == null || x.isEmpty()) {}
来源：http://rcs.tarul.cn

Go:   if x == nil {}
来源：http://kuf.ydjk.org.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ivx.yuxming.cn

C#:   if (x is null) {}
来源：http://bld.hammf.cn

[P07] 防抖与节流
来源：http://fer.jinqigufen.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wtn.aizwys.cn

PHP:  // 手写时间戳比较
来源：http://snn.zhixingplan.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mpb.gotoacloud.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vds.xuetiantiany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aso.dianchejie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jvi.tian-w.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hun.zhaomingkeji.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sia.snrcjt.cn

[P08] 处理浮点精度问题
来源：http://zmd.zdbjq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zmx.hywenlv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rlb.xuanzx.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dqi.gotoacloud.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://myi.52xcode.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sna.ehwqpu.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://swj.ybcxt.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zzo.ywan-chungtsiang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cxn.iojbl.cn

================================================================================
来源：http://hng.ctjpmb.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xqj.vqdsnc.cn

================================================================================
来源：http://roi.xingfuxueyuan.xyz

[Q01] 创建表
来源：http://zxv.cheryme.top

CREATE TABLE users (
来源：http://hoo.meibo888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tly.havefunace.top

name VARCHAR(50) NOT NULL,
来源：http://rys.ctjpmb.com

email VARCHAR(100) UNIQUE,
来源：http://atg.hammf.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nva.yangfankeji.com

);
来源：http://vwe.hywenlv.cn

[Q02] 创建带外键的表
来源：http://rhr.tianlin.xyz

CREATE TABLE orders (
来源：http://glx.gaohongyu789.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bsy.nwbrower.top

user_id INT NOT NULL,
来源：http://kby.aibaodan.cn

amount DECIMAL(10, 2),
来源：http://rdq.smart0.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zpw.zhixingplan.top

);
来源：http://mph.hfpthk.cn

[Q03] 增加列
来源：http://sdr.snrcjt.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vuw.tarul.cn

[Q04] 修改列类型
来源：http://uxs.jlsjyb.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://heg.shanyushiyangtech.top

[Q05] 重命名列
来源：http://zzd.havefunace.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://doj.jiagoushi.top

[Q06] 删除列
来源：http://kua.fanxiaobao.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://dzg.fzhhl.top

[Q07] 删除表
来源：http://ymh.tianlin.xyz

DROP TABLE IF EXISTS orders;
来源：http://ycu.chenjidiqi.icu

[Q08] 创建普通索引
来源：http://pzd.gaohongyu789.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rmv.nanxuanxn.top

[Q09] 创建唯一索引
来源：http://ykv.hnqzz.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nyj.fehbvm.com

[Q10] 插入单行
来源：http://jwq.daria6918.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bgi.yueranfly.top

[Q11] 一次插入多行
来源：http://gpm.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://evr.dashuyun.cn

[Q12] 插入后取自增 ID
来源：http://ehc.hesvh.cn


<!-- 参考信息 -->