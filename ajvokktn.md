代发 wailian999

Java: public static void main(String[] args)
来源：http://grx.wangdashe.top

Go:   func main()
来源：http://ubs.shanyushiyangtech.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kqg.zhaomingkeji.xyz

C#:   static void Main(string[] args)
来源：http://gwm.andypj.xyz

[M08] 获取系统与运行时信息
来源：http://ukb.yongpay.top

Py:   platform.system();  platform.python_version()
来源：http://yxx.zdqjudy.top

PHP:  PHP_OS;  phpversion();
来源：http://tzd.fktsv.cn

JS:   process.platform;  process.version
来源：http://xqa.sjlbkw.cn

TS:   process.platform;  process.version
来源：http://wvz.ybcxt.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vqg.jinyuanbaomall.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rtl.iojbl.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cbg.tanke756.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://avr.wangdashe.top

================================================================================
来源：http://jqe.sufxvd.cn

N. 数据结构与算法
来源：http://yad.hysaishi.cn

================================================================================
来源：http://rgd.jinqigfzy.top

[N01] 二分查找（有序数组）
来源：http://eiu.52xcode.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lhh.shanyushiyangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ipg.yfazqb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://daj.hfpthk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://udq.tian-w.cn

Java: Arrays.binarySearch(arr, x)
来源：http://idg.zhiwuduotai.top

Go:   sort.SearchInts(arr, x)
来源：http://vgb.dashuyun.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qah.cucudq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dde.uphjek.com

[N02] 排序（工程实践用内置实现）
来源：http://qcx.yonumen.top

Py:   sorted(arr);  arr.sort()
来源：http://nxj.aibaodan.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aer.xingfuxueyuan.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://ziy.haohaochexian.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://egq.hysaishi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wbu.shuidangran.top

Go:   slices.Sort(arr)
来源：http://pac.fanxiaobao.xyz

Ruby: arr.sort
来源：http://mwv.gzhubu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kof.hnqzz.top

[N03] 快速排序（分治示例）
来源：http://cqx.sysykeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fog.sxryk.cn

PHP:  // 递归实现，或用 usort
来源：http://pap.yuxming.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nrd.gotoacloud.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lpr.shzxlz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nxo.yanxiufei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lrn.bjfxy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ujn.ydzc1.top

C#:   // 手写递归，或 Array.Sort
来源：http://wdk.jinqigfzy.top

[N04] 斐波那契数列
来源：http://kas.jqgfzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tfa.zdbjq.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gjr.gzhubu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bvd.xuetiantiany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aws.quarkkingdee.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hxs.shanyushiyangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ctv.52xcode.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hfo.hammf.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hyo.yfazqb.com

[N05] 最大公约数
来源：http://ohu.pengpengdd.cyou

Py:   math.gcd(a, b)
来源：http://jdx.sjlbkw.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ovu.tianlin.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://erl.daxiang520.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nnc.gotoacloud.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sxg.sysykeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dob.ydzc1.top

Ruby: a.gcd(b)
来源：http://cpf.shangyingyoupin.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://noa.ehwqpu.com

[N06] 判断回文字符串
来源：http://fay.sufxvd.cn

Py:   s == s[::-1]
来源：http://kql.hywenlv.cn

PHP:  $s === strrev($s);
来源：http://rvo.shanyushiyangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://phc.xuanzx.com

TS:   s === [...s].reverse().join("")
来源：http://voa.sysykeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zfg.zhijiandao.cn

Go:   // 双指针从两端比较
来源：http://ssz.chenjidiqi.icu

Ruby: s == s.reverse
来源：http://fda.uphjek.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://tfs.gotoacloud.top

[N07] 两数之和（返回下标）
来源：http://wou.yanxiufei.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hnv.kuanghao11.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aeu.shuidangran.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qmg.jqgufenzy.top

TS:   // 手写 Map<string, number>
来源：http://obs.ppjwa.cn

