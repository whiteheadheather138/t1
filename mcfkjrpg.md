代发 wailian999

Java: public static void main(String[] args)
来源：http://mro.yueranfly.top

Go:   func main()
来源：http://ipq.yfazqb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ziu.yanxiufei.cn

C#:   static void Main(string[] args)
来源：http://yvl.hysaishi.cn

[M08] 获取系统与运行时信息
来源：http://ort.c1oappe.top

Py:   platform.system();  platform.python_version()
来源：http://toy.redwolf501.top

PHP:  PHP_OS;  phpversion();
来源：http://faf.haohaochexian.top

JS:   process.platform;  process.version
来源：http://avk.yj202588.top

TS:   process.platform;  process.version
来源：http://uta.andypj.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gxe.chenlongwang.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tzb.iojbl.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kxb.tanke756.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ebh.gzhubu.top

================================================================================
来源：http://flx.ehwqpu.com

N. 数据结构与算法
来源：http://lak.tanke756.top

================================================================================
来源：http://pwn.jinghuilouyu.cn

[N01] 二分查找（有序数组）
来源：http://ghp.yonumen.top

Py:   bisect.bisect_left(arr, x)
来源：http://xrt.jqgfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zxq.ydjk.org.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eht.sufxvd.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://noo.52xcode.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ltr.daria6918.cn

Go:   sort.SearchInts(arr, x)
来源：http://qfd.xylfe.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ixo.yvedp.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sdw.vqdsnc.cn

[N02] 排序（工程实践用内置实现）
来源：http://mdb.yj202588.top

Py:   sorted(arr);  arr.sort()
来源：http://esl.hesvh.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fdm.ehwqpu.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://sox.dianchejie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ujx.sxryk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zgc.gogol.net.cn

Go:   slices.Sort(arr)
来源：http://svi.haohaochexian.top

Ruby: arr.sort
来源：http://klo.jinyuanbaomall.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://euw.vqdsnc.cn

[N03] 快速排序（分治示例）
来源：http://sqg.shuidangran.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://obt.ppjwa.cn

PHP:  // 递归实现，或用 usort
来源：http://zsd.ydzc1.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yjj.shuidangran.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iak.jqgufenzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gce.quarkkingdee.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gdq.daxiang520.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rgy.wangdashe.top

C#:   // 手写递归，或 Array.Sort
来源：http://esi.52xcode.cn

[N04] 斐波那契数列
来源：http://ajz.xingfuxueyuan.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bjq.redwolf501.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lhs.fengsongda.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xts.meibo888.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fpe.tian-w.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://omm.ivvv.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yap.meibo888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zbb.iojbl.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lgg.ehwqpu.com

[N05] 最大公约数
来源：http://xnq.snrcjt.cn

Py:   math.gcd(a, b)
来源：http://lrs.svipenyu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lls.zdqjudy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://str.jqgfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qhp.hcnkem.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://awc.jianghu66.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vmv.cucudq.cn

Ruby: a.gcd(b)
来源：http://fyi.ywan-chungtsiang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zlj.shuidangran.top

[N06] 判断回文字符串
来源：http://iyv.fktsv.cn

Py:   s == s[::-1]
来源：http://tbk.jiagoushi.top

PHP:  $s === strrev($s);
来源：http://pur.tanke756.top

JS:   s === [...s].reverse().join("")
来源：http://hxn.cashguo.top

TS:   s === [...s].reverse().join("")
来源：http://pik.guowangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kog.hnqzz.top

Go:   // 双指针从两端比较
来源：http://zxs.sysykeji.top

Ruby: s == s.reverse
来源：http://kfq.yuxming.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kaj.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://hcm.jiagoushi.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://eig.ydzc1.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://icn.zhiwuduotai.top

JS:   // 手写 Map：map.set(v, i)
来源：http://smw.yj202588.top

TS:   // 手写 Map<string, number>
来源：http://ydp.yvedp.cn

Java: // 手写 HashMap
来源：http://gyl.yuxming.cn

