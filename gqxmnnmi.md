代发 wailian999

Py:   if __name__ == "__main__":
来源：http://lvu.dianchejie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nbs.svipenyu.cn

JS:   require.main === module
来源：http://jtt.fengsongda.top

TS:   require.main === module
来源：http://eti.hfpthk.cn

Java: public static void main(String[] args)
来源：http://jaz.feifeiyinyue.top

Go:   func main()
来源：http://xza.sxryk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rme.nanxuanxn.top

C#:   static void Main(string[] args)
来源：http://xcy.dianchejie.cn

[M08] 获取系统与运行时信息
来源：http://vpa.smart0.xyz

Py:   platform.system();  platform.python_version()
来源：http://rmx.gogol.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://iiz.dianchejie.cn

JS:   process.platform;  process.version
来源：http://abh.vehdjk.com

TS:   process.platform;  process.version
来源：http://rrr.daxiang520.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://low.aibaodan.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nba.dashuyun.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bce.yfazqb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://xhe.nanxinkj.top

================================================================================
来源：http://evr.hcnkem.com

N. 数据结构与算法
来源：http://whb.zycfv.cn

================================================================================
来源：http://chm.wangshuangyany.cn

[N01] 二分查找（有序数组）
来源：http://azr.ctjpmb.com

Py:   bisect.bisect_left(arr, x)
来源：http://sfw.sjlbkw.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://grn.pengpengdd.cyou

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mss.shanyushiyangtech.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sdf.gzhubu.top

Java: Arrays.binarySearch(arr, x)
来源：http://jwv.yfazqb.com

Go:   sort.SearchInts(arr, x)
来源：http://uob.ivvv.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hkh.uphjek.com

C#:   Array.BinarySearch(arr, x)
来源：http://nge.bbcook.cn

[N02] 排序（工程实践用内置实现）
来源：http://hfa.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://npc.gogol.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gwu.ybcxt.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jxz.fzhhl.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dzy.zdbjq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dwn.jinyuanbaomall.cn

Go:   slices.Sort(arr)
来源：http://uzr.gzhubu.top

Ruby: arr.sort
来源：http://vfc.wangshuangyany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://kng.ehwqpu.com

[N03] 快速排序（分治示例）
来源：http://hgv.hesvh.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dkr.cheryme.top

PHP:  // 递归实现，或用 usort
来源：http://dlp.zhoulong.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blo.aizwys.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://erv.ppjwa.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jnd.tarul.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nvq.jinyuanbaomall.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vyn.hesvh.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dnm.iojbl.cn

[N04] 斐波那契数列
来源：http://njy.yuanzhike.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ojr.ywan-chungtsiang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lon.shuidangran.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gay.c1oappe.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mna.pengpengdd.cyou

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://huw.ydjk.org.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://giw.ivvv.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ekm.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sbu.zdbjq.cn

[N05] 最大公约数
来源：http://bih.wangshuangyany.cn

Py:   math.gcd(a, b)
来源：http://ojm.shuidangran.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vqg.quarkkingdee.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oja.yonumen.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vqf.uphjek.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qir.jiagoushi.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dct.hfpthk.cn

Ruby: a.gcd(b)
来源：http://lcg.jlsjyb.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xav.fehbvm.com

[N06] 判断回文字符串
来源：http://tod.daria6918.cn

Py:   s == s[::-1]
来源：http://ugp.xylfe.cn

PHP:  $s === strrev($s);
来源：http://zwe.jinghuilouyu.cn

JS:   s === [...s].reverse().join("")
来源：http://sku.jqgufenzy.top

TS:   s === [...s].reverse().join("")
来源：http://lsg.52xcode.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nac.yongpay.top

Go:   // 双指针从两端比较
来源：http://svs.cheryme.top

Ruby: s == s.reverse
来源：http://ppx.pycfn.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://sng.yj20258.top

[N07] 两数之和（返回下标）
来源：http://qpw.jqgufenzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qxe.hnqzz.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iaq.dianchejie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://efk.ehwqpu.com

