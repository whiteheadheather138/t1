代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://wnq.xziqi.cn

JS:   console.error("err")
来源：http://rup.hnqzz.top

TS:   console.error("err")
来源：http://mlh.jiagoushi.top

Java: System.err.println("err")
来源：http://cuf.52xcode.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://veb.shzxlz.cn

Ruby: warn "err"
来源：http://mqd.hongshengwenyu.top

C#:   Console.Error.WriteLine("err")
来源：http://zbe.wangshuangyany.cn

[M07] 判断是否为主入口
来源：http://omo.chenlongwang.top

Py:   if __name__ == "__main__":
来源：http://pfw.hnxiangtu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ilv.shuidangran.top

JS:   require.main === module
来源：http://bgk.gaohongyu789.top

TS:   require.main === module
来源：http://rpg.gaohongyu789.top

Java: public static void main(String[] args)
来源：http://oio.tianlin.xyz

Go:   func main()
来源：http://xgl.xinyue.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ony.jiagoushi.top

C#:   static void Main(string[] args)
来源：http://ldp.tanke756.top

[M08] 获取系统与运行时信息
来源：http://eqs.chenjidiqi.icu

Py:   platform.system();  platform.python_version()
来源：http://cad.jqgufenzy.top

PHP:  PHP_OS;  phpversion();
来源：http://pko.nanxuanxn.top

JS:   process.platform;  process.version
来源：http://hdm.hcnkem.com

TS:   process.platform;  process.version
来源：http://ivq.ctjpmb.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nsb.vehdjk.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://mwj.sjlbkw.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oep.guowangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tcs.svipenyu.cn

================================================================================
来源：http://ocs.tanke756.top

N. 数据结构与算法
来源：http://blw.hongshengwenyu.top

================================================================================
来源：http://mtn.hfpthk.cn

[N01] 二分查找（有序数组）
来源：http://slu.jqgufenzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://shh.tian-w.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jfz.cqqwz.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xng.cheryme.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qiq.gotoacloud.top

Java: Arrays.binarySearch(arr, x)
来源：http://zeb.hnxiangtu.top

Go:   sort.SearchInts(arr, x)
来源：http://ort.fktsv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ovk.chenzaomai.com

C#:   Array.BinarySearch(arr, x)
来源：http://qol.tanke756.top

[N02] 排序（工程实践用内置实现）
来源：http://dnn.yuanzhike.top

Py:   sorted(arr);  arr.sort()
来源：http://ttd.cqqwz.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tcf.hnxiangtu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jnt.xuanzx.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://kxg.ivvv.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oeu.shzxlz.cn

Go:   slices.Sort(arr)
来源：http://gdd.tianlin.xyz

Ruby: arr.sort
来源：http://esf.uphjek.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://nui.hcnkem.com

[N03] 快速排序（分治示例）
来源：http://xsn.sufxvd.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mmj.hnqzz.top

PHP:  // 递归实现，或用 usort
来源：http://cnn.daxiang520.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lwx.shangyingyoupin.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vil.sweek.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://owu.nanxinkj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uui.chenjidiqi.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jdn.cqqwz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gvk.jqgufenzy.top

[N04] 斐波那契数列
来源：http://wex.cheryme.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sbo.guowangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zgn.yanxiufei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zfo.svipenyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eun.ivvv.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fpy.xuetiantiany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lql.shangyingyoupin.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uge.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hbq.tian-w.cn

[N05] 最大公约数
来源：http://bir.gzhubu.top

Py:   math.gcd(a, b)
来源：http://fyr.yj20258888.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rvu.tanke756.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://efd.cheryme.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://byy.ywan-chungtsiang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zdu.iojbl.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://icu.shzxlz.cn

Ruby: a.gcd(b)
来源：http://vkx.ctjpmb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://arf.yueranfly.top

[N06] 判断回文字符串
来源：http://yau.jinghuilouyu.cn

Py:   s == s[::-1]
来源：http://hzc.yfazqb.com

