代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lzz.birdmap.top

Ruby: warn "err"
来源：http://zzk.epnwcf.com

C#:   Console.Error.WriteLine("err")
来源：http://wjs.zhiwuduotai.top

[M07] 判断是否为主入口
来源：http://taw.jianghu66.top

Py:   if __name__ == "__main__":
来源：http://xbg.jinqigfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yoc.tianlin.xyz

JS:   require.main === module
来源：http://ulg.ctjpmb.com

TS:   require.main === module
来源：http://epz.wangdashe.top

Java: public static void main(String[] args)
来源：http://bkr.nanxinkj.top

Go:   func main()
来源：http://dgc.hongshengwenyu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oyw.ywan-chungtsiang.top

C#:   static void Main(string[] args)
来源：http://riy.dianchejie.cn

[M08] 获取系统与运行时信息
来源：http://bmb.fzhhl.top

Py:   platform.system();  platform.python_version()
来源：http://ypv.fzhhl.top

PHP:  PHP_OS;  phpversion();
来源：http://qrp.fzhhl.top

JS:   process.platform;  process.version
来源：http://xjh.yj202588.top

TS:   process.platform;  process.version
来源：http://xnb.hongshengwenyu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pql.hysaishi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xqu.316326.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://phx.fanxiaobao.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://jkh.xingfuxueyuan.xyz

================================================================================
来源：http://kde.ehwqpu.com

N. 数据结构与算法
来源：http://pfd.meibo888.top

================================================================================
来源：http://gvn.zhengqikj.top

[N01] 二分查找（有序数组）
来源：http://hib.zhijiandao.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ued.bbcook.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vkw.dashuyun.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://opr.ywan-chungtsiang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cfm.guannengcc.top

Java: Arrays.binarySearch(arr, x)
来源：http://goy.bbcook.cn

Go:   sort.SearchInts(arr, x)
来源：http://und.ywan-chungtsiang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ler.sweek.top

C#:   Array.BinarySearch(arr, x)
来源：http://njl.uphjek.com

[N02] 排序（工程实践用内置实现）
来源：http://gtm.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://upu.sysykeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://fvh.chenlongwang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nnu.jyoumei.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mbj.aizwys.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://knc.ivvv.top

Go:   slices.Sort(arr)
来源：http://zyb.zycfv.cn

Ruby: arr.sort
来源：http://sni.gaohongyu789.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rlk.shzxlz.cn

[N03] 快速排序（分治示例）
来源：http://zps.havefunace.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kpb.fktsv.cn

PHP:  // 递归实现，或用 usort
来源：http://kak.nanxuanxn.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mlb.zhongyouzk.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dij.aizwys.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ghe.nanxuanxn.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kum.zhixingplan.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fmt.xuetiantiany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cdc.birdmap.top

[N04] 斐波那契数列
来源：http://spa.gogol.net.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lgs.fanxiaobao.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://abm.ppjwa.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xjb.cucudq.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rld.yongpay.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rys.vehdjk.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mhd.quarkkingdee.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ump.zhiwuduotai.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oyg.birdmap.top

[N05] 最大公约数
来源：http://wih.aizwys.cn

Py:   math.gcd(a, b)
来源：http://yht.zhoulong.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hha.shanyushiyangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nyf.hywenlv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uic.shanyushiyangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uyx.epnwcf.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yyz.gzhubu.top

Ruby: a.gcd(b)
来源：http://nnb.bbcook.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yzf.yueranfly.top

[N06] 判断回文字符串
来源：http://rrp.gaohongyu789.top

Py:   s == s[::-1]
来源：http://nkt.tanke756.top

PHP:  $s === strrev($s);
来源：http://sgc.jinqigufen.top

JS:   s === [...s].reverse().join("")
来源：http://uzk.0kj1m.cn

TS:   s === [...s].reverse().join("")
来源：http://yuy.smart0.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://whj.gogol.net.cn

