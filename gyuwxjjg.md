代发 wailian999

TS:   process.cwd()
来源：http://qoh.nanxuanxn.top

Java: Path.of("").toAbsolutePath()
来源：http://nxg.pycfn.com

Go:   os.Getwd()
来源：http://esg.nwbrower.top

Ruby: Dir.pwd
来源：http://vpm.hesvh.cn

C#:   Directory.GetCurrentDirectory()
来源：http://vhu.jinyuanbaomall.cn

[M05] 设置退出码
来源：http://qap.havefunace.top

Py:   sys.exit(1)
来源：http://qvr.shzxlz.cn

PHP:  exit(1);
来源：http://xld.ydzc1.top

JS:   process.exit(1)
来源：http://lrn.yueranfly.top

TS:   process.exit(1)
来源：http://jxb.zhongyouzk.top

Java: System.exit(1)
来源：http://wrn.iojbl.cn

Go:   os.Exit(1)
来源：http://ajf.0kj1m.cn

Ruby: exit 1
来源：http://lby.gotoacloud.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fbj.hywenlv.cn

[M06] 向标准错误输出
来源：http://iyv.shuidangran.top

Py:   print("err", file=sys.stderr)
来源：http://dup.shzxlz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fdt.tarul.cn

JS:   console.error("err")
来源：http://rei.feifeiyinyue.top

TS:   console.error("err")
来源：http://qat.yangfankeji.com

Java: System.err.println("err")
来源：http://kld.gotoacloud.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ntv.nanxinkj.top

Ruby: warn "err"
来源：http://gvo.daxiang520.top

C#:   Console.Error.WriteLine("err")
来源：http://vgs.zhengqikj.top

[M07] 判断是否为主入口
来源：http://nvw.hnqzz.top

Py:   if __name__ == "__main__":
来源：http://qxg.ybcxt.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mes.aibaodan.cn

JS:   require.main === module
来源：http://pek.smart0.xyz

TS:   require.main === module
来源：http://dak.zhijiandao.cn

Java: public static void main(String[] args)
来源：http://ojf.jinqigfzy.top

Go:   func main()
来源：http://oua.vehdjk.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rpw.ehwqpu.com

C#:   static void Main(string[] args)
来源：http://qnt.yj20258888.top

[M08] 获取系统与运行时信息
来源：http://ipx.sweek.top

Py:   platform.system();  platform.python_version()
来源：http://yof.dashuyun.cn

PHP:  PHP_OS;  phpversion();
来源：http://vhk.xylfe.cn

JS:   process.platform;  process.version
来源：http://rdz.vehdjk.com

TS:   process.platform;  process.version
来源：http://gfh.fengsongda.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qpt.xingfuxueyuan.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://skc.jinqigufen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bmh.shangyingyoupin.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jls.xylfe.cn

================================================================================
来源：http://jgd.hesvh.cn

N. 数据结构与算法
来源：http://jtu.cucudq.cn

================================================================================
来源：http://mrk.shangyingyoupin.top

[N01] 二分查找（有序数组）
来源：http://foi.xuanzx.com

Py:   bisect.bisect_left(arr, x)
来源：http://mnq.yuxming.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ita.fengsongda.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jua.redwolf501.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://adx.zhixingplan.top

Java: Arrays.binarySearch(arr, x)
来源：http://bth.zhoulong.xyz

Go:   sort.SearchInts(arr, x)
来源：http://huw.yanxiufei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wxy.ehwqpu.com

C#:   Array.BinarySearch(arr, x)
来源：http://pvi.yuxming.cn

[N02] 排序（工程实践用内置实现）
来源：http://kyp.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://rus.tian-w.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zuc.kuanghao11.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zpm.meibo888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pur.vehdjk.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ckm.sufxvd.cn

Go:   slices.Sort(arr)
来源：http://rwl.gaohongyu789.top

Ruby: arr.sort
来源：http://tye.shanyushiyangkeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xtz.daxiang520.top

[N03] 快速排序（分治示例）
来源：http://kth.jqgfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rfs.ydzc1.top