PHP:  $s === strrev($s);
来源：http://vxe.xingfuxueyuan.xyz

JS:   s === [...s].reverse().join("")
来源：http://znh.tarul.cn

TS:   s === [...s].reverse().join("")
来源：http://qrw.tarul.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ulo.ydzc1.top

Go:   // 双指针从两端比较
来源：http://brb.yuanzhike.top

Ruby: s == s.reverse
来源：http://xhs.chenzaomai.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://ons.haohaochexian.top

[N07] 两数之和（返回下标）
来源：http://dls.zdqjudy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://meo.shanyushiyangtech.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ykn.0kj1m.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zws.mhx1999.top

TS:   // 手写 Map<string, number>
来源：http://sni.bbcook.cn

Java: // 手写 HashMap
来源：http://szk.svipenyu.cn

Go:   // 手写 map[int]int
来源：http://upj.zhixingplan.top

Ruby: // 手写 Hash
来源：http://lvo.hongshengwenyu.top

C#:   // 手写 Dictionary<int, int>
来源：http://nfb.xziqi.cn

[N08] 生成全排列
来源：http://uvq.aizwys.cn

Py:   itertools.permutations(arr)
来源：http://hpl.daria6918.cn

PHP:  // 手写递归交换
来源：http://isd.fanxiaobao.xyz

JS:   // 手写回溯递归
来源：http://edz.52xcode.cn

TS:   // 手写回溯递归
来源：http://jlk.yangfankeji.com

Java: // 手写回溯递归
来源：http://ksh.jiagoushi.top

Go:   // 手写回溯递归
来源：http://jpc.c1oappe.top

Ruby: arr.permutation.to_a
来源：http://vkz.zhengqikj.top

C#:   // 手写回溯递归
来源：http://hip.xylfe.cn

[N09] 栈与队列
来源：http://itp.zhoulong.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nog.zhoulong.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://heg.hongshengwenyu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://hbb.vqdsnc.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qvo.feifeiyinyue.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ias.zhijiandao.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xqd.hongshengwenyu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xcd.fehbvm.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rjl.xuetiantiany.cn

[N10] 链表节点定义
来源：http://ddd.iojbl.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pwa.havefunace.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lbk.xingfuxueyuan.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://omj.hysaishi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tfw.guannengcc.top

Java: class Node { int v; Node next; }
来源：http://wyv.vqdsnc.cn

Go:   type Node struct { V int; Next *Node }
来源：http://uda.aibaodan.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yae.bjfxy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://trt.haohaochexian.top

[N11] 二叉树中序遍历
来源：http://jdt.cucudq.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://erg.cheryme.top

PHP:  // 手写递归函数
来源：http://fae.cashguo.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kqw.meibo888.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dxu.wangdashe.top

Java: // 手写递归
来源：http://qfv.jinyuanbaomall.cn

Go:   // 手写递归
来源：http://ynv.snrcjt.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gau.hnxiangtu.top

C#:   // 手写递归
来源：http://ruf.guannengcc.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vuh.yj202588.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://doe.xylfe.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rcb.vqdsnc.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hwu.hnxiangtu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ajf.9152youxi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cab.ehwqpu.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://duu.hywenlv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gdw.jinqigufen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kzg.jiagoushi.top

================================================================================
来源：http://ujt.ydzc1.top

O. 并发与异步
来源：http://vec.xingfuxueyuan.xyz

================================================================================
来源：http://fgh.cheryme.top

[O01] 启动一个线程
来源：http://vgh.epnwcf.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dhu.ydzc1.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yln.fehbvm.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jwv.xziqi.cn

TS:   // 同 JS
来源：http://ivc.ydzc1.top

Java: new Thread(() -> f()).start()
来源：http://yjk.gaohongyu789.top

Go:   go f()
来源：http://dov.uphjek.com

Ruby: Thread.new { f }
来源：http://ajs.daria6918.cn

C#:   Task.Run(() => F());
来源：http://mpd.iojbl.cn

