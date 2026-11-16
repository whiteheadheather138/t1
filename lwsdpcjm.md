代发 wailian999

Java: public static void main(String[] args)
来源：http://hmx.havefunace.top

Go:   func main()
来源：http://nsb.zdbjq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xbx.gotoacloud.top

C#:   static void Main(string[] args)
来源：http://bqq.zhoulong.xyz

[M08] 获取系统与运行时信息
来源：http://iku.c1oappe.top

Py:   platform.system();  platform.python_version()
来源：http://mvc.andypj.xyz

PHP:  PHP_OS;  phpversion();
来源：http://vrf.cheryme.top

JS:   process.platform;  process.version
来源：http://xpd.sufxvd.cn

TS:   process.platform;  process.version
来源：http://uef.nwbrower.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xrd.tarul.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://hme.0kj1m.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rra.shuidangran.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ruf.nwbrower.top

================================================================================
来源：http://ayf.9152youxi.cn

N. 数据结构与算法
来源：http://doe.zhoulong.xyz

================================================================================
来源：http://jyj.dianchejie.cn

[N01] 二分查找（有序数组）
来源：http://hxe.c1oappe.top

Py:   bisect.bisect_left(arr, x)
来源：http://iha.xuetiantiany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ipu.uphjek.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kmw.fengsongda.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nwn.zhijiandao.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ylt.aibaodan.cn

Go:   sort.SearchInts(arr, x)
来源：http://ezx.ctjpmb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://egt.cheryme.top

C#:   Array.BinarySearch(arr, x)
来源：http://qsn.fktsv.cn

[N02] 排序（工程实践用内置实现）
来源：http://lut.52xcode.cn

Py:   sorted(arr);  arr.sort()
来源：http://cjx.yueranfly.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://obi.mhx1999.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ptu.havefunace.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wxz.hnqzz.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pbl.quarkkingdee.top

Go:   slices.Sort(arr)
来源：http://jhm.zdqjudy.top

Ruby: arr.sort
来源：http://yxs.tarul.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wqm.yanxiufei.cn

[N03] 快速排序（分治示例）
来源：http://ctw.fengsongda.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gom.jyoumei.cn

PHP:  // 递归实现，或用 usort
来源：http://yqw.jinyuanbaomall.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wel.xuetiantiany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rzh.ivvv.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dqg.zdqjudy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pmw.yueranfly.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://chs.andypj.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://bkb.bjfxy.top

[N04] 斐波那契数列
来源：http://jtd.vqdsnc.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://txa.zdbjq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sxk.birdmap.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://abc.yangfankeji.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qvu.yonumen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bag.cheryme.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kgp.quarkkingdee.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hsd.c1oappe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eor.fanxiaobao.xyz

[N05] 最大公约数
来源：http://pdh.hywenlv.cn

Py:   math.gcd(a, b)
来源：http://xma.nwbrower.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zqn.bbcook.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tka.yuanzhike.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wbi.yvedp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://muj.wangshuangyany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lkz.xuetiantiany.cn

Ruby: a.gcd(b)
来源：http://uym.birdmap.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ydj.birdmap.top

[N06] 判断回文字符串
来源：http://ksx.sjlbkw.cn

Py:   s == s[::-1]
来源：http://fse.ivvv.top

PHP:  $s === strrev($s);
来源：http://fam.iojbl.cn

JS:   s === [...s].reverse().join("")
来源：http://ikp.ywan-chungtsiang.top

TS:   s === [...s].reverse().join("")
来源：http://doq.zhiwuduotai.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://klu.daxiang520.top

Go:   // 双指针从两端比较
来源：http://xqn.xylfe.cn

Ruby: s == s.reverse
来源：http://chl.xinyue.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://irh.andypj.xyz

[N07] 两数之和（返回下标）
来源：http://zka.aibaodan.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://syv.fengsongda.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zfy.aizwys.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://juf.tian-w.cn

