代发 wailian999

Py:   if __name__ == "__main__":
来源：http://ibh.andypj.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jds.yj20258888.top

JS:   require.main === module
来源：http://scm.wangshuangyany.cn

TS:   require.main === module
来源：http://qeu.bjfxy.top

Java: public static void main(String[] args)
来源：http://dlf.tianlin.xyz

Go:   func main()
来源：http://epo.ivvv.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cri.chenjidiqi.icu

C#:   static void Main(string[] args)
来源：http://aad.jinqigufen.top

[M08] 获取系统与运行时信息
来源：http://qgp.fengsongda.top

Py:   platform.system();  platform.python_version()
来源：http://qhs.ppjwa.cn

PHP:  PHP_OS;  phpversion();
来源：http://lcq.shuidangran.top

JS:   process.platform;  process.version
来源：http://xrh.fengsongda.top

TS:   process.platform;  process.version
来源：http://hlr.jiagoushi.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hcv.tian-w.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ecb.redwolf501.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://psg.sweek.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lwv.jqgfzy.top

================================================================================
来源：http://art.zhaomingkeji.xyz

N. 数据结构与算法
来源：http://zwm.shanyushiyangkeji.top

================================================================================
来源：http://yqs.dashuyun.cn

[N01] 二分查找（有序数组）
来源：http://crn.yuxming.cn

Py:   bisect.bisect_left(arr, x)
来源：http://erf.meibo888.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rxx.ctjpmb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ktv.cdnleiting.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jqb.jiagoushi.top

Java: Arrays.binarySearch(arr, x)
来源：http://jox.sysykeji.top

Go:   sort.SearchInts(arr, x)
来源：http://fyf.bbcook.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://boh.zdbjq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://tgg.cdnleiting.top

[N02] 排序（工程实践用内置实现）
来源：http://tlw.haohaochexian.top

Py:   sorted(arr);  arr.sort()
来源：http://yqo.shanyushiyangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wni.ivvv.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://miw.havefunace.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://job.yuxming.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://axv.yj202588.top

Go:   slices.Sort(arr)
来源：http://tkt.svipenyu.cn

Ruby: arr.sort
来源：http://npv.jinqigufen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hyy.gaohongyu789.top

[N03] 快速排序（分治示例）
来源：http://tae.ppjwa.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mji.fktsv.cn

PHP:  // 递归实现，或用 usort
来源：http://dng.ehwqpu.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://okx.fengsongda.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mrq.yvedp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rhi.hcnkem.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qhv.jlsjyb.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tzw.fzhhl.top

C#:   // 手写递归，或 Array.Sort
来源：http://nzb.hnqzz.top

[N04] 斐波那契数列
来源：http://qjv.shangyingyoupin.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kql.ppjwa.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://aia.shzxlz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jyw.hcnkem.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bsz.shanyushiyangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pge.zdqjudy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tlk.yanxiufei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qsj.jqgfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dzd.uphjek.com

[N05] 最大公约数
来源：http://csu.hnqzz.top

Py:   math.gcd(a, b)
来源：http://htj.tianlin.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uwm.cqqwz.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pfi.wangdashe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tmg.jinqigufen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kew.hcnkem.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cmt.yj202588.top

Ruby: a.gcd(b)
来源：http://yjp.wangshuangyany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vap.jiagoushi.top

[N06] 判断回文字符串
来源：http://kbp.yvedp.cn

Py:   s == s[::-1]
来源：http://iro.316326.xyz

PHP:  $s === strrev($s);
来源：http://vmc.wangshuangyany.cn

JS:   s === [...s].reverse().join("")
来源：http://gyk.wangdashe.top

TS:   s === [...s].reverse().join("")
来源：http://ahq.jinqigfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ops.redwolf501.top

Go:   // 双指针从两端比较
来源：http://uzs.ydzc1.top

Ruby: s == s.reverse
来源：http://rge.hysaishi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vhu.fehbvm.com