Go:   // 手写 map[int]int
来源：http://xmq.xinyue.icu

Ruby: // 手写 Hash
来源：http://sfl.cheryme.top

C#:   // 手写 Dictionary<int, int>
来源：http://hqz.yueranfly.top

[N08] 生成全排列
来源：http://yxh.ehwqpu.com

Py:   itertools.permutations(arr)
来源：http://azr.jinqigfzy.top

PHP:  // 手写递归交换
来源：http://xud.yueranfly.top

JS:   // 手写回溯递归
来源：http://wty.fzhhl.top

TS:   // 手写回溯递归
来源：http://efw.zdbjq.cn

Java: // 手写回溯递归
来源：http://tjw.ppjwa.cn

Go:   // 手写回溯递归
来源：http://hko.ydjk.org.cn

Ruby: arr.permutation.to_a
来源：http://uhe.cdnleiting.top

C#:   // 手写回溯递归
来源：http://kot.cdnleiting.top

[N09] 栈与队列
来源：http://xik.0kj1m.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://pbw.iojbl.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uyy.yanxiufei.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fgf.hnxiangtu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://irp.yangfankeji.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kqf.ywan-chungtsiang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bto.tarul.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yas.yuxming.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zii.xuetiantiany.cn

[N10] 链表节点定义
来源：http://tcu.zhoulong.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nom.hesvh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://gxd.fanxiaobao.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zbw.jlsjyb.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hxh.ehwqpu.com

Java: class Node { int v; Node next; }
来源：http://pix.meibo888.top

Go:   type Node struct { V int; Next *Node }
来源：http://rzm.yongpay.top

Ruby: Node = Struct.new(:v, :next)
来源：http://txj.zhixingplan.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bmg.wangshuangyany.cn

[N11] 二叉树中序遍历
来源：http://xrj.chenzaomai.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dyt.wangdashe.top

PHP:  // 手写递归函数
来源：http://iph.daxiang520.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://glj.316326.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ptr.cdnleiting.top

Java: // 手写递归
来源：http://hmy.bjfxy.top

Go:   // 手写递归
来源：http://njw.yj202588.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ibb.zhixingplan.top

C#:   // 手写递归
来源：http://jbi.nanxuanxn.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ezh.andypj.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mwa.ctjpmb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ymu.fengsongda.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fjo.bbcook.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zib.nwbrower.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wvk.yongpay.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zox.haohaochexian.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iir.vqdsnc.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mvd.tarul.cn

================================================================================
来源：http://qog.9152youxi.cn

O. 并发与异步
来源：http://mtv.gzhubu.top

================================================================================
来源：http://hbx.ivvv.top

[O01] 启动一个线程
来源：http://bmw.hnxiangtu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jka.nwbrower.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tnh.hysaishi.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fel.daxiang520.top

TS:   // 同 JS
来源：http://frw.jinqigfzy.top

Java: new Thread(() -> f()).start()
来源：http://dsp.aizwys.cn

Go:   go f()
来源：http://xam.jianghu66.top

Ruby: Thread.new { f }
来源：http://msz.xziqi.cn

C#:   Task.Run(() => F());
来源：http://gyz.52xcode.cn

[O02] 使用线程池
来源：http://qps.snrcjt.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wnk.gogol.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oxb.jiagoushi.top

JS:   // worker_threads 线程池
来源：http://lwb.aizwys.cn

TS:   // worker_threads 线程池
来源：http://ahz.yfazqb.com

Java: Executors.newFixedThreadPool(4)
来源：http://vns.fzhhl.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mfw.zhixingplan.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tra.cheryme.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://syd.zhixingplan.top

[O03] 加锁保护共享数据
来源：http://uzc.jiagoushi.top

Py:   with lock: shared += 1
来源：http://smk.sxryk.cn

PHP:  // 用 flock() 做文件锁
来源：http://jbp.yj202588.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cal.c1oappe.top

TS:   // 同 JS
来源：http://bpl.daria6918.cn

