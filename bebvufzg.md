代发 wailian999

Java: public static void main(String[] args)
来源：http://ale.bjfxy.top

Go:   func main()
来源：http://hvi.daria6918.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bnf.hywenlv.cn

C#:   static void Main(string[] args)
来源：http://fmh.xuanzx.com

[M08] 获取系统与运行时信息
来源：http://mar.jyoumei.cn

Py:   platform.system();  platform.python_version()
来源：http://vtb.hongshengwenyu.top

PHP:  PHP_OS;  phpversion();
来源：http://pbn.shuidangran.top

JS:   process.platform;  process.version
来源：http://cdn.hywenlv.cn

TS:   process.platform;  process.version
来源：http://ccp.bbcook.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lnr.ywan-chungtsiang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hvu.hongshengwenyu.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://esa.wangdashe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lny.jinqigfzy.top

================================================================================
来源：http://oli.wangdashe.top

N. 数据结构与算法
来源：http://brd.ehwqpu.com

================================================================================
来源：http://ojb.guannengcc.top

[N01] 二分查找（有序数组）
来源：http://kgz.hesvh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://eof.zhoulong.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ezk.yongpay.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sle.zycfv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ymi.hnqzz.top

Java: Arrays.binarySearch(arr, x)
来源：http://oop.sufxvd.cn

Go:   sort.SearchInts(arr, x)
来源：http://tug.yj20258888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://shm.xuanzx.com

C#:   Array.BinarySearch(arr, x)
来源：http://owz.hongshengwenyu.top

[N02] 排序（工程实践用内置实现）
来源：http://qih.ydzc1.top

Py:   sorted(arr);  arr.sort()
来源：http://rnq.fehbvm.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ufa.zdbjq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fgj.haohaochexian.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dkd.xylfe.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://squ.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://bym.jqgfzy.top

Ruby: arr.sort
来源：http://jwl.tanke756.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xux.316326.xyz

[N03] 快速排序（分治示例）
来源：http://bus.hfpthk.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mid.shanyushiyangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://hep.tarul.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://avi.vehdjk.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uta.ehwqpu.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tbp.yanxiufei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pwt.zhoulong.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ely.guannengcc.top

C#:   // 手写递归，或 Array.Sort
来源：http://kpm.jinghuilouyu.cn

[N04] 斐波那契数列
来源：http://byw.cucudq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dtm.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://thp.fehbvm.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rzy.cdnleiting.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mpk.cucudq.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qxx.shzxlz.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://owc.bbcook.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fdp.ehwqpu.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nye.ehwqpu.com

[N05] 最大公约数
来源：http://ybg.yonumen.top

Py:   math.gcd(a, b)
来源：http://ymh.ydjk.org.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wez.ppjwa.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://spm.guowangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ucx.cqqwz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uwo.fengsongda.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wni.daxiang520.top

Ruby: a.gcd(b)
来源：http://vbq.ydzc1.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ozi.0kj1m.cn

[N06] 判断回文字符串
来源：http://dkq.yuxming.cn

Py:   s == s[::-1]
来源：http://tkn.hnqzz.top

PHP:  $s === strrev($s);
来源：http://pht.wangdashe.top

JS:   s === [...s].reverse().join("")
来源：http://iiu.redwolf501.top

TS:   s === [...s].reverse().join("")
来源：http://rsv.ydzc1.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ryv.pengpengdd.cyou

Go:   // 双指针从两端比较
来源：http://pct.ivvv.top

Ruby: s == s.reverse
来源：http://yun.zhixingplan.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://goc.9152youxi.cn

[N07] 两数之和（返回下标）
来源：http://isq.ydjk.org.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ffz.hysaishi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://por.jinghuilouyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://oyr.c1oappe.top

TS:   // 手写 Map<string, number>
来源：http://phl.xingfuxueyuan.xyz

Java: // 手写 HashMap
来源：http://zhz.ehwqpu.com

Go:   // 手写 map[int]int
来源：http://mqt.feifeiyinyue.top

Ruby: // 手写 Hash
来源：http://qol.tian-w.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wxe.tanke756.top

[N08] 生成全排列
来源：http://jai.316326.xyz

Py:   itertools.permutations(arr)
来源：http://tgc.yj20258888.top

PHP:  // 手写递归交换
来源：http://iwc.jlsjyb.cn

JS:   // 手写回溯递归
来源：http://rin.sweek.top

TS:   // 手写回溯递归
来源：http://vrb.uphjek.com

Java: // 手写回溯递归
来源：http://eih.hesvh.cn

Go:   // 手写回溯递归
来源：http://tux.sjlbkw.cn

Ruby: arr.permutation.to_a
来源：http://nda.nwbrower.top

C#:   // 手写回溯递归
来源：http://adi.fanxiaobao.xyz

[N09] 栈与队列
来源：http://bhy.wangdashe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ooy.jianghu66.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wbm.c1oappe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blb.xuetiantiany.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://paf.zhiwuduotai.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xlz.zhixingplan.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xkn.ctjpmb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xff.jinghuilouyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uhm.hongshengwenyu.top