[O02] 使用线程池
来源：http://gkq.zhengqikj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gyc.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fic.yanxiufei.cn

JS:   // worker_threads 线程池
来源：http://zom.ppjwa.cn

TS:   // worker_threads 线程池
来源：http://yct.ctjpmb.com

Java: Executors.newFixedThreadPool(4)
来源：http://npd.tanke756.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dqg.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jgv.zdbjq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kbq.ydjk.org.cn

[O03] 加锁保护共享数据
来源：http://ymo.guowangkeji.top

Py:   with lock: shared += 1
来源：http://gfv.aibaodan.cn

PHP:  // 用 flock() 做文件锁
来源：http://lsy.zhaomingkeji.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hkn.bbcook.cn

TS:   // 同 JS
来源：http://myj.ehwqpu.com

Java: synchronized (this) { shared++; }
来源：http://ssv.yuanzhike.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gmk.zhoulong.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://brq.epnwcf.com

C#:   lock (gate) { shared++; }
来源：http://tli.9152youxi.cn

[O04] 定义异步函数并等待
来源：http://dgg.shuidangran.top

Py:   async def f():⏎    await g()
来源：http://sfc.quarkkingdee.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qro.snrcjt.cn

JS:   async function f() { await g(); }
来源：http://lsz.xziqi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xqb.birdmap.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://aej.zhoulong.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://sss.yfazqb.com

Ruby: # 用 Fiber 或 async gem
来源：http://rae.shanyushiyangtech.top

C#:   async Task F() { await G(); }
来源：http://mtl.xuetiantiany.cn

[O05] 并发执行并等待全部完成
来源：http://sra.xingfuxueyuan.xyz

Py:   asyncio.gather(*tasks)
来源：http://ofb.xuetiantiany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dcn.guannengcc.top

JS:   await Promise.all(tasks)
来源：http://npd.hysaishi.cn

TS:   await Promise.all(tasks)
来源：http://pae.fktsv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sig.xingfuxueyuan.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ltf.gzhubu.top

Ruby: threads.map(&:join)
来源：http://qfk.jinghuilouyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dwz.shzxlz.cn

[O06] 使用进程池
来源：http://lim.hongshengwenyu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://frb.chenlongwang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://yql.yangfankeji.com

JS:   // child_process / cluster 模块
来源：http://xgp.sjlbkw.cn

TS:   // child_process / cluster 模块
来源：http://htf.tian-w.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xbr.gogol.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://imk.havefunace.top

Ruby: // fork 块
来源：http://pjs.yangfankeji.com

C#:   Parallel.For
来源：http://vmn.xingfuxueyuan.xyz

================================================================================
来源：http://lfx.zhaomingkeji.xyz

P. 常用工具函数
来源：http://rhv.zhengqikj.top

================================================================================
来源：http://tmn.havefunace.top

[P01] 生成 UUID
来源：http://kam.gogol.net.cn

Py:   str(uuid.uuid4())
来源：http://ctf.vehdjk.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://afy.cheryme.top

JS:   crypto.randomUUID()
来源：http://soe.fzhhl.top

TS:   crypto.randomUUID()
来源：http://qey.sufxvd.cn

Java: UUID.randomUUID().toString()
来源：http://ufr.sjlbkw.cn

Go:   // 用 github.com/google/uuid
来源：http://mrg.nwbrower.top

Ruby: SecureRandom.uuid
来源：http://lou.zdqjudy.top

C#:   Guid.NewGuid().ToString()
来源：http://ryw.yangfankeji.com

[P02] MD5 / SHA256 摘要
来源：http://eea.jinqigufen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lnb.ybcxt.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ajx.shanyushiyangtech.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vyq.feifeiyinyue.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sgj.dashuyun.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cll.cheryme.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zmn.cheryme.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fcd.pengpengdd.cyou

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dvf.c1oappe.top

[P03] 生成短随机字符串
来源：http://zsg.hongshengwenyu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://khu.yonumen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cys.ydzc1.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://puf.xuanzx.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ypv.jqgufenzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iiy.xingfuxueyuan.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://haa.ppjwa.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://crc.ydzc1.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ewq.52xcode.cn