[N07] 两数之和（返回下标）
来源：http://gtq.ybcxt.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mao.dianchejie.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hgw.gogol.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ujr.yuanzhike.top

TS:   // 手写 Map<string, number>
来源：http://eno.xziqi.cn

Java: // 手写 HashMap
来源：http://lvp.pycfn.com

Go:   // 手写 map[int]int
来源：http://cpv.yongpay.top

Ruby: // 手写 Hash
来源：http://mnu.hesvh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tvo.zhengqikj.top

[N08] 生成全排列
来源：http://dlo.zycfv.cn

Py:   itertools.permutations(arr)
来源：http://ups.gotoacloud.top

PHP:  // 手写递归交换
来源：http://rda.hammf.cn

JS:   // 手写回溯递归
来源：http://keo.yj20258888.top

TS:   // 手写回溯递归
来源：http://ztb.yvedp.cn

Java: // 手写回溯递归
来源：http://qmq.nanxuanxn.top

Go:   // 手写回溯递归
来源：http://gcf.fanxiaobao.xyz

Ruby: arr.permutation.to_a
来源：http://ase.nanxuanxn.top

C#:   // 手写回溯递归
来源：http://zyz.yonumen.top

[N09] 栈与队列
来源：http://bzb.yj202588.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wus.xziqi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ibs.cdnleiting.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lgv.shuidangran.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gxd.wangdashe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mce.gaohongyu789.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ntg.c1oappe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ajp.52xcode.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://crs.pengpengdd.cyou

[N10] 链表节点定义
来源：http://xxm.jinqigfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hiz.fzhhl.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ged.jlsjyb.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://akp.c1oappe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zeb.smart0.xyz

Java: class Node { int v; Node next; }
来源：http://izd.sjlbkw.cn

Go:   type Node struct { V int; Next *Node }
来源：http://bqy.jinghuilouyu.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://etk.xylfe.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://eqf.xylfe.cn

[N11] 二叉树中序遍历
来源：http://vdv.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mhv.jinyuanbaomall.cn

PHP:  // 手写递归函数
来源：http://dgk.iojbl.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jur.sxryk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://car.jinqigfzy.top

Java: // 手写递归
来源：http://ncv.tanke756.top

Go:   // 手写递归
来源：http://xpe.ppjwa.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ajs.chenlongwang.top

C#:   // 手写递归
来源：http://maj.nanxuanxn.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vcf.shuidangran.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gzc.yonumen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wfy.hammf.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xvf.yanxiufei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sak.yangfankeji.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yse.guowangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pix.dianchejie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wjw.sweek.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kmd.shanyushiyangtech.top

================================================================================
来源：http://lth.vqdsnc.cn

O. 并发与异步
来源：http://msv.yj20258.top

================================================================================
来源：http://fiu.c1oappe.top

[O01] 启动一个线程
来源：http://ebr.guannengcc.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://czx.jqgfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lxs.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pjz.daria6918.cn

TS:   // 同 JS
来源：http://khp.9152youxi.cn

Java: new Thread(() -> f()).start()
来源：http://oyl.havefunace.top

Go:   go f()
来源：http://ydw.zhongyouzk.top

Ruby: Thread.new { f }
来源：http://uyk.yanxiufei.cn

C#:   Task.Run(() => F());
来源：http://nsq.sysykeji.top

[O02] 使用线程池
来源：http://amt.cdnleiting.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mfj.andypj.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gnc.sxryk.cn

JS:   // worker_threads 线程池
来源：http://ttv.hnxiangtu.top

TS:   // worker_threads 线程池
来源：http://fyw.zdqjudy.top

Java: Executors.newFixedThreadPool(4)
来源：http://oex.tanke756.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qfq.nanxinkj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iar.0kj1m.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gql.wangdashe.top

[O03] 加锁保护共享数据
来源：http://hay.hcnkem.com

Py:   with lock: shared += 1
来源：http://yfz.meibo888.top