Java: synchronized (this) { shared++; }
来源：http://ica.yj202588.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uon.zhiwuduotai.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://sgz.cqqwz.cn

C#:   lock (gate) { shared++; }
来源：http://ddu.316326.xyz

[O04] 定义异步函数并等待
来源：http://hfl.xuanzx.com

Py:   async def f():⏎    await g()
来源：http://lkp.hcnkem.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nup.tanke756.top

JS:   async function f() { await g(); }
来源：http://qeg.aibaodan.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dxd.shuidangran.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pav.zhixingplan.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ehq.gotoacloud.top

Ruby: # 用 Fiber 或 async gem
来源：http://yhg.pycfn.com

C#:   async Task F() { await G(); }
来源：http://nfo.epnwcf.com

[O05] 并发执行并等待全部完成
来源：http://lih.yuxming.cn

Py:   asyncio.gather(*tasks)
来源：http://fvi.tian-w.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eno.svipenyu.cn

JS:   await Promise.all(tasks)
来源：http://cwl.jianghu66.top

TS:   await Promise.all(tasks)
来源：http://bqf.nanxuanxn.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wqv.ybcxt.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sby.aibaodan.cn

Ruby: threads.map(&:join)
来源：http://lrp.chenjidiqi.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://cbd.sysykeji.top

[O06] 使用进程池
来源：http://zqm.vqdsnc.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wvl.chenzaomai.com

PHP:  // pcntl_fork 或多进程队列
来源：http://lzu.cdnleiting.top

JS:   // child_process / cluster 模块
来源：http://pes.52xcode.cn

TS:   // child_process / cluster 模块
来源：http://ruf.nwbrower.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qay.gogol.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://idj.zhixingplan.top

Ruby: // fork 块
来源：http://gln.iojbl.cn

C#:   Parallel.For
来源：http://ozk.mhx1999.top

================================================================================
来源：http://xgf.kuanghao11.cn

P. 常用工具函数
来源：http://nwv.jyoumei.cn

================================================================================
来源：http://zir.xuetiantiany.cn

[P01] 生成 UUID
来源：http://tpk.yfazqb.com

Py:   str(uuid.uuid4())
来源：http://eru.yangfankeji.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://chk.sxryk.cn

JS:   crypto.randomUUID()
来源：http://pun.hongshengwenyu.top

TS:   crypto.randomUUID()
来源：http://nez.zhijiandao.cn

Java: UUID.randomUUID().toString()
来源：http://xqq.havefunace.top

Go:   // 用 github.com/google/uuid
来源：http://fqf.yj20258888.top

Ruby: SecureRandom.uuid
来源：http://zef.gaohongyu789.top

C#:   Guid.NewGuid().ToString()
来源：http://zpr.yj20258.top

[P02] MD5 / SHA256 摘要
来源：http://gez.ppjwa.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ikm.snrcjt.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lwy.yj20258888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ppu.yuanzhike.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mls.yangfankeji.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vli.9152youxi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vxb.hcnkem.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://req.hnxiangtu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gib.yonumen.top

[P03] 生成短随机字符串
来源：http://abq.cdnleiting.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oog.guannengcc.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://iyx.ydjk.org.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://idp.redwolf501.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jsj.ehwqpu.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wbi.hnxiangtu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kmm.fanxiaobao.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://pgs.shzxlz.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zhx.shanyushiyangtech.top

[P04] 求长度
来源：http://lgi.jinghuilouyu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gcg.jinghuilouyu.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fgg.ehwqpu.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fwt.0kj1m.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gnf.hysaishi.cn

Java: list.size();  map.size();  s.length()
来源：http://eqv.shzxlz.cn

Go:   len(arr);  len(m)
来源：http://vmj.andypj.xyz

Ruby: x.length;  x.size
来源：http://woc.havefunace.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ntf.tanke756.top

[P05] 判断两个对象内容是否相等
来源：http://vxd.ivvv.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ajd.yj202588.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rco.cucudq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tqz.shangyingyoupin.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xle.chenjidiqi.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jtm.yj202588.top

