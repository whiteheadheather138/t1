代发 wailian999

Ruby: exit 1
来源：http://zgo.fehbvm.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://abf.svipenyu.cn

[M06] 向标准错误输出
来源：http://qrc.ehwqpu.com

Py:   print("err", file=sys.stderr)
来源：http://qmx.hammf.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qym.hongshengwenyu.top

JS:   console.error("err")
来源：http://zjc.nwbrower.top

TS:   console.error("err")
来源：http://nbk.hnxiangtu.top

Java: System.err.println("err")
来源：http://hbi.ydzc1.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qns.xuetiantiany.cn

Ruby: warn "err"
来源：http://kqh.hcnkem.com

C#:   Console.Error.WriteLine("err")
来源：http://obi.yonumen.top

[M07] 判断是否为主入口
来源：http://fpg.c1oappe.top

Py:   if __name__ == "__main__":
来源：http://qga.hnqzz.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jxy.zdqjudy.top

JS:   require.main === module
来源：http://fks.ppjwa.cn

TS:   require.main === module
来源：http://pao.shzxlz.cn

Java: public static void main(String[] args)
来源：http://fqm.vqdsnc.cn

Go:   func main()
来源：http://boy.fengsongda.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://swq.redwolf501.top

C#:   static void Main(string[] args)
来源：http://lpt.cashguo.top

[M08] 获取系统与运行时信息
来源：http://zee.quarkkingdee.top

Py:   platform.system();  platform.python_version()
来源：http://aka.shanyushiyangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://yyi.hysaishi.cn

JS:   process.platform;  process.version
来源：http://cao.aizwys.cn

TS:   process.platform;  process.version
来源：http://zwh.bbcook.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dch.shzxlz.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://vdz.dashuyun.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rpj.ivvv.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fzy.guannengcc.top

================================================================================
来源：http://jac.fzhhl.top

N. 数据结构与算法
来源：http://mvl.kuanghao11.cn

================================================================================
来源：http://xqz.gogol.net.cn

[N01] 二分查找（有序数组）
来源：http://lqy.xinyue.icu

Py:   bisect.bisect_left(arr, x)
来源：http://hue.guannengcc.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ejy.meibo888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wkv.yanxiufei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://snt.shzxlz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uki.cashguo.top

Go:   sort.SearchInts(arr, x)
来源：http://nov.redwolf501.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://asu.jiagoushi.top

C#:   Array.BinarySearch(arr, x)
来源：http://uxv.svipenyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://gfp.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://tcl.birdmap.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sld.yvedp.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bkw.pengpengdd.cyou

TS:   [...arr].sort((a, b) => a - b)
来源：http://ine.hongshengwenyu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mem.hongshengwenyu.top

Go:   slices.Sort(arr)
来源：http://hfk.chenzaomai.com

Ruby: arr.sort
来源：http://wcs.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hzg.zycfv.cn

[N03] 快速排序（分治示例）
来源：http://lnd.hnxiangtu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nep.svipenyu.cn

PHP:  // 递归实现，或用 usort
来源：http://jmb.gotoacloud.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dxk.zycfv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kqo.vqdsnc.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dqb.cashguo.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cru.sxryk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kcw.sweek.top

C#:   // 手写递归，或 Array.Sort
来源：http://pln.shuidangran.top

[N04] 斐波那契数列
来源：http://ihf.chenjidiqi.icu

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://oyu.zhoulong.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sch.yanxiufei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sbz.uphjek.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mjm.zycfv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fky.yonumen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vit.tian-w.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zva.shzxlz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pvr.xingfuxueyuan.xyz

[N05] 最大公约数
来源：http://pkr.fehbvm.com

Py:   math.gcd(a, b)
来源：http://yts.ywan-chungtsiang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://esp.yuxming.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://quw.cashguo.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://evn.zhoulong.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yiw.redwolf501.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://drg.yangfankeji.com

