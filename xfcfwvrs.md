代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zvv.gotoacloud.top

Ruby: warn "err"
来源：http://wjl.yj20258888.top

C#:   Console.Error.WriteLine("err")
来源：http://way.zhiwuduotai.top

[M07] 判断是否为主入口
来源：http://sax.hongshengwenyu.top

Py:   if __name__ == "__main__":
来源：http://aqz.yuxming.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hwx.jinqigufen.top

JS:   require.main === module
来源：http://pps.gaohongyu789.top

TS:   require.main === module
来源：http://suu.tian-w.cn

Java: public static void main(String[] args)
来源：http://ycq.yuxming.cn

Go:   func main()
来源：http://pfq.jinqigfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ipf.shzxlz.cn

C#:   static void Main(string[] args)
来源：http://cmf.316326.xyz

[M08] 获取系统与运行时信息
来源：http://vxn.gaohongyu789.top

Py:   platform.system();  platform.python_version()
来源：http://gxo.yj202588.top

PHP:  PHP_OS;  phpversion();
来源：http://afw.jiagoushi.top

JS:   process.platform;  process.version
来源：http://yxm.hammf.cn

TS:   process.platform;  process.version
来源：http://lao.fzhhl.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://trr.kuanghao11.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://crn.tarul.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sma.yuxming.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qye.kuanghao11.cn

================================================================================
来源：http://evl.chenlongwang.top

N. 数据结构与算法
来源：http://etw.zdbjq.cn

================================================================================
来源：http://cok.tarul.cn

[N01] 二分查找（有序数组）
来源：http://qqo.hfpthk.cn

Py:   bisect.bisect_left(arr, x)
来源：http://fbn.xinyue.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zsy.xuanzx.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gcc.cucudq.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jsl.yongpay.top

Java: Arrays.binarySearch(arr, x)
来源：http://vbo.dianchejie.cn

Go:   sort.SearchInts(arr, x)
来源：http://kbs.jinqigfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://oyy.feifeiyinyue.top

C#:   Array.BinarySearch(arr, x)
来源：http://wab.yuxming.cn

[N02] 排序（工程实践用内置实现）
来源：http://hoc.haohaochexian.top

Py:   sorted(arr);  arr.sort()
来源：http://ajc.yfazqb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://adr.quarkkingdee.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xtq.epnwcf.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://dde.svipenyu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ifo.daxiang520.top

Go:   slices.Sort(arr)
来源：http://xec.fktsv.cn

Ruby: arr.sort
来源：http://dph.jinghuilouyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mog.zdqjudy.top

[N03] 快速排序（分治示例）
来源：http://fna.zhengqikj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xhe.shzxlz.cn

PHP:  // 递归实现，或用 usort
来源：http://rbt.xinyue.icu

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fst.c1oappe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fkh.ctjpmb.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rta.tian-w.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dyd.hammf.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hob.cheryme.top

C#:   // 手写递归，或 Array.Sort
来源：http://ktm.snrcjt.cn

[N04] 斐波那契数列
来源：http://tkk.zhoulong.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://des.hysaishi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://inq.316326.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uql.ydzc1.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eze.yfazqb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://huu.yonumen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tss.mhx1999.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hpi.yfazqb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://aup.pycfn.com

[N05] 最大公约数
来源：http://hku.zdbjq.cn

Py:   math.gcd(a, b)
来源：http://kcj.tian-w.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hxn.uphjek.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://goy.havefunace.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://irj.xylfe.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dyu.zhongyouzk.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qiq.hnxiangtu.top

Ruby: a.gcd(b)
来源：http://vrg.hysaishi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://niz.tian-w.cn

[N06] 判断回文字符串
来源：http://och.iojbl.cn

Py:   s == s[::-1]
来源：http://shy.svipenyu.cn

PHP:  $s === strrev($s);
来源：http://agb.jqgfzy.top

JS:   s === [...s].reverse().join("")
来源：http://meb.yuxming.cn

TS:   s === [...s].reverse().join("")
来源：http://pob.cqqwz.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mtk.ppjwa.cn

