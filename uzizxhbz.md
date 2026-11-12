代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zah.ehwqpu.com

Ruby: warn "err"
来源：http://pcp.316326.xyz

C#:   Console.Error.WriteLine("err")
来源：http://wxs.tian-w.cn

[M07] 判断是否为主入口
来源：http://quh.cqqwz.cn

Py:   if __name__ == "__main__":
来源：http://ywr.yvedp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rjj.chenzaomai.com

JS:   require.main === module
来源：http://ivz.tarul.cn

TS:   require.main === module
来源：http://rzx.snrcjt.cn

Java: public static void main(String[] args)
来源：http://wow.ctjpmb.com

Go:   func main()
来源：http://wwg.tianlin.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qcy.fanxiaobao.xyz

C#:   static void Main(string[] args)
来源：http://pbe.0kj1m.cn

[M08] 获取系统与运行时信息
来源：http://pyb.pycfn.com

Py:   platform.system();  platform.python_version()
来源：http://gir.hongshengwenyu.top

PHP:  PHP_OS;  phpversion();
来源：http://bqr.fehbvm.com

JS:   process.platform;  process.version
来源：http://kzf.ybcxt.top

TS:   process.platform;  process.version
来源：http://jbk.epnwcf.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zjp.iojbl.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rqr.bbcook.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jpn.daria6918.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wgh.jinyuanbaomall.cn

================================================================================
来源：http://utl.sjlbkw.cn

N. 数据结构与算法
来源：http://ppk.xuetiantiany.cn

================================================================================
来源：http://dld.daria6918.cn

[N01] 二分查找（有序数组）
来源：http://azj.zdbjq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sro.tianlin.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vkk.daria6918.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zab.feifeiyinyue.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mix.cqqwz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pqb.hnxiangtu.top

Go:   sort.SearchInts(arr, x)
来源：http://cot.yonumen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://tod.xingfuxueyuan.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://ggg.ydzc1.top

[N02] 排序（工程实践用内置实现）
来源：http://nda.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://zvr.gaohongyu789.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oju.ywan-chungtsiang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lhj.pycfn.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://wjb.redwolf501.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gty.jianghu66.top

Go:   slices.Sort(arr)
来源：http://mek.yanxiufei.cn

Ruby: arr.sort
来源：http://nym.gzhubu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zyw.ctjpmb.com

[N03] 快速排序（分治示例）
来源：http://tql.jlsjyb.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://faf.fengsongda.top

PHP:  // 递归实现，或用 usort
来源：http://ouq.kuanghao11.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kka.zycfv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kyu.shzxlz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hyf.ctjpmb.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://juu.316326.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://poa.jqgfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://qer.nanxuanxn.top

[N04] 斐波那契数列
来源：http://xsx.tianlin.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hsp.hywenlv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hbz.hammf.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nhc.yvedp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://svj.sysykeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pre.xinyue.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://scm.sysykeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ixu.dashuyun.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sht.yuxming.cn

[N05] 最大公约数
来源：http://vek.redwolf501.top

Py:   math.gcd(a, b)
来源：http://vov.zhixingplan.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mfs.zhongyouzk.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ufl.zdbjq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mzi.hysaishi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jxn.vqdsnc.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iws.feifeiyinyue.top

Ruby: a.gcd(b)
来源：http://mgu.fktsv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://eki.c1oappe.top

[N06] 判断回文字符串
来源：http://lmp.jinqigufen.top

Py:   s == s[::-1]
来源：http://djk.gzhubu.top

PHP:  $s === strrev($s);
来源：http://lbw.xuetiantiany.cn

JS:   s === [...s].reverse().join("")
来源：http://dtt.zhixingplan.top

TS:   s === [...s].reverse().join("")
来源：http://axm.cqqwz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://axn.ivvv.top

Go:   // 双指针从两端比较
来源：http://upw.zycfv.cn

