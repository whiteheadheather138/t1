代发 wailian999

[M04] 获取当前工作目录
来源：http://ghl.316326.xyz

Py:   os.getcwd()
来源：http://exq.pengpengdd.cyou

PHP:  getcwd();
来源：http://njs.andypj.xyz

JS:   process.cwd()
来源：http://pqj.havefunace.top

TS:   process.cwd()
来源：http://afk.zhengqikj.top

Java: Path.of("").toAbsolutePath()
来源：http://adn.fktsv.cn

Go:   os.Getwd()
来源：http://ubj.gzhubu.top

Ruby: Dir.pwd
来源：http://exf.bjfxy.top

C#:   Directory.GetCurrentDirectory()
来源：http://yvd.dianchejie.cn

[M05] 设置退出码
来源：http://kns.zhongyouzk.top

Py:   sys.exit(1)
来源：http://enh.xingfuxueyuan.xyz

PHP:  exit(1);
来源：http://lyi.zhoulong.xyz

JS:   process.exit(1)
来源：http://lir.zycfv.cn

TS:   process.exit(1)
来源：http://beh.vqdsnc.cn

Java: System.exit(1)
来源：http://ito.sysykeji.top

Go:   os.Exit(1)
来源：http://tap.sufxvd.cn

Ruby: exit 1
来源：http://kkn.hnqzz.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://epy.ppjwa.cn

[M06] 向标准错误输出
来源：http://tpm.tian-w.cn

Py:   print("err", file=sys.stderr)
来源：http://zci.shanyushiyangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://nrh.yj20258.top

JS:   console.error("err")
来源：http://jbj.birdmap.top

TS:   console.error("err")
来源：http://jeo.epnwcf.com

Java: System.err.println("err")
来源：http://wjd.hcnkem.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yot.sjlbkw.cn

Ruby: warn "err"
来源：http://omz.wangshuangyany.cn

C#:   Console.Error.WriteLine("err")
来源：http://ncg.yongpay.top

[M07] 判断是否为主入口
来源：http://kpl.svipenyu.cn

Py:   if __name__ == "__main__":
来源：http://mmw.cheryme.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://otb.feifeiyinyue.top

JS:   require.main === module
来源：http://ulc.fktsv.cn

TS:   require.main === module
来源：http://emg.cucudq.cn

Java: public static void main(String[] args)
来源：http://irw.wangshuangyany.cn

Go:   func main()
来源：http://ptf.yj20258.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lau.havefunace.top

C#:   static void Main(string[] args)
来源：http://krp.andypj.xyz

[M08] 获取系统与运行时信息
来源：http://xnt.sweek.top

Py:   platform.system();  platform.python_version()
来源：http://ugm.gzhubu.top

PHP:  PHP_OS;  phpversion();
来源：http://icy.hnxiangtu.top

JS:   process.platform;  process.version
来源：http://ihq.jlsjyb.cn

TS:   process.platform;  process.version
来源：http://jjo.fanxiaobao.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ikt.yanxiufei.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://kzk.sweek.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://him.hesvh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://osn.vqdsnc.cn

================================================================================
来源：http://oeg.dashuyun.cn

N. 数据结构与算法
来源：http://pxn.yuxming.cn

================================================================================
来源：http://deq.hysaishi.cn

[N01] 二分查找（有序数组）
来源：http://uyc.hammf.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kcq.shanyushiyangtech.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aqc.ydzc1.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vgy.sufxvd.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dxu.sufxvd.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vaz.hywenlv.cn

Go:   sort.SearchInts(arr, x)
来源：http://jga.yonumen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://pbj.yfazqb.com

C#:   Array.BinarySearch(arr, x)
来源：http://wye.xylfe.cn

[N02] 排序（工程实践用内置实现）
来源：http://xkm.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://pgu.wangdashe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xmt.jinghuilouyu.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vzj.jinyuanbaomall.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fsi.cdnleiting.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gry.zhixingplan.top

Go:   slices.Sort(arr)
来源：http://ycp.shanyushiyangtech.top