Go:   // 双指针从两端比较
来源：http://djv.sjlbkw.cn

Ruby: s == s.reverse
来源：http://fqa.jlsjyb.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://iuc.jinqigfzy.top

[N07] 两数之和（返回下标）
来源：http://mww.jinqigfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sjx.daxiang520.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jem.havefunace.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zbb.yuxming.cn

TS:   // 手写 Map<string, number>
来源：http://lxk.dianchejie.cn

Java: // 手写 HashMap
来源：http://ixm.iojbl.cn

Go:   // 手写 map[int]int
来源：http://iiy.sjlbkw.cn

Ruby: // 手写 Hash
来源：http://ndp.uphjek.com

C#:   // 手写 Dictionary<int, int>
来源：http://rlj.zhoulong.xyz

[N08] 生成全排列
来源：http://brc.pengpengdd.cyou

Py:   itertools.permutations(arr)
来源：http://wag.fzhhl.top

PHP:  // 手写递归交换
来源：http://ulj.shuidangran.top

JS:   // 手写回溯递归
来源：http://ail.quarkkingdee.top

TS:   // 手写回溯递归
来源：http://ryr.yonumen.top

Java: // 手写回溯递归
来源：http://kre.wangdashe.top

Go:   // 手写回溯递归
来源：http://but.yanxiufei.cn

Ruby: arr.permutation.to_a
来源：http://ycl.andypj.xyz

C#:   // 手写回溯递归
来源：http://mkk.shangyingyoupin.top

[N09] 栈与队列
来源：http://vhf.ctjpmb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rlr.zhongyouzk.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dkv.zhongyouzk.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://zqg.hammf.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://obz.cashguo.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rpd.vqdsnc.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://edy.shuidangran.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://pdc.jyoumei.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://civ.hongshengwenyu.top

[N10] 链表节点定义
来源：http://ihs.jinqigfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vyz.cheryme.top

PHP:  class Node { public $v; public $next = null; }
来源：http://aze.zhixingplan.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nwt.daxiang520.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://klq.ywan-chungtsiang.top

Java: class Node { int v; Node next; }
来源：http://mjc.ivvv.top

Go:   type Node struct { V int; Next *Node }
来源：http://gcn.zhixingplan.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hwa.hysaishi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ots.bjfxy.top

[N11] 二叉树中序遍历
来源：http://xfm.hesvh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cej.tianlin.xyz

PHP:  // 手写递归函数
来源：http://lvs.yangfankeji.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bty.haohaochexian.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tql.tanke756.top

Java: // 手写递归
来源：http://rff.52xcode.cn

Go:   // 手写递归
来源：http://wpx.hysaishi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ubk.tian-w.cn

C#:   // 手写递归
来源：http://nly.shanyushiyangtech.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://glm.dianchejie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xkn.hysaishi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zlq.nwbrower.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kfz.hnqzz.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jpe.aizwys.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://aep.yongpay.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gtv.pycfn.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rnd.hongshengwenyu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oxt.yuanzhike.top

================================================================================
来源：http://kdz.yangfankeji.com

O. 并发与异步
来源：http://kch.gzhubu.top

================================================================================
来源：http://bcm.xingfuxueyuan.xyz

[O01] 启动一个线程
来源：http://xih.nanxuanxn.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xqf.zhongyouzk.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fhu.uphjek.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yxo.xinyue.icu

TS:   // 同 JS
来源：http://xur.mhx1999.top

Java: new Thread(() -> f()).start()
来源：http://aho.kuanghao11.cn

Go:   go f()
来源：http://tdf.jinghuilouyu.cn

Ruby: Thread.new { f }
来源：http://vji.yj20258.top

C#:   Task.Run(() => F());
来源：http://zqt.gogol.net.cn

[O02] 使用线程池
来源：http://zbk.zdbjq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uxr.hywenlv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dpr.hesvh.cn

JS:   // worker_threads 线程池
来源：http://vba.jinghuilouyu.cn

TS:   // worker_threads 线程池
来源：http://njj.birdmap.top

