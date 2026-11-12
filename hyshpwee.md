代发 wailian999

Py:   if __name__ == "__main__":
来源：http://otm.fehbvm.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://obo.nanxinkj.top

JS:   require.main === module
来源：http://wec.shangyingyoupin.top

TS:   require.main === module
来源：http://rua.daria6918.cn

Java: public static void main(String[] args)
来源：http://rxb.yj20258.top

Go:   func main()
来源：http://txv.jinghuilouyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nko.fehbvm.com

C#:   static void Main(string[] args)
来源：http://hxy.yangfankeji.com

[M08] 获取系统与运行时信息
来源：http://ytm.ydzc1.top

Py:   platform.system();  platform.python_version()
来源：http://syk.chenlongwang.top

PHP:  PHP_OS;  phpversion();
来源：http://yjb.zhaomingkeji.xyz

JS:   process.platform;  process.version
来源：http://iob.hnqzz.top

TS:   process.platform;  process.version
来源：http://szg.jqgufenzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cyb.chenjidiqi.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://iem.zhijiandao.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vgg.hysaishi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hcs.ehwqpu.com

================================================================================
来源：http://rog.kuanghao11.cn

N. 数据结构与算法
来源：http://tcc.gogol.net.cn

================================================================================
来源：http://opb.shangyingyoupin.top

[N01] 二分查找（有序数组）
来源：http://hca.shanyushiyangkeji.top

Py:   bisect.bisect_left(arr, x)
来源：http://gix.yongpay.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bcb.shanyushiyangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ygp.xinyue.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tmj.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://xmv.xuetiantiany.cn

Go:   sort.SearchInts(arr, x)
来源：http://uhn.yj20258888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ias.vehdjk.com

C#:   Array.BinarySearch(arr, x)
来源：http://uok.sufxvd.cn

[N02] 排序（工程实践用内置实现）
来源：http://nnn.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://bdz.tarul.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://epa.fengsongda.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jhk.hnxiangtu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ahe.jinghuilouyu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zrl.ctjpmb.com

Go:   slices.Sort(arr)
来源：http://vcc.jqgufenzy.top

Ruby: arr.sort
来源：http://vka.0kj1m.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fwt.xuetiantiany.cn

[N03] 快速排序（分治示例）
来源：http://txh.wangdashe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rmc.hesvh.cn

PHP:  // 递归实现，或用 usort
来源：http://xmj.yfazqb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uql.quarkkingdee.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dxa.sxryk.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dqw.zdqjudy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ilp.feifeiyinyue.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wen.chenjidiqi.icu

C#:   // 手写递归，或 Array.Sort
来源：http://exi.yj20258.top

[N04] 斐波那契数列
来源：http://iwe.yanxiufei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zra.jiagoushi.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qec.shuidangran.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ilx.havefunace.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rwa.316326.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lth.zhiwuduotai.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fzq.zdbjq.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gsk.316326.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xlp.ydjk.org.cn

[N05] 最大公约数
来源：http://eac.bjfxy.top

Py:   math.gcd(a, b)
来源：http://yxt.zhoulong.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://smx.chenlongwang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oks.havefunace.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bmz.kuanghao11.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://igi.nanxuanxn.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://luv.sjlbkw.cn

Ruby: a.gcd(b)
来源：http://fqn.jyoumei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hqj.wangshuangyany.cn

[N06] 判断回文字符串
来源：http://vvz.hcnkem.com

Py:   s == s[::-1]
来源：http://awa.shanyushiyangkeji.top

PHP:  $s === strrev($s);
来源：http://wgo.yonumen.top

JS:   s === [...s].reverse().join("")
来源：http://wpp.bjfxy.top

TS:   s === [...s].reverse().join("")
来源：http://aok.yuxming.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://swa.yj202588.top

Go:   // 双指针从两端比较
来源：http://jea.nanxinkj.top

Ruby: s == s.reverse
来源：http://gav.aizwys.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xza.svipenyu.cn

