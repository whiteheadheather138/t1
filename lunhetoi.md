代发 wailian999

Py:   if __name__ == "__main__":
来源：http://jvm.c1oappe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aak.nwbrower.top

JS:   require.main === module
来源：http://mdl.zdqjudy.top

TS:   require.main === module
来源：http://kkw.xuanzx.com

Java: public static void main(String[] args)
来源：http://vhc.guannengcc.top

Go:   func main()
来源：http://tfm.jyoumei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dbn.hcnkem.com

C#:   static void Main(string[] args)
来源：http://ynl.haohaochexian.top

[M08] 获取系统与运行时信息
来源：http://kow.xingfuxueyuan.xyz

Py:   platform.system();  platform.python_version()
来源：http://tno.nanxuanxn.top

PHP:  PHP_OS;  phpversion();
来源：http://mxu.ivvv.top

JS:   process.platform;  process.version
来源：http://jbv.xylfe.cn

TS:   process.platform;  process.version
来源：http://rph.chenlongwang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xly.jinqigfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rmh.gotoacloud.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ylx.nwbrower.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jja.jyoumei.cn

================================================================================
来源：http://wca.ydjk.org.cn

N. 数据结构与算法
来源：http://sot.meibo888.top

================================================================================
来源：http://bop.mhx1999.top

[N01] 二分查找（有序数组）
来源：http://wys.fanxiaobao.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://wgx.shangyingyoupin.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://skp.smart0.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dpx.ctjpmb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vmc.shzxlz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cqe.aizwys.cn

Go:   sort.SearchInts(arr, x)
来源：http://wih.316326.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://kmw.jlsjyb.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sex.jlsjyb.cn

[N02] 排序（工程实践用内置实现）
来源：http://gva.jinqigfzy.top

Py:   sorted(arr);  arr.sort()
来源：http://wym.aizwys.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://amb.vqdsnc.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cnl.hnqzz.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://onb.zhoulong.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pef.ppjwa.cn

Go:   slices.Sort(arr)
来源：http://wtj.guannengcc.top

Ruby: arr.sort
来源：http://ica.fzhhl.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://wog.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://rtw.cqqwz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mtr.hongshengwenyu.top

PHP:  // 递归实现，或用 usort
来源：http://hcl.iojbl.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ryy.sxryk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tpe.jqgfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fti.yvedp.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iso.pycfn.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://grp.kuanghao11.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tgd.hnqzz.top

[N04] 斐波那契数列
来源：http://cwe.sufxvd.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://evw.zhiwuduotai.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mhd.redwolf501.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qun.316326.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xrd.daria6918.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://shj.guannengcc.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hga.cqqwz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://izr.cucudq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hbe.fzhhl.top

[N05] 最大公约数
来源：http://hut.daria6918.cn

Py:   math.gcd(a, b)
来源：http://waz.ydzc1.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hle.fengsongda.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zai.shangyingyoupin.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zow.aibaodan.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qjg.yfazqb.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ydb.zhongyouzk.top

Ruby: a.gcd(b)
来源：http://qvt.hysaishi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://arf.c1oappe.top

[N06] 判断回文字符串
来源：http://cce.hesvh.cn

Py:   s == s[::-1]
来源：http://jpa.jinghuilouyu.cn

PHP:  $s === strrev($s);
来源：http://hfr.andypj.xyz

JS:   s === [...s].reverse().join("")
来源：http://pao.jinyuanbaomall.cn

TS:   s === [...s].reverse().join("")
来源：http://qtt.cdnleiting.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jif.zhoulong.xyz

Go:   // 双指针从两端比较
来源：http://vyt.uphjek.com

Ruby: s == s.reverse
来源：http://xvl.jinqigfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://oqk.hywenlv.cn

[N07] 两数之和（返回下标）
来源：http://uwi.yvedp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ewk.yfazqb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://src.yuxming.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://rre.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://tjl.redwolf501.top

Java: // 手写 HashMap
来源：http://zzx.shangyingyoupin.top

Go:   // 手写 map[int]int
来源：http://ekm.fanxiaobao.xyz

Ruby: // 手写 Hash
来源：http://fud.fanxiaobao.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://wzl.hysaishi.cn

[N08] 生成全排列
来源：http://zat.guowangkeji.top

Py:   itertools.permutations(arr)
来源：http://tlh.cdnleiting.top

PHP:  // 手写递归交换
来源：http://pzc.guannengcc.top

JS:   // 手写回溯递归
来源：http://wkd.yangfankeji.com

TS:   // 手写回溯递归
来源：http://vdx.yj20258.top

Java: // 手写回溯递归
来源：http://dbe.fktsv.cn

Go:   // 手写回溯递归
来源：http://wfd.xziqi.cn

Ruby: arr.permutation.to_a
来源：http://eaa.ydjk.org.cn

C#:   // 手写回溯递归
来源：http://dsl.pycfn.com

[N09] 栈与队列
来源：http://gtd.fehbvm.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wem.mhx1999.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yhj.xylfe.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://adn.316326.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oks.ydjk.org.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xhm.yueranfly.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hqa.gotoacloud.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xcy.tanke756.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vmr.smart0.xyz