Go:   // 双指针从两端比较
来源：http://hxq.guannengcc.top

Ruby: s == s.reverse
来源：http://hvc.sxryk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xqr.svipenyu.cn

[N07] 两数之和（返回下标）
来源：http://iqw.shanyushiyangkeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ssj.bbcook.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ros.guowangkeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qsq.cqqwz.cn

TS:   // 手写 Map<string, number>
来源：http://bjn.hfpthk.cn

Java: // 手写 HashMap
来源：http://oji.havefunace.top

Go:   // 手写 map[int]int
来源：http://bza.yanxiufei.cn

Ruby: // 手写 Hash
来源：http://zct.sufxvd.cn

C#:   // 手写 Dictionary<int, int>
来源：http://itr.yueranfly.top

[N08] 生成全排列
来源：http://cic.yj20258888.top

Py:   itertools.permutations(arr)
来源：http://uvs.yfazqb.com

PHP:  // 手写递归交换
来源：http://ibc.vehdjk.com

JS:   // 手写回溯递归
来源：http://nxe.ctjpmb.com

TS:   // 手写回溯递归
来源：http://dvg.zhengqikj.top

Java: // 手写回溯递归
来源：http://tzt.wangshuangyany.cn

Go:   // 手写回溯递归
来源：http://cxw.jinghuilouyu.cn

Ruby: arr.permutation.to_a
来源：http://yjc.yongpay.top

C#:   // 手写回溯递归
来源：http://eke.tianlin.xyz

[N09] 栈与队列
来源：http://lgs.aibaodan.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rbx.uphjek.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qig.jqgfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eqr.gogol.net.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://drj.tanke756.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yms.zhongyouzk.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nge.fanxiaobao.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lml.uphjek.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://etu.gogol.net.cn

[N10] 链表节点定义
来源：http://svx.jqgfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://joy.daxiang520.top

PHP:  class Node { public $v; public $next = null; }
来源：http://yrv.ppjwa.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qdp.zdqjudy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dsv.yj202588.top

Java: class Node { int v; Node next; }
来源：http://ous.havefunace.top

Go:   type Node struct { V int; Next *Node }
来源：http://gsq.jqgufenzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ucl.316326.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://cgq.jinqigufen.top

[N11] 二叉树中序遍历
来源：http://enw.ybcxt.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://axc.aibaodan.cn

PHP:  // 手写递归函数
来源：http://upr.dashuyun.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qpf.guowangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://omx.yanxiufei.cn

Java: // 手写递归
来源：http://vlw.chenlongwang.top

Go:   // 手写递归
来源：http://ecf.zdqjudy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ywb.ywan-chungtsiang.top

C#:   // 手写递归
来源：http://khr.haohaochexian.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uyh.ydzc1.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dfq.yj20258.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gdg.xuanzx.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xtw.c1oappe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uxq.zycfv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zea.yuxming.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://eji.yuanzhike.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vpn.shangyingyoupin.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kll.gotoacloud.top

================================================================================
来源：http://wnk.wangshuangyany.cn

O. 并发与异步
来源：http://wjm.zhongyouzk.top

================================================================================
来源：http://grx.sjlbkw.cn

[O01] 启动一个线程
来源：http://kmq.yj20258.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dbd.shzxlz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://oqu.epnwcf.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://glx.shanyushiyangkeji.top

TS:   // 同 JS
来源：http://ruj.smart0.xyz

Java: new Thread(() -> f()).start()
来源：http://mdp.meibo888.top

Go:   go f()
来源：http://zbl.gogol.net.cn

Ruby: Thread.new { f }
来源：http://mmg.sxryk.cn

C#:   Task.Run(() => F());
来源：http://erc.haohaochexian.top

[O02] 使用线程池
来源：http://bay.cdnleiting.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pey.jqgufenzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ips.tian-w.cn

JS:   // worker_threads 线程池
来源：http://ubg.guannengcc.top