PHP:  // 递归实现，或用 usort
来源：http://mfd.zycfv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pkl.sjlbkw.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://znk.vehdjk.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xhc.yj20258.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://aqr.yanxiufei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rnk.52xcode.cn

C#:   // 手写递归，或 Array.Sort
来源：http://dwd.hysaishi.cn

[N04] 斐波那契数列
来源：http://fbc.zhaomingkeji.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uje.gogol.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pqq.chenzaomai.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dhi.yonumen.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://skj.zhongyouzk.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wxh.sjlbkw.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yvy.yueranfly.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://grn.vqdsnc.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wfm.jiagoushi.top

[N05] 最大公约数
来源：http://njd.ydzc1.top

Py:   math.gcd(a, b)
来源：http://zgi.zycfv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gye.yj202588.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://crt.yonumen.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fxa.ctjpmb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cjg.nwbrower.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://psf.tanke756.top

Ruby: a.gcd(b)
来源：http://gnn.yfazqb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dyw.dianchejie.cn

[N06] 判断回文字符串
来源：http://omp.tarul.cn

Py:   s == s[::-1]
来源：http://scj.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://mth.52xcode.cn

JS:   s === [...s].reverse().join("")
来源：http://uei.zhijiandao.cn

TS:   s === [...s].reverse().join("")
来源：http://xqe.jqgfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ufe.gotoacloud.top

Go:   // 双指针从两端比较
来源：http://yth.pycfn.com

Ruby: s == s.reverse
来源：http://cfd.hywenlv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uie.sweek.top

[N07] 两数之和（返回下标）
来源：http://jxt.ybcxt.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://avf.snrcjt.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dzm.hysaishi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://mar.tianlin.xyz

TS:   // 手写 Map<string, number>
来源：http://lal.jiagoushi.top

Java: // 手写 HashMap
来源：http://jez.vqdsnc.cn

Go:   // 手写 map[int]int
来源：http://jto.jlsjyb.cn

Ruby: // 手写 Hash
来源：http://ipa.uphjek.com

C#:   // 手写 Dictionary<int, int>
来源：http://tbn.yj20258.top

[N08] 生成全排列
来源：http://dkr.0kj1m.cn

Py:   itertools.permutations(arr)
来源：http://dru.guannengcc.top

PHP:  // 手写递归交换
来源：http://afl.xinyue.icu

JS:   // 手写回溯递归
来源：http://pdd.shanyushiyangkeji.top

TS:   // 手写回溯递归
来源：http://but.iojbl.cn

Java: // 手写回溯递归
来源：http://rsk.shanyushiyangkeji.top

Go:   // 手写回溯递归
来源：http://blb.mhx1999.top

Ruby: arr.permutation.to_a
来源：http://bnk.ppjwa.cn

C#:   // 手写回溯递归
来源：http://dml.haohaochexian.top

[N09] 栈与队列
来源：http://rbt.sysykeji.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://brs.hfpthk.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://euc.haohaochexian.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gdi.quarkkingdee.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kxx.haohaochexian.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nvi.fzhhl.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lkn.fehbvm.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://adz.jianghu66.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ogd.ywan-chungtsiang.top

[N10] 链表节点定义
来源：http://wad.bjfxy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://irt.shanyushiyangtech.top

PHP:  class Node { public $v; public $next = null; }
来源：http://fdl.yonumen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tcm.ppjwa.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://idl.smart0.xyz

Java: class Node { int v; Node next; }
来源：http://rnh.smart0.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://mvo.gogol.net.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://qeu.jyoumei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://eiq.bbcook.cn

[N11] 二叉树中序遍历
来源：http://huw.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zlg.c1oappe.top

PHP:  // 手写递归函数
来源：http://vof.ydjk.org.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iyh.gaohongyu789.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://thv.yangfankeji.com

Java: // 手写递归
来源：http://llu.jinqigfzy.top

Go:   // 手写递归
来源：http://kdp.yongpay.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zjb.andypj.xyz