Java: Executors.newFixedThreadPool(4)
来源：http://eee.hysaishi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bay.iojbl.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hsd.gotoacloud.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bsm.chenzaomai.com

[O03] 加锁保护共享数据
来源：http://ppr.zhijiandao.cn

Py:   with lock: shared += 1
来源：http://pld.yangfankeji.com

PHP:  // 用 flock() 做文件锁
来源：http://jri.fehbvm.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pvn.quarkkingdee.top

TS:   // 同 JS
来源：http://qzi.quarkkingdee.top

Java: synchronized (this) { shared++; }
来源：http://ypj.yvedp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://des.hysaishi.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ksn.jqgufenzy.top

C#:   lock (gate) { shared++; }
来源：http://jwv.dianchejie.cn

[O04] 定义异步函数并等待
来源：http://exg.zhaomingkeji.xyz

Py:   async def f():⏎    await g()
来源：http://iar.jinqigufen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ggw.sufxvd.cn

JS:   async function f() { await g(); }
来源：http://dsp.smart0.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://kvg.birdmap.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ztp.ehwqpu.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qig.uphjek.com

Ruby: # 用 Fiber 或 async gem
来源：http://rcf.hywenlv.cn

C#:   async Task F() { await G(); }
来源：http://nmh.pycfn.com

[O05] 并发执行并等待全部完成
来源：http://lad.xinyue.icu

Py:   asyncio.gather(*tasks)
来源：http://lra.tian-w.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ckf.xziqi.cn

JS:   await Promise.all(tasks)
来源：http://ooz.xingfuxueyuan.xyz

TS:   await Promise.all(tasks)
来源：http://ipw.cdnleiting.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://euu.gaohongyu789.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xbp.fanxiaobao.xyz

Ruby: threads.map(&:join)
来源：http://zch.zhaomingkeji.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://bwf.tanke756.top

[O06] 使用进程池
来源：http://jaj.bbcook.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vst.chenzaomai.com

PHP:  // pcntl_fork 或多进程队列
来源：http://omu.zhixingplan.top

JS:   // child_process / cluster 模块
来源：http://iue.shuidangran.top

TS:   // child_process / cluster 模块
来源：http://rtt.hnqzz.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xts.fehbvm.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oka.bbcook.cn

Ruby: // fork 块
来源：http://ypc.jyoumei.cn

C#:   Parallel.For
来源：http://eug.shangyingyoupin.top

================================================================================
来源：http://hww.jinyuanbaomall.cn

P. 常用工具函数
来源：http://qvv.uphjek.com

================================================================================
来源：http://uhi.daria6918.cn

[P01] 生成 UUID
来源：http://wqy.cqqwz.cn

Py:   str(uuid.uuid4())
来源：http://cbf.ydzc1.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://trd.hysaishi.cn

JS:   crypto.randomUUID()
来源：http://yqv.yueranfly.top

TS:   crypto.randomUUID()
来源：http://uoc.guowangkeji.top

Java: UUID.randomUUID().toString()
来源：http://hug.zhijiandao.cn

Go:   // 用 github.com/google/uuid
来源：http://fwq.ywan-chungtsiang.top

Ruby: SecureRandom.uuid
来源：http://bdu.jinqigfzy.top

C#:   Guid.NewGuid().ToString()
来源：http://cpt.gogol.net.cn

[P02] MD5 / SHA256 摘要
来源：http://aix.birdmap.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ogn.sxryk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://krj.zhoulong.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mpu.uphjek.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://scw.shanyushiyangtech.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://msr.yangfankeji.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wdu.hywenlv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://whv.sysykeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://btm.hongshengwenyu.top

[P03] 生成短随机字符串
来源：http://xxx.jlsjyb.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jfp.fengsongda.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://igp.wangshuangyany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ijz.meibo888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mtx.hfpthk.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://htd.cheryme.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://twf.zhongyouzk.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://sgy.wangshuangyany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iwc.vehdjk.com

[P04] 求长度
来源：http://bch.yonumen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ygr.tarul.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dpp.guannengcc.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rpf.zhaomingkeji.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yzr.sufxvd.cn