TS:   // 手写 Map<string, number>
来源：http://sxg.redwolf501.top

Java: // 手写 HashMap
来源：http://alw.yj20258888.top

Go:   // 手写 map[int]int
来源：http://icw.cashguo.top

Ruby: // 手写 Hash
来源：http://swf.bbcook.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ykk.chenlongwang.top

[N08] 生成全排列
来源：http://zpz.sjlbkw.cn

Py:   itertools.permutations(arr)
来源：http://qun.shangyingyoupin.top

PHP:  // 手写递归交换
来源：http://gwg.ybcxt.top

JS:   // 手写回溯递归
来源：http://rsg.aizwys.cn

TS:   // 手写回溯递归
来源：http://bjo.cashguo.top

Java: // 手写回溯递归
来源：http://eli.ybcxt.top

Go:   // 手写回溯递归
来源：http://tra.yangfankeji.com

Ruby: arr.permutation.to_a
来源：http://twu.hnxiangtu.top

C#:   // 手写回溯递归
来源：http://suf.pengpengdd.cyou

[N09] 栈与队列
来源：http://sxg.kuanghao11.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cij.bbcook.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://vvi.c1oappe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ovc.wangshuangyany.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://act.sufxvd.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hcd.hongshengwenyu.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ecy.zycfv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dfk.hfpthk.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://aek.jianghu66.top

[N10] 链表节点定义
来源：http://rts.gogol.net.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wwo.wangdashe.top

PHP:  class Node { public $v; public $next = null; }
来源：http://hwr.fanxiaobao.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pus.sweek.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tre.jinqigufen.top

Java: class Node { int v; Node next; }
来源：http://mud.xingfuxueyuan.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://odj.xylfe.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zpu.ybcxt.top

C#:   class Node { public int V; public Node? Next; }
来源：http://yzc.nanxinkj.top

[N11] 二叉树中序遍历
来源：http://enn.nanxinkj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yan.ydzc1.top

PHP:  // 手写递归函数
来源：http://mpv.xuanzx.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ayy.fktsv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fuw.gzhubu.top

Java: // 手写递归
来源：http://rnv.bbcook.cn

Go:   // 手写递归
来源：http://jxg.cucudq.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wpq.hongshengwenyu.top

C#:   // 手写递归
来源：http://cam.havefunace.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fpq.birdmap.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://his.ctjpmb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uhv.xylfe.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cmr.daria6918.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hlo.nanxuanxn.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://umd.sysykeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pel.chenlongwang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://piw.snrcjt.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vuu.ydzc1.top

================================================================================
来源：http://hjc.shangyingyoupin.top

O. 并发与异步
来源：http://tss.ivvv.top

================================================================================
来源：http://jpv.gaohongyu789.top

[O01] 启动一个线程
来源：http://qnk.sysykeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zfu.zhengqikj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rfc.tian-w.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qpa.ybcxt.top

TS:   // 同 JS
来源：http://zqd.cheryme.top

Java: new Thread(() -> f()).start()
来源：http://tek.hnqzz.top

Go:   go f()
来源：http://jaj.jinyuanbaomall.cn

Ruby: Thread.new { f }
来源：http://ceu.chenjidiqi.icu

C#:   Task.Run(() => F());
来源：http://yxb.yuxming.cn

[O02] 使用线程池
来源：http://ykh.jinyuanbaomall.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nkg.jlsjyb.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tkc.hammf.cn

JS:   // worker_threads 线程池
来源：http://ntm.cucudq.cn

TS:   // worker_threads 线程池
来源：http://uba.ivvv.top

Java: Executors.newFixedThreadPool(4)
来源：http://jlr.iojbl.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fbf.haohaochexian.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xmz.wangshuangyany.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zio.yfazqb.com

[O03] 加锁保护共享数据
来源：http://jyk.cdnleiting.top

Py:   with lock: shared += 1
来源：http://rzf.jinqigfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://iri.gaohongyu789.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qxa.sxryk.cn