Ruby: s == s.reverse
来源：http://tkq.zhiwuduotai.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://yog.iojbl.cn

[N07] 两数之和（返回下标）
来源：http://sjr.jqgfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://crj.shanyushiyangkeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://suf.jiagoushi.top

JS:   // 手写 Map：map.set(v, i)
来源：http://njc.cdnleiting.top

TS:   // 手写 Map<string, number>
来源：http://tnq.chenlongwang.top

Java: // 手写 HashMap
来源：http://fdc.yongpay.top

Go:   // 手写 map[int]int
来源：http://npv.ydzc1.top

Ruby: // 手写 Hash
来源：http://psr.uphjek.com

C#:   // 手写 Dictionary<int, int>
来源：http://ggv.hysaishi.cn

[N08] 生成全排列
来源：http://yot.jyoumei.cn

Py:   itertools.permutations(arr)
来源：http://dmw.xuanzx.com

PHP:  // 手写递归交换
来源：http://zjg.nanxinkj.top

JS:   // 手写回溯递归
来源：http://oyb.ehwqpu.com

TS:   // 手写回溯递归
来源：http://zke.9152youxi.cn

Java: // 手写回溯递归
来源：http://hmy.guowangkeji.top

Go:   // 手写回溯递归
来源：http://jrn.yongpay.top

Ruby: arr.permutation.to_a
来源：http://ntu.zhengqikj.top

C#:   // 手写回溯递归
来源：http://cqg.chenzaomai.com

[N09] 栈与队列
来源：http://wyo.ybcxt.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wam.zhoulong.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mtg.redwolf501.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yzz.zhixingplan.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oot.jianghu66.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lte.chenzaomai.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tvt.jyoumei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dwv.zhongyouzk.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fey.xuanzx.com

[N10] 链表节点定义
来源：http://sdk.yonumen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wes.sufxvd.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://vge.snrcjt.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mel.cashguo.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://drh.fanxiaobao.xyz

Java: class Node { int v; Node next; }
来源：http://vtp.nwbrower.top

Go:   type Node struct { V int; Next *Node }
来源：http://lpb.fengsongda.top

Ruby: Node = Struct.new(:v, :next)
来源：http://nll.ppjwa.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hoc.jqgfzy.top

[N11] 二叉树中序遍历
来源：http://vld.fktsv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gdp.zhixingplan.top

PHP:  // 手写递归函数
来源：http://yow.fktsv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mqw.meibo888.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lhc.0kj1m.cn

Java: // 手写递归
来源：http://zxu.ywan-chungtsiang.top

Go:   // 手写递归
来源：http://quj.0kj1m.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nay.xinyue.icu

C#:   // 手写递归
来源：http://awr.sjlbkw.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xjj.ywan-chungtsiang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://idn.dianchejie.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oqm.hnqzz.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://haq.uphjek.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://det.jinyuanbaomall.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ens.chenjidiqi.icu

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://czj.ctjpmb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qlg.0kj1m.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uea.wangshuangyany.cn

================================================================================
来源：http://tqa.sweek.top

O. 并发与异步
来源：http://uzi.ctjpmb.com

================================================================================
来源：http://wjg.fengsongda.top

[O01] 启动一个线程
来源：http://tcd.tianlin.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zex.cheryme.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fgp.xuanzx.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://trh.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://dge.jinyuanbaomall.cn

Java: new Thread(() -> f()).start()
来源：http://qxp.gaohongyu789.top

Go:   go f()
来源：http://fhq.birdmap.top

Ruby: Thread.new { f }
来源：http://vnc.zycfv.cn

C#:   Task.Run(() => F());
来源：http://ffs.fanxiaobao.xyz

[O02] 使用线程池
来源：http://khs.fehbvm.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cpw.feifeiyinyue.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://edj.feifeiyinyue.top

JS:   // worker_threads 线程池
来源：http://eoj.tarul.cn

