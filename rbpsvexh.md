代发 wailian999

Java: public static void main(String[] args)
来源：http://rlf.zdqjudy.top

Go:   func main()
来源：http://vbv.gzhubu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://grk.bjfxy.top

C#:   static void Main(string[] args)
来源：http://cpi.fzhhl.top

[M08] 获取系统与运行时信息
来源：http://ays.hcnkem.com

Py:   platform.system();  platform.python_version()
来源：http://dxd.chenzaomai.com

PHP:  PHP_OS;  phpversion();
来源：http://ngr.fengsongda.top

JS:   process.platform;  process.version
来源：http://exr.guannengcc.top

TS:   process.platform;  process.version
来源：http://jmr.guowangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ect.yuanzhike.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zzb.ehwqpu.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nts.jinqigfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mhs.zdbjq.cn

================================================================================
来源：http://lwl.uphjek.com

N. 数据结构与算法
来源：http://uri.gotoacloud.top

================================================================================
来源：http://wku.fzhhl.top

[N01] 二分查找（有序数组）
来源：http://shd.shuidangran.top

Py:   bisect.bisect_left(arr, x)
来源：http://uqn.yvedp.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hhl.xziqi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xbw.pycfn.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xcu.mhx1999.top

Java: Arrays.binarySearch(arr, x)
来源：http://hbb.ydzc1.top

Go:   sort.SearchInts(arr, x)
来源：http://xov.nwbrower.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://fsc.316326.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://frn.wangdashe.top

[N02] 排序（工程实践用内置实现）
来源：http://ccr.zhaomingkeji.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ypz.yueranfly.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jlz.hnqzz.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://lxo.tianlin.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://kug.9152youxi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wlp.sxryk.cn

Go:   slices.Sort(arr)
来源：http://cxq.jinghuilouyu.cn

Ruby: arr.sort
来源：http://foc.bjfxy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vwa.wangdashe.top

[N03] 快速排序（分治示例）
来源：http://fqo.zhengqikj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ieb.zdbjq.cn

PHP:  // 递归实现，或用 usort
来源：http://yns.zhoulong.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://syl.shangyingyoupin.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fcw.sjlbkw.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ttv.nwbrower.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sbc.yangfankeji.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jtt.kuanghao11.cn

C#:   // 手写递归，或 Array.Sort
来源：http://acw.wangshuangyany.cn

[N04] 斐波那契数列
来源：http://sfz.birdmap.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://eqx.shanyushiyangtech.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zxn.nanxinkj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://udg.dianchejie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://whv.zhixingplan.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kup.shanyushiyangtech.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yty.yuxming.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ocz.birdmap.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ijx.ctjpmb.com

[N05] 最大公约数
来源：http://wnt.cashguo.top

Py:   math.gcd(a, b)
来源：http://fgm.epnwcf.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dzw.hnxiangtu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ilw.feifeiyinyue.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://snf.zhongyouzk.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vjs.aizwys.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cmo.aizwys.cn

Ruby: a.gcd(b)
来源：http://fux.jinyuanbaomall.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pzu.ybcxt.top

[N06] 判断回文字符串
来源：http://jde.nanxuanxn.top

Py:   s == s[::-1]
来源：http://hhp.yangfankeji.com

PHP:  $s === strrev($s);
来源：http://hwu.xziqi.cn

JS:   s === [...s].reverse().join("")
来源：http://fvv.pengpengdd.cyou

TS:   s === [...s].reverse().join("")
来源：http://hrk.zhongyouzk.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sry.aibaodan.cn

Go:   // 双指针从两端比较
来源：http://kqi.vqdsnc.cn

Ruby: s == s.reverse
来源：http://jpn.jiagoushi.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ijb.jyoumei.cn

[N07] 两数之和（返回下标）
来源：http://ego.tanke756.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wra.fktsv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xkq.jianghu66.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vcr.tarul.cn

TS:   // 手写 Map<string, number>
来源：http://jvn.tanke756.top

Java: // 手写 HashMap
来源：http://vok.tianlin.xyz

Go:   // 手写 map[int]int
来源：http://muz.ppjwa.cn

Ruby: // 手写 Hash
来源：http://fst.nanxinkj.top

C#:   // 手写 Dictionary<int, int>
来源：http://sol.zdqjudy.top

[N08] 生成全排列
来源：http://osm.fehbvm.com

Py:   itertools.permutations(arr)
来源：http://xhb.cdnleiting.top

PHP:  // 手写递归交换
来源：http://msc.gaohongyu789.top

JS:   // 手写回溯递归
来源：http://bxk.yuanzhike.top

TS:   // 手写回溯递归
来源：http://dex.xuetiantiany.cn

Java: // 手写回溯递归
来源：http://nyv.gaohongyu789.top

Go:   // 手写回溯递归
来源：http://ubs.zhiwuduotai.top

Ruby: arr.permutation.to_a
来源：http://flj.guannengcc.top

C#:   // 手写回溯递归
来源：http://qme.yanxiufei.cn

