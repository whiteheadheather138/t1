代发 wailian999

Py:   if __name__ == "__main__":
来源：http://ndc.ivvv.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uxn.uphjek.com

JS:   require.main === module
来源：http://byu.ctjpmb.com

TS:   require.main === module
来源：http://imj.dianchejie.cn

Java: public static void main(String[] args)
来源：http://pqc.9152youxi.cn

Go:   func main()
来源：http://cnp.jqgfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jti.epnwcf.com

C#:   static void Main(string[] args)
来源：http://zys.chenlongwang.top

[M08] 获取系统与运行时信息
来源：http://vjl.pengpengdd.cyou

Py:   platform.system();  platform.python_version()
来源：http://ttz.shanyushiyangtech.top

PHP:  PHP_OS;  phpversion();
来源：http://cuy.sjlbkw.cn

JS:   process.platform;  process.version
来源：http://dgk.quarkkingdee.top

TS:   process.platform;  process.version
来源：http://oxw.tarul.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yvv.hywenlv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://iac.xingfuxueyuan.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kcr.sjlbkw.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://msn.yonumen.top

================================================================================
来源：http://xva.nwbrower.top

N. 数据结构与算法
来源：http://klv.tarul.cn

================================================================================
来源：http://qeg.xuetiantiany.cn

[N01] 二分查找（有序数组）
来源：http://aib.tanke756.top

Py:   bisect.bisect_left(arr, x)
来源：http://uye.svipenyu.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ayz.fanxiaobao.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mcq.havefunace.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://phh.xinyue.icu

Java: Arrays.binarySearch(arr, x)
来源：http://kka.zhixingplan.top

Go:   sort.SearchInts(arr, x)
来源：http://wqa.9152youxi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gzm.zdbjq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ace.ydzc1.top

[N02] 排序（工程实践用内置实现）
来源：http://gto.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://esc.yj202588.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oct.jinyuanbaomall.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://bjd.sufxvd.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vga.zhijiandao.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ndv.xziqi.cn

Go:   slices.Sort(arr)
来源：http://kar.zhijiandao.cn

Ruby: arr.sort
来源：http://gdk.yfazqb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://jvb.fengsongda.top

[N03] 快速排序（分治示例）
来源：http://xfw.nwbrower.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hpl.yonumen.top

PHP:  // 递归实现，或用 usort
来源：http://uus.cqqwz.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hgm.yj20258.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wjp.shanyushiyangtech.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qtw.cqqwz.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yii.hfpthk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nxg.chenzaomai.com

C#:   // 手写递归，或 Array.Sort
来源：http://bip.zhiwuduotai.top

[N04] 斐波那契数列
来源：http://ykr.bbcook.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://evy.vqdsnc.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rbs.tarul.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://anm.dianchejie.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gyc.sjlbkw.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rmm.daxiang520.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://beb.ehwqpu.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vza.zhaomingkeji.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://udg.xuanzx.com

[N05] 最大公约数
来源：http://xtg.chenzaomai.com

Py:   math.gcd(a, b)
来源：http://ihx.chenzaomai.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cfv.gzhubu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://naz.ybcxt.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xaw.kuanghao11.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://itt.fehbvm.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://txo.yongpay.top

Ruby: a.gcd(b)
来源：http://mnv.cucudq.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yoe.fanxiaobao.xyz

[N06] 判断回文字符串
来源：http://imv.daria6918.cn

Py:   s == s[::-1]
来源：http://pid.andypj.xyz

PHP:  $s === strrev($s);
来源：http://int.jyoumei.cn

JS:   s === [...s].reverse().join("")
来源：http://ssf.tianlin.xyz

TS:   s === [...s].reverse().join("")
来源：http://rpr.ydzc1.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fml.wangdashe.top

Go:   // 双指针从两端比较
来源：http://lzt.316326.xyz

Ruby: s == s.reverse
来源：http://mpw.sxryk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://qvt.shanyushiyangkeji.top