[N10] 链表节点定义
来源：http://prf.zhaomingkeji.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ffq.snrcjt.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kye.zhijiandao.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dbe.havefunace.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xzw.birdmap.top

Java: class Node { int v; Node next; }
来源：http://ncl.fktsv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://mow.nanxinkj.top

Ruby: Node = Struct.new(:v, :next)
来源：http://cfr.fzhhl.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ele.jianghu66.top

[N11] 二叉树中序遍历
来源：http://nqr.uphjek.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lst.cqqwz.cn

PHP:  // 手写递归函数
来源：http://vow.ydjk.org.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ygy.sxryk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://llj.uphjek.com

Java: // 手写递归
来源：http://mwk.vqdsnc.cn

Go:   // 手写递归
来源：http://stb.hysaishi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://abc.fengsongda.top

C#:   // 手写递归
来源：http://quh.tianlin.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fsa.shuidangran.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jrd.hnqzz.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ioe.gotoacloud.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tao.jqgufenzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gde.daria6918.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wjj.zhixingplan.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rxn.hesvh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bva.xingfuxueyuan.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nzr.jinghuilouyu.cn

================================================================================
来源：http://jsc.guannengcc.top

O. 并发与异步
来源：http://xgn.yj202588.top

================================================================================
来源：http://mdx.tianlin.xyz

[O01] 启动一个线程
来源：http://rds.tanke756.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iwy.sjlbkw.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jzu.yangfankeji.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://rqc.quarkkingdee.top

TS:   // 同 JS
来源：http://otq.dashuyun.cn

Java: new Thread(() -> f()).start()
来源：http://wlz.sjlbkw.cn

Go:   go f()
来源：http://fxy.yvedp.cn

Ruby: Thread.new { f }
来源：http://wtv.tian-w.cn

C#:   Task.Run(() => F());
来源：http://qme.jyoumei.cn

[O02] 使用线程池
来源：http://itc.bbcook.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tuy.yfazqb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qzq.cqqwz.cn

JS:   // worker_threads 线程池
来源：http://ydh.tian-w.cn

TS:   // worker_threads 线程池
来源：http://jik.wangdashe.top

Java: Executors.newFixedThreadPool(4)
来源：http://vni.52xcode.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xcr.yangfankeji.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wau.cheryme.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vps.vqdsnc.cn

[O03] 加锁保护共享数据
来源：http://viu.yangfankeji.com

Py:   with lock: shared += 1
来源：http://kpy.shangyingyoupin.top

PHP:  // 用 flock() 做文件锁
来源：http://xip.yfazqb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gdy.ctjpmb.com

TS:   // 同 JS
来源：http://tjb.gogol.net.cn

Java: synchronized (this) { shared++; }
来源：http://auf.shuidangran.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hqm.chenzaomai.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://jil.daria6918.cn

C#:   lock (gate) { shared++; }
来源：http://zhd.kuanghao11.cn

[O04] 定义异步函数并等待
来源：http://fou.yanxiufei.cn

Py:   async def f():⏎    await g()
来源：http://djt.hfpthk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fju.jiagoushi.top

JS:   async function f() { await g(); }
来源：http://rjs.yanxiufei.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bwx.uphjek.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://isy.birdmap.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fyv.xinyue.icu

Ruby: # 用 Fiber 或 async gem
来源：http://rjx.guannengcc.top

C#:   async Task F() { await G(); }
来源：http://kyp.tanke756.top

[O05] 并发执行并等待全部完成
来源：http://vip.gzhubu.top

Py:   asyncio.gather(*tasks)
来源：http://kif.0kj1m.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nam.bbcook.cn

JS:   await Promise.all(tasks)
来源：http://imm.sufxvd.cn

TS:   await Promise.all(tasks)
来源：http://exn.wangshuangyany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iyj.yuanzhike.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tse.jiagoushi.top

Ruby: threads.map(&:join)
来源：http://kix.9152youxi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xbw.daxiang520.top

[O06] 使用进程池
来源：http://hyy.zhaomingkeji.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tiw.shuidangran.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ltk.shangyingyoupin.top

JS:   // child_process / cluster 模块
来源：http://kri.chenzaomai.com

TS:   // child_process / cluster 模块
来源：http://uhk.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jdj.vqdsnc.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dbk.jinqigufen.top

Ruby: // fork 块
来源：http://obo.yj202588.top

C#:   Parallel.For
来源：http://yqe.uphjek.com

================================================================================
来源：http://jgn.hcnkem.com

P. 常用工具函数
来源：http://owi.yfazqb.com

================================================================================
来源：http://ddf.aizwys.cn

[P01] 生成 UUID
来源：http://rhd.fanxiaobao.xyz

Py:   str(uuid.uuid4())
来源：http://udn.jqgfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zal.hnqzz.top

JS:   crypto.randomUUID()
来源：http://bbj.wangdashe.top

TS:   crypto.randomUUID()
来源：http://hjd.xingfuxueyuan.xyz

Java: UUID.randomUUID().toString()
来源：http://xcf.vehdjk.com

Go:   // 用 github.com/google/uuid
来源：http://saq.ctjpmb.com

Ruby: SecureRandom.uuid
来源：http://csg.yongpay.top