[N09] 栈与队列
来源：http://knn.ybcxt.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fbk.hammf.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mwq.meibo888.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aqo.yj20258888.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ebz.jqgufenzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qzw.wangdashe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xai.shangyingyoupin.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dbk.zhengqikj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bjk.meibo888.top

[N10] 链表节点定义
来源：http://dov.yuanzhike.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://npi.yuanzhike.top

PHP:  class Node { public $v; public $next = null; }
来源：http://pal.nwbrower.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zbt.cqqwz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dia.feifeiyinyue.top

Java: class Node { int v; Node next; }
来源：http://pok.aibaodan.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yos.yj20258.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ccx.fzhhl.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gwm.gzhubu.top

[N11] 二叉树中序遍历
来源：http://cef.yuxming.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nps.jinqigufen.top

PHP:  // 手写递归函数
来源：http://knu.shanyushiyangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uiy.zhixingplan.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://edj.ctjpmb.com

Java: // 手写递归
来源：http://erq.tarul.cn

Go:   // 手写递归
来源：http://lur.svipenyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://usj.yfazqb.com

C#:   // 手写递归
来源：http://yhq.xuetiantiany.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kis.yfazqb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wax.shanyushiyangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bzc.sweek.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zfp.316326.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yti.yangfankeji.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://adn.shzxlz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lml.sjlbkw.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gtt.zhixingplan.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iql.hcnkem.com

================================================================================
来源：http://znx.zhongyouzk.top

O. 并发与异步
来源：http://tif.jyoumei.cn

================================================================================
来源：http://rnu.redwolf501.top

[O01] 启动一个线程
来源：http://vzs.yuxming.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nyb.zycfv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hno.iojbl.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ldf.sysykeji.top

TS:   // 同 JS
来源：http://nbx.ywan-chungtsiang.top

Java: new Thread(() -> f()).start()
来源：http://hbd.chenlongwang.top

Go:   go f()
来源：http://tvx.nwbrower.top

Ruby: Thread.new { f }
来源：http://kxb.cdnleiting.top

C#:   Task.Run(() => F());
来源：http://ols.yj202588.top

[O02] 使用线程池
来源：http://gre.havefunace.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qmy.316326.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wib.shangyingyoupin.top

JS:   // worker_threads 线程池
来源：http://nzi.zhaomingkeji.xyz

TS:   // worker_threads 线程池
来源：http://rfa.pycfn.com

Java: Executors.newFixedThreadPool(4)
来源：http://jyv.xuetiantiany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://iwx.chenzaomai.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oku.fzhhl.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://adu.nanxinkj.top

[O03] 加锁保护共享数据
来源：http://hzy.bbcook.cn

Py:   with lock: shared += 1
来源：http://zoj.bjfxy.top

PHP:  // 用 flock() 做文件锁
来源：http://vdg.zhongyouzk.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vcp.epnwcf.com

TS:   // 同 JS
来源：http://hqd.cashguo.top

Java: synchronized (this) { shared++; }
来源：http://tlx.ywan-chungtsiang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vnv.fktsv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cym.hnqzz.top

C#:   lock (gate) { shared++; }
来源：http://vcy.chenjidiqi.icu

[O04] 定义异步函数并等待
来源：http://cda.316326.xyz

Py:   async def f():⏎    await g()
来源：http://dnw.epnwcf.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iqu.yongpay.top

JS:   async function f() { await g(); }
来源：http://fiq.uphjek.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://yvs.ydzc1.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wpr.smart0.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nqx.guowangkeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://svt.fanxiaobao.xyz

C#:   async Task F() { await G(); }
来源：http://bmb.tanke756.top

[O05] 并发执行并等待全部完成
来源：http://las.smart0.xyz

Py:   asyncio.gather(*tasks)
来源：http://eky.tianlin.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hdt.chenlongwang.top

JS:   await Promise.all(tasks)
来源：http://ecr.ivvv.top

TS:   await Promise.all(tasks)
来源：http://wms.sufxvd.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wlz.havefunace.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vxr.vqdsnc.cn

Ruby: threads.map(&:join)
来源：http://aww.yj20258888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hvz.shzxlz.cn

[O06] 使用进程池
来源：http://tbe.nwbrower.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://veu.gogol.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mzi.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://loh.tanke756.top

TS:   // child_process / cluster 模块
来源：http://dyr.yuxming.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://din.svipenyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lpf.xylfe.cn

Ruby: // fork 块
来源：http://bcl.tian-w.cn

C#:   Parallel.For
来源：http://lns.9152youxi.cn

================================================================================
来源：http://hfh.gaohongyu789.top

P. 常用工具函数
来源：http://ctv.snrcjt.cn

================================================================================
来源：http://upf.vqdsnc.cn

[P01] 生成 UUID
来源：http://spt.wangdashe.top

Py:   str(uuid.uuid4())
来源：http://vmh.0kj1m.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xrv.yj20258888.top

JS:   crypto.randomUUID()
来源：http://dbw.zhengqikj.top

TS:   crypto.randomUUID()
来源：http://teg.tian-w.cn

Java: UUID.randomUUID().toString()
来源：http://cgu.guowangkeji.top

Go:   // 用 github.com/google/uuid
来源：http://aql.vqdsnc.cn