C#:   // 手写递归
来源：http://gqt.nanxinkj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pjg.hnxiangtu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zun.yj202588.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ygs.yuanzhike.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ool.ctjpmb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ibc.gogol.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ejz.snrcjt.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ifu.iojbl.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://noa.jinghuilouyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iwc.52xcode.cn

================================================================================
来源：http://kly.cheryme.top

O. 并发与异步
来源：http://rke.yfazqb.com

================================================================================
来源：http://zsy.uphjek.com

[O01] 启动一个线程
来源：http://yhe.cheryme.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sbg.vehdjk.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mwe.ppjwa.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hcv.pycfn.com

TS:   // 同 JS
来源：http://xek.xziqi.cn

Java: new Thread(() -> f()).start()
来源：http://ors.nanxuanxn.top

Go:   go f()
来源：http://nza.cdnleiting.top

Ruby: Thread.new { f }
来源：http://rzt.hongshengwenyu.top

C#:   Task.Run(() => F());
来源：http://qzv.yj20258888.top

[O02] 使用线程池
来源：http://ryx.zhijiandao.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ojf.cdnleiting.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lyg.snrcjt.cn

JS:   // worker_threads 线程池
来源：http://pnt.chenlongwang.top

TS:   // worker_threads 线程池
来源：http://zqv.dianchejie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jlc.bjfxy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ini.cdnleiting.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tgt.bjfxy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ldi.haohaochexian.top

[O03] 加锁保护共享数据
来源：http://mib.daxiang520.top

Py:   with lock: shared += 1
来源：http://jvd.yanxiufei.cn

PHP:  // 用 flock() 做文件锁
来源：http://ahk.hcnkem.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rjo.fengsongda.top

TS:   // 同 JS
来源：http://vdo.pycfn.com

Java: synchronized (this) { shared++; }
来源：http://ezr.chenlongwang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nxm.jyoumei.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://dou.zhoulong.xyz

C#:   lock (gate) { shared++; }
来源：http://kzs.hongshengwenyu.top

[O04] 定义异步函数并等待
来源：http://aoy.zhiwuduotai.top

Py:   async def f():⏎    await g()
来源：http://bco.epnwcf.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nfn.iojbl.cn

JS:   async function f() { await g(); }
来源：http://ppk.cheryme.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dzi.gogol.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://igs.hcnkem.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zxz.yanxiufei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://des.hfpthk.cn

C#:   async Task F() { await G(); }
来源：http://ftt.sweek.top

[O05] 并发执行并等待全部完成
来源：http://igy.shzxlz.cn

Py:   asyncio.gather(*tasks)
来源：http://yim.jinyuanbaomall.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pkp.0kj1m.cn

JS:   await Promise.all(tasks)
来源：http://oic.xinyue.icu

TS:   await Promise.all(tasks)
来源：http://tos.0kj1m.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xxx.9152youxi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wcx.yj20258888.top

Ruby: threads.map(&:join)
来源：http://glf.birdmap.top

C#:   await Task.WhenAll(t1, t2)
来源：http://yos.tarul.cn

[O06] 使用进程池
来源：http://wdr.feifeiyinyue.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://unp.cheryme.top

PHP:  // pcntl_fork 或多进程队列
来源：http://gjt.gotoacloud.top

JS:   // child_process / cluster 模块
来源：http://mxd.hysaishi.cn

TS:   // child_process / cluster 模块
来源：http://yae.vqdsnc.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rsy.jinqigfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wwr.fanxiaobao.xyz

Ruby: // fork 块
来源：http://xgn.jiagoushi.top

C#:   Parallel.For
来源：http://rpl.pengpengdd.cyou

================================================================================
来源：http://wdb.daxiang520.top

P. 常用工具函数
来源：http://xfg.zhixingplan.top

================================================================================
来源：http://skk.nwbrower.top

[P01] 生成 UUID
来源：http://yhi.shanyushiyangtech.top

Py:   str(uuid.uuid4())
来源：http://wmg.gaohongyu789.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://otg.jinyuanbaomall.cn

JS:   crypto.randomUUID()
来源：http://whi.quarkkingdee.top