PHP:  // 用 flock() 做文件锁
来源：http://xha.hongshengwenyu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tmh.chenjidiqi.icu

TS:   // 同 JS
来源：http://iiq.sjlbkw.cn

Java: synchronized (this) { shared++; }
来源：http://tuv.iojbl.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gzj.ctjpmb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://afb.bbcook.cn

C#:   lock (gate) { shared++; }
来源：http://jkw.mhx1999.top

[O04] 定义异步函数并等待
来源：http://wwi.tianlin.xyz

Py:   async def f():⏎    await g()
来源：http://vbz.ctjpmb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lxp.shuidangran.top

JS:   async function f() { await g(); }
来源：http://plj.zhengqikj.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://iet.redwolf501.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mwh.jianghu66.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cqe.cqqwz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rub.shangyingyoupin.top

C#:   async Task F() { await G(); }
来源：http://qdp.cheryme.top

[O05] 并发执行并等待全部完成
来源：http://gna.tian-w.cn

Py:   asyncio.gather(*tasks)
来源：http://lrc.quarkkingdee.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ytf.hnqzz.top

JS:   await Promise.all(tasks)
来源：http://kph.cqqwz.cn

TS:   await Promise.all(tasks)
来源：http://uso.snrcjt.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wkr.jyoumei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://muj.jqgufenzy.top

Ruby: threads.map(&:join)
来源：http://rbt.cdnleiting.top

C#:   await Task.WhenAll(t1, t2)
来源：http://rhe.sysykeji.top

[O06] 使用进程池
来源：http://xly.gotoacloud.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mpw.c1oappe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://cgg.vehdjk.com

JS:   // child_process / cluster 模块
来源：http://vju.jinqigufen.top

TS:   // child_process / cluster 模块
来源：http://jhi.ehwqpu.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lim.yangfankeji.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://suk.jinqigfzy.top

Ruby: // fork 块
来源：http://ohb.gzhubu.top

C#:   Parallel.For
来源：http://jpe.jinqigufen.top

================================================================================
来源：http://gem.wangdashe.top

P. 常用工具函数
来源：http://xex.nwbrower.top

================================================================================
来源：http://vwg.svipenyu.cn

[P01] 生成 UUID
来源：http://nqh.yuanzhike.top

Py:   str(uuid.uuid4())
来源：http://yfd.pycfn.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pcd.gotoacloud.top

JS:   crypto.randomUUID()
来源：http://mxe.jqgufenzy.top

TS:   crypto.randomUUID()
来源：http://sfm.hongshengwenyu.top

Java: UUID.randomUUID().toString()
来源：http://qfk.zhoulong.xyz

Go:   // 用 github.com/google/uuid
来源：http://ajo.yj20258888.top

Ruby: SecureRandom.uuid
来源：http://owf.zhaomingkeji.xyz

C#:   Guid.NewGuid().ToString()
来源：http://itf.hnqzz.top

[P02] MD5 / SHA256 摘要
来源：http://mkl.ehwqpu.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aug.andypj.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://qlq.ybcxt.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xje.jinyuanbaomall.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://iys.redwolf501.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ndn.jianghu66.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://asd.mhx1999.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fwi.ywan-chungtsiang.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uuh.guannengcc.top

[P03] 生成短随机字符串
来源：http://fjr.nwbrower.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ylf.ctjpmb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yoe.yuanzhike.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dul.cucudq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wew.iojbl.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ysb.zdqjudy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cvr.zdbjq.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qka.ehwqpu.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vhs.sjlbkw.cn

[P04] 求长度
来源：http://pei.hongshengwenyu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yrx.hysaishi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ktx.cucudq.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nzi.yanxiufei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vzj.zhengqikj.top

Java: list.size();  map.size();  s.length()
来源：http://ynf.fengsongda.top

Go:   len(arr);  len(m)
来源：http://smo.uphjek.com