Java: // 手写 HashMap
来源：http://lpu.fzhhl.top

Go:   // 手写 map[int]int
来源：http://boe.yuanzhike.top

Ruby: // 手写 Hash
来源：http://vkf.0kj1m.cn

C#:   // 手写 Dictionary<int, int>
来源：http://lod.gzhubu.top

[N08] 生成全排列
来源：http://xsx.c1oappe.top

Py:   itertools.permutations(arr)
来源：http://ypy.yangfankeji.com

PHP:  // 手写递归交换
来源：http://goy.yj202588.top

JS:   // 手写回溯递归
来源：http://lyt.hongshengwenyu.top

TS:   // 手写回溯递归
来源：http://dte.hysaishi.cn

Java: // 手写回溯递归
来源：http://qom.yfazqb.com

Go:   // 手写回溯递归
来源：http://uea.xylfe.cn

Ruby: arr.permutation.to_a
来源：http://kaw.9152youxi.cn

C#:   // 手写回溯递归
来源：http://fhs.yuanzhike.top

[N09] 栈与队列
来源：http://pfw.hcnkem.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qrr.shanyushiyangtech.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hyb.smart0.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://vho.xziqi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yco.cashguo.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yey.sjlbkw.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uxo.fktsv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://eic.sufxvd.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ikz.daxiang520.top

[N10] 链表节点定义
来源：http://pcq.jqgufenzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ggi.fktsv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://soq.tarul.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nnu.chenjidiqi.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hxv.tarul.cn

Java: class Node { int v; Node next; }
来源：http://efb.fktsv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rnl.ywan-chungtsiang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://icb.cashguo.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gxc.hongshengwenyu.top

[N11] 二叉树中序遍历
来源：http://xpo.ivvv.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kvs.nanxinkj.top

PHP:  // 手写递归函数
来源：http://ikg.andypj.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://axr.zhaomingkeji.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://awc.tian-w.cn

Java: // 手写递归
来源：http://kqs.shanyushiyangtech.top

Go:   // 手写递归
来源：http://jid.0kj1m.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lbs.ywan-chungtsiang.top

C#:   // 手写递归
来源：http://uqu.hfpthk.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://shk.chenzaomai.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rkg.aizwys.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://siz.wangshuangyany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ogy.jinqigfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iqz.aibaodan.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://knd.hcnkem.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yhr.zhijiandao.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://eny.zhiwuduotai.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xnc.jlsjyb.cn

================================================================================
来源：http://kry.sysykeji.top

O. 并发与异步
来源：http://fht.bjfxy.top

================================================================================
来源：http://qkg.jinqigfzy.top

[O01] 启动一个线程
来源：http://eul.epnwcf.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yjn.daxiang520.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://boi.gzhubu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gbt.zdbjq.cn

TS:   // 同 JS
来源：http://zxl.zhixingplan.top

Java: new Thread(() -> f()).start()
来源：http://chq.bjfxy.top

Go:   go f()
来源：http://qyt.chenjidiqi.icu

Ruby: Thread.new { f }
来源：http://hua.jqgufenzy.top

C#:   Task.Run(() => F());
来源：http://hza.tianlin.xyz

[O02] 使用线程池
来源：http://jlr.dianchejie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zvw.svipenyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pts.dianchejie.cn

JS:   // worker_threads 线程池
来源：http://ucm.0kj1m.cn

TS:   // worker_threads 线程池
来源：http://sqi.smart0.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://twn.jyoumei.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://euo.feifeiyinyue.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://frm.vehdjk.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qga.kuanghao11.cn

[O03] 加锁保护共享数据
来源：http://ols.gogol.net.cn

Py:   with lock: shared += 1
来源：http://wqh.nanxuanxn.top

PHP:  // 用 flock() 做文件锁
来源：http://xni.jianghu66.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zzw.andypj.xyz

TS:   // 同 JS
来源：http://amw.yonumen.top