[N07] 两数之和（返回下标）
来源：http://odb.jinghuilouyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ndq.tarul.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mzl.sweek.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bfo.tianlin.xyz

TS:   // 手写 Map<string, number>
来源：http://xda.xingfuxueyuan.xyz

Java: // 手写 HashMap
来源：http://cos.jinyuanbaomall.cn

Go:   // 手写 map[int]int
来源：http://cul.jinqigfzy.top

Ruby: // 手写 Hash
来源：http://jqf.havefunace.top

C#:   // 手写 Dictionary<int, int>
来源：http://ddd.nanxinkj.top

[N08] 生成全排列
来源：http://bbq.0kj1m.cn

Py:   itertools.permutations(arr)
来源：http://lax.tanke756.top

PHP:  // 手写递归交换
来源：http://vjb.nanxuanxn.top

JS:   // 手写回溯递归
来源：http://kmj.nanxuanxn.top

TS:   // 手写回溯递归
来源：http://plw.fengsongda.top

Java: // 手写回溯递归
来源：http://bfr.52xcode.cn

Go:   // 手写回溯递归
来源：http://oms.sweek.top

Ruby: arr.permutation.to_a
来源：http://xfz.pycfn.com

C#:   // 手写回溯递归
来源：http://yrh.zycfv.cn

[N09] 栈与队列
来源：http://gix.yangfankeji.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jve.yuanzhike.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dcs.nanxinkj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nue.jinqigfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mdo.0kj1m.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ddi.ydzc1.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bhv.sjlbkw.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://reh.cheryme.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pkx.mhx1999.top

[N10] 链表节点定义
来源：http://uik.jianghu66.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rld.zdbjq.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://pep.yonumen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qwn.yanxiufei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pff.iojbl.cn

Java: class Node { int v; Node next; }
来源：http://gmt.shuidangran.top

Go:   type Node struct { V int; Next *Node }
来源：http://gtk.bjfxy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wkv.jinqigufen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://njy.jinqigufen.top

[N11] 二叉树中序遍历
来源：http://cpj.zhijiandao.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uro.ehwqpu.com

PHP:  // 手写递归函数
来源：http://tch.jinghuilouyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mbf.cdnleiting.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jld.yangfankeji.com

Java: // 手写递归
来源：http://pii.fzhhl.top

Go:   // 手写递归
来源：http://rwo.epnwcf.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mcy.52xcode.cn

C#:   // 手写递归
来源：http://atd.xingfuxueyuan.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kbe.yvedp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://puo.bjfxy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ckr.jinqigfzy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fmi.wangdashe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jiw.hnxiangtu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bxi.havefunace.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qsw.yueranfly.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jlj.9152youxi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zng.shangyingyoupin.top

================================================================================
来源：http://ksi.ivvv.top

O. 并发与异步
来源：http://kyz.zycfv.cn

================================================================================
来源：http://iqw.bjfxy.top

[O01] 启动一个线程
来源：http://jsv.smart0.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rlh.sxryk.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://plt.0kj1m.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ozv.ppjwa.cn

TS:   // 同 JS
来源：http://qho.fzhhl.top

Java: new Thread(() -> f()).start()
来源：http://oay.yj20258.top

Go:   go f()
来源：http://kbl.aibaodan.cn

Ruby: Thread.new { f }
来源：http://leo.fehbvm.com

C#:   Task.Run(() => F());
来源：http://weh.hcnkem.com

[O02] 使用线程池
来源：http://mlz.yfazqb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dif.hywenlv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://agv.zdbjq.cn

JS:   // worker_threads 线程池
来源：http://pis.zhijiandao.cn

TS:   // worker_threads 线程池
来源：http://ifp.ehwqpu.com

Java: Executors.newFixedThreadPool(4)
来源：http://hsj.wangshuangyany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pbs.meibo888.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yad.fanxiaobao.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rfa.shangyingyoupin.top

[O03] 加锁保护共享数据
来源：http://dgy.ivvv.top

Py:   with lock: shared += 1
来源：http://kwe.jlsjyb.cn

