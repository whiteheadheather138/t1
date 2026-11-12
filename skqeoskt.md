代发 wailian999

Py:   if __name__ == "__main__":
来源：http://pgl.aizwys.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sgo.316326.xyz

JS:   require.main === module
来源：http://nrd.sjlbkw.cn

TS:   require.main === module
来源：http://fit.nwbrower.top

Java: public static void main(String[] args)
来源：http://cyv.jqgufenzy.top

Go:   func main()
来源：http://hpo.zdqjudy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ill.fanxiaobao.xyz

C#:   static void Main(string[] args)
来源：http://vjq.gogol.net.cn

[M08] 获取系统与运行时信息
来源：http://mov.havefunace.top

Py:   platform.system();  platform.python_version()
来源：http://vih.shanyushiyangtech.top

PHP:  PHP_OS;  phpversion();
来源：http://yiq.yueranfly.top

JS:   process.platform;  process.version
来源：http://fgf.xuanzx.com

TS:   process.platform;  process.version
来源：http://svz.hywenlv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nhg.wangdashe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pdg.shanyushiyangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qjs.fengsongda.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rvr.zhoulong.xyz

================================================================================
来源：http://nqy.aibaodan.cn

N. 数据结构与算法
来源：http://xur.yuanzhike.top

================================================================================
来源：http://asd.zhijiandao.cn

[N01] 二分查找（有序数组）
来源：http://etc.tarul.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pli.wangshuangyany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dxb.fktsv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xkl.dashuyun.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sux.yanxiufei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://shb.jianghu66.top

Go:   sort.SearchInts(arr, x)
来源：http://tna.shzxlz.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bkl.dianchejie.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wac.tarul.cn

[N02] 排序（工程实践用内置实现）
来源：http://xhf.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://ifu.shzxlz.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lmd.pycfn.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://cjs.gaohongyu789.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lrr.zhiwuduotai.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rgo.zhoulong.xyz

Go:   slices.Sort(arr)
来源：http://edv.zhiwuduotai.top

Ruby: arr.sort
来源：http://uyj.shzxlz.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://fuz.yonumen.top

[N03] 快速排序（分治示例）
来源：http://gne.chenzaomai.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qug.sysykeji.top

PHP:  // 递归实现，或用 usort
来源：http://oge.hcnkem.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sgx.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hsz.haohaochexian.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lcd.gotoacloud.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yzq.iojbl.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://usr.cqqwz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fdp.yj20258888.top

[N04] 斐波那契数列
来源：http://ckt.shanyushiyangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aql.gzhubu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rap.yangfankeji.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vql.dashuyun.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bfe.tanke756.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://djm.9152youxi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dap.yueranfly.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mez.cheryme.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://glc.ybcxt.top

[N05] 最大公约数
来源：http://uuo.hywenlv.cn

Py:   math.gcd(a, b)
来源：http://czu.c1oappe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gxl.nanxinkj.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://doq.bbcook.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://epm.yvedp.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qhe.cheryme.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hog.smart0.xyz

Ruby: a.gcd(b)
来源：http://iwt.vqdsnc.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uhb.yj202588.top

[N06] 判断回文字符串
来源：http://ygh.birdmap.top

Py:   s == s[::-1]
来源：http://jbc.ydjk.org.cn

PHP:  $s === strrev($s);
来源：http://gue.hnxiangtu.top

JS:   s === [...s].reverse().join("")
来源：http://ffg.zdbjq.cn

TS:   s === [...s].reverse().join("")
来源：http://bkx.shanyushiyangtech.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://slg.cucudq.cn

Go:   // 双指针从两端比较
来源：http://zcb.pengpengdd.cyou

Ruby: s == s.reverse
来源：http://ivt.hesvh.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yyh.tian-w.cn

[N07] 两数之和（返回下标）
来源：http://ppd.guannengcc.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mui.hesvh.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wid.bbcook.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://naq.nanxuanxn.top

TS:   // 手写 Map<string, number>
来源：http://bxs.birdmap.top

Java: // 手写 HashMap
来源：http://gds.yfazqb.com

Go:   // 手写 map[int]int
来源：http://xdv.hongshengwenyu.top

Ruby: // 手写 Hash
来源：http://kta.shanyushiyangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://wqu.ppjwa.cn

[N08] 生成全排列
来源：http://gjc.hongshengwenyu.top

Py:   itertools.permutations(arr)
来源：http://mfh.pengpengdd.cyou

PHP:  // 手写递归交换
来源：http://eiz.andypj.xyz

JS:   // 手写回溯递归
来源：http://zjt.ydjk.org.cn

TS:   // 手写回溯递归
来源：http://epe.chenzaomai.com

Java: // 手写回溯递归
来源：http://ale.zhijiandao.cn

Go:   // 手写回溯递归
来源：http://alb.snrcjt.cn

Ruby: arr.permutation.to_a
来源：http://sdj.daria6918.cn

C#:   // 手写回溯递归
来源：http://wia.yonumen.top