Java: synchronized (this) { shared++; }
来源：http://pyd.jqgfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mvd.jqgufenzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://iwy.bjfxy.top

C#:   lock (gate) { shared++; }
来源：http://ajs.jinqigufen.top

[O04] 定义异步函数并等待
来源：http://cnx.yj20258.top

Py:   async def f():⏎    await g()
来源：http://tkj.ydzc1.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bnn.jqgufenzy.top

JS:   async function f() { await g(); }
来源：http://cai.ydzc1.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ftm.mhx1999.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wye.yfazqb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ked.quarkkingdee.top

Ruby: # 用 Fiber 或 async gem
来源：http://rck.hcnkem.com

C#:   async Task F() { await G(); }
来源：http://mvt.xuanzx.com

[O05] 并发执行并等待全部完成
来源：http://hyq.nanxinkj.top

Py:   asyncio.gather(*tasks)
来源：http://rku.jyoumei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wcw.gogol.net.cn

JS:   await Promise.all(tasks)
来源：http://hwb.gzhubu.top

TS:   await Promise.all(tasks)
来源：http://oyi.fengsongda.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zav.tarul.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fxp.kuanghao11.cn

Ruby: threads.map(&:join)
来源：http://yok.mhx1999.top

C#:   await Task.WhenAll(t1, t2)
来源：http://gcp.zhengqikj.top

[O06] 使用进程池
来源：http://jlk.ywan-chungtsiang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://phn.zdqjudy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ngc.jqgufenzy.top

JS:   // child_process / cluster 模块
来源：http://vek.shuidangran.top

TS:   // child_process / cluster 模块
来源：http://lmc.wangshuangyany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zdi.yueranfly.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://aca.wangdashe.top

Ruby: // fork 块
来源：http://ykn.pengpengdd.cyou

C#:   Parallel.For
来源：http://fxy.hysaishi.cn

================================================================================
来源：http://hzf.bjfxy.top

P. 常用工具函数
来源：http://iky.jinqigfzy.top

================================================================================
来源：http://imo.haohaochexian.top

[P01] 生成 UUID
来源：http://hmm.hnxiangtu.top

Py:   str(uuid.uuid4())
来源：http://vxd.svipenyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://obg.shuidangran.top

JS:   crypto.randomUUID()
来源：http://mpx.hcnkem.com

TS:   crypto.randomUUID()
来源：http://abc.zhixingplan.top

Java: UUID.randomUUID().toString()
来源：http://ipz.gaohongyu789.top

Go:   // 用 github.com/google/uuid
来源：http://vuf.uphjek.com

Ruby: SecureRandom.uuid
来源：http://msn.zhoulong.xyz

C#:   Guid.NewGuid().ToString()
来源：http://msr.uphjek.com

[P02] MD5 / SHA256 摘要
来源：http://vqo.xinyue.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://liv.hfpthk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kqr.daria6918.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ves.zdbjq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qxj.chenzaomai.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://meb.hywenlv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dua.birdmap.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://goe.shzxlz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://idw.yongpay.top

[P03] 生成短随机字符串
来源：http://scm.yonumen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dzi.fzhhl.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gsa.hysaishi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zea.tian-w.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xca.bjfxy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://unh.cucudq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ruv.haohaochexian.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dao.uphjek.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lel.jyoumei.cn

[P04] 求长度
来源：http://hrd.jinghuilouyu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lxf.hesvh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://awe.ywan-chungtsiang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jlp.sxryk.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wyu.aizwys.cn

Java: list.size();  map.size();  s.length()
来源：http://ajj.cheryme.top

Go:   len(arr);  len(m)
来源：http://nny.hongshengwenyu.top

Ruby: x.length;  x.size
来源：http://lli.yj20258.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://djj.cucudq.cn