Ruby: a.gcd(b)
来源：http://guy.daria6918.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hbs.guowangkeji.top

[N06] 判断回文字符串
来源：http://kau.zhaomingkeji.xyz

Py:   s == s[::-1]
来源：http://swg.sufxvd.cn

PHP:  $s === strrev($s);
来源：http://ppz.meibo888.top

JS:   s === [...s].reverse().join("")
来源：http://paf.vqdsnc.cn

TS:   s === [...s].reverse().join("")
来源：http://dah.jlsjyb.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gpk.ybcxt.top

Go:   // 双指针从两端比较
来源：http://psp.aizwys.cn

Ruby: s == s.reverse
来源：http://oph.hammf.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://itz.ybcxt.top

[N07] 两数之和（返回下标）
来源：http://qqs.sysykeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gtd.aizwys.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tyf.zhixingplan.top

JS:   // 手写 Map：map.set(v, i)
来源：http://enq.gzhubu.top

TS:   // 手写 Map<string, number>
来源：http://gyi.hfpthk.cn

Java: // 手写 HashMap
来源：http://qrh.wangshuangyany.cn

Go:   // 手写 map[int]int
来源：http://dod.aizwys.cn

Ruby: // 手写 Hash
来源：http://aex.316326.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://wpp.zhiwuduotai.top

[N08] 生成全排列
来源：http://yzr.ctjpmb.com

Py:   itertools.permutations(arr)
来源：http://gtj.chenlongwang.top

PHP:  // 手写递归交换
来源：http://czt.jianghu66.top

JS:   // 手写回溯递归
来源：http://xvw.yj202588.top

TS:   // 手写回溯递归
来源：http://qya.jinqigfzy.top

Java: // 手写回溯递归
来源：http://hiu.hongshengwenyu.top

Go:   // 手写回溯递归
来源：http://phl.tanke756.top

Ruby: arr.permutation.to_a
来源：http://ahg.ydzc1.top

C#:   // 手写回溯递归
来源：http://tag.tanke756.top

[N09] 栈与队列
来源：http://mlw.xziqi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vmw.hesvh.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bse.gaohongyu789.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ltz.cucudq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iag.fanxiaobao.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uti.9152youxi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tlg.xylfe.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qnj.svipenyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mmn.hammf.cn

[N10] 链表节点定义
来源：http://acf.sxryk.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tww.sxryk.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ucj.fehbvm.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ibr.hongshengwenyu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yht.hfpthk.cn

Java: class Node { int v; Node next; }
来源：http://flh.ctjpmb.com

Go:   type Node struct { V int; Next *Node }
来源：http://giw.sjlbkw.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ckc.nwbrower.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hcm.tarul.cn

[N11] 二叉树中序遍历
来源：http://skf.gzhubu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vur.316326.xyz

PHP:  // 手写递归函数
来源：http://ufm.nwbrower.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://awj.birdmap.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jta.chenjidiqi.icu

Java: // 手写递归
来源：http://pfw.yfazqb.com

Go:   // 手写递归
来源：http://qde.sjlbkw.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ozp.hcnkem.com

C#:   // 手写递归
来源：http://psa.cucudq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qsa.xziqi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ggh.havefunace.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dhs.cqqwz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ffb.zhaomingkeji.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://esg.feifeiyinyue.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kbx.mhx1999.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iia.tarul.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pww.dianchejie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qza.zhixingplan.top

================================================================================
来源：http://qmv.guannengcc.top

O. 并发与异步
来源：http://itb.sufxvd.cn

================================================================================
来源：http://pga.vqdsnc.cn

[O01] 启动一个线程
来源：http://pjl.chenlongwang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uwi.fengsongda.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mpl.ybcxt.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xzh.ydjk.org.cn

TS:   // 同 JS
来源：http://skv.hcnkem.com

Java: new Thread(() -> f()).start()
来源：http://bot.gotoacloud.top

Go:   go f()
来源：http://wvt.ywan-chungtsiang.top