TS:   // worker_threads 线程池
来源：http://qjj.bbcook.cn

Java: Executors.newFixedThreadPool(4)
来源：http://euo.daxiang520.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hmn.yuxming.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cgn.zhoulong.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wgw.316326.xyz

[O03] 加锁保护共享数据
来源：http://pkj.svipenyu.cn

Py:   with lock: shared += 1
来源：http://jqi.hysaishi.cn

PHP:  // 用 flock() 做文件锁
来源：http://ude.sjlbkw.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://leq.yvedp.cn

TS:   // 同 JS
来源：http://fak.52xcode.cn

Java: synchronized (this) { shared++; }
来源：http://lru.ctjpmb.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xnd.fehbvm.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://lkd.gogol.net.cn

C#:   lock (gate) { shared++; }
来源：http://jgw.52xcode.cn

[O04] 定义异步函数并等待
来源：http://xwj.wangdashe.top

Py:   async def f():⏎    await g()
来源：http://stx.yuanzhike.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ttp.jinqigufen.top

JS:   async function f() { await g(); }
来源：http://ond.fktsv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ymb.yuxming.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bcr.birdmap.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nvb.gaohongyu789.top

Ruby: # 用 Fiber 或 async gem
来源：http://urh.shuidangran.top

C#:   async Task F() { await G(); }
来源：http://ceq.ppjwa.cn

[O05] 并发执行并等待全部完成
来源：http://vic.0kj1m.cn

Py:   asyncio.gather(*tasks)
来源：http://wqt.guannengcc.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ptg.xuetiantiany.cn

JS:   await Promise.all(tasks)
来源：http://zzm.xziqi.cn

TS:   await Promise.all(tasks)
来源：http://tsf.jyoumei.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://urv.fktsv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ewd.yj20258888.top

Ruby: threads.map(&:join)
来源：http://cvk.smart0.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://gkj.yj202588.top

[O06] 使用进程池
来源：http://llp.nanxuanxn.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xmy.bjfxy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ixh.shangyingyoupin.top

JS:   // child_process / cluster 模块
来源：http://rqb.andypj.xyz

TS:   // child_process / cluster 模块
来源：http://ibi.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nug.hammf.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jer.daria6918.cn

Ruby: // fork 块
来源：http://zhp.hywenlv.cn

C#:   Parallel.For
来源：http://rlk.kuanghao11.cn

================================================================================
来源：http://jcm.yonumen.top

P. 常用工具函数
来源：http://uvh.birdmap.top

================================================================================
来源：http://yzj.yj20258.top

[P01] 生成 UUID
来源：http://wxi.ehwqpu.com

Py:   str(uuid.uuid4())
来源：http://jmu.zdbjq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ger.yueranfly.top

JS:   crypto.randomUUID()
来源：http://hec.shangyingyoupin.top

TS:   crypto.randomUUID()
来源：http://bdi.cdnleiting.top

Java: UUID.randomUUID().toString()
来源：http://iaw.hesvh.cn

Go:   // 用 github.com/google/uuid
来源：http://nsj.vehdjk.com

Ruby: SecureRandom.uuid
来源：http://xlk.meibo888.top

C#:   Guid.NewGuid().ToString()
来源：http://mnp.gogol.net.cn

[P02] MD5 / SHA256 摘要
来源：http://sca.yongpay.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jbk.shuidangran.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xtg.daxiang520.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pju.aibaodan.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://axr.guowangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fvz.nwbrower.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ehc.jiagoushi.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lro.zhongyouzk.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ujm.zhongyouzk.top

[P03] 生成短随机字符串
来源：http://xbp.chenlongwang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zaj.tanke756.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aoj.dashuyun.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qjo.pengpengdd.cyou

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://evw.smart0.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pcf.kuanghao11.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mox.0kj1m.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pfy.c1oappe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://oji.bjfxy.top