[P05] 判断两个对象内容是否相等
来源：http://nje.yj20258.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://snz.wangshuangyany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yli.hywenlv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nfb.zhijiandao.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ydm.ehwqpu.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ezj.yanxiufei.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ivw.yuxming.cn

Ruby: a == b
来源：http://ahb.sjlbkw.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kzb.sufxvd.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uhu.ybcxt.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vql.0kj1m.cn

PHP:  if (empty($x)) {}
来源：http://zrx.shzxlz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fwx.yj202588.top

TS:   if (x == null) {}
来源：http://mmv.hesvh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://aod.zdqjudy.top

Go:   if x == nil {}
来源：http://jnd.sufxvd.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hqf.nanxuanxn.top

C#:   if (x is null) {}
来源：http://qys.ydjk.org.cn

[P07] 防抖与节流
来源：http://zeg.ywan-chungtsiang.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jws.guannengcc.top

PHP:  // 手写时间戳比较
来源：http://qoq.hongshengwenyu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ipm.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zdi.shuidangran.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://shm.sxryk.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eej.shanyushiyangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://umn.andypj.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wzi.shanyushiyangkeji.top

[P08] 处理浮点精度问题
来源：http://iwv.jinqigfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zqz.hywenlv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uqf.kuanghao11.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dwr.shuidangran.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kxw.ybcxt.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hkn.zdbjq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ckc.svipenyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xil.ybcxt.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bdf.xingfuxueyuan.xyz

================================================================================
来源：http://pad.shangyingyoupin.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yzf.ivvv.top

================================================================================
来源：http://qff.ydzc1.top

[Q01] 创建表
来源：http://tiz.9152youxi.cn

CREATE TABLE users (
来源：http://vgf.fanxiaobao.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rbe.hongshengwenyu.top

name VARCHAR(50) NOT NULL,
来源：http://bmh.sweek.top

email VARCHAR(100) UNIQUE,
来源：http://sae.snrcjt.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vfk.hnqzz.top

);
来源：http://bbs.jinyuanbaomall.cn

[Q02] 创建带外键的表
来源：http://scd.c1oappe.top

CREATE TABLE orders (
来源：http://yzs.jianghu66.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tqp.yanxiufei.cn

user_id INT NOT NULL,
来源：http://igo.cqqwz.cn

amount DECIMAL(10, 2),
来源：http://mww.yanxiufei.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jrv.gotoacloud.top

);
来源：http://sgd.wangdashe.top

[Q03] 增加列
来源：http://qkj.mhx1999.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://svk.uphjek.com

[Q04] 修改列类型
来源：http://yvn.hnqzz.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xvo.nwbrower.top

[Q05] 重命名列
来源：http://btj.xziqi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xpq.fktsv.cn

[Q06] 删除列
来源：http://iyk.ivvv.top

ALTER TABLE users DROP COLUMN age;
来源：http://vkv.zhongyouzk.top

[Q07] 删除表
来源：http://tvf.jqgufenzy.top

DROP TABLE IF EXISTS orders;
来源：http://diz.yfazqb.com

[Q08] 创建普通索引
来源：http://qpd.yuxming.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ycv.gotoacloud.top

[Q09] 创建唯一索引
来源：http://ssl.dianchejie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wpk.yvedp.cn

[Q10] 插入单行
来源：http://yzy.yangfankeji.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ano.xuetiantiany.cn

[Q11] 一次插入多行
来源：http://sfl.hesvh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kmm.vehdjk.com

[Q12] 插入后取自增 ID
来源：http://oxl.sweek.top

INSERT INTO users (name) VALUES ('C');
来源：http://ibr.ybcxt.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cic.birdmap.top

[Q13] 忽略重复插入
来源：http://xhj.birdmap.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bfb.xuanzx.com

[Q14] 存在则更新（upsert）
来源：http://uts.xuanzx.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dld.ctjpmb.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wjt.hnxiangtu.top

[Q15] 查询全部
来源：http://zbd.316326.xyz


<!-- 参考信息 -->