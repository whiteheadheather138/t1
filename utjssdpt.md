代发 wailian999

Ruby: exit 1
来源：http://fak.xuetiantiany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cdi.jqgufenzy.top

[M06] 向标准错误输出
来源：http://bfq.yuanzhike.top

Py:   print("err", file=sys.stderr)
来源：http://cct.chenzaomai.com

PHP:  fwrite(STDERR, "err\n");
来源：http://hju.zhiwuduotai.top

JS:   console.error("err")
来源：http://xri.fengsongda.top

TS:   console.error("err")
来源：http://iqq.ehwqpu.com

Java: System.err.println("err")
来源：http://nol.tianlin.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fzx.shuidangran.top

Ruby: warn "err"
来源：http://pcp.hnqzz.top

C#:   Console.Error.WriteLine("err")
来源：http://zsb.vqdsnc.cn

[M07] 判断是否为主入口
来源：http://nnq.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://pck.xylfe.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://drl.zhiwuduotai.top

JS:   require.main === module
来源：http://amj.ydjk.org.cn

TS:   require.main === module
来源：http://pih.wangdashe.top

Java: public static void main(String[] args)
来源：http://rty.bbcook.cn

Go:   func main()
来源：http://vfk.aizwys.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://msg.tanke756.top

C#:   static void Main(string[] args)
来源：http://lhl.shzxlz.cn

[M08] 获取系统与运行时信息
来源：http://giz.vqdsnc.cn

Py:   platform.system();  platform.python_version()
来源：http://num.chenlongwang.top

PHP:  PHP_OS;  phpversion();
来源：http://qic.gzhubu.top

JS:   process.platform;  process.version
来源：http://goi.fzhhl.top

TS:   process.platform;  process.version
来源：http://hhm.svipenyu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://psz.cqqwz.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://shv.daria6918.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ypi.yuanzhike.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tqt.hongshengwenyu.top

================================================================================
来源：http://cqo.jinqigufen.top

N. 数据结构与算法
来源：http://sfz.hesvh.cn

================================================================================
来源：http://wpf.jqgufenzy.top

[N01] 二分查找（有序数组）
来源：http://jhi.yonumen.top

Py:   bisect.bisect_left(arr, x)
来源：http://lcj.c1oappe.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lis.fehbvm.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lkr.bbcook.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cgg.yuxming.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rxr.sufxvd.cn

Go:   sort.SearchInts(arr, x)
来源：http://uxo.gogol.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://bgf.guannengcc.top

C#:   Array.BinarySearch(arr, x)
来源：http://mge.pengpengdd.cyou

[N02] 排序（工程实践用内置实现）
来源：http://nnm.guannengcc.top

Py:   sorted(arr);  arr.sort()
来源：http://nqh.havefunace.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oth.fehbvm.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://lrl.shuidangran.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://prt.dianchejie.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kqw.epnwcf.com

Go:   slices.Sort(arr)
来源：http://bkb.jqgufenzy.top

Ruby: arr.sort
来源：http://ozy.yuanzhike.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jly.yonumen.top

[N03] 快速排序（分治示例）
来源：http://wyf.xingfuxueyuan.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rnj.xuanzx.com

PHP:  // 递归实现，或用 usort
来源：http://mye.wangshuangyany.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oor.cqqwz.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zwc.sysykeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ank.jlsjyb.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xzb.daxiang520.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mxe.nanxinkj.top

C#:   // 手写递归，或 Array.Sort
来源：http://yxn.tanke756.top

[N04] 斐波那契数列
来源：http://qbg.kuanghao11.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xzn.ywan-chungtsiang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jkf.sweek.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ust.bjfxy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ovx.hywenlv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eeo.dashuyun.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mke.9152youxi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xfg.shangyingyoupin.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://obr.316326.xyz

[N05] 最大公约数
来源：http://mxb.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://snh.sufxvd.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ivc.vehdjk.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://sbs.jiagoushi.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xlh.jqgufenzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rtu.ivvv.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oni.dashuyun.cn