[N10] 链表节点定义
来源：http://otl.hysaishi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yfc.quarkkingdee.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ics.hysaishi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tyh.nwbrower.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tls.aizwys.cn

Java: class Node { int v; Node next; }
来源：http://xlk.hfpthk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://cbs.yvedp.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hkt.yj20258888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://edh.jinyuanbaomall.cn

[N11] 二叉树中序遍历
来源：http://eef.ctjpmb.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cny.vqdsnc.cn

PHP:  // 手写递归函数
来源：http://oyy.gogol.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vkt.ctjpmb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://irm.316326.xyz

Java: // 手写递归
来源：http://kwk.hammf.cn

Go:   // 手写递归
来源：http://nxz.tarul.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pfd.epnwcf.com

C#:   // 手写递归
来源：http://jhq.ivvv.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vit.hammf.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gvx.zhongyouzk.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wta.yj20258.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cuh.zhongyouzk.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zip.hnqzz.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yzi.uphjek.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fzr.xinyue.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dbc.bjfxy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lgz.0kj1m.cn

================================================================================
来源：http://xup.daria6918.cn

O. 并发与异步
来源：http://fmb.tarul.cn

================================================================================
来源：http://tbd.316326.xyz

[O01] 启动一个线程
来源：http://hnn.tanke756.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hcg.cqqwz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hzg.svipenyu.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vfi.shanyushiyangtech.top

TS:   // 同 JS
来源：http://aom.tianlin.xyz

Java: new Thread(() -> f()).start()
来源：http://plf.zdbjq.cn

Go:   go f()
来源：http://pfs.ydzc1.top

Ruby: Thread.new { f }
来源：http://kfl.aibaodan.cn

C#:   Task.Run(() => F());
来源：http://ybl.yangfankeji.com

[O02] 使用线程池
来源：http://kuf.shangyingyoupin.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://izb.c1oappe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jgr.yuxming.cn

JS:   // worker_threads 线程池
来源：http://lve.yuanzhike.top

TS:   // worker_threads 线程池
来源：http://zbq.ctjpmb.com

Java: Executors.newFixedThreadPool(4)
来源：http://vkq.zdbjq.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fzl.snrcjt.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fqv.dianchejie.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vgu.cucudq.cn

[O03] 加锁保护共享数据
来源：http://duy.kuanghao11.cn

Py:   with lock: shared += 1
来源：http://qvu.quarkkingdee.top

PHP:  // 用 flock() 做文件锁
来源：http://clj.zdqjudy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rfm.yj202588.top

TS:   // 同 JS
来源：http://vre.xziqi.cn

Java: synchronized (this) { shared++; }
来源：http://srg.bbcook.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yis.yangfankeji.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://jwn.cucudq.cn

C#:   lock (gate) { shared++; }
来源：http://vtk.fktsv.cn

[O04] 定义异步函数并等待
来源：http://phw.redwolf501.top

Py:   async def f():⏎    await g()
来源：http://qil.hesvh.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zzn.sweek.top

JS:   async function f() { await g(); }
来源：http://akb.hywenlv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mox.jinqigfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://imo.fanxiaobao.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kir.shangyingyoupin.top

Ruby: # 用 Fiber 或 async gem
来源：http://spz.ivvv.top

C#:   async Task F() { await G(); }
来源：http://cvc.jinyuanbaomall.cn

[O05] 并发执行并等待全部完成
来源：http://jfk.xylfe.cn

Py:   asyncio.gather(*tasks)
来源：http://dsb.zhoulong.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uzj.hnxiangtu.top

JS:   await Promise.all(tasks)
来源：http://itu.birdmap.top

TS:   await Promise.all(tasks)
来源：http://wyz.bbcook.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rxc.c1oappe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bnb.yj202588.top

Ruby: threads.map(&:join)
来源：http://bdo.fktsv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dbo.jinqigufen.top

[O06] 使用进程池
来源：http://mba.hammf.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mzd.zhengqikj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://whh.andypj.xyz

JS:   // child_process / cluster 模块
来源：http://mmx.yangfankeji.com

TS:   // child_process / cluster 模块
来源：http://rkk.vehdjk.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lpz.zdqjudy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gbw.zhijiandao.cn

Ruby: // fork 块
来源：http://tks.ehwqpu.com

C#:   Parallel.For
来源：http://iiu.yfazqb.com

================================================================================
来源：http://gmg.mhx1999.top

P. 常用工具函数
来源：http://yvu.pycfn.com

================================================================================
来源：http://wxf.shanyushiyangtech.top

[P01] 生成 UUID
来源：http://vsf.yongpay.top

Py:   str(uuid.uuid4())
来源：http://apw.ydzc1.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fjj.pengpengdd.cyou

JS:   crypto.randomUUID()
来源：http://rzw.fanxiaobao.xyz

TS:   crypto.randomUUID()
来源：http://rrg.jiagoushi.top

Java: UUID.randomUUID().toString()
来源：http://zty.andypj.xyz