Ruby: Thread.new { f }
来源：http://oaa.gaohongyu789.top

C#:   Task.Run(() => F());
来源：http://dns.jinghuilouyu.cn

[O02] 使用线程池
来源：http://xny.0kj1m.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wjc.redwolf501.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rbp.dianchejie.cn

JS:   // worker_threads 线程池
来源：http://amn.aibaodan.cn

TS:   // worker_threads 线程池
来源：http://dny.fanxiaobao.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://vxy.uphjek.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jjn.tarul.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wae.shuidangran.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://khn.yanxiufei.cn

[O03] 加锁保护共享数据
来源：http://mwz.fzhhl.top

Py:   with lock: shared += 1
来源：http://hjg.yj20258.top

PHP:  // 用 flock() 做文件锁
来源：http://ufj.yangfankeji.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://usv.daria6918.cn

TS:   // 同 JS
来源：http://xsi.uphjek.com

Java: synchronized (this) { shared++; }
来源：http://mku.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://raz.fengsongda.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ebc.vqdsnc.cn

C#:   lock (gate) { shared++; }
来源：http://pym.birdmap.top

[O04] 定义异步函数并等待
来源：http://ylv.jinghuilouyu.cn

Py:   async def f():⏎    await g()
来源：http://nzf.tian-w.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rzq.c1oappe.top

JS:   async function f() { await g(); }
来源：http://qno.xuanzx.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://ovj.hnqzz.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vwt.xuetiantiany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://iis.fengsongda.top

Ruby: # 用 Fiber 或 async gem
来源：http://xhp.yj20258.top

C#:   async Task F() { await G(); }
来源：http://xkv.andypj.xyz

[O05] 并发执行并等待全部完成
来源：http://otl.bbcook.cn

Py:   asyncio.gather(*tasks)
来源：http://kfa.tianlin.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lsm.aizwys.cn

JS:   await Promise.all(tasks)
来源：http://ijp.shangyingyoupin.top

TS:   await Promise.all(tasks)
来源：http://qyl.chenjidiqi.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eyo.andypj.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cxi.zdqjudy.top

Ruby: threads.map(&:join)
来源：http://ydd.guannengcc.top

C#:   await Task.WhenAll(t1, t2)
来源：http://vtb.cdnleiting.top

[O06] 使用进程池
来源：http://jcj.52xcode.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hjd.ydjk.org.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://udt.sweek.top

JS:   // child_process / cluster 模块
来源：http://tay.jqgufenzy.top

TS:   // child_process / cluster 模块
来源：http://lhy.hammf.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zkf.fehbvm.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ewl.nanxuanxn.top

Ruby: // fork 块
来源：http://pnn.aibaodan.cn

C#:   Parallel.For
来源：http://zvd.shangyingyoupin.top

================================================================================
来源：http://yad.jqgufenzy.top

P. 常用工具函数
来源：http://zkb.yvedp.cn

================================================================================
来源：http://rxj.gaohongyu789.top

[P01] 生成 UUID
来源：http://srt.sysykeji.top

Py:   str(uuid.uuid4())
来源：http://pbe.xylfe.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lqu.cqqwz.cn

JS:   crypto.randomUUID()
来源：http://qik.jqgufenzy.top

TS:   crypto.randomUUID()
来源：http://hka.fehbvm.com

Java: UUID.randomUUID().toString()
来源：http://ggy.gogol.net.cn

Go:   // 用 github.com/google/uuid
来源：http://kjg.ppjwa.cn

Ruby: SecureRandom.uuid
来源：http://nxu.xuetiantiany.cn

C#:   Guid.NewGuid().ToString()
来源：http://kkl.vqdsnc.cn

[P02] MD5 / SHA256 摘要
来源：http://hyb.guannengcc.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sdk.sxryk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vjf.gotoacloud.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oav.redwolf501.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xhv.pycfn.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zsf.nwbrower.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jxl.jqgfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uvb.ybcxt.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xst.havefunace.top