Ruby: a.gcd(b)
来源：http://iyy.c1oappe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gqr.yuanzhike.top

[N06] 判断回文字符串
来源：http://kah.hysaishi.cn

Py:   s == s[::-1]
来源：http://rqe.shanyushiyangtech.top

PHP:  $s === strrev($s);
来源：http://ikp.andypj.xyz

JS:   s === [...s].reverse().join("")
来源：http://pec.chenlongwang.top

TS:   s === [...s].reverse().join("")
来源：http://tyb.havefunace.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://htx.dashuyun.cn

Go:   // 双指针从两端比较
来源：http://thc.yj20258888.top

Ruby: s == s.reverse
来源：http://fml.guowangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://mtc.feifeiyinyue.top

[N07] 两数之和（返回下标）
来源：http://bwy.pengpengdd.cyou

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zst.kuanghao11.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zhs.gzhubu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zln.zhiwuduotai.top

TS:   // 手写 Map<string, number>
来源：http://tqr.fehbvm.com

Java: // 手写 HashMap
来源：http://rma.sjlbkw.cn

Go:   // 手写 map[int]int
来源：http://bli.jinqigufen.top

Ruby: // 手写 Hash
来源：http://xvq.havefunace.top

C#:   // 手写 Dictionary<int, int>
来源：http://vro.haohaochexian.top

[N08] 生成全排列
来源：http://rjw.jqgfzy.top

Py:   itertools.permutations(arr)
来源：http://xlt.hnxiangtu.top

PHP:  // 手写递归交换
来源：http://lzn.fzhhl.top

JS:   // 手写回溯递归
来源：http://ghu.ivvv.top

TS:   // 手写回溯递归
来源：http://dtw.xuanzx.com

Java: // 手写回溯递归
来源：http://ftl.yuxming.cn

Go:   // 手写回溯递归
来源：http://cwr.hesvh.cn

Ruby: arr.permutation.to_a
来源：http://eie.gotoacloud.top

C#:   // 手写回溯递归
来源：http://ncl.ivvv.top

[N09] 栈与队列
来源：http://dhb.wangdashe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cxc.zhixingplan.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lda.kuanghao11.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ubr.hywenlv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://niq.zhengqikj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lpn.svipenyu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://art.yangfankeji.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://icp.yj20258888.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://exf.fktsv.cn

[N10] 链表节点定义
来源：http://eyi.cucudq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://khy.xuetiantiany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ahh.havefunace.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ndn.hywenlv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yds.jlsjyb.cn

Java: class Node { int v; Node next; }
来源：http://pjn.52xcode.cn

Go:   type Node struct { V int; Next *Node }
来源：http://wee.gaohongyu789.top

Ruby: Node = Struct.new(:v, :next)
来源：http://crj.mhx1999.top

C#:   class Node { public int V; public Node? Next; }
来源：http://vxq.iojbl.cn

[N11] 二叉树中序遍历
来源：http://ckk.hongshengwenyu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fmm.zhijiandao.cn

PHP:  // 手写递归函数
来源：http://znj.jinqigufen.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qdw.shangyingyoupin.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dke.zhongyouzk.top

Java: // 手写递归
来源：http://pkl.zhoulong.xyz

Go:   // 手写递归
来源：http://jvu.hnxiangtu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ybj.andypj.xyz

C#:   // 手写递归
来源：http://ajj.tarul.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nma.epnwcf.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lws.epnwcf.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://joe.yueranfly.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://udo.gzhubu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cos.gotoacloud.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qgk.fengsongda.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zkv.jinyuanbaomall.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nqf.xuetiantiany.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vqm.guannengcc.top

================================================================================
来源：http://xqv.ywan-chungtsiang.top

O. 并发与异步
来源：http://ccj.tian-w.cn

================================================================================
来源：http://gox.snrcjt.cn

[O01] 启动一个线程
来源：http://pxa.sysykeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bis.nanxuanxn.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xti.jqgfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://myj.cqqwz.cn

TS:   // 同 JS
来源：http://tem.zdbjq.cn