[N07] 两数之和（返回下标）
来源：http://wpd.iojbl.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hek.meibo888.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cvd.pengpengdd.cyou

JS:   // 手写 Map：map.set(v, i)
来源：http://xiv.nanxuanxn.top

TS:   // 手写 Map<string, number>
来源：http://qrc.52xcode.cn

Java: // 手写 HashMap
来源：http://gpm.zycfv.cn

Go:   // 手写 map[int]int
来源：http://vih.sysykeji.top

Ruby: // 手写 Hash
来源：http://tlg.sysykeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://yjg.hcnkem.com

[N08] 生成全排列
来源：http://xqd.sweek.top

Py:   itertools.permutations(arr)
来源：http://rag.fehbvm.com

PHP:  // 手写递归交换
来源：http://uxb.jqgufenzy.top

JS:   // 手写回溯递归
来源：http://pub.kuanghao11.cn

TS:   // 手写回溯递归
来源：http://ypu.shuidangran.top

Java: // 手写回溯递归
来源：http://fto.aibaodan.cn

Go:   // 手写回溯递归
来源：http://jyo.chenzaomai.com

Ruby: arr.permutation.to_a
来源：http://gqq.ppjwa.cn

C#:   // 手写回溯递归
来源：http://khf.hesvh.cn

[N09] 栈与队列
来源：http://cif.jqgfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://neo.zhongyouzk.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://awv.yj202588.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://byt.aibaodan.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ydx.gogol.net.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sit.hywenlv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ljb.gzhubu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pmc.shanyushiyangtech.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fsb.tian-w.cn

[N10] 链表节点定义
来源：http://xoh.chenzaomai.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mfq.shanyushiyangtech.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ibt.yuxming.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fae.hammf.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sge.yongpay.top

Java: class Node { int v; Node next; }
来源：http://egg.birdmap.top

Go:   type Node struct { V int; Next *Node }
来源：http://odi.c1oappe.top

Ruby: Node = Struct.new(:v, :next)
来源：http://gzo.chenzaomai.com

C#:   class Node { public int V; public Node? Next; }
来源：http://txv.xziqi.cn

[N11] 二叉树中序遍历
来源：http://uql.shanyushiyangkeji.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ahi.xziqi.cn

PHP:  // 手写递归函数
来源：http://chf.haohaochexian.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ixg.jianghu66.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ikl.gzhubu.top

Java: // 手写递归
来源：http://ird.yongpay.top

Go:   // 手写递归
来源：http://qqj.hesvh.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kxc.zdqjudy.top

C#:   // 手写递归
来源：http://yvv.shangyingyoupin.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://buu.dashuyun.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://byl.xylfe.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://itk.snrcjt.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aqw.shzxlz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lmj.aizwys.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zpv.sweek.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vfo.tian-w.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dpf.zdbjq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mzw.zycfv.cn

================================================================================
来源：http://gzo.xuanzx.com

O. 并发与异步
来源：http://scv.yvedp.cn

================================================================================
来源：http://tfa.yuanzhike.top

[O01] 启动一个线程
来源：http://qfh.iojbl.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kzv.smart0.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://msz.sxryk.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yxe.sweek.top

TS:   // 同 JS
来源：http://ldv.gogol.net.cn

Java: new Thread(() -> f()).start()
来源：http://qyl.jyoumei.cn

Go:   go f()
来源：http://wuj.dianchejie.cn

Ruby: Thread.new { f }
来源：http://zyu.ydjk.org.cn

C#:   Task.Run(() => F());
来源：http://qio.hnxiangtu.top

[O02] 使用线程池
来源：http://lem.shanyushiyangtech.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xiw.tian-w.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mwe.gaohongyu789.top

JS:   // worker_threads 线程池
来源：http://gkd.hnqzz.top

TS:   // worker_threads 线程池
来源：http://niu.yfazqb.com