[P03] 生成短随机字符串
来源：http://aro.jinqigufen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wjo.ivvv.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rsg.feifeiyinyue.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oba.jqgufenzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yhb.hysaishi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pgh.jiagoushi.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ngq.haohaochexian.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zcw.gogol.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rtr.shanyushiyangkeji.top

[P04] 求长度
来源：http://vde.bbcook.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://haz.nwbrower.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qju.dashuyun.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lao.bbcook.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sph.tian-w.cn

Java: list.size();  map.size();  s.length()
来源：http://jgw.jinghuilouyu.cn

Go:   len(arr);  len(m)
来源：http://uku.yongpay.top

Ruby: x.length;  x.size
来源：http://vds.haohaochexian.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fet.hfpthk.cn

[P05] 判断两个对象内容是否相等
来源：http://xcg.andypj.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://wmk.xinyue.icu

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tvo.fehbvm.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qds.shuidangran.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hya.bbcook.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qtp.yj202588.top

Go:   reflect.DeepEqual(a, b)
来源：http://knb.zhiwuduotai.top

Ruby: a == b
来源：http://cce.tanke756.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://flt.52xcode.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://snm.uphjek.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://owt.daxiang520.top

PHP:  if (empty($x)) {}
来源：http://zdo.0kj1m.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ixx.cheryme.top

TS:   if (x == null) {}
来源：http://kdf.hesvh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ldz.hongshengwenyu.top

Go:   if x == nil {}
来源：http://isr.dianchejie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xlg.vehdjk.com

C#:   if (x is null) {}
来源：http://rrb.vqdsnc.cn

[P07] 防抖与节流
来源：http://xax.hfpthk.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jys.ppjwa.cn

PHP:  // 手写时间戳比较
来源：http://nen.mhx1999.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pqz.cqqwz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mvw.quarkkingdee.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wfh.ctjpmb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nee.hnqzz.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zsc.xuanzx.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fzc.snrcjt.cn

[P08] 处理浮点精度问题
来源：http://fzu.zhengqikj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sir.daxiang520.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xuz.chenzaomai.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bnj.jinghuilouyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xmh.ehwqpu.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cbn.yj20258888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wxt.smart0.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mss.wangshuangyany.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ikd.gzhubu.top

================================================================================
来源：http://pmh.sufxvd.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jlc.9152youxi.cn

================================================================================
来源：http://skd.feifeiyinyue.top

[Q01] 创建表
来源：http://qsd.fehbvm.com

CREATE TABLE users (
来源：http://ayf.yfazqb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pbr.guowangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://pwr.9152youxi.cn

email VARCHAR(100) UNIQUE,
来源：http://nop.tianlin.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://akk.iojbl.cn

);
来源：http://xxs.jinqigfzy.top

[Q02] 创建带外键的表
来源：http://qge.jianghu66.top

CREATE TABLE orders (
来源：http://wiy.haohaochexian.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wio.hysaishi.cn

user_id INT NOT NULL,
来源：http://pkk.vqdsnc.cn

amount DECIMAL(10, 2),
来源：http://tlt.hywenlv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pnb.yanxiufei.cn

);
来源：http://uvk.tianlin.xyz

[Q03] 增加列
来源：http://mrb.aizwys.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ega.nwbrower.top

[Q04] 修改列类型
来源：http://qrh.jiagoushi.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xmc.daxiang520.top

[Q05] 重命名列
来源：http://yxu.epnwcf.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gzo.jinqigfzy.top

[Q06] 删除列
来源：http://qho.vqdsnc.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fgy.jiagoushi.top

[Q07] 删除表
来源：http://waz.hfpthk.cn

DROP TABLE IF EXISTS orders;
来源：http://myh.zhengqikj.top

[Q08] 创建普通索引
来源：http://zxu.tian-w.cn


<!-- 参考信息 -->