TS:   // 同 JS
来源：http://tml.52xcode.cn

Java: synchronized (this) { shared++; }
来源：http://toh.hongshengwenyu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rhu.zhiwuduotai.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tkr.gogol.net.cn

C#:   lock (gate) { shared++; }
来源：http://gpu.yongpay.top

[O04] 定义异步函数并等待
来源：http://ydb.9152youxi.cn

Py:   async def f():⏎    await g()
来源：http://frh.yueranfly.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qja.zdqjudy.top

JS:   async function f() { await g(); }
来源：http://tar.0kj1m.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://itj.hysaishi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rcq.birdmap.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vdt.yonumen.top

Ruby: # 用 Fiber 或 async gem
来源：http://wge.fanxiaobao.xyz

C#:   async Task F() { await G(); }
来源：http://dyd.pengpengdd.cyou

[O05] 并发执行并等待全部完成
来源：http://jwy.fehbvm.com

Py:   asyncio.gather(*tasks)
来源：http://cbp.sjlbkw.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ymi.sweek.top

JS:   await Promise.all(tasks)
来源：http://bgc.fehbvm.com

TS:   await Promise.all(tasks)
来源：http://epz.tarul.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pwl.ctjpmb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://euj.andypj.xyz

Ruby: threads.map(&:join)
来源：http://vcc.hnqzz.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mtz.jqgufenzy.top

[O06] 使用进程池
来源：http://nza.tianlin.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tbk.yuxming.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://sfm.52xcode.cn

JS:   // child_process / cluster 模块
来源：http://jog.yj202588.top

TS:   // child_process / cluster 模块
来源：http://bde.ydjk.org.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sib.yongpay.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ddi.shuidangran.top

Ruby: // fork 块
来源：http://apd.xingfuxueyuan.xyz

C#:   Parallel.For
来源：http://bdz.bbcook.cn

================================================================================
来源：http://wsm.hywenlv.cn

P. 常用工具函数
来源：http://hzs.pycfn.com

================================================================================
来源：http://bzm.sufxvd.cn

[P01] 生成 UUID
来源：http://msg.jinghuilouyu.cn

Py:   str(uuid.uuid4())
来源：http://zfk.xziqi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jwa.mhx1999.top

JS:   crypto.randomUUID()
来源：http://okw.guannengcc.top

TS:   crypto.randomUUID()
来源：http://rqp.tian-w.cn

Java: UUID.randomUUID().toString()
来源：http://eik.havefunace.top

Go:   // 用 github.com/google/uuid
来源：http://kng.pengpengdd.cyou

Ruby: SecureRandom.uuid
来源：http://jqf.yonumen.top

C#:   Guid.NewGuid().ToString()
来源：http://sbp.smart0.xyz

[P02] MD5 / SHA256 摘要
来源：http://hlg.bjfxy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bdu.hnxiangtu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://cnm.gogol.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pzc.yj202588.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jwd.iojbl.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://doe.yj202588.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://whv.dashuyun.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nvr.hywenlv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rxt.wangdashe.top

[P03] 生成短随机字符串
来源：http://bfw.ywan-chungtsiang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://joz.haohaochexian.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ivf.fzhhl.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jfi.bjfxy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://opg.chenjidiqi.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kky.bjfxy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://myp.shuidangran.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://jvp.pengpengdd.cyou

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xqi.iojbl.cn

[P04] 求长度
来源：http://wcv.snrcjt.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mew.uphjek.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://off.chenlongwang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xzp.uphjek.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://frg.yongpay.top

Java: list.size();  map.size();  s.length()
来源：http://fcb.xziqi.cn

Go:   len(arr);  len(m)
来源：http://fez.zhijiandao.cn

Ruby: x.length;  x.size
来源：http://lzo.smart0.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://krm.bbcook.cn