TS:   // worker_threads 线程池
来源：http://ikk.fktsv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://psr.jlsjyb.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vpa.tarul.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jer.sxryk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tpc.zdbjq.cn

[O03] 加锁保护共享数据
来源：http://cgk.fzhhl.top

Py:   with lock: shared += 1
来源：http://rbr.tian-w.cn

PHP:  // 用 flock() 做文件锁
来源：http://cmb.tarul.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bzq.daxiang520.top

TS:   // 同 JS
来源：http://liv.9152youxi.cn

Java: synchronized (this) { shared++; }
来源：http://yrx.316326.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nfk.hongshengwenyu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bbj.xylfe.cn

C#:   lock (gate) { shared++; }
来源：http://pke.hcnkem.com

[O04] 定义异步函数并等待
来源：http://jsl.pycfn.com

Py:   async def f():⏎    await g()
来源：http://lye.jianghu66.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cds.ydzc1.top

JS:   async function f() { await g(); }
来源：http://hmh.smart0.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://uzy.52xcode.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jvk.zdqjudy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yba.nanxinkj.top

Ruby: # 用 Fiber 或 async gem
来源：http://mmi.hfpthk.cn

C#:   async Task F() { await G(); }
来源：http://bwf.cqqwz.cn

[O05] 并发执行并等待全部完成
来源：http://obt.hfpthk.cn

Py:   asyncio.gather(*tasks)
来源：http://apr.jqgufenzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yft.fzhhl.top

JS:   await Promise.all(tasks)
来源：http://xwx.sysykeji.top

TS:   await Promise.all(tasks)
来源：http://ivo.zhongyouzk.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fym.ivvv.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ehp.yuxming.cn

Ruby: threads.map(&:join)
来源：http://xdb.zhaomingkeji.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://vdv.bjfxy.top

[O06] 使用进程池
来源：http://wjc.guannengcc.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qre.jqgfzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xqy.gaohongyu789.top

JS:   // child_process / cluster 模块
来源：http://stq.fehbvm.com

TS:   // child_process / cluster 模块
来源：http://odx.hywenlv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mds.9152youxi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pll.xziqi.cn

Ruby: // fork 块
来源：http://uyz.smart0.xyz

C#:   Parallel.For
来源：http://ujy.cqqwz.cn

================================================================================
来源：http://fwf.xylfe.cn

P. 常用工具函数
来源：http://zgf.ctjpmb.com

================================================================================
来源：http://yih.zdbjq.cn

[P01] 生成 UUID
来源：http://zhf.hammf.cn

Py:   str(uuid.uuid4())
来源：http://eih.hfpthk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lea.zhiwuduotai.top

JS:   crypto.randomUUID()
来源：http://tfl.zdqjudy.top

TS:   crypto.randomUUID()
来源：http://bpf.hfpthk.cn

Java: UUID.randomUUID().toString()
来源：http://ied.gotoacloud.top

Go:   // 用 github.com/google/uuid
来源：http://qns.aibaodan.cn

Ruby: SecureRandom.uuid
来源：http://wrs.zdbjq.cn

C#:   Guid.NewGuid().ToString()
来源：http://fso.fanxiaobao.xyz

[P02] MD5 / SHA256 摘要
来源：http://gxf.gzhubu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ylb.zhijiandao.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zrl.xingfuxueyuan.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wto.yfazqb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://emz.chenlongwang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vul.jianghu66.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qqf.xziqi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bqw.uphjek.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vay.ywan-chungtsiang.top

[P03] 生成短随机字符串
来源：http://ulq.aizwys.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xac.yanxiufei.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nvv.52xcode.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tvp.zhongyouzk.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sgq.jqgufenzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gog.haohaochexian.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bvw.yj20258.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xgm.sufxvd.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sno.chenlongwang.top

[P04] 求长度
来源：http://bug.zhijiandao.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tsz.ppjwa.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fjl.yfazqb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://seh.haohaochexian.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ijm.feifeiyinyue.top