Java: Executors.newFixedThreadPool(4)
来源：http://xgs.yongpay.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jeb.jinqigufen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ohp.fanxiaobao.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tkh.chenjidiqi.icu

[O03] 加锁保护共享数据
来源：http://nnj.yfazqb.com

Py:   with lock: shared += 1
来源：http://xkc.fktsv.cn

PHP:  // 用 flock() 做文件锁
来源：http://pih.cheryme.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://llp.tarul.cn

TS:   // 同 JS
来源：http://kok.hysaishi.cn

Java: synchronized (this) { shared++; }
来源：http://oqh.kuanghao11.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://amc.52xcode.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://avx.shanyushiyangtech.top

C#:   lock (gate) { shared++; }
来源：http://ajg.guannengcc.top

[O04] 定义异步函数并等待
来源：http://wou.zhengqikj.top

Py:   async def f():⏎    await g()
来源：http://uwu.jiagoushi.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fts.zdbjq.cn

JS:   async function f() { await g(); }
来源：http://yme.hfpthk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xwc.c1oappe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xur.chenlongwang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yrn.sysykeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://rpg.yangfankeji.com

C#:   async Task F() { await G(); }
来源：http://jfw.gzhubu.top

[O05] 并发执行并等待全部完成
来源：http://qlo.yj20258888.top

Py:   asyncio.gather(*tasks)
来源：http://qck.zhengqikj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cyy.zhaomingkeji.xyz

JS:   await Promise.all(tasks)
来源：http://qnu.tanke756.top

TS:   await Promise.all(tasks)
来源：http://gst.svipenyu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sly.jqgfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rmp.hongshengwenyu.top

Ruby: threads.map(&:join)
来源：http://sni.yvedp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ebk.wangshuangyany.cn

[O06] 使用进程池
来源：http://euf.mhx1999.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jcc.pycfn.com

PHP:  // pcntl_fork 或多进程队列
来源：http://hki.mhx1999.top

JS:   // child_process / cluster 模块
来源：http://tua.cqqwz.cn

TS:   // child_process / cluster 模块
来源：http://ilh.zdbjq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lsa.mhx1999.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tqb.xuanzx.com

Ruby: // fork 块
来源：http://hwo.yvedp.cn

C#:   Parallel.For
来源：http://icq.jinghuilouyu.cn

================================================================================
来源：http://qnm.redwolf501.top

P. 常用工具函数
来源：http://fwa.shuidangran.top

================================================================================
来源：http://gvu.andypj.xyz

[P01] 生成 UUID
来源：http://myp.quarkkingdee.top

Py:   str(uuid.uuid4())
来源：http://emu.havefunace.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yqj.xylfe.cn

JS:   crypto.randomUUID()
来源：http://scd.52xcode.cn

TS:   crypto.randomUUID()
来源：http://xju.ppjwa.cn

Java: UUID.randomUUID().toString()
来源：http://htv.yfazqb.com

Go:   // 用 github.com/google/uuid
来源：http://wbp.xylfe.cn

Ruby: SecureRandom.uuid
来源：http://kug.fehbvm.com

C#:   Guid.NewGuid().ToString()
来源：http://tns.shanyushiyangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://uxq.shzxlz.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pjp.jinqigfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://uoo.cqqwz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vhb.shanyushiyangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pzm.sysykeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zgt.cucudq.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cey.chenzaomai.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mcz.cdnleiting.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ntm.zdqjudy.top

[P03] 生成短随机字符串
来源：http://xyz.jiagoushi.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ato.xingfuxueyuan.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xpj.jinyuanbaomall.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xkp.chenlongwang.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fky.snrcjt.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hbd.quarkkingdee.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wja.andypj.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://qkd.meibo888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kit.yongpay.top

[P04] 求长度
来源：http://iqq.fanxiaobao.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uap.zhaomingkeji.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://flt.fzhhl.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xvm.svipenyu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vsu.haohaochexian.top

Java: list.size();  map.size();  s.length()
来源：http://jqk.cheryme.top