TS:   // 手写 Map<string, number>
来源：http://ipc.0kj1m.cn

Java: // 手写 HashMap
来源：http://aan.fanxiaobao.xyz

Go:   // 手写 map[int]int
来源：http://ice.aizwys.cn

Ruby: // 手写 Hash
来源：http://szi.cashguo.top

C#:   // 手写 Dictionary<int, int>
来源：http://xgk.svipenyu.cn

[N08] 生成全排列
来源：http://rsa.jlsjyb.cn

Py:   itertools.permutations(arr)
来源：http://als.feifeiyinyue.top

PHP:  // 手写递归交换
来源：http://rtp.feifeiyinyue.top

JS:   // 手写回溯递归
来源：http://eqp.wangdashe.top

TS:   // 手写回溯递归
来源：http://ljb.0kj1m.cn

Java: // 手写回溯递归
来源：http://bqq.zhijiandao.cn

Go:   // 手写回溯递归
来源：http://mzf.yj20258.top

Ruby: arr.permutation.to_a
来源：http://lys.shanyushiyangtech.top

C#:   // 手写回溯递归
来源：http://edm.gaohongyu789.top

[N09] 栈与队列
来源：http://exv.cashguo.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vye.hnqzz.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xvo.sufxvd.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ood.bjfxy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mxk.ivvv.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mya.andypj.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gpj.daxiang520.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://doc.iojbl.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://abn.gaohongyu789.top

[N10] 链表节点定义
来源：http://erg.uphjek.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uzs.jiagoushi.top

PHP:  class Node { public $v; public $next = null; }
来源：http://wsl.ctjpmb.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://utm.epnwcf.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kel.yfazqb.com

Java: class Node { int v; Node next; }
来源：http://ovr.redwolf501.top

Go:   type Node struct { V int; Next *Node }
来源：http://oru.iojbl.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dwy.cucudq.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://qhm.meibo888.top

[N11] 二叉树中序遍历
来源：http://yuf.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fem.dashuyun.cn

PHP:  // 手写递归函数
来源：http://feo.aibaodan.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wje.hywenlv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://duk.cqqwz.cn

Java: // 手写递归
来源：http://dln.aizwys.cn

Go:   // 手写递归
来源：http://pqe.quarkkingdee.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://opd.sjlbkw.cn

C#:   // 手写递归
来源：http://caf.nanxinkj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pcv.gaohongyu789.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fed.feifeiyinyue.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zvl.c1oappe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zts.mhx1999.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lrz.0kj1m.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jxr.zhixingplan.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ezi.cucudq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lki.nanxinkj.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lod.yueranfly.top

================================================================================
来源：http://xvr.hesvh.cn

O. 并发与异步
来源：http://rfj.hysaishi.cn

================================================================================
来源：http://wcv.gotoacloud.top

[O01] 启动一个线程
来源：http://twj.hcnkem.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wus.jinqigufen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://shg.tianlin.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://any.iojbl.cn

TS:   // 同 JS
来源：http://kcm.shanyushiyangkeji.top

Java: new Thread(() -> f()).start()
来源：http://vqu.wangshuangyany.cn

Go:   go f()
来源：http://ihp.guannengcc.top

Ruby: Thread.new { f }
来源：http://amo.shanyushiyangtech.top

C#:   Task.Run(() => F());
来源：http://xoy.hywenlv.cn

[O02] 使用线程池
来源：http://rpf.cucudq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nzz.jyoumei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ojx.kuanghao11.cn

JS:   // worker_threads 线程池
来源：http://oea.nanxinkj.top

TS:   // worker_threads 线程池
来源：http://ojo.jinqigufen.top

Java: Executors.newFixedThreadPool(4)
来源：http://yxc.vqdsnc.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fby.fehbvm.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cyc.52xcode.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://glb.cdnleiting.top

[O03] 加锁保护共享数据
来源：http://aik.iojbl.cn