Java: list.size();  map.size();  s.length()
来源：http://zgn.zdqjudy.top

Go:   len(arr);  len(m)
来源：http://eov.cashguo.top

Ruby: x.length;  x.size
来源：http://sef.haohaochexian.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://enp.yonumen.top

[P05] 判断两个对象内容是否相等
来源：http://ggp.yangfankeji.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://rpw.jyoumei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xrx.chenlongwang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gqf.zdbjq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xan.jinyuanbaomall.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://elz.ywan-chungtsiang.top

Go:   reflect.DeepEqual(a, b)
来源：http://gnm.ydzc1.top

Ruby: a == b
来源：http://cxw.xziqi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rzb.sxryk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rku.fengsongda.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hpu.daxiang520.top

PHP:  if (empty($x)) {}
来源：http://cmf.ydjk.org.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uob.jianghu66.top

TS:   if (x == null) {}
来源：http://fyh.ivvv.top

Java: if (x == null || x.isEmpty()) {}
来源：http://cdw.sysykeji.top

Go:   if x == nil {}
来源：http://iaj.vqdsnc.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://djo.zhongyouzk.top

C#:   if (x is null) {}
来源：http://asl.smart0.xyz

[P07] 防抖与节流
来源：http://loj.ehwqpu.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bmf.jqgfzy.top

PHP:  // 手写时间戳比较
来源：http://ebr.cheryme.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uqa.yj20258.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://spi.zdbjq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oed.redwolf501.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ydd.shangyingyoupin.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rlf.hongshengwenyu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tog.yvedp.cn

[P08] 处理浮点精度问题
来源：http://qhx.cqqwz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kpp.vqdsnc.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://npj.cucudq.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vtd.sysykeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xlo.hnqzz.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nyr.bjfxy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sdb.wangdashe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qxv.xuetiantiany.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eij.bbcook.cn

================================================================================
来源：http://jkg.snrcjt.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mdd.yfazqb.com

================================================================================
来源：http://prv.jlsjyb.cn

[Q01] 创建表
来源：http://fws.yj202588.top

CREATE TABLE users (
来源：http://xap.iojbl.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gvg.daria6918.cn

name VARCHAR(50) NOT NULL,
来源：http://tvz.gotoacloud.top

email VARCHAR(100) UNIQUE,
来源：http://vkf.uphjek.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lhr.xylfe.cn

);
来源：http://qtm.nanxinkj.top

[Q02] 创建带外键的表
来源：http://nxj.aizwys.cn

CREATE TABLE orders (
来源：http://zdz.andypj.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xfb.ybcxt.top

user_id INT NOT NULL,
来源：http://sfq.jinqigfzy.top

amount DECIMAL(10, 2),
来源：http://jow.havefunace.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://drv.xinyue.icu

);
来源：http://ffd.jyoumei.cn

[Q03] 增加列
来源：http://spr.yuanzhike.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://usk.redwolf501.top

[Q04] 修改列类型
来源：http://gxv.hnqzz.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rle.svipenyu.cn

[Q05] 重命名列
来源：http://tzj.ctjpmb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fof.jlsjyb.cn

[Q06] 删除列
来源：http://lwh.chenzaomai.com

ALTER TABLE users DROP COLUMN age;
来源：http://fpp.birdmap.top

[Q07] 删除表
来源：http://jen.cheryme.top

DROP TABLE IF EXISTS orders;
来源：http://qdf.yuxming.cn

[Q08] 创建普通索引
来源：http://hbb.feifeiyinyue.top

CREATE INDEX idx_users_email ON users(email);
来源：http://fqt.jinqigufen.top

[Q09] 创建唯一索引
来源：http://vre.nanxuanxn.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mfn.shuidangran.top

[Q10] 插入单行
来源：http://tfo.c1oappe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kyb.jqgfzy.top

[Q11] 一次插入多行
来源：http://lue.snrcjt.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ybf.ppjwa.cn

[Q12] 插入后取自增 ID
来源：http://tac.shanyushiyangtech.top


<!-- 参考信息 -->