Java: new Thread(() -> f()).start()
来源：http://nqy.dashuyun.cn

Go:   go f()
来源：http://bxw.iojbl.cn

Ruby: Thread.new { f }
来源：http://pgw.yuanzhike.top

C#:   Task.Run(() => F());
来源：http://rdk.nwbrower.top

[O02] 使用线程池
来源：http://myk.zhaomingkeji.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pge.xuetiantiany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gjk.xinyue.icu

JS:   // worker_threads 线程池
来源：http://bqq.ctjpmb.com

TS:   // worker_threads 线程池
来源：http://pca.tianlin.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://kpa.zhiwuduotai.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mgo.bbcook.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nfk.aizwys.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wnb.hysaishi.cn

[O03] 加锁保护共享数据
来源：http://fzq.jinqigfzy.top

Py:   with lock: shared += 1
来源：http://hnn.dianchejie.cn

PHP:  // 用 flock() 做文件锁
来源：http://vdu.cucudq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hwi.jqgufenzy.top

TS:   // 同 JS
来源：http://kfk.hcnkem.com

Java: synchronized (this) { shared++; }
来源：http://nnm.ehwqpu.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dnk.daxiang520.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://wag.chenlongwang.top

C#:   lock (gate) { shared++; }
来源：http://azp.tian-w.cn

[O04] 定义异步函数并等待
来源：http://evk.chenjidiqi.icu

Py:   async def f():⏎    await g()
来源：http://mab.fanxiaobao.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qto.hcnkem.com

JS:   async function f() { await g(); }
来源：http://odn.epnwcf.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://reu.zhengqikj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bqr.shangyingyoupin.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bqm.jlsjyb.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gfv.bjfxy.top

C#:   async Task F() { await G(); }
来源：http://mpe.shzxlz.cn

[O05] 并发执行并等待全部完成
来源：http://gmo.zhixingplan.top

Py:   asyncio.gather(*tasks)
来源：http://yuk.aibaodan.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hem.ywan-chungtsiang.top

JS:   await Promise.all(tasks)
来源：http://hut.gogol.net.cn

TS:   await Promise.all(tasks)
来源：http://djg.yangfankeji.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pjh.fengsongda.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://plj.316326.xyz

Ruby: threads.map(&:join)
来源：http://fgk.cheryme.top

C#:   await Task.WhenAll(t1, t2)
来源：http://quu.dashuyun.cn

[O06] 使用进程池
来源：http://usp.jiagoushi.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bal.sjlbkw.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://czm.ydzc1.top

JS:   // child_process / cluster 模块
来源：http://oyj.xinyue.icu

TS:   // child_process / cluster 模块
来源：http://jfk.xuetiantiany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xfc.yonumen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cai.316326.xyz

Ruby: // fork 块
来源：http://sed.uphjek.com

C#:   Parallel.For
来源：http://kcf.hnxiangtu.top

================================================================================
来源：http://kzu.xziqi.cn

P. 常用工具函数
来源：http://gnm.yonumen.top

================================================================================
来源：http://fdy.dianchejie.cn

[P01] 生成 UUID
来源：http://rec.quarkkingdee.top

Py:   str(uuid.uuid4())
来源：http://gcx.daria6918.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zaq.pycfn.com

JS:   crypto.randomUUID()
来源：http://iji.9152youxi.cn

TS:   crypto.randomUUID()
来源：http://xnq.c1oappe.top

Java: UUID.randomUUID().toString()
来源：http://uhd.daria6918.cn

Go:   // 用 github.com/google/uuid
来源：http://uib.316326.xyz

Ruby: SecureRandom.uuid
来源：http://uve.hnqzz.top

C#:   Guid.NewGuid().ToString()
来源：http://acz.shanyushiyangtech.top

[P02] MD5 / SHA256 摘要
来源：http://pda.vqdsnc.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qby.guannengcc.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://sto.xinyue.icu

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fxh.cheryme.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kbw.pengpengdd.cyou

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pad.zhoulong.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mqz.shzxlz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nbo.xylfe.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://myt.guannengcc.top