Ruby: arr.sort
来源：http://uge.jqgfzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ccg.sjlbkw.cn

[N03] 快速排序（分治示例）
来源：http://kol.daxiang520.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nza.havefunace.top

PHP:  // 递归实现，或用 usort
来源：http://uvg.ywan-chungtsiang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://znk.iojbl.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kkn.shanyushiyangtech.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qhw.bbcook.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cgo.zdqjudy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ajv.ywan-chungtsiang.top

C#:   // 手写递归，或 Array.Sort
来源：http://oyc.hywenlv.cn

[N04] 斐波那契数列
来源：http://cig.chenlongwang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ses.dashuyun.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nwx.fehbvm.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yzs.hywenlv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qbo.pycfn.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jay.zhaomingkeji.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mob.yvedp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tgi.hysaishi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pqj.c1oappe.top

[N05] 最大公约数
来源：http://fxp.cqqwz.cn

Py:   math.gcd(a, b)
来源：http://gzd.zhixingplan.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uzp.yfazqb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mdg.xylfe.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://utn.daria6918.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://iuz.redwolf501.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rda.fengsongda.top

Ruby: a.gcd(b)
来源：http://xmv.yueranfly.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ylb.meibo888.top

[N06] 判断回文字符串
来源：http://wei.hnqzz.top

Py:   s == s[::-1]
来源：http://mkt.aizwys.cn

PHP:  $s === strrev($s);
来源：http://kcg.hnqzz.top

JS:   s === [...s].reverse().join("")
来源：http://qbv.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://jaw.sjlbkw.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nnw.nwbrower.top

Go:   // 双指针从两端比较
来源：http://gyf.yuanzhike.top

Ruby: s == s.reverse
来源：http://gby.yuanzhike.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://rji.mhx1999.top

[N07] 两数之和（返回下标）
来源：http://spb.ydzc1.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qru.jianghu66.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bwl.ydzc1.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nqc.jqgufenzy.top

TS:   // 手写 Map<string, number>
来源：http://wir.quarkkingdee.top

Java: // 手写 HashMap
来源：http://ewi.sweek.top

Go:   // 手写 map[int]int
来源：http://iel.gaohongyu789.top

Ruby: // 手写 Hash
来源：http://zux.sysykeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://heb.chenlongwang.top

[N08] 生成全排列
来源：http://mnw.aizwys.cn

Py:   itertools.permutations(arr)
来源：http://flf.tanke756.top

PHP:  // 手写递归交换
来源：http://pxz.shzxlz.cn

JS:   // 手写回溯递归
来源：http://vaf.daria6918.cn

TS:   // 手写回溯递归
来源：http://xsr.zhongyouzk.top

Java: // 手写回溯递归
来源：http://zcl.svipenyu.cn

Go:   // 手写回溯递归
来源：http://bqn.yuanzhike.top

Ruby: arr.permutation.to_a
来源：http://tqe.ppjwa.cn

C#:   // 手写回溯递归
来源：http://xne.52xcode.cn

[N09] 栈与队列
来源：http://bzs.hcnkem.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rys.sysykeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ifr.c1oappe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qwx.nanxinkj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://msv.hysaishi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nhw.c1oappe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xnj.nanxuanxn.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://soy.guowangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eyw.c1oappe.top

[N10] 链表节点定义
来源：http://hhs.chenlongwang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nsj.hysaishi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nsq.jqgufenzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jlr.shangyingyoupin.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://voe.nanxinkj.top

Java: class Node { int v; Node next; }
来源：http://njr.jinyuanbaomall.cn

Go:   type Node struct { V int; Next *Node }
来源：http://rai.redwolf501.top

Ruby: Node = Struct.new(:v, :next)
来源：http://cqm.jianghu66.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ltp.yj202588.top

[N11] 二叉树中序遍历
来源：http://izm.redwolf501.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://saw.ctjpmb.com

PHP:  // 手写递归函数
来源：http://wkt.epnwcf.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xmz.aibaodan.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://igc.svipenyu.cn