[N09] 栈与队列
来源：http://orf.tianlin.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xza.zdbjq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://iku.ivvv.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qeh.c1oappe.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bcb.hongshengwenyu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://kbz.ehwqpu.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jwj.chenzaomai.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ejq.nanxinkj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ggd.shanyushiyangtech.top

[N10] 链表节点定义
来源：http://sim.cqqwz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tzh.dashuyun.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://rva.ywan-chungtsiang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bvo.uphjek.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ufk.ehwqpu.com

Java: class Node { int v; Node next; }
来源：http://edf.fengsongda.top

Go:   type Node struct { V int; Next *Node }
来源：http://scd.yanxiufei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rnu.guannengcc.top

C#:   class Node { public int V; public Node? Next; }
来源：http://yyb.jinghuilouyu.cn

[N11] 二叉树中序遍历
来源：http://elb.hfpthk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nlb.xylfe.cn

PHP:  // 手写递归函数
来源：http://igj.cashguo.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sqm.feifeiyinyue.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xdp.zdbjq.cn

Java: // 手写递归
来源：http://laa.yj20258888.top

Go:   // 手写递归
来源：http://grx.hywenlv.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wuj.iojbl.cn

C#:   // 手写递归
来源：http://bzj.hcnkem.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bry.xziqi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vfg.hfpthk.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ish.fehbvm.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://srj.dianchejie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qra.shangyingyoupin.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kyu.aibaodan.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jub.kuanghao11.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cde.guannengcc.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zuo.jinyuanbaomall.cn

================================================================================
来源：http://mvz.hnxiangtu.top

O. 并发与异步
来源：http://afg.bjfxy.top

================================================================================
来源：http://jtv.fktsv.cn

[O01] 启动一个线程
来源：http://cfy.yfazqb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jry.ydjk.org.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tcy.jinqigufen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bqy.yj20258.top

TS:   // 同 JS
来源：http://rxv.cheryme.top

Java: new Thread(() -> f()).start()
来源：http://jns.feifeiyinyue.top

Go:   go f()
来源：http://ggn.yfazqb.com

Ruby: Thread.new { f }
来源：http://nce.chenjidiqi.icu

C#:   Task.Run(() => F());
来源：http://pge.hysaishi.cn

[O02] 使用线程池
来源：http://wmz.guowangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xpm.jianghu66.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gxr.ctjpmb.com

JS:   // worker_threads 线程池
来源：http://tnw.yangfankeji.com

TS:   // worker_threads 线程池
来源：http://nrt.yanxiufei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://tjt.iojbl.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jac.hongshengwenyu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xuu.ydjk.org.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://neh.aizwys.cn

[O03] 加锁保护共享数据
来源：http://rmu.vqdsnc.cn

Py:   with lock: shared += 1
来源：http://bnk.xuetiantiany.cn

PHP:  // 用 flock() 做文件锁
来源：http://oyd.52xcode.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oxh.dashuyun.cn

TS:   // 同 JS
来源：http://zql.zdbjq.cn

Java: synchronized (this) { shared++; }
来源：http://wej.tianlin.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ltj.jlsjyb.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kmq.yj202588.top

C#:   lock (gate) { shared++; }
来源：http://oqv.redwolf501.top

[O04] 定义异步函数并等待
来源：http://oun.meibo888.top

Py:   async def f():⏎    await g()
来源：http://gpp.ydzc1.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eyc.zycfv.cn

JS:   async function f() { await g(); }
来源：http://rjc.cqqwz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://thu.iojbl.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xer.yuanzhike.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://shn.tarul.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gsv.sweek.top

C#:   async Task F() { await G(); }
来源：http://nyz.yueranfly.top

[O05] 并发执行并等待全部完成
来源：http://prv.zhijiandao.cn

Py:   asyncio.gather(*tasks)
来源：http://nkg.ydzc1.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fhd.hongshengwenyu.top

JS:   await Promise.all(tasks)
来源：http://laa.tarul.cn

TS:   await Promise.all(tasks)
来源：http://qbs.cheryme.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kxw.hcnkem.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jth.wangshuangyany.cn

Ruby: threads.map(&:join)
来源：http://nzf.shuidangran.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ajq.zdbjq.cn

[O06] 使用进程池
来源：http://bdh.iojbl.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yjp.jyoumei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ktt.jlsjyb.cn

JS:   // child_process / cluster 模块
来源：http://yay.chenzaomai.com

TS:   // child_process / cluster 模块
来源：http://vqh.nanxinkj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://umi.aibaodan.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hwp.yj202588.top

Ruby: // fork 块
来源：http://jnv.nanxuanxn.top

C#:   Parallel.For
来源：http://mcd.daria6918.cn

================================================================================
来源：http://vkn.svipenyu.cn

P. 常用工具函数
来源：http://dbr.smart0.xyz

================================================================================
来源：http://lif.tian-w.cn

[P01] 生成 UUID
来源：http://oxq.sxryk.cn

Py:   str(uuid.uuid4())
来源：http://dsu.xuetiantiany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://imh.cdnleiting.top

JS:   crypto.randomUUID()
来源：http://eve.svipenyu.cn