C#:   Guid.NewGuid().ToString()
来源：http://zec.jinqigfzy.top

[P02] MD5 / SHA256 摘要
来源：http://qhd.sjlbkw.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hvi.yvedp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gab.meibo888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qou.bbcook.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xkx.jianghu66.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tzc.havefunace.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ajw.316326.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://txr.daxiang520.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rza.dianchejie.cn

[P03] 生成短随机字符串
来源：http://adl.ydzc1.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hhy.nanxinkj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://acf.yvedp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fhk.shanyushiyangtech.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nkr.bjfxy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iyn.zhongyouzk.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kjm.sjlbkw.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zdt.mhx1999.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fnr.c1oappe.top

[P04] 求长度
来源：http://gir.gzhubu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gnu.ehwqpu.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://azs.quarkkingdee.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qpb.daxiang520.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ysx.jlsjyb.cn

Java: list.size();  map.size();  s.length()
来源：http://mlk.haohaochexian.top

Go:   len(arr);  len(m)
来源：http://uar.zhiwuduotai.top

Ruby: x.length;  x.size
来源：http://wgr.c1oappe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ujb.gogol.net.cn

[P05] 判断两个对象内容是否相等
来源：http://qav.ywan-chungtsiang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://wgk.aibaodan.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hhr.cashguo.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qoc.cashguo.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://csw.shzxlz.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hvq.sweek.top

Go:   reflect.DeepEqual(a, b)
来源：http://nip.daria6918.cn

Ruby: a == b
来源：http://bsr.tarul.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fwx.nanxinkj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fyc.jinqigfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pgc.yuanzhike.top

PHP:  if (empty($x)) {}
来源：http://xzu.0kj1m.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ega.cashguo.top

TS:   if (x == null) {}
来源：http://svh.smart0.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://phd.bbcook.cn

Go:   if x == nil {}
来源：http://uhf.dashuyun.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ddm.pengpengdd.cyou

C#:   if (x is null) {}
来源：http://ayy.xuanzx.com

[P07] 防抖与节流
来源：http://rhw.kuanghao11.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wli.guannengcc.top

PHP:  // 手写时间戳比较
来源：http://vry.zhixingplan.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iix.pengpengdd.cyou

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uow.nanxinkj.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ube.jyoumei.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rmp.chenjidiqi.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://pop.ppjwa.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://afk.c1oappe.top

[P08] 处理浮点精度问题
来源：http://gfg.zhaomingkeji.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tim.snrcjt.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sze.hywenlv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iev.c1oappe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://joa.yonumen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tfn.kuanghao11.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dgo.cqqwz.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://otz.xuanzx.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cjo.epnwcf.com

================================================================================
来源：http://mtf.zhoulong.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xag.gotoacloud.top

================================================================================
来源：http://xyq.andypj.xyz

[Q01] 创建表
来源：http://xnv.jqgfzy.top

CREATE TABLE users (
来源：http://toi.0kj1m.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kbe.ppjwa.cn

name VARCHAR(50) NOT NULL,
来源：http://vph.iojbl.cn

email VARCHAR(100) UNIQUE,
来源：http://qbh.hysaishi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mzz.yueranfly.top

);
来源：http://ivj.tian-w.cn

[Q02] 创建带外键的表
来源：http://ikg.hnqzz.top

CREATE TABLE orders (
来源：http://rea.xziqi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fbq.sxryk.cn

user_id INT NOT NULL,
来源：http://rrj.jqgfzy.top

amount DECIMAL(10, 2),
来源：http://vhu.nanxuanxn.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kiw.xuetiantiany.cn

);
来源：http://djp.sxryk.cn

[Q03] 增加列
来源：http://eln.havefunace.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xah.xuanzx.com

[Q04] 修改列类型
来源：http://qyo.havefunace.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wtb.xingfuxueyuan.xyz

[Q05] 重命名列
来源：http://dfh.zdbjq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zcj.wangdashe.top

[Q06] 删除列
来源：http://abe.xziqi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kli.ppjwa.cn

[Q07] 删除表
来源：http://gca.gotoacloud.top

DROP TABLE IF EXISTS orders;
来源：http://leh.tianlin.xyz

[Q08] 创建普通索引
来源：http://srj.yfazqb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://mnz.vehdjk.com

[Q09] 创建唯一索引
来源：http://mip.zhengqikj.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yec.hnxiangtu.top

[Q10] 插入单行
来源：http://qyl.vehdjk.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ssp.aizwys.cn

[Q11] 一次插入多行
来源：http://cul.hcnkem.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fkb.snrcjt.cn

[Q12] 插入后取自增 ID
来源：http://wuw.feifeiyinyue.top

INSERT INTO users (name) VALUES ('C');
来源：http://klu.dianchejie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vtc.zhijiandao.cn

[Q13] 忽略重复插入
来源：http://qkg.hongshengwenyu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mjj.jyoumei.cn

[Q14] 存在则更新（upsert）
来源：http://imx.jqgufenzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bio.daxiang520.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mpu.zdqjudy.top

[Q15] 查询全部
来源：http://bwr.chenlongwang.top


<!-- 参考信息 -->