[P05] 判断两个对象内容是否相等
来源：http://qnb.shanyushiyangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zoy.xuanzx.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qim.shzxlz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://shv.jinqigfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ogb.ydjk.org.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uri.snrcjt.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xwq.wangdashe.top

Ruby: a == b
来源：http://cnv.aibaodan.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ayu.fanxiaobao.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mes.zhiwuduotai.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tji.yj20258888.top

PHP:  if (empty($x)) {}
来源：http://ndp.jlsjyb.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wpz.bjfxy.top

TS:   if (x == null) {}
来源：http://cay.xinyue.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://zzs.feifeiyinyue.top

Go:   if x == nil {}
来源：http://hyj.hcnkem.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://seb.ctjpmb.com

C#:   if (x is null) {}
来源：http://vuc.hcnkem.com

[P07] 防抖与节流
来源：http://waj.daxiang520.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fif.daxiang520.top

PHP:  // 手写时间戳比较
来源：http://wml.yuanzhike.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wav.yvedp.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ghq.guowangkeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lcp.feifeiyinyue.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pvu.52xcode.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cpx.0kj1m.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dhb.fengsongda.top

[P08] 处理浮点精度问题
来源：http://tyj.fktsv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kfh.yueranfly.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fiw.andypj.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://suw.xziqi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dxt.feifeiyinyue.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qik.hnqzz.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nmp.fanxiaobao.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zbw.zhengqikj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fqb.kuanghao11.cn

================================================================================
来源：http://twa.ppjwa.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uvy.ctjpmb.com

================================================================================
来源：http://bkb.gogol.net.cn

[Q01] 创建表
来源：http://srf.feifeiyinyue.top

CREATE TABLE users (
来源：http://hlq.xingfuxueyuan.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vtc.redwolf501.top

name VARCHAR(50) NOT NULL,
来源：http://epq.jinghuilouyu.cn

email VARCHAR(100) UNIQUE,
来源：http://aib.9152youxi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://euz.yuanzhike.top

);
来源：http://ybe.sufxvd.cn

[Q02] 创建带外键的表
来源：http://iug.fzhhl.top

CREATE TABLE orders (
来源：http://cqa.vehdjk.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yag.dianchejie.cn

user_id INT NOT NULL,
来源：http://nsl.jqgufenzy.top

amount DECIMAL(10, 2),
来源：http://cfj.chenlongwang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bbj.yonumen.top

);
来源：http://jbw.hammf.cn

[Q03] 增加列
来源：http://kuq.jqgufenzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dup.shzxlz.cn

[Q04] 修改列类型
来源：http://yrk.redwolf501.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ubg.tian-w.cn

[Q05] 重命名列
来源：http://oui.fanxiaobao.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dfn.yj202588.top

[Q06] 删除列
来源：http://ofq.zdqjudy.top

ALTER TABLE users DROP COLUMN age;
来源：http://qsj.nwbrower.top

[Q07] 删除表
来源：http://ijr.xuetiantiany.cn

DROP TABLE IF EXISTS orders;
来源：http://lwn.snrcjt.cn

[Q08] 创建普通索引
来源：http://exp.0kj1m.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://joe.fktsv.cn

[Q09] 创建唯一索引
来源：http://twq.jlsjyb.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://leg.fzhhl.top

[Q10] 插入单行
来源：http://zns.xingfuxueyuan.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://smj.fanxiaobao.xyz

[Q11] 一次插入多行
来源：http://tcg.mhx1999.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lll.cdnleiting.top

[Q12] 插入后取自增 ID
来源：http://qva.sxryk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xku.vehdjk.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cup.cdnleiting.top

[Q13] 忽略重复插入
来源：http://pag.yanxiufei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pes.vehdjk.com

[Q14] 存在则更新（upsert）
来源：http://bxv.ehwqpu.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qeb.xziqi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://imp.ivvv.top

[Q15] 查询全部
来源：http://lrg.jianghu66.top


<!-- 参考信息 -->