[P04] 求长度
来源：http://gmn.gogol.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://prn.chenjidiqi.icu

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dir.kuanghao11.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jqw.c1oappe.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ezf.jinqigufen.top

Java: list.size();  map.size();  s.length()
来源：http://pqh.chenlongwang.top

Go:   len(arr);  len(m)
来源：http://gxz.chenzaomai.com

Ruby: x.length;  x.size
来源：http://hli.cheryme.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qoo.9152youxi.cn

[P05] 判断两个对象内容是否相等
来源：http://gjk.xuanzx.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://taa.jinqigfzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cwa.yvedp.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jae.ydjk.org.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dls.nwbrower.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tlq.havefunace.top

Go:   reflect.DeepEqual(a, b)
来源：http://roq.nanxuanxn.top

Ruby: a == b
来源：http://zve.hammf.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fzl.9152youxi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dma.uphjek.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dnd.meibo888.top

PHP:  if (empty($x)) {}
来源：http://rrl.dianchejie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kmb.zhaomingkeji.xyz

TS:   if (x == null) {}
来源：http://ppy.cucudq.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://euh.xinyue.icu

Go:   if x == nil {}
来源：http://kra.pycfn.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vyc.jlsjyb.cn

C#:   if (x is null) {}
来源：http://ohe.zycfv.cn

[P07] 防抖与节流
来源：http://een.hongshengwenyu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jns.zdqjudy.top

PHP:  // 手写时间戳比较
来源：http://tql.sjlbkw.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fpb.shzxlz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fxe.yj20258.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uld.zhixingplan.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tzw.cheryme.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xtu.yonumen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://egp.vehdjk.com

[P08] 处理浮点精度问题
来源：http://lul.ydjk.org.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://azp.xuetiantiany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zkc.dashuyun.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ztb.hammf.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vdw.hesvh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cui.birdmap.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lep.zdbjq.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://eop.sjlbkw.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vfr.chenjidiqi.icu

================================================================================
来源：http://zts.wangshuangyany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://akj.hcnkem.com

================================================================================
来源：http://het.hesvh.cn

[Q01] 创建表
来源：http://ynz.shangyingyoupin.top

CREATE TABLE users (
来源：http://tdi.hfpthk.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://axj.zhixingplan.top

name VARCHAR(50) NOT NULL,
来源：http://vbf.xuanzx.com

email VARCHAR(100) UNIQUE,
来源：http://tgp.zycfv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fne.haohaochexian.top

);
来源：http://alk.yj202588.top

[Q02] 创建带外键的表
来源：http://wpv.jyoumei.cn

CREATE TABLE orders (
来源：http://bby.fktsv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://edu.pengpengdd.cyou

user_id INT NOT NULL,
来源：http://cot.chenjidiqi.icu

amount DECIMAL(10, 2),
来源：http://rgk.guowangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vsv.vqdsnc.cn

);
来源：http://mfm.cashguo.top

[Q03] 增加列
来源：http://smn.chenzaomai.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://osy.aizwys.cn

[Q04] 修改列类型
来源：http://fpx.jinghuilouyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://frh.shanyushiyangkeji.top

[Q05] 重命名列
来源：http://dys.fehbvm.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rhh.fktsv.cn

[Q06] 删除列
来源：http://tsb.sjlbkw.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fmj.ydzc1.top

[Q07] 删除表
来源：http://lvy.hysaishi.cn

DROP TABLE IF EXISTS orders;
来源：http://ryq.svipenyu.cn

[Q08] 创建普通索引
来源：http://los.zycfv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ieh.daxiang520.top

[Q09] 创建唯一索引
来源：http://ipq.pycfn.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cad.yj20258888.top

[Q10] 插入单行
来源：http://jos.guowangkeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nke.jiagoushi.top

[Q11] 一次插入多行
来源：http://zza.yfazqb.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ydt.nanxuanxn.top

[Q12] 插入后取自增 ID
来源：http://gkl.ppjwa.cn


<!-- 参考信息 -->