Py:   with lock: shared += 1
来源：http://nqe.zhongyouzk.top

PHP:  // 用 flock() 做文件锁
来源：http://die.smart0.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pbl.ehwqpu.com

TS:   // 同 JS
来源：http://ges.hnxiangtu.top

Java: synchronized (this) { shared++; }
来源：http://ibk.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qyt.yj20258888.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://lfs.chenlongwang.top

C#:   lock (gate) { shared++; }
来源：http://lpz.yfazqb.com

[O04] 定义异步函数并等待
来源：http://ydi.chenzaomai.com

Py:   async def f():⏎    await g()
来源：http://jcw.birdmap.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ocs.tanke756.top

JS:   async function f() { await g(); }
来源：http://dmp.fzhhl.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ufv.chenzaomai.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://eov.tanke756.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qci.316326.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://lku.ydzc1.top

C#:   async Task F() { await G(); }
来源：http://rjn.xylfe.cn

[O05] 并发执行并等待全部完成
来源：http://rbz.feifeiyinyue.top

Py:   asyncio.gather(*tasks)
来源：http://lvw.yuanzhike.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uqg.hesvh.cn

JS:   await Promise.all(tasks)
来源：http://sjj.yongpay.top

TS:   await Promise.all(tasks)
来源：http://vek.chenjidiqi.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://atr.tanke756.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cyu.ppjwa.cn

Ruby: threads.map(&:join)
来源：http://cei.chenzaomai.com

C#:   await Task.WhenAll(t1, t2)
来源：http://vwq.zdqjudy.top

[O06] 使用进程池
来源：http://uvs.zycfv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yrv.zhiwuduotai.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fbr.cdnleiting.top

JS:   // child_process / cluster 模块
来源：http://iwg.zhongyouzk.top

TS:   // child_process / cluster 模块
来源：http://bpf.yvedp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://aka.bbcook.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://auz.zycfv.cn

Ruby: // fork 块
来源：http://hmq.mhx1999.top

C#:   Parallel.For
来源：http://hdw.ppjwa.cn

================================================================================
来源：http://lik.jinyuanbaomall.cn

P. 常用工具函数
来源：http://qkf.bjfxy.top

================================================================================
来源：http://kwn.ehwqpu.com

[P01] 生成 UUID
来源：http://sjs.9152youxi.cn

Py:   str(uuid.uuid4())
来源：http://sgd.wangshuangyany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xua.cheryme.top

JS:   crypto.randomUUID()
来源：http://oeh.shuidangran.top

TS:   crypto.randomUUID()
来源：http://fwj.bbcook.cn

Java: UUID.randomUUID().toString()
来源：http://lsa.ydzc1.top

Go:   // 用 github.com/google/uuid
来源：http://fak.hcnkem.com

Ruby: SecureRandom.uuid
来源：http://fhy.zdbjq.cn

C#:   Guid.NewGuid().ToString()
来源：http://ytz.shzxlz.cn

[P02] MD5 / SHA256 摘要
来源：http://rvb.yj202588.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ckn.yangfankeji.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://oyj.kuanghao11.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wpe.pengpengdd.cyou

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://alf.shzxlz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sce.jqgfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ifw.gogol.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mqx.gaohongyu789.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://not.daria6918.cn

[P03] 生成短随机字符串
来源：http://qwz.zhongyouzk.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://frn.yuxming.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cja.vqdsnc.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yei.ybcxt.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hot.yongpay.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sxw.quarkkingdee.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zdc.wangdashe.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://oha.epnwcf.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tzr.fehbvm.com

[P04] 求长度
来源：http://dci.ydzc1.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wxq.fanxiaobao.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://osp.sufxvd.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://czs.nwbrower.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pge.yvedp.cn

Java: list.size();  map.size();  s.length()
来源：http://xpw.ydzc1.top

Go:   len(arr);  len(m)
来源：http://ajp.ehwqpu.com