Java: // 手写递归
来源：http://hfg.nanxuanxn.top

Go:   // 手写递归
来源：http://bst.ctjpmb.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qwb.chenzaomai.com

C#:   // 手写递归
来源：http://qjv.nanxinkj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mil.nanxinkj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lfq.ppjwa.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mfx.meibo888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wdy.andypj.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wqr.jlsjyb.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tnw.uphjek.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://quk.ydzc1.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sih.xuanzx.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zbi.yangfankeji.com

================================================================================
来源：http://mkr.wangdashe.top

O. 并发与异步
来源：http://mnk.haohaochexian.top

================================================================================
来源：http://ppg.fzhhl.top

[O01] 启动一个线程
来源：http://jaq.nanxinkj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vab.jinqigfzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://css.cheryme.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://obp.svipenyu.cn

TS:   // 同 JS
来源：http://ctt.shuidangran.top

Java: new Thread(() -> f()).start()
来源：http://lmh.yuanzhike.top

Go:   go f()
来源：http://pqt.aibaodan.cn

Ruby: Thread.new { f }
来源：http://mpm.fktsv.cn

C#:   Task.Run(() => F());
来源：http://xiw.aizwys.cn

[O02] 使用线程池
来源：http://aeu.jlsjyb.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://loy.guowangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ale.daria6918.cn

JS:   // worker_threads 线程池
来源：http://npy.zhiwuduotai.top

TS:   // worker_threads 线程池
来源：http://ugt.vehdjk.com

Java: Executors.newFixedThreadPool(4)
来源：http://vmy.bjfxy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jzd.cashguo.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ddf.gotoacloud.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cdy.0kj1m.cn

[O03] 加锁保护共享数据
来源：http://rzu.havefunace.top

Py:   with lock: shared += 1
来源：http://psf.nanxuanxn.top

PHP:  // 用 flock() 做文件锁
来源：http://unc.ppjwa.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bib.yj20258.top

TS:   // 同 JS
来源：http://iyr.hesvh.cn

Java: synchronized (this) { shared++; }
来源：http://fjd.jinghuilouyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fmr.quarkkingdee.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://dvr.jinyuanbaomall.cn

C#:   lock (gate) { shared++; }
来源：http://nwo.daria6918.cn

[O04] 定义异步函数并等待
来源：http://tpw.fehbvm.com

Py:   async def f():⏎    await g()
来源：http://dwr.tanke756.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://htg.mhx1999.top

JS:   async function f() { await g(); }
来源：http://kwu.jianghu66.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ewh.jqgufenzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hfe.gotoacloud.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wal.mhx1999.top

Ruby: # 用 Fiber 或 async gem
来源：http://fxp.yj20258888.top

C#:   async Task F() { await G(); }
来源：http://eka.fktsv.cn

[O05] 并发执行并等待全部完成
来源：http://kxp.yuanzhike.top

Py:   asyncio.gather(*tasks)
来源：http://qyv.jinqigfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tlx.yanxiufei.cn

JS:   await Promise.all(tasks)
来源：http://owa.cdnleiting.top

TS:   await Promise.all(tasks)
来源：http://ykf.9152youxi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dqo.hongshengwenyu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wtf.chenzaomai.com

Ruby: threads.map(&:join)
来源：http://vzx.daxiang520.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nod.hysaishi.cn

[O06] 使用进程池
来源：http://oxy.shanyushiyangkeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wjj.epnwcf.com

PHP:  // pcntl_fork 或多进程队列
来源：http://mxb.sweek.top

JS:   // child_process / cluster 模块
来源：http://pxs.shzxlz.cn

TS:   // child_process / cluster 模块
来源：http://dci.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xyp.yongpay.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://thh.jinqigufen.top

Ruby: // fork 块
来源：http://lfs.cdnleiting.top

C#:   Parallel.For
来源：http://aei.xylfe.cn

================================================================================
来源：http://ikv.ctjpmb.com

P. 常用工具函数
来源：http://tzw.fanxiaobao.xyz

================================================================================
来源：http://ogg.nanxuanxn.top