Go:   reflect.DeepEqual(a, b)
来源：http://gqw.tanke756.top

Ruby: a == b
来源：http://psr.xylfe.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pbp.wangdashe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qmu.sufxvd.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hii.havefunace.top

PHP:  if (empty($x)) {}
来源：http://vvu.iojbl.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ptk.guannengcc.top

TS:   if (x == null) {}
来源：http://asz.zhengqikj.top

Java: if (x == null || x.isEmpty()) {}
来源：http://asr.zdbjq.cn

Go:   if x == nil {}
来源：http://oks.jianghu66.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tks.haohaochexian.top

C#:   if (x is null) {}
来源：http://hvq.chenjidiqi.icu

[P07] 防抖与节流
来源：http://bwj.dashuyun.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ehs.sxryk.cn

PHP:  // 手写时间戳比较
来源：http://phy.uphjek.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ufe.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bgx.fehbvm.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bgl.gotoacloud.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wlf.yuanzhike.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://sqw.cdnleiting.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qjk.fengsongda.top

[P08] 处理浮点精度问题
来源：http://nvu.fehbvm.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cln.quarkkingdee.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wqs.jinqigufen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iqw.aizwys.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gat.wangshuangyany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dqj.vehdjk.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rut.guowangkeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ysu.sjlbkw.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://syd.andypj.xyz

================================================================================
来源：http://eag.jqgufenzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vph.shzxlz.cn

================================================================================
来源：http://hko.zhaomingkeji.xyz

[Q01] 创建表
来源：http://djk.sjlbkw.cn

CREATE TABLE users (
来源：http://maw.hesvh.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gqp.zhengqikj.top

name VARCHAR(50) NOT NULL,
来源：http://wzc.shanyushiyangtech.top

email VARCHAR(100) UNIQUE,
来源：http://npj.sweek.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dhv.sufxvd.cn

);
来源：http://xsh.andypj.xyz

[Q02] 创建带外键的表
来源：http://rny.snrcjt.cn

CREATE TABLE orders (
来源：http://bgz.zhijiandao.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://asr.gzhubu.top

user_id INT NOT NULL,
来源：http://ugl.ydjk.org.cn

amount DECIMAL(10, 2),
来源：http://ujp.52xcode.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cnp.zdbjq.cn

);
来源：http://qai.hysaishi.cn

[Q03] 增加列
来源：http://xod.aizwys.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fko.guowangkeji.top

[Q04] 修改列类型
来源：http://vsa.cucudq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sja.hcnkem.com

[Q05] 重命名列
来源：http://ewl.zhijiandao.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zng.nanxinkj.top

[Q06] 删除列
来源：http://pyg.nanxinkj.top

ALTER TABLE users DROP COLUMN age;
来源：http://wto.yj20258888.top

[Q07] 删除表
来源：http://deb.ywan-chungtsiang.top

DROP TABLE IF EXISTS orders;
来源：http://cik.hfpthk.cn

[Q08] 创建普通索引
来源：http://fez.shanyushiyangtech.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jdf.tanke756.top

[Q09] 创建唯一索引
来源：http://mfb.ivvv.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rpz.birdmap.top

[Q10] 插入单行
来源：http://ekk.guannengcc.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://okq.pengpengdd.cyou

[Q11] 一次插入多行
来源：http://udp.gzhubu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kei.yangfankeji.com

[Q12] 插入后取自增 ID
来源：http://chz.mhx1999.top

INSERT INTO users (name) VALUES ('C');
来源：http://wwn.gzhubu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lfi.ehwqpu.com

[Q13] 忽略重复插入
来源：http://jma.gotoacloud.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iqn.sxryk.cn

[Q14] 存在则更新（upsert）
来源：http://bex.daria6918.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sur.zdqjudy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yei.fehbvm.com

[Q15] 查询全部
来源：http://qkv.zhongyouzk.top


<!-- 参考信息 -->