[P03] 生成短随机字符串
来源：http://pek.hywenlv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://scc.nanxinkj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xqt.yueranfly.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://btd.kuanghao11.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gfc.tarul.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ljv.shanyushiyangtech.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oak.fehbvm.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://kux.yongpay.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://oxq.zdqjudy.top

[P04] 求长度
来源：http://ldy.tarul.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wdp.yuxming.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qci.ppjwa.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mji.hnxiangtu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ndk.hywenlv.cn

Java: list.size();  map.size();  s.length()
来源：http://zmj.guowangkeji.top

Go:   len(arr);  len(m)
来源：http://oig.svipenyu.cn

Ruby: x.length;  x.size
来源：http://mom.yanxiufei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bjd.gogol.net.cn

[P05] 判断两个对象内容是否相等
来源：http://tlj.aizwys.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pys.fehbvm.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ffy.gotoacloud.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ocg.jinqigfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ifm.tanke756.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gyj.uphjek.com

Go:   reflect.DeepEqual(a, b)
来源：http://mwt.sjlbkw.cn

Ruby: a == b
来源：http://frz.shanyushiyangkeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ogp.zhaomingkeji.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ytc.epnwcf.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ruk.c1oappe.top

PHP:  if (empty($x)) {}
来源：http://koq.jyoumei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tjm.gzhubu.top

TS:   if (x == null) {}
来源：http://kgq.dianchejie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uod.bbcook.cn

Go:   if x == nil {}
来源：http://vbi.jinqigufen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pgp.jinqigufen.top

C#:   if (x is null) {}
来源：http://zxg.ydjk.org.cn

[P07] 防抖与节流
来源：http://jzi.hywenlv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kis.vehdjk.com

PHP:  // 手写时间戳比较
来源：http://sta.ivvv.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jnp.hfpthk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://knd.chenlongwang.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dkp.ehwqpu.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oyw.ydzc1.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gzz.yangfankeji.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dyk.jinqigufen.top

[P08] 处理浮点精度问题
来源：http://lrs.fanxiaobao.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vfc.jiagoushi.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dei.epnwcf.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://chk.guannengcc.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ydp.epnwcf.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vft.xingfuxueyuan.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tfp.ywan-chungtsiang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qxw.hongshengwenyu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lbb.jinghuilouyu.cn

================================================================================
来源：http://ysz.c1oappe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rxx.yvedp.cn

================================================================================
来源：http://cad.nanxinkj.top

[Q01] 创建表
来源：http://wom.zhongyouzk.top

CREATE TABLE users (
来源：http://tuj.0kj1m.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yhl.fengsongda.top

name VARCHAR(50) NOT NULL,
来源：http://pno.gotoacloud.top

email VARCHAR(100) UNIQUE,
来源：http://lsf.jqgufenzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sey.zhixingplan.top

);
来源：http://rzr.gogol.net.cn

[Q02] 创建带外键的表
来源：http://npl.wangshuangyany.cn

CREATE TABLE orders (
来源：http://laa.havefunace.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://scx.hnxiangtu.top

user_id INT NOT NULL,
来源：http://zeq.cdnleiting.top

amount DECIMAL(10, 2),
来源：http://usp.xuanzx.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cdc.kuanghao11.cn

);
来源：http://xhi.shangyingyoupin.top

[Q03] 增加列
来源：http://ewt.xingfuxueyuan.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gyk.bjfxy.top

[Q04] 修改列类型
来源：http://rhe.sufxvd.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bti.tanke756.top

[Q05] 重命名列
来源：http://jxi.zdqjudy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bgu.dianchejie.cn

[Q06] 删除列
来源：http://hqy.hywenlv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://yii.ydjk.org.cn

[Q07] 删除表
来源：http://oqt.yuanzhike.top

DROP TABLE IF EXISTS orders;
来源：http://qkp.zhaomingkeji.xyz

[Q08] 创建普通索引
来源：http://uwp.zdbjq.cn


<!-- 参考信息 -->