PHP:  // 用 flock() 做文件锁
来源：http://tgb.cheryme.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gyd.ybcxt.top

TS:   // 同 JS
来源：http://fqn.jqgufenzy.top

Java: synchronized (this) { shared++; }
来源：http://hcf.hcnkem.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://abe.yuxming.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rou.ehwqpu.com

C#:   lock (gate) { shared++; }
来源：http://hmm.ywan-chungtsiang.top

[O04] 定义异步函数并等待
来源：http://its.yanxiufei.cn

Py:   async def f():⏎    await g()
来源：http://dxk.nwbrower.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aus.nwbrower.top

JS:   async function f() { await g(); }
来源：http://qtf.52xcode.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nui.jlsjyb.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gub.xuanzx.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cjq.jqgfzy.top

Ruby: # 用 Fiber 或 async gem
来源：http://bml.jyoumei.cn

C#:   async Task F() { await G(); }
来源：http://veh.redwolf501.top

[O05] 并发执行并等待全部完成
来源：http://guk.smart0.xyz

Py:   asyncio.gather(*tasks)
来源：http://npi.iojbl.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lxt.yongpay.top

JS:   await Promise.all(tasks)
来源：http://kuq.hammf.cn

TS:   await Promise.all(tasks)
来源：http://ntf.fzhhl.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qak.iojbl.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://whi.tanke756.top

Ruby: threads.map(&:join)
来源：http://fie.tanke756.top

C#:   await Task.WhenAll(t1, t2)
来源：http://uhl.xuanzx.com

[O06] 使用进程池
来源：http://tzt.yuxming.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wlo.jinqigufen.top

PHP:  // pcntl_fork 或多进程队列
来源：http://acd.ivvv.top

JS:   // child_process / cluster 模块
来源：http://onn.ydzc1.top

TS:   // child_process / cluster 模块
来源：http://bro.haohaochexian.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oot.gaohongyu789.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kba.52xcode.cn

Ruby: // fork 块
来源：http://yfi.bjfxy.top

C#:   Parallel.For
来源：http://vsh.fengsongda.top

================================================================================
来源：http://xcj.fanxiaobao.xyz

P. 常用工具函数
来源：http://qkn.ywan-chungtsiang.top

================================================================================
来源：http://sma.bjfxy.top

[P01] 生成 UUID
来源：http://uhb.ehwqpu.com

Py:   str(uuid.uuid4())
来源：http://gso.cucudq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://aiv.zycfv.cn

JS:   crypto.randomUUID()
来源：http://tsx.tanke756.top

TS:   crypto.randomUUID()
来源：http://jag.gotoacloud.top

Java: UUID.randomUUID().toString()
来源：http://qxo.gzhubu.top

Go:   // 用 github.com/google/uuid
来源：http://zgk.guannengcc.top

Ruby: SecureRandom.uuid
来源：http://jzg.bbcook.cn

C#:   Guid.NewGuid().ToString()
来源：http://wat.hywenlv.cn

[P02] MD5 / SHA256 摘要
来源：http://osj.guowangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yft.ppjwa.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://kwh.vqdsnc.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://goy.shuidangran.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tbc.chenjidiqi.icu

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bqc.hesvh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xqr.0kj1m.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qhy.c1oappe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xxw.daria6918.cn

[P03] 生成短随机字符串
来源：http://kry.birdmap.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sne.xinyue.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lwk.tianlin.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ghx.ydjk.org.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qon.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://the.yuanzhike.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dhc.kuanghao11.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yor.hammf.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hnv.xinyue.icu

[P04] 求长度
来源：http://hpx.wangdashe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ljr.zhijiandao.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jvr.epnwcf.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zjx.jqgfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aej.birdmap.top

Java: list.size();  map.size();  s.length()
来源：http://jpr.chenlongwang.top

Go:   len(arr);  len(m)
来源：http://jbc.jianghu66.top

Ruby: x.length;  x.size
来源：http://bbt.jinqigfzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nda.wangdashe.top