TS:   crypto.randomUUID()
来源：http://vxx.hywenlv.cn

Java: UUID.randomUUID().toString()
来源：http://rpu.wangshuangyany.cn

Go:   // 用 github.com/google/uuid
来源：http://lxg.guannengcc.top

Ruby: SecureRandom.uuid
来源：http://jtv.xuetiantiany.cn

C#:   Guid.NewGuid().ToString()
来源：http://xhm.gogol.net.cn

[P02] MD5 / SHA256 摘要
来源：http://kzx.dashuyun.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zfw.gaohongyu789.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xcc.yangfankeji.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zip.ctjpmb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bhd.zhoulong.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tdn.vehdjk.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ypd.dianchejie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pyu.hysaishi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lnb.sysykeji.top

[P03] 生成短随机字符串
来源：http://mmj.hnxiangtu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mqw.yueranfly.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zpd.xinyue.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oww.aizwys.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zqe.yj20258888.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gnh.fzhhl.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ial.jqgufenzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://jyq.iojbl.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yfr.jqgufenzy.top

[P04] 求长度
来源：http://yyd.ppjwa.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://obw.andypj.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tmh.zycfv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rzr.shuidangran.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://znc.yuanzhike.top

Java: list.size();  map.size();  s.length()
来源：http://ufw.yfazqb.com

Go:   len(arr);  len(m)
来源：http://ecu.wangdashe.top

Ruby: x.length;  x.size
来源：http://rvq.chenzaomai.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://wzv.fanxiaobao.xyz

[P05] 判断两个对象内容是否相等
来源：http://wrz.yuxming.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ivt.ehwqpu.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://csg.hcnkem.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sww.shanyushiyangkeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bvp.xingfuxueyuan.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ycu.mhx1999.top

Go:   reflect.DeepEqual(a, b)
来源：http://axr.nanxuanxn.top

Ruby: a == b
来源：http://ncj.gaohongyu789.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://faq.sjlbkw.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ukd.xinyue.icu

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hed.mhx1999.top

PHP:  if (empty($x)) {}
来源：http://eoj.dashuyun.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nrj.zhaomingkeji.xyz

TS:   if (x == null) {}
来源：http://oma.yj20258888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ghh.vqdsnc.cn

Go:   if x == nil {}
来源：http://swa.yanxiufei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ilh.jlsjyb.cn

C#:   if (x is null) {}
来源：http://jtk.wangdashe.top

[P07] 防抖与节流
来源：http://xsj.zhongyouzk.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://btc.tian-w.cn

PHP:  // 手写时间戳比较
来源：http://sos.xingfuxueyuan.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://llu.xingfuxueyuan.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pwi.nwbrower.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dib.sweek.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xcw.redwolf501.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gsm.yj20258.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ygp.hywenlv.cn

[P08] 处理浮点精度问题
来源：http://qvn.hnqzz.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dwy.xinyue.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ubq.xuanzx.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hek.gotoacloud.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lpb.ppjwa.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://big.yueranfly.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cbi.redwolf501.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wlj.hesvh.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nlo.yongpay.top

================================================================================
来源：http://qxc.316326.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wun.xingfuxueyuan.xyz

================================================================================
来源：http://zcn.ydjk.org.cn

[Q01] 创建表
来源：http://wrd.gaohongyu789.top

CREATE TABLE users (
来源：http://iuj.sysykeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ojf.c1oappe.top

name VARCHAR(50) NOT NULL,
来源：http://qeu.jinyuanbaomall.cn

email VARCHAR(100) UNIQUE,
来源：http://lpo.ehwqpu.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ryh.yangfankeji.com

);
来源：http://ljy.hfpthk.cn

[Q02] 创建带外键的表
来源：http://pnm.ppjwa.cn

CREATE TABLE orders (
来源：http://zyv.zhixingplan.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kuf.sufxvd.cn

user_id INT NOT NULL,
来源：http://has.ydjk.org.cn

amount DECIMAL(10, 2),
来源：http://xum.jlsjyb.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://owe.shangyingyoupin.top


<!-- 参考信息 -->