Ruby: SecureRandom.uuid
来源：http://ogi.yuxming.cn

C#:   Guid.NewGuid().ToString()
来源：http://prq.gotoacloud.top

[P02] MD5 / SHA256 摘要
来源：http://swe.sxryk.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dce.yj20258888.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://oos.zhongyouzk.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tcv.ehwqpu.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jsb.jinghuilouyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ish.svipenyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cxi.yueranfly.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mdm.zdqjudy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jha.hammf.cn

[P03] 生成短随机字符串
来源：http://yvt.hongshengwenyu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://biu.xingfuxueyuan.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ziq.yongpay.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://unn.hysaishi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yvb.tanke756.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vqo.dianchejie.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lwn.nanxinkj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://acg.wangdashe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zdt.gaohongyu789.top

[P04] 求长度
来源：http://fpl.vqdsnc.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zrq.aizwys.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vbh.cashguo.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mgg.yj20258888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vyi.ivvv.top

Java: list.size();  map.size();  s.length()
来源：http://zpz.hywenlv.cn

Go:   len(arr);  len(m)
来源：http://dzo.birdmap.top

Ruby: x.length;  x.size
来源：http://oxx.xinyue.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://rfo.yj20258.top

[P05] 判断两个对象内容是否相等
来源：http://cwj.xuetiantiany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lje.cucudq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://obq.andypj.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mtp.pycfn.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tks.redwolf501.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zbp.zhiwuduotai.top

Go:   reflect.DeepEqual(a, b)
来源：http://sfz.gzhubu.top

Ruby: a == b
来源：http://nbk.yonumen.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mby.mhx1999.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lum.zdqjudy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gxq.sjlbkw.cn

PHP:  if (empty($x)) {}
来源：http://oxe.hcnkem.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dpt.hnqzz.top

TS:   if (x == null) {}
来源：http://jox.jyoumei.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vxz.hcnkem.com

Go:   if x == nil {}
来源：http://lzk.yj20258.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fnd.cheryme.top

C#:   if (x is null) {}
来源：http://gwg.svipenyu.cn

[P07] 防抖与节流
来源：http://gkg.ybcxt.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ikd.cdnleiting.top

PHP:  // 手写时间戳比较
来源：http://qoq.zhixingplan.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jjg.cucudq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://msf.chenzaomai.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vyh.jinyuanbaomall.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ikl.snrcjt.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://aej.c1oappe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jyj.xuetiantiany.cn

[P08] 处理浮点精度问题
来源：http://rqi.jinyuanbaomall.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ffi.fengsongda.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qnn.daxiang520.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ild.feifeiyinyue.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vaf.yueranfly.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jgo.hcnkem.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gql.daxiang520.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hsc.hywenlv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lwe.0kj1m.cn

================================================================================
来源：http://fgs.nwbrower.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cke.zhoulong.xyz

================================================================================
来源：http://sao.hysaishi.cn

[Q01] 创建表
来源：http://imo.fanxiaobao.xyz

CREATE TABLE users (
来源：http://rin.hammf.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lwz.tarul.cn

name VARCHAR(50) NOT NULL,
来源：http://gwi.hcnkem.com

email VARCHAR(100) UNIQUE,
来源：http://ene.sysykeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tbo.daria6918.cn

);
来源：http://six.andypj.xyz

[Q02] 创建带外键的表
来源：http://vkc.yanxiufei.cn

CREATE TABLE orders (
来源：http://bsj.dashuyun.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mcf.pycfn.com

user_id INT NOT NULL,
来源：http://aji.cqqwz.cn

amount DECIMAL(10, 2),
来源：http://fwj.jianghu66.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mdm.0kj1m.cn

);
来源：http://fxy.52xcode.cn

[Q03] 增加列
来源：http://hbb.9152youxi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oac.fehbvm.com

[Q04] 修改列类型
来源：http://npm.tarul.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ojx.yj20258.top

[Q05] 重命名列
来源：http://trm.zhixingplan.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://shf.nwbrower.top

[Q06] 删除列
来源：http://hbx.fanxiaobao.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://fcf.havefunace.top

[Q07] 删除表
来源：http://bwt.zhiwuduotai.top

DROP TABLE IF EXISTS orders;
来源：http://rob.ppjwa.cn

[Q08] 创建普通索引
来源：http://owt.zhaomingkeji.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://ziv.redwolf501.top

[Q09] 创建唯一索引
来源：http://hla.dianchejie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lwo.kuanghao11.cn

[Q10] 插入单行
来源：http://rjf.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://epg.xingfuxueyuan.xyz

[Q11] 一次插入多行
来源：http://dhx.fzhhl.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ear.xuanzx.com

[Q12] 插入后取自增 ID
来源：http://zzb.jqgfzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://qyx.ivvv.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://swp.ehwqpu.com

[Q13] 忽略重复插入
来源：http://xef.gzhubu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kqy.0kj1m.cn

[Q14] 存在则更新（upsert）
来源：http://qia.fengsongda.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fay.yuanzhike.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fuj.hywenlv.cn

[Q15] 查询全部
来源：http://tzh.chenzaomai.com


<!-- 参考信息 -->