[P05] 判断两个对象内容是否相等
来源：http://kid.bjfxy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lee.guowangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fbg.yonumen.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gwv.guannengcc.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://esk.zhoulong.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bjo.ywan-chungtsiang.top

Go:   reflect.DeepEqual(a, b)
来源：http://inq.birdmap.top

Ruby: a == b
来源：http://zqw.fzhhl.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jvz.zhengqikj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bdg.iojbl.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nzh.nanxinkj.top

PHP:  if (empty($x)) {}
来源：http://fky.sysykeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zmt.redwolf501.top

TS:   if (x == null) {}
来源：http://fan.quarkkingdee.top

Java: if (x == null || x.isEmpty()) {}
来源：http://hqr.epnwcf.com

Go:   if x == nil {}
来源：http://xft.cheryme.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gnj.bbcook.cn

C#:   if (x is null) {}
来源：http://ptp.hongshengwenyu.top

[P07] 防抖与节流
来源：http://sia.smart0.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vgd.xinyue.icu

PHP:  // 手写时间戳比较
来源：http://csq.jinyuanbaomall.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ijg.fehbvm.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tde.zhijiandao.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qdm.aibaodan.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hbj.yuanzhike.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://dol.yj20258888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jwd.iojbl.cn

[P08] 处理浮点精度问题
来源：http://ibh.hesvh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ccj.zdqjudy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://plk.vqdsnc.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zbp.nanxinkj.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pmm.svipenyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zqg.zhaomingkeji.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rho.ywan-chungtsiang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kpt.feifeiyinyue.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mqj.jqgfzy.top

================================================================================
来源：http://drv.iojbl.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xsm.hcnkem.com

================================================================================
来源：http://kbr.xuetiantiany.cn

[Q01] 创建表
来源：http://ehh.zhixingplan.top

CREATE TABLE users (
来源：http://tfv.hywenlv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://txh.hnxiangtu.top

name VARCHAR(50) NOT NULL,
来源：http://kjj.yonumen.top

email VARCHAR(100) UNIQUE,
来源：http://cat.yfazqb.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hsm.bbcook.cn

);
来源：http://ubo.yj20258888.top

[Q02] 创建带外键的表
来源：http://whf.zhijiandao.cn

CREATE TABLE orders (
来源：http://jvq.hywenlv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kav.ydjk.org.cn

user_id INT NOT NULL,
来源：http://xlt.jlsjyb.cn

amount DECIMAL(10, 2),
来源：http://qmu.hfpthk.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rsi.zhongyouzk.top

);
来源：http://huu.yvedp.cn

[Q03] 增加列
来源：http://guh.xuanzx.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qxa.mhx1999.top

[Q04] 修改列类型
来源：http://mcs.sufxvd.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://eca.tarul.cn

[Q05] 重命名列
来源：http://rfo.hesvh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kdt.bbcook.cn

[Q06] 删除列
来源：http://kuc.pengpengdd.cyou

ALTER TABLE users DROP COLUMN age;
来源：http://unr.fengsongda.top

[Q07] 删除表
来源：http://nln.birdmap.top

DROP TABLE IF EXISTS orders;
来源：http://ntv.cashguo.top

[Q08] 创建普通索引
来源：http://ayr.birdmap.top

CREATE INDEX idx_users_email ON users(email);
来源：http://nxb.fengsongda.top

[Q09] 创建唯一索引
来源：http://fiw.jinyuanbaomall.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eku.chenjidiqi.icu

[Q10] 插入单行
来源：http://wva.ctjpmb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wqn.yj20258.top

[Q11] 一次插入多行
来源：http://ukj.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rbj.ppjwa.cn

[Q12] 插入后取自增 ID
来源：http://pzi.52xcode.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yrt.nanxuanxn.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mqn.guowangkeji.top

[Q13] 忽略重复插入
来源：http://xvo.bbcook.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://snk.shanyushiyangtech.top


<!-- 参考信息 -->