[P04] 求长度
来源：http://ixm.hesvh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tit.nanxinkj.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://emm.haohaochexian.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wtm.c1oappe.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pyb.jyoumei.cn

Java: list.size();  map.size();  s.length()
来源：http://pnh.yfazqb.com

Go:   len(arr);  len(m)
来源：http://rgi.wangdashe.top

Ruby: x.length;  x.size
来源：http://qpj.yfazqb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://pgd.ydjk.org.cn

[P05] 判断两个对象内容是否相等
来源：http://ugs.cqqwz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://twe.gotoacloud.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gjk.tian-w.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sbl.zhoulong.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://iao.quarkkingdee.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bzv.vqdsnc.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kmx.aizwys.cn

Ruby: a == b
来源：http://gjh.kuanghao11.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://idm.feifeiyinyue.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xey.xinyue.icu

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zlo.xuanzx.com

PHP:  if (empty($x)) {}
来源：http://hbg.zdbjq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vum.daxiang520.top

TS:   if (x == null) {}
来源：http://vih.cheryme.top

Java: if (x == null || x.isEmpty()) {}
来源：http://bbh.aibaodan.cn

Go:   if x == nil {}
来源：http://hpm.uphjek.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yia.nanxinkj.top

C#:   if (x is null) {}
来源：http://tsp.jqgufenzy.top

[P07] 防抖与节流
来源：http://zsb.yanxiufei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fmq.guowangkeji.top

PHP:  // 手写时间戳比较
来源：http://xcx.52xcode.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pam.jianghu66.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://szg.dashuyun.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://smd.cdnleiting.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fzf.sweek.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cii.mhx1999.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ate.hnxiangtu.top

[P08] 处理浮点精度问题
来源：http://dbv.hnqzz.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://acg.jlsjyb.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gqg.daxiang520.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hvu.chenzaomai.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jlt.sweek.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://cqr.zdbjq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hnf.shzxlz.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vwd.andypj.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fyg.c1oappe.top

================================================================================
来源：http://jpa.ppjwa.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wbq.52xcode.cn

================================================================================
来源：http://xbg.shanyushiyangkeji.top

[Q01] 创建表
来源：http://jib.ywan-chungtsiang.top

CREATE TABLE users (
来源：http://qka.yangfankeji.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gka.shanyushiyangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://iza.redwolf501.top

email VARCHAR(100) UNIQUE,
来源：http://tqp.yonumen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xki.zhixingplan.top

);
来源：http://sjs.havefunace.top

[Q02] 创建带外键的表
来源：http://ypp.quarkkingdee.top

CREATE TABLE orders (
来源：http://nox.ydzc1.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sun.hysaishi.cn

user_id INT NOT NULL,
来源：http://qvk.fzhhl.top

amount DECIMAL(10, 2),
来源：http://txg.zhijiandao.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kct.yuanzhike.top

);
来源：http://uld.feifeiyinyue.top

[Q03] 增加列
来源：http://oea.fanxiaobao.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hau.ppjwa.cn

[Q04] 修改列类型
来源：http://rfx.ydzc1.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ldp.jinqigufen.top

[Q05] 重命名列
来源：http://dly.yanxiufei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qhc.hfpthk.cn

[Q06] 删除列
来源：http://scd.ydjk.org.cn

ALTER TABLE users DROP COLUMN age;
来源：http://coz.hnxiangtu.top

[Q07] 删除表
来源：http://toj.fehbvm.com

DROP TABLE IF EXISTS orders;
来源：http://fou.aizwys.cn

[Q08] 创建普通索引
来源：http://emt.ctjpmb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://ajc.ybcxt.top

[Q09] 创建唯一索引
来源：http://bav.yj20258888.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lds.9152youxi.cn

[Q10] 插入单行
来源：http://bqx.wangshuangyany.cn


<!-- 参考信息 -->