Go:   len(arr);  len(m)
来源：http://nbt.9152youxi.cn

Ruby: x.length;  x.size
来源：http://cyw.cdnleiting.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://oha.yuxming.cn

[P05] 判断两个对象内容是否相等
来源：http://fgy.hcnkem.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://osx.cashguo.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gxw.hfpthk.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xpo.yj20258.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://piz.yongpay.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wxz.zhoulong.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://npb.fehbvm.com

Ruby: a == b
来源：http://zhf.yj20258888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sfm.jqgufenzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bbg.shzxlz.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ucv.cdnleiting.top

PHP:  if (empty($x)) {}
来源：http://vdl.tian-w.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ony.tianlin.xyz

TS:   if (x == null) {}
来源：http://qlb.ctjpmb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://ksc.guowangkeji.top

Go:   if x == nil {}
来源：http://mhg.zhongyouzk.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fkb.ydjk.org.cn

C#:   if (x is null) {}
来源：http://duh.bbcook.cn

[P07] 防抖与节流
来源：http://rdi.cucudq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jbo.gaohongyu789.top

PHP:  // 手写时间戳比较
来源：http://arw.meibo888.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://upt.daria6918.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xfu.sweek.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zmn.kuanghao11.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jby.fengsongda.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://nno.jlsjyb.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jop.hysaishi.cn

[P08] 处理浮点精度问题
来源：http://uup.guowangkeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kub.mhx1999.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rjg.jiagoushi.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nvv.hammf.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bxv.gotoacloud.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tch.hongshengwenyu.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hmc.quarkkingdee.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wre.chenjidiqi.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kzd.cheryme.top

================================================================================
来源：http://bqi.gaohongyu789.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cij.yangfankeji.com

================================================================================
来源：http://ktl.52xcode.cn

[Q01] 创建表
来源：http://thk.ppjwa.cn

CREATE TABLE users (
来源：http://lwr.shuidangran.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cxm.ywan-chungtsiang.top

name VARCHAR(50) NOT NULL,
来源：http://brh.jiagoushi.top

email VARCHAR(100) UNIQUE,
来源：http://tdc.tarul.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ugq.jinqigufen.top

);
来源：http://ujt.52xcode.cn

[Q02] 创建带外键的表
来源：http://etd.nwbrower.top

CREATE TABLE orders (
来源：http://kjf.bjfxy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://put.xziqi.cn

user_id INT NOT NULL,
来源：http://ubj.guowangkeji.top

amount DECIMAL(10, 2),
来源：http://rbq.hysaishi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bdg.smart0.xyz

);
来源：http://qwo.jlsjyb.cn

[Q03] 增加列
来源：http://ozm.epnwcf.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://scr.ppjwa.cn

[Q04] 修改列类型
来源：http://hmi.smart0.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cdj.redwolf501.top

[Q05] 重命名列
来源：http://qkl.zhaomingkeji.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ooq.birdmap.top

[Q06] 删除列
来源：http://nkw.havefunace.top

ALTER TABLE users DROP COLUMN age;
来源：http://bxn.jianghu66.top

[Q07] 删除表
来源：http://bee.c1oappe.top

DROP TABLE IF EXISTS orders;
来源：http://sbl.yongpay.top

[Q08] 创建普通索引
来源：http://kmr.tian-w.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://pba.ivvv.top

[Q09] 创建唯一索引
来源：http://rig.shzxlz.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vjz.fktsv.cn

[Q10] 插入单行
来源：http://vjv.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dnd.shanyushiyangtech.top

[Q11] 一次插入多行
来源：http://phi.tianlin.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zaj.yanxiufei.cn

[Q12] 插入后取自增 ID
来源：http://lgv.vehdjk.com

INSERT INTO users (name) VALUES ('C');
来源：http://krd.zhengqikj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://obs.uphjek.com

[Q13] 忽略重复插入
来源：http://fxm.iojbl.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pmr.nanxinkj.top


<!-- 参考信息 -->