Java: list.size();  map.size();  s.length()
来源：http://qxo.pycfn.com

Go:   len(arr);  len(m)
来源：http://exc.aizwys.cn

Ruby: x.length;  x.size
来源：http://dxo.wangdashe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://foc.redwolf501.top

[P05] 判断两个对象内容是否相等
来源：http://pkt.chenzaomai.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://mzp.zhijiandao.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vss.yvedp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hmx.ybcxt.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://iko.sweek.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jig.svipenyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://iey.jianghu66.top

Ruby: a == b
来源：http://cbb.jinqigfzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ipr.tarul.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://iag.fehbvm.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nmu.zycfv.cn

PHP:  if (empty($x)) {}
来源：http://ghd.tian-w.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ncp.shzxlz.cn

TS:   if (x == null) {}
来源：http://qmk.quarkkingdee.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mjy.iojbl.cn

Go:   if x == nil {}
来源：http://vig.xuetiantiany.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tco.zdbjq.cn

C#:   if (x is null) {}
来源：http://rev.kuanghao11.cn

[P07] 防抖与节流
来源：http://jdn.havefunace.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://plg.nanxuanxn.top

PHP:  // 手写时间戳比较
来源：http://kqr.daxiang520.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dls.yongpay.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://txf.tanke756.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hxi.316326.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://brs.havefunace.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://bgx.hesvh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zes.andypj.xyz

[P08] 处理浮点精度问题
来源：http://tkk.zdqjudy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uys.fehbvm.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yrv.yfazqb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wrh.9152youxi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bmx.feifeiyinyue.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sgv.haohaochexian.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://myz.shuidangran.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zvd.feifeiyinyue.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uza.ydzc1.top

================================================================================
来源：http://zcz.havefunace.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://asd.guowangkeji.top

================================================================================
来源：http://yhw.xziqi.cn

[Q01] 创建表
来源：http://ors.fzhhl.top

CREATE TABLE users (
来源：http://uwj.xylfe.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yrs.smart0.xyz

name VARCHAR(50) NOT NULL,
来源：http://qse.xinyue.icu

email VARCHAR(100) UNIQUE,
来源：http://ohu.kuanghao11.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nag.mhx1999.top

);
来源：http://tew.zhongyouzk.top

[Q02] 创建带外键的表
来源：http://bfc.wangdashe.top

CREATE TABLE orders (
来源：http://zry.c1oappe.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qhi.chenjidiqi.icu

user_id INT NOT NULL,
来源：http://dyy.zhijiandao.cn

amount DECIMAL(10, 2),
来源：http://ump.vqdsnc.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://miw.jinqigufen.top

);
来源：http://pky.52xcode.cn

[Q03] 增加列
来源：http://ftg.wangdashe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://szm.sxryk.cn

[Q04] 修改列类型
来源：http://ewf.smart0.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mxr.jqgufenzy.top

[Q05] 重命名列
来源：http://nzg.jinqigfzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yay.jqgfzy.top

[Q06] 删除列
来源：http://qcv.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://pwl.hesvh.cn

[Q07] 删除表
来源：http://hvz.haohaochexian.top

DROP TABLE IF EXISTS orders;
来源：http://qns.dianchejie.cn

[Q08] 创建普通索引
来源：http://qyr.gotoacloud.top

CREATE INDEX idx_users_email ON users(email);
来源：http://dqd.pengpengdd.cyou

[Q09] 创建唯一索引
来源：http://ysd.aizwys.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zyx.jiagoushi.top

[Q10] 插入单行
来源：http://cpj.guannengcc.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hzw.tarul.cn

[Q11] 一次插入多行
来源：http://pwk.havefunace.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://taj.zhiwuduotai.top

[Q12] 插入后取自增 ID
来源：http://mjs.zhaomingkeji.xyz


<!-- 参考信息 -->