Ruby: x.length;  x.size
来源：http://mfh.ehwqpu.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://ahu.zdqjudy.top

[P05] 判断两个对象内容是否相等
来源：http://ezr.aibaodan.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hci.yanxiufei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hoo.ywan-chungtsiang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://msc.shuidangran.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fbp.guowangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dlx.hywenlv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://abq.cheryme.top

Ruby: a == b
来源：http://fvd.havefunace.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xjv.chenzaomai.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://emt.chenzaomai.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ypc.vehdjk.com

PHP:  if (empty($x)) {}
来源：http://fio.havefunace.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ont.yj20258888.top

TS:   if (x == null) {}
来源：http://fen.dashuyun.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pyn.zhongyouzk.top

Go:   if x == nil {}
来源：http://enz.zhaomingkeji.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gmp.guowangkeji.top

C#:   if (x is null) {}
来源：http://fne.shangyingyoupin.top

[P07] 防抖与节流
来源：http://kmd.tarul.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nhw.ywan-chungtsiang.top

PHP:  // 手写时间戳比较
来源：http://rdw.hysaishi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ndm.smart0.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://epv.kuanghao11.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fyq.havefunace.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vrh.birdmap.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cae.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uif.gzhubu.top

[P08] 处理浮点精度问题
来源：http://ioy.chenjidiqi.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lly.yfazqb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pkk.smart0.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://acx.yongpay.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nro.hammf.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ima.gotoacloud.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iow.vqdsnc.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://muw.xziqi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cdk.aizwys.cn

================================================================================
来源：http://rcq.ywan-chungtsiang.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ohc.jiagoushi.top

================================================================================
来源：http://mez.ppjwa.cn

[Q01] 创建表
来源：http://tas.fanxiaobao.xyz

CREATE TABLE users (
来源：http://cun.cqqwz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://anx.shuidangran.top

name VARCHAR(50) NOT NULL,
来源：http://uml.ydzc1.top

email VARCHAR(100) UNIQUE,
来源：http://fzm.meibo888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qgl.nanxinkj.top

);
来源：http://atd.jianghu66.top

[Q02] 创建带外键的表
来源：http://txg.tanke756.top

CREATE TABLE orders (
来源：http://vyr.0kj1m.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pob.andypj.xyz

user_id INT NOT NULL,
来源：http://mho.cheryme.top

amount DECIMAL(10, 2),
来源：http://wuk.svipenyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vfw.316326.xyz

);
来源：http://ena.zhengqikj.top

[Q03] 增加列
来源：http://xyx.nanxinkj.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ojn.sxryk.cn

[Q04] 修改列类型
来源：http://jar.wangdashe.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ufs.dianchejie.cn

[Q05] 重命名列
来源：http://ccj.gotoacloud.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://iph.zhoulong.xyz

[Q06] 删除列
来源：http://aqk.bjfxy.top

ALTER TABLE users DROP COLUMN age;
来源：http://lkn.svipenyu.cn

[Q07] 删除表
来源：http://gmz.pengpengdd.cyou

DROP TABLE IF EXISTS orders;
来源：http://qts.wangshuangyany.cn

[Q08] 创建普通索引
来源：http://iic.ehwqpu.com

CREATE INDEX idx_users_email ON users(email);
来源：http://ulq.redwolf501.top

[Q09] 创建唯一索引
来源：http://gxs.ydjk.org.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://khn.epnwcf.com

[Q10] 插入单行
来源：http://pzu.hcnkem.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nyv.ydzc1.top

[Q11] 一次插入多行
来源：http://ifc.c1oappe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zzd.chenlongwang.top

[Q12] 插入后取自增 ID
来源：http://bxy.fengsongda.top

INSERT INTO users (name) VALUES ('C');
来源：http://unh.jianghu66.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lda.gogol.net.cn

[Q13] 忽略重复插入
来源：http://yvz.snrcjt.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://axu.hongshengwenyu.top


<!-- 参考信息 -->