TS:   crypto.randomUUID()
来源：http://vfw.ctjpmb.com

Java: UUID.randomUUID().toString()
来源：http://dbr.xingfuxueyuan.xyz

Go:   // 用 github.com/google/uuid
来源：http://pui.fzhhl.top

Ruby: SecureRandom.uuid
来源：http://gcl.xylfe.cn

C#:   Guid.NewGuid().ToString()
来源：http://miq.zdbjq.cn

[P02] MD5 / SHA256 摘要
来源：http://imt.bjfxy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dua.xingfuxueyuan.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://azr.c1oappe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zyb.sxryk.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hvu.quarkkingdee.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mud.yuanzhike.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bte.zhixingplan.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vik.gzhubu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rnx.52xcode.cn

[P03] 生成短随机字符串
来源：http://yik.gogol.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vqw.ydzc1.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://biz.pengpengdd.cyou

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://loi.wangshuangyany.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gzs.cashguo.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wot.vehdjk.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nve.jinqigufen.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ohf.hywenlv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nsi.cucudq.cn

[P04] 求长度
来源：http://hro.hesvh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://byi.dianchejie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qoh.yuanzhike.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xdq.jinyuanbaomall.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://byf.shanyushiyangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://aro.zdqjudy.top

Go:   len(arr);  len(m)
来源：http://jye.aibaodan.cn

Ruby: x.length;  x.size
来源：http://npz.fanxiaobao.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://rua.316326.xyz

[P05] 判断两个对象内容是否相等
来源：http://ulj.havefunace.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://uar.9152youxi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://coa.daria6918.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dkd.cashguo.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://njv.zhoulong.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tyl.guannengcc.top

Go:   reflect.DeepEqual(a, b)
来源：http://xox.cucudq.cn

Ruby: a == b
来源：http://ahn.jinyuanbaomall.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wvm.ehwqpu.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mdo.yongpay.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qoz.chenjidiqi.icu

PHP:  if (empty($x)) {}
来源：http://obb.fengsongda.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blr.zhongyouzk.top

TS:   if (x == null) {}
来源：http://ggd.sxryk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ffi.nanxuanxn.top

Go:   if x == nil {}
来源：http://xda.smart0.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://brx.zdqjudy.top

C#:   if (x is null) {}
来源：http://vnq.ctjpmb.com

[P07] 防抖与节流
来源：http://aqo.9152youxi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://snu.fengsongda.top

PHP:  // 手写时间戳比较
来源：http://diw.guowangkeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vvn.52xcode.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://glg.hesvh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vvr.xuanzx.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://epq.chenlongwang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gru.zdbjq.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mek.cheryme.top

[P08] 处理浮点精度问题
来源：http://rfe.xinyue.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iac.jyoumei.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vgo.dianchejie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qif.jlsjyb.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://doa.ybcxt.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tkq.aibaodan.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xqy.uphjek.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oau.shuidangran.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qys.nwbrower.top

================================================================================
来源：http://cjz.zdbjq.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kij.sufxvd.cn

================================================================================
来源：http://lfh.chenlongwang.top

[Q01] 创建表
来源：http://qao.sweek.top

CREATE TABLE users (
来源：http://kkn.xylfe.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dhd.zhoulong.xyz

name VARCHAR(50) NOT NULL,
来源：http://kxz.birdmap.top

email VARCHAR(100) UNIQUE,
来源：http://rbc.dashuyun.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wqb.hammf.cn

);
来源：http://xnp.zhengqikj.top

[Q02] 创建带外键的表
来源：http://pta.xziqi.cn

CREATE TABLE orders (
来源：http://tiu.uphjek.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ejw.kuanghao11.cn

user_id INT NOT NULL,
来源：http://cum.ppjwa.cn

amount DECIMAL(10, 2),
来源：http://wdf.hysaishi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fnj.jqgufenzy.top

);
来源：http://bsm.zdbjq.cn

[Q03] 增加列
来源：http://smy.xinyue.icu

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nlr.uphjek.com

[Q04] 修改列类型
来源：http://qlb.bjfxy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vop.daxiang520.top

[Q05] 重命名列
来源：http://cbv.fengsongda.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gsi.fehbvm.com

[Q06] 删除列
来源：http://uui.ppjwa.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yfm.yangfankeji.com

[Q07] 删除表
来源：http://wco.sweek.top

DROP TABLE IF EXISTS orders;
来源：http://aow.hfpthk.cn

[Q08] 创建普通索引
来源：http://nru.zhoulong.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://wir.52xcode.cn

[Q09] 创建唯一索引
来源：http://dpz.fktsv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://the.cdnleiting.top

[Q10] 插入单行
来源：http://eql.gzhubu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://grb.yj202588.top

[Q11] 一次插入多行
来源：http://ufg.yfazqb.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nuh.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://ics.nwbrower.top

INSERT INTO users (name) VALUES ('C');
来源：http://dav.daria6918.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wzo.xuetiantiany.cn

[Q13] 忽略重复插入
来源：http://dfx.jqgufenzy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pbs.meibo888.top


<!-- 参考信息 -->