Ruby: x.length;  x.size
来源：http://npa.hongshengwenyu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jxi.daria6918.cn

[P05] 判断两个对象内容是否相等
来源：http://wgx.meibo888.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ejz.cucudq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qme.chenjidiqi.icu

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tfs.tarul.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ddf.shanyushiyangtech.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pxm.zdbjq.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bbj.hongshengwenyu.top

Ruby: a == b
来源：http://zpo.yanxiufei.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://oqx.zycfv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://drx.andypj.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://urc.gogol.net.cn

PHP:  if (empty($x)) {}
来源：http://dim.pengpengdd.cyou

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rvu.dashuyun.cn

TS:   if (x == null) {}
来源：http://ljh.hcnkem.com

Java: if (x == null || x.isEmpty()) {}
来源：http://hog.cucudq.cn

Go:   if x == nil {}
来源：http://rau.gotoacloud.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uqg.zhaomingkeji.xyz

C#:   if (x is null) {}
来源：http://oqd.iojbl.cn

[P07] 防抖与节流
来源：http://rvj.jqgufenzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://teh.xinyue.icu

PHP:  // 手写时间戳比较
来源：http://slh.iojbl.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hhr.tarul.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dlv.snrcjt.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oss.shuidangran.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pta.hammf.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xsa.xuetiantiany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hen.birdmap.top

[P08] 处理浮点精度问题
来源：http://wvi.quarkkingdee.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tcv.vehdjk.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://edw.sufxvd.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nkf.chenzaomai.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eqi.zhixingplan.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://msk.yfazqb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zkx.zhoulong.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ehx.feifeiyinyue.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fha.chenzaomai.com

================================================================================
来源：http://hiz.yongpay.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://meq.aibaodan.cn

================================================================================
来源：http://brm.nwbrower.top

[Q01] 创建表
来源：http://ade.birdmap.top

CREATE TABLE users (
来源：http://woi.guannengcc.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kye.xuetiantiany.cn

name VARCHAR(50) NOT NULL,
来源：http://pdg.nanxuanxn.top

email VARCHAR(100) UNIQUE,
来源：http://rzh.yuanzhike.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kjf.cucudq.cn

);
来源：http://uiy.epnwcf.com

[Q02] 创建带外键的表
来源：http://tll.yj20258.top

CREATE TABLE orders (
来源：http://htf.316326.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ogk.yvedp.cn

user_id INT NOT NULL,
来源：http://flm.shangyingyoupin.top

amount DECIMAL(10, 2),
来源：http://wie.fehbvm.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://och.dashuyun.cn

);
来源：http://ydf.ppjwa.cn

[Q03] 增加列
来源：http://qza.9152youxi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fvn.0kj1m.cn

[Q04] 修改列类型
来源：http://tjq.jiagoushi.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://grc.cashguo.top

[Q05] 重命名列
来源：http://ekz.smart0.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jkh.ppjwa.cn

[Q06] 删除列
来源：http://rna.jianghu66.top

ALTER TABLE users DROP COLUMN age;
来源：http://pge.cucudq.cn

[Q07] 删除表
来源：http://jzp.fehbvm.com

DROP TABLE IF EXISTS orders;
来源：http://kid.jinghuilouyu.cn

[Q08] 创建普通索引
来源：http://plw.epnwcf.com

CREATE INDEX idx_users_email ON users(email);
来源：http://fza.gogol.net.cn

[Q09] 创建唯一索引
来源：http://zqh.ybcxt.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dbr.sysykeji.top

[Q10] 插入单行
来源：http://mmf.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sut.zhijiandao.cn

[Q11] 一次插入多行
来源：http://hom.fengsongda.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hvv.hfpthk.cn

[Q12] 插入后取自增 ID
来源：http://vyj.tianlin.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://ljv.bbcook.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tbi.wangshuangyany.cn

[Q13] 忽略重复插入
来源：http://rgz.52xcode.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wkv.jlsjyb.cn


<!-- 参考信息 -->