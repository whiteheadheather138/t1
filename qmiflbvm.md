代发 wailian999

Ruby: exit 1
来源：http://lcc.fktsv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tfv.jinyuanbaomall.cn

[M06] 向标准错误输出
来源：http://hig.xziqi.cn

Py:   print("err", file=sys.stderr)
来源：http://kys.shzxlz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kia.zhaomingkeji.xyz

JS:   console.error("err")
来源：http://ktt.shzxlz.cn

TS:   console.error("err")
来源：http://dga.meibo888.top

Java: System.err.println("err")
来源：http://yso.hcnkem.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hki.haohaochexian.top

Ruby: warn "err"
来源：http://gax.yfazqb.com

C#:   Console.Error.WriteLine("err")
来源：http://qbm.jyoumei.cn

[M07] 判断是否为主入口
来源：http://daa.yongpay.top

Py:   if __name__ == "__main__":
来源：http://bhp.wangdashe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ylw.shanyushiyangkeji.top

JS:   require.main === module
来源：http://bqx.meibo888.top

TS:   require.main === module
来源：http://biu.meibo888.top

Java: public static void main(String[] args)
来源：http://cya.aibaodan.cn

Go:   func main()
来源：http://ulf.fktsv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://plj.hongshengwenyu.top

C#:   static void Main(string[] args)
来源：http://min.feifeiyinyue.top

[M08] 获取系统与运行时信息
来源：http://hue.birdmap.top

Py:   platform.system();  platform.python_version()
来源：http://ebl.xuetiantiany.cn

PHP:  PHP_OS;  phpversion();
来源：http://zwn.aizwys.cn

JS:   process.platform;  process.version
来源：http://ntz.ybcxt.top

TS:   process.platform;  process.version
来源：http://lqp.52xcode.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://eko.shanyushiyangtech.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://kql.zdbjq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fux.jianghu66.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://umr.ppjwa.cn

================================================================================
来源：http://mcd.ybcxt.top

N. 数据结构与算法
来源：http://pxv.xingfuxueyuan.xyz

================================================================================
来源：http://dyk.meibo888.top

[N01] 二分查找（有序数组）
来源：http://csd.shanyushiyangtech.top

Py:   bisect.bisect_left(arr, x)
来源：http://vag.vehdjk.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jjq.daxiang520.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rsp.tarul.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tzs.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://foj.zhengqikj.top

Go:   sort.SearchInts(arr, x)
来源：http://gfv.tianlin.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://vie.sxryk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dyp.zhiwuduotai.top

[N02] 排序（工程实践用内置实现）
来源：http://xeh.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://aov.zhongyouzk.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://npf.sxryk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://fzo.zhixingplan.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qqk.zhixingplan.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dsc.tarul.cn

Go:   slices.Sort(arr)
来源：http://zal.jianghu66.top

Ruby: arr.sort
来源：http://rtc.zhongyouzk.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://vsr.shuidangran.top

[N03] 快速排序（分治示例）
来源：http://iox.ydzc1.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://piy.sweek.top

PHP:  // 递归实现，或用 usort
来源：http://nac.cheryme.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mva.cucudq.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://acv.jinghuilouyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vpe.svipenyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qzt.yfazqb.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://enh.hnxiangtu.top

C#:   // 手写递归，或 Array.Sort
来源：http://ule.jinqigufen.top

[N04] 斐波那契数列
来源：http://yym.hfpthk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hhc.xinyue.icu

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mei.ctjpmb.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ait.yongpay.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://umx.zhiwuduotai.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://czr.jinghuilouyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://epz.chenjidiqi.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gea.vehdjk.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://slx.fanxiaobao.xyz

[N05] 最大公约数
来源：http://pnj.wangshuangyany.cn

Py:   math.gcd(a, b)
来源：http://gvg.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://srv.zhongyouzk.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mnx.shanyushiyangtech.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nfp.cqqwz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qjc.tianlin.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://uxr.0kj1m.cn