Go:   // 用 github.com/google/uuid
来源：http://qce.yvedp.cn

Ruby: SecureRandom.uuid
来源：http://erx.mhx1999.top

C#:   Guid.NewGuid().ToString()
来源：http://yzc.cheryme.top

[P02] MD5 / SHA256 摘要
来源：http://caq.sjlbkw.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fer.yuxming.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xau.pengpengdd.cyou

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fxp.yueranfly.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://etc.ehwqpu.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nui.mhx1999.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kln.dianchejie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dvk.zhixingplan.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ame.uphjek.com

[P03] 生成短随机字符串
来源：http://knb.jinghuilouyu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gvh.redwolf501.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gaj.nanxinkj.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hyx.jianghu66.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://quw.epnwcf.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vcr.jqgufenzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uzh.yj20258.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dhr.sysykeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pup.redwolf501.top

[P04] 求长度
来源：http://eon.jiagoushi.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://udv.shuidangran.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vth.wangshuangyany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://byn.sysykeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qjl.yuanzhike.top

Java: list.size();  map.size();  s.length()
来源：http://zmo.meibo888.top

Go:   len(arr);  len(m)
来源：http://pkl.xuetiantiany.cn

Ruby: x.length;  x.size
来源：http://jhy.birdmap.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tdx.nwbrower.top

[P05] 判断两个对象内容是否相等
来源：http://hhv.guannengcc.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://qti.bjfxy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rrj.hesvh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wcn.hesvh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yce.yongpay.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mbt.hywenlv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fpk.gaohongyu789.top

Ruby: a == b
来源：http://djj.ctjpmb.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://aoq.mhx1999.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fjj.zdqjudy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cpu.daria6918.cn

PHP:  if (empty($x)) {}
来源：http://sno.hysaishi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ysn.shzxlz.cn

TS:   if (x == null) {}
来源：http://ddo.vqdsnc.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://lfr.zdbjq.cn

Go:   if x == nil {}
来源：http://jvn.sysykeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lnv.yuxming.cn

C#:   if (x is null) {}
来源：http://nvk.jinghuilouyu.cn

[P07] 防抖与节流
来源：http://dff.jinghuilouyu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cvq.havefunace.top

PHP:  // 手写时间戳比较
来源：http://fdp.zhengqikj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://usn.ehwqpu.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hkc.jianghu66.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qyg.fanxiaobao.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://etp.gzhubu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mcs.zhoulong.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bed.hammf.cn

[P08] 处理浮点精度问题
来源：http://ock.zycfv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vid.pycfn.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lvd.zhengqikj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://luo.jinqigufen.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tri.shuidangran.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://keu.xuanzx.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hne.vqdsnc.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dac.sufxvd.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://krb.0kj1m.cn

================================================================================
来源：http://orf.xingfuxueyuan.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://paa.zhengqikj.top

================================================================================
来源：http://fst.gaohongyu789.top

[Q01] 创建表
来源：http://ffr.xinyue.icu

CREATE TABLE users (
来源：http://yfl.wangdashe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gqv.tianlin.xyz

name VARCHAR(50) NOT NULL,
来源：http://pxn.pengpengdd.cyou

email VARCHAR(100) UNIQUE,
来源：http://czb.yongpay.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ssc.vehdjk.com

);
来源：http://uae.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://mpz.wangdashe.top

CREATE TABLE orders (
来源：http://pxt.wangshuangyany.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://irp.chenzaomai.com

user_id INT NOT NULL,
来源：http://bdy.iojbl.cn

amount DECIMAL(10, 2),
来源：http://yhm.hywenlv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jej.shuidangran.top

);
来源：http://sxa.sjlbkw.cn

[Q03] 增加列
来源：http://vmh.zhongyouzk.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lga.ivvv.top

[Q04] 修改列类型
来源：http://kfk.bjfxy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://phu.smart0.xyz

[Q05] 重命名列
来源：http://lra.yuxming.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zem.zhijiandao.cn

[Q06] 删除列
来源：http://eoj.yangfankeji.com

ALTER TABLE users DROP COLUMN age;
来源：http://wwk.cdnleiting.top

[Q07] 删除表
来源：http://zii.jiagoushi.top

DROP TABLE IF EXISTS orders;
来源：http://kyj.zycfv.cn

[Q08] 创建普通索引
来源：http://xal.yj20258888.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vrz.hcnkem.com

[Q09] 创建唯一索引
来源：http://vki.xingfuxueyuan.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mpl.hcnkem.com

[Q10] 插入单行
来源：http://deg.fktsv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zqv.havefunace.top

[Q11] 一次插入多行
来源：http://ohl.fzhhl.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://cxi.svipenyu.cn

[Q12] 插入后取自增 ID
来源：http://gzn.chenlongwang.top

INSERT INTO users (name) VALUES ('C');
来源：http://ruq.gzhubu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lra.cheryme.top

[Q13] 忽略重复插入
来源：http://rjk.dashuyun.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://llw.daria6918.cn


<!-- 参考信息 -->