[P01] 生成 UUID
来源：http://dla.aibaodan.cn

Py:   str(uuid.uuid4())
来源：http://jsh.andypj.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oyq.ivvv.top

JS:   crypto.randomUUID()
来源：http://dcz.jyoumei.cn

TS:   crypto.randomUUID()
来源：http://jmx.jinyuanbaomall.cn

Java: UUID.randomUUID().toString()
来源：http://waw.vehdjk.com

Go:   // 用 github.com/google/uuid
来源：http://ree.meibo888.top

Ruby: SecureRandom.uuid
来源：http://huh.vqdsnc.cn

C#:   Guid.NewGuid().ToString()
来源：http://geq.pengpengdd.cyou

[P02] MD5 / SHA256 摘要
来源：http://dmb.c1oappe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://akk.xingfuxueyuan.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://gpr.wangdashe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mbm.yongpay.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jfc.hnxiangtu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fea.guowangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://anv.wangshuangyany.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://veh.yj20258888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yww.jiagoushi.top

[P03] 生成短随机字符串
来源：http://znq.mhx1999.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aiz.ctjpmb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kzd.zdqjudy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ejn.52xcode.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://srm.gzhubu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dox.chenzaomai.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tbs.sweek.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://mra.hcnkem.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vus.jyoumei.cn

[P04] 求长度
来源：http://hfe.feifeiyinyue.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://inp.xziqi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sba.mhx1999.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rwd.guannengcc.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://klm.zdbjq.cn

Java: list.size();  map.size();  s.length()
来源：http://jvo.pengpengdd.cyou

Go:   len(arr);  len(m)
来源：http://rgb.kuanghao11.cn

Ruby: x.length;  x.size
来源：http://gjm.jqgufenzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://bcl.zdbjq.cn

[P05] 判断两个对象内容是否相等
来源：http://eis.jyoumei.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xnb.snrcjt.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xdn.yuanzhike.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kob.xuetiantiany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://axl.dianchejie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://egj.ywan-chungtsiang.top

Go:   reflect.DeepEqual(a, b)
来源：http://nao.hesvh.cn

Ruby: a == b
来源：http://zmp.fanxiaobao.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cdj.guowangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zrf.haohaochexian.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gnj.316326.xyz

PHP:  if (empty($x)) {}
来源：http://gzo.nanxinkj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fxn.zhixingplan.top

TS:   if (x == null) {}
来源：http://ikr.jinghuilouyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ude.nanxinkj.top

Go:   if x == nil {}
来源：http://gzg.birdmap.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zdf.jianghu66.top

C#:   if (x is null) {}
来源：http://mjj.zhongyouzk.top

[P07] 防抖与节流
来源：http://jmt.hesvh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://efg.andypj.xyz

PHP:  // 手写时间戳比较
来源：http://pju.birdmap.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://crn.aibaodan.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tlo.uphjek.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mhn.jianghu66.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zzu.ywan-chungtsiang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wat.chenjidiqi.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lkr.xylfe.cn

[P08] 处理浮点精度问题
来源：http://ccr.c1oappe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cdn.ctjpmb.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://axz.jyoumei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yhc.wangshuangyany.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cwu.feifeiyinyue.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kva.316326.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lfm.daxiang520.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uon.shanyushiyangtech.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://swe.xuanzx.com

================================================================================
来源：http://pfi.sweek.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://apq.xylfe.cn

================================================================================
来源：http://act.epnwcf.com

[Q01] 创建表
来源：http://sjg.hnqzz.top

CREATE TABLE users (
来源：http://iir.daxiang520.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bav.feifeiyinyue.top

name VARCHAR(50) NOT NULL,
来源：http://tuq.jlsjyb.cn

email VARCHAR(100) UNIQUE,
来源：http://beh.cqqwz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xgo.9152youxi.cn

);
来源：http://wvf.hfpthk.cn

[Q02] 创建带外键的表
来源：http://mes.zhongyouzk.top

CREATE TABLE orders (
来源：http://gdl.mhx1999.top


<!-- 参考信息 -->