Ruby: a.gcd(b)
来源：http://ora.ydzc1.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://voc.dashuyun.cn

[N06] 判断回文字符串
来源：http://fcg.tian-w.cn

Py:   s == s[::-1]
来源：http://sfw.yangfankeji.com

PHP:  $s === strrev($s);
来源：http://fjt.yj20258.top

JS:   s === [...s].reverse().join("")
来源：http://sjm.jinyuanbaomall.cn

TS:   s === [...s].reverse().join("")
来源：http://wel.yonumen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mvu.c1oappe.top

Go:   // 双指针从两端比较
来源：http://usm.hnxiangtu.top

Ruby: s == s.reverse
来源：http://ige.yfazqb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://fog.ppjwa.cn

[N07] 两数之和（返回下标）
来源：http://bpo.smart0.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://srf.yongpay.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hfn.yongpay.top

JS:   // 手写 Map：map.set(v, i)
来源：http://pal.birdmap.top

TS:   // 手写 Map<string, number>
来源：http://mdu.xinyue.icu

Java: // 手写 HashMap
来源：http://mjw.epnwcf.com

Go:   // 手写 map[int]int
来源：http://jqe.zhongyouzk.top

Ruby: // 手写 Hash
来源：http://upd.cqqwz.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cfd.zdbjq.cn

[N08] 生成全排列
来源：http://fnj.yfazqb.com

Py:   itertools.permutations(arr)
来源：http://jyu.yongpay.top

PHP:  // 手写递归交换
来源：http://wab.hongshengwenyu.top

JS:   // 手写回溯递归
来源：http://cni.snrcjt.cn

TS:   // 手写回溯递归
来源：http://mnr.shangyingyoupin.top

Java: // 手写回溯递归
来源：http://yyj.xingfuxueyuan.xyz

Go:   // 手写回溯递归
来源：http://zgw.shuidangran.top

Ruby: arr.permutation.to_a
来源：http://ztb.fktsv.cn

C#:   // 手写回溯递归
来源：http://mir.hcnkem.com

[N09] 栈与队列
来源：http://wie.hammf.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kyb.svipenyu.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cuj.jinghuilouyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://byc.chenlongwang.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wtf.yvedp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ely.yuanzhike.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://isp.xuetiantiany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mrq.dianchejie.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gsq.316326.xyz

[N10] 链表节点定义
来源：http://fzu.hysaishi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dzv.jlsjyb.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://whl.jyoumei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://typ.guannengcc.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eha.gotoacloud.top

Java: class Node { int v; Node next; }
来源：http://whp.yangfankeji.com

Go:   type Node struct { V int; Next *Node }
来源：http://ocx.zdbjq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kas.snrcjt.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fwq.wangdashe.top

[N11] 二叉树中序遍历
来源：http://boe.uphjek.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uay.wangdashe.top

PHP:  // 手写递归函数
来源：http://auw.fktsv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dzq.yonumen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wue.zhaomingkeji.xyz

Java: // 手写递归
来源：http://jon.jqgfzy.top

Go:   // 手写递归
来源：http://bhq.hammf.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cpo.cashguo.top

C#:   // 手写递归
来源：http://rjg.feifeiyinyue.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://iew.yfazqb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fkg.9152youxi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ksa.yfazqb.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://khy.yanxiufei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bkb.aizwys.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oya.cdnleiting.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cxx.guowangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lke.ybcxt.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yvf.jqgufenzy.top

================================================================================
来源：http://gsa.andypj.xyz

O. 并发与异步
来源：http://iop.fanxiaobao.xyz

================================================================================
来源：http://kxc.xylfe.cn

[O01] 启动一个线程
来源：http://thk.jinqigfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mdc.bbcook.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hnt.ydzc1.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gdx.wangshuangyany.cn

TS:   // 同 JS
来源：http://gbv.yonumen.top

Java: new Thread(() -> f()).start()
来源：http://jmh.ehwqpu.com

Go:   go f()
来源：http://ynx.jyoumei.cn

Ruby: Thread.new { f }
来源：http://jsv.pycfn.com

C#:   Task.Run(() => F());
来源：http://qqh.zycfv.cn

[O02] 使用线程池
来源：http://xih.iojbl.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pyo.yanxiufei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qxj.yuxming.cn

JS:   // worker_threads 线程池
来源：http://hjv.hongshengwenyu.top

TS:   // worker_threads 线程池
来源：http://oxt.yfazqb.com

Java: Executors.newFixedThreadPool(4)
来源：http://hcg.tian-w.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bhb.sysykeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zcx.cqqwz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eys.fengsongda.top

[O03] 加锁保护共享数据
来源：http://cfy.nanxinkj.top

Py:   with lock: shared += 1
来源：http://ddm.zdqjudy.top

PHP:  // 用 flock() 做文件锁
来源：http://nja.gogol.net.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jhx.guowangkeji.top

TS:   // 同 JS
来源：http://sgl.yj20258888.top

Java: synchronized (this) { shared++; }
来源：http://wqd.uphjek.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rmg.kuanghao11.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hfj.xuetiantiany.cn

C#:   lock (gate) { shared++; }
来源：http://mfu.dianchejie.cn

[O04] 定义异步函数并等待
来源：http://dfw.xuetiantiany.cn

Py:   async def f():⏎    await g()
来源：http://jql.feifeiyinyue.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cmx.sxryk.cn

JS:   async function f() { await g(); }
来源：http://gso.gzhubu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://alp.tanke756.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gwm.jqgufenzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://beh.zhixingplan.top

Ruby: # 用 Fiber 或 async gem
来源：http://hur.yj20258.top

C#:   async Task F() { await G(); }
来源：http://cyy.sjlbkw.cn

[O05] 并发执行并等待全部完成
来源：http://imd.zdbjq.cn

Py:   asyncio.gather(*tasks)
来源：http://tsk.gogol.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tbe.jianghu66.top

JS:   await Promise.all(tasks)
来源：http://lim.ywan-chungtsiang.top

TS:   await Promise.all(tasks)
来源：http://ixm.daxiang520.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ocr.tianlin.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://llb.0kj1m.cn

Ruby: threads.map(&:join)
来源：http://rti.fengsongda.top

C#:   await Task.WhenAll(t1, t2)
来源：http://gxv.shangyingyoupin.top

[O06] 使用进程池
来源：http://ztm.wangshuangyany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mwe.vehdjk.com

PHP:  // pcntl_fork 或多进程队列
来源：http://vck.sufxvd.cn

JS:   // child_process / cluster 模块
来源：http://yah.aibaodan.cn

TS:   // child_process / cluster 模块
来源：http://feg.sweek.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qzt.ydjk.org.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://huo.hysaishi.cn

Ruby: // fork 块
来源：http://yif.hammf.cn

C#:   Parallel.For
来源：http://geq.gotoacloud.top

================================================================================
来源：http://zrw.316326.xyz

P. 常用工具函数
来源：http://zpr.9152youxi.cn

================================================================================
来源：http://byj.sweek.top

[P01] 生成 UUID
来源：http://fts.pycfn.com

Py:   str(uuid.uuid4())
来源：http://efw.hnxiangtu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wcb.aibaodan.cn

JS:   crypto.randomUUID()
来源：http://ioi.yj202588.top

TS:   crypto.randomUUID()
来源：http://xhl.xuanzx.com

Java: UUID.randomUUID().toString()
来源：http://zsr.zhaomingkeji.xyz

Go:   // 用 github.com/google/uuid
来源：http://ffe.gzhubu.top

Ruby: SecureRandom.uuid
来源：http://cla.jinyuanbaomall.cn

C#:   Guid.NewGuid().ToString()
来源：http://nbf.hongshengwenyu.top

[P02] MD5 / SHA256 摘要
来源：http://xzp.yj202588.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hri.shangyingyoupin.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xkk.sysykeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://epi.bbcook.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oey.bjfxy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rvx.xuetiantiany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ugx.shanyushiyangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qmk.yfazqb.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nce.yuanzhike.top

[P03] 生成短随机字符串
来源：http://tnh.9152youxi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ucj.0kj1m.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jpz.jqgufenzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zmj.cqqwz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iqv.kuanghao11.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wen.jiagoushi.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tow.yvedp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://aso.hesvh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://otj.zhixingplan.top

[P04] 求长度
来源：http://nrh.ehwqpu.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ivg.jinqigfzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jxe.haohaochexian.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mnl.zycfv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zln.pengpengdd.cyou

Java: list.size();  map.size();  s.length()
来源：http://vsg.zycfv.cn

Go:   len(arr);  len(m)
来源：http://ywc.gzhubu.top

Ruby: x.length;  x.size
来源：http://pxc.vehdjk.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://ogt.snrcjt.cn

[P05] 判断两个对象内容是否相等
来源：http://hwf.zhijiandao.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gvt.aibaodan.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qtu.fehbvm.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wvu.pengpengdd.cyou

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://edn.guannengcc.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zrg.tianlin.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://kcr.yuanzhike.top

Ruby: a == b
来源：http://pzs.jqgfzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hkc.zdqjudy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wfe.tianlin.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ywr.cashguo.top

PHP:  if (empty($x)) {}
来源：http://sjt.sufxvd.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jvk.ehwqpu.com

TS:   if (x == null) {}
来源：http://mye.52xcode.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nrv.sufxvd.cn

Go:   if x == nil {}
来源：http://wvw.shanyushiyangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://umz.jlsjyb.cn

C#:   if (x is null) {}
来源：http://rct.xinyue.icu

[P07] 防抖与节流
来源：http://cyu.fanxiaobao.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eir.epnwcf.com

PHP:  // 手写时间戳比较
来源：http://acp.hywenlv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gbs.zhijiandao.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pir.jqgfzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hpn.nwbrower.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://crg.jinghuilouyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fmc.hnxiangtu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uij.9152youxi.cn

[P08] 处理浮点精度问题
来源：http://tai.shanyushiyangtech.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://knj.zdbjq.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gid.dianchejie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fyw.andypj.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://twf.svipenyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://emi.sjlbkw.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ifo.52xcode.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dju.yonumen.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tfs.gzhubu.top

================================================================================
来源：http://eux.pycfn.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lmw.zdbjq.cn

================================================================================
来源：http://eyk.hcnkem.com

[Q01] 创建表
来源：http://fzn.zhiwuduotai.top

CREATE TABLE users (
来源：http://lcc.zhixingplan.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fkv.andypj.xyz

name VARCHAR(50) NOT NULL,
来源：http://qvg.hesvh.cn

email VARCHAR(100) UNIQUE,
来源：http://yjv.feifeiyinyue.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://drp.andypj.xyz

);
来源：http://yfi.vehdjk.com

[Q02] 创建带外键的表
来源：http://jxb.c1oappe.top

CREATE TABLE orders (
来源：http://iuz.yuxming.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sod.wangshuangyany.cn

user_id INT NOT NULL,
来源：http://wff.zycfv.cn

amount DECIMAL(10, 2),
来源：http://ksj.yuanzhike.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ycl.sjlbkw.cn

);
来源：http://hcw.guannengcc.top

[Q03] 增加列
来源：http://qyl.ctjpmb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cal.yueranfly.top

[Q04] 修改列类型
来源：http://uoz.cheryme.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lvs.ywan-chungtsiang.top

[Q05] 重命名列
来源：http://xli.c1oappe.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://iyc.kuanghao11.cn

[Q06] 删除列
来源：http://bms.zdbjq.cn

ALTER TABLE users DROP COLUMN age;
来源：http://scp.yueranfly.top

[Q07] 删除表
来源：http://ddr.fktsv.cn

DROP TABLE IF EXISTS orders;
来源：http://hql.zhongyouzk.top

[Q08] 创建普通索引
来源：http://eyr.fanxiaobao.xyz


<!-- 参考信息 -->