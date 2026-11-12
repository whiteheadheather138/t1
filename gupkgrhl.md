代发 wailian999

[M04] 获取当前工作目录
来源：http://mwc.nanxinkj.top

Py:   os.getcwd()
来源：http://keg.wangshuangyany.cn

PHP:  getcwd();
来源：http://oux.zhixingplan.top

JS:   process.cwd()
来源：http://duf.jinqigfzy.top

TS:   process.cwd()
来源：http://hfs.zycfv.cn

Java: Path.of("").toAbsolutePath()
来源：http://bgp.daxiang520.top

Go:   os.Getwd()
来源：http://wvq.bjfxy.top

Ruby: Dir.pwd
来源：http://thq.jqgufenzy.top

C#:   Directory.GetCurrentDirectory()
来源：http://iqi.hnqzz.top

[M05] 设置退出码
来源：http://ofv.epnwcf.com

Py:   sys.exit(1)
来源：http://nmz.vehdjk.com

PHP:  exit(1);
来源：http://gbl.redwolf501.top

JS:   process.exit(1)
来源：http://zhy.shuidangran.top

TS:   process.exit(1)
来源：http://rcc.sufxvd.cn

Java: System.exit(1)
来源：http://hcf.mhx1999.top

Go:   os.Exit(1)
来源：http://fwo.quarkkingdee.top

Ruby: exit 1
来源：http://dxm.fengsongda.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rsl.xinyue.icu

[M06] 向标准错误输出
来源：http://vxa.yj20258888.top

Py:   print("err", file=sys.stderr)
来源：http://dov.aibaodan.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zrb.chenjidiqi.icu

JS:   console.error("err")
来源：http://bby.yanxiufei.cn

TS:   console.error("err")
来源：http://fda.0kj1m.cn

Java: System.err.println("err")
来源：http://wnt.zhixingplan.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lqu.sjlbkw.cn

Ruby: warn "err"
来源：http://ead.hammf.cn

C#:   Console.Error.WriteLine("err")
来源：http://axt.chenlongwang.top

[M07] 判断是否为主入口
来源：http://gej.nwbrower.top

Py:   if __name__ == "__main__":
来源：http://gbn.ydjk.org.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ljy.xziqi.cn

JS:   require.main === module
来源：http://lom.316326.xyz

TS:   require.main === module
来源：http://qbf.yvedp.cn

Java: public static void main(String[] args)
来源：http://lsy.hnqzz.top

Go:   func main()
来源：http://ahc.hnxiangtu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://asf.yangfankeji.com

C#:   static void Main(string[] args)
来源：http://yni.hongshengwenyu.top

[M08] 获取系统与运行时信息
来源：http://csq.nanxuanxn.top

Py:   platform.system();  platform.python_version()
来源：http://ore.zycfv.cn

PHP:  PHP_OS;  phpversion();
来源：http://fxf.vehdjk.com

JS:   process.platform;  process.version
来源：http://ahi.tanke756.top

TS:   process.platform;  process.version
来源：http://zjf.gotoacloud.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lbb.nwbrower.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://fmh.yuxming.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kmr.yfazqb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://eif.vehdjk.com

================================================================================
来源：http://ofi.yangfankeji.com

N. 数据结构与算法
来源：http://kpb.uphjek.com

================================================================================
来源：http://cna.shuidangran.top

[N01] 二分查找（有序数组）
来源：http://ecq.52xcode.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ovs.jinyuanbaomall.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tnb.smart0.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://osu.yonumen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hls.aibaodan.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kkg.jiagoushi.top

Go:   sort.SearchInts(arr, x)
来源：http://ppg.yuxming.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qqh.shuidangran.top

C#:   Array.BinarySearch(arr, x)
来源：http://gsh.jlsjyb.cn

[N02] 排序（工程实践用内置实现）
来源：http://ckm.wangshuangyany.cn

Py:   sorted(arr);  arr.sort()
来源：http://olw.jyoumei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gki.jiagoushi.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://jbs.jlsjyb.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kfd.nanxuanxn.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://znz.hfpthk.cn

Go:   slices.Sort(arr)
来源：http://kxb.316326.xyz

Ruby: arr.sort
来源：http://kkd.redwolf501.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://oyt.c1oappe.top

[N03] 快速排序（分治示例）
来源：http://gca.dashuyun.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ztl.jianghu66.top

PHP:  // 递归实现，或用 usort
来源：http://ugz.hnqzz.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ljp.sufxvd.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mpr.fengsongda.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ndm.jianghu66.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qrt.yangfankeji.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yke.sysykeji.top

C#:   // 手写递归，或 Array.Sort
来源：http://bkb.jiagoushi.top

[N04] 斐波那契数列
来源：http://uvp.shzxlz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xvz.aibaodan.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qtx.xinyue.icu

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cpv.jinghuilouyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yko.yj20258888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kbc.hywenlv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://umt.nanxuanxn.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qbh.guowangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cxu.snrcjt.cn

[N05] 最大公约数
来源：http://srd.aizwys.cn

Py:   math.gcd(a, b)
来源：http://izz.yj20258.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bfw.zdqjudy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xcv.yj20258888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ukf.feifeiyinyue.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gvd.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pyb.hesvh.cn

Ruby: a.gcd(b)
来源：http://oyf.yueranfly.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nyd.zhongyouzk.top

[N06] 判断回文字符串
来源：http://mez.zhiwuduotai.top

Py:   s == s[::-1]
来源：http://zqj.bjfxy.top

PHP:  $s === strrev($s);
来源：http://ink.shzxlz.cn

JS:   s === [...s].reverse().join("")
来源：http://ujw.svipenyu.cn

TS:   s === [...s].reverse().join("")
来源：http://gpt.fktsv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ckj.jinqigfzy.top

Go:   // 双指针从两端比较
来源：http://xwm.jiagoushi.top

Ruby: s == s.reverse
来源：http://lwa.meibo888.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ywn.hnqzz.top

[N07] 两数之和（返回下标）
来源：http://slx.0kj1m.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lut.xingfuxueyuan.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rkq.andypj.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://dxf.guowangkeji.top

TS:   // 手写 Map<string, number>
来源：http://aor.aibaodan.cn

Java: // 手写 HashMap
来源：http://edg.fengsongda.top

Go:   // 手写 map[int]int
来源：http://bdt.kuanghao11.cn

Ruby: // 手写 Hash
来源：http://qzu.cheryme.top

C#:   // 手写 Dictionary<int, int>
来源：http://gsy.shuidangran.top

[N08] 生成全排列
来源：http://gzh.hfpthk.cn

Py:   itertools.permutations(arr)
来源：http://npp.yongpay.top

PHP:  // 手写递归交换
来源：http://qyp.cdnleiting.top

JS:   // 手写回溯递归
来源：http://cmp.jinqigufen.top

TS:   // 手写回溯递归
来源：http://rwj.cqqwz.cn

Java: // 手写回溯递归
来源：http://xhd.wangshuangyany.cn

Go:   // 手写回溯递归
来源：http://sgg.jianghu66.top

Ruby: arr.permutation.to_a
来源：http://rpl.zhiwuduotai.top

C#:   // 手写回溯递归
来源：http://mvr.nanxuanxn.top

[N09] 栈与队列
来源：http://awp.tarul.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://akm.zhaomingkeji.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tyj.cqqwz.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ifz.yonumen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://lfn.ppjwa.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tjr.sufxvd.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qak.ybcxt.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mud.hysaishi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tmk.shangyingyoupin.top

[N10] 链表节点定义
来源：http://unn.shangyingyoupin.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://akz.ctjpmb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://brs.gaohongyu789.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ezi.tarul.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kju.jinghuilouyu.cn

Java: class Node { int v; Node next; }
来源：http://jim.cheryme.top

Go:   type Node struct { V int; Next *Node }
来源：http://vla.smart0.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://qiz.redwolf501.top

C#:   class Node { public int V; public Node? Next; }
来源：http://sqo.pycfn.com

[N11] 二叉树中序遍历
来源：http://orw.zhaomingkeji.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://chy.fanxiaobao.xyz

PHP:  // 手写递归函数
来源：http://kfs.shangyingyoupin.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://puv.jinqigufen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nrj.wangdashe.top

Java: // 手写递归
来源：http://ebx.cashguo.top

Go:   // 手写递归
来源：http://zpo.gaohongyu789.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nau.shzxlz.cn

C#:   // 手写递归
来源：http://meq.jinqigfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://uvn.cheryme.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uvj.yj202588.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jgq.fanxiaobao.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://usn.jinqigfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ttg.hesvh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iao.ywan-chungtsiang.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kds.0kj1m.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ieg.gotoacloud.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ugy.pycfn.com

================================================================================
来源：http://eez.jinyuanbaomall.cn

O. 并发与异步
来源：http://dnh.jlsjyb.cn

================================================================================
来源：http://tll.cdnleiting.top

[O01] 启动一个线程
来源：http://vwb.9152youxi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://yxr.hammf.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://euk.pycfn.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://krn.daxiang520.top

TS:   // 同 JS
来源：http://phq.cashguo.top

Java: new Thread(() -> f()).start()
来源：http://xyw.daxiang520.top

Go:   go f()
来源：http://bol.yueranfly.top

Ruby: Thread.new { f }
来源：http://caq.smart0.xyz

C#:   Task.Run(() => F());
来源：http://pfc.fktsv.cn

[O02] 使用线程池
来源：http://gxg.shuidangran.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://auu.daxiang520.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tha.daxiang520.top

JS:   // worker_threads 线程池
来源：http://zbn.hywenlv.cn

TS:   // worker_threads 线程池
来源：http://wmb.jinqigfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://yfx.vqdsnc.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xwf.dashuyun.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gyz.chenlongwang.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gfl.jinqigfzy.top

[O03] 加锁保护共享数据
来源：http://jij.gotoacloud.top

Py:   with lock: shared += 1
来源：http://eqg.pengpengdd.cyou

PHP:  // 用 flock() 做文件锁
来源：http://enn.nwbrower.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mjq.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://pdt.hywenlv.cn

Java: synchronized (this) { shared++; }
来源：http://ydb.aizwys.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lsr.shanyushiyangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://gdh.svipenyu.cn

C#:   lock (gate) { shared++; }
来源：http://spr.chenjidiqi.icu

[O04] 定义异步函数并等待
来源：http://and.cheryme.top

Py:   async def f():⏎    await g()
来源：http://ooy.shanyushiyangtech.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zyj.shanyushiyangkeji.top

JS:   async function f() { await g(); }
来源：http://gcu.haohaochexian.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://eju.ivvv.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ohi.hnxiangtu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ucp.dianchejie.cn

Ruby: # 用 Fiber 或 async gem
来源：http://twm.pycfn.com

C#:   async Task F() { await G(); }
来源：http://dhh.yuanzhike.top

[O05] 并发执行并等待全部完成
来源：http://drt.hywenlv.cn

Py:   asyncio.gather(*tasks)
来源：http://rhv.cucudq.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://aro.vqdsnc.cn

JS:   await Promise.all(tasks)
来源：http://rcb.vehdjk.com

TS:   await Promise.all(tasks)
来源：http://rre.svipenyu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qvw.cheryme.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ins.bbcook.cn

Ruby: threads.map(&:join)
来源：http://mls.shanyushiyangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://wtp.xylfe.cn

[O06] 使用进程池
来源：http://usw.hnxiangtu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lxg.yfazqb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://gie.zhiwuduotai.top

JS:   // child_process / cluster 模块
来源：http://nqh.sjlbkw.cn

TS:   // child_process / cluster 模块
来源：http://ycj.smart0.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iwi.0kj1m.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tph.ctjpmb.com

Ruby: // fork 块
来源：http://bnp.birdmap.top

C#:   Parallel.For
来源：http://wsk.shangyingyoupin.top

================================================================================
来源：http://lvw.yj20258.top

P. 常用工具函数
来源：http://uma.gogol.net.cn

================================================================================
来源：http://hgp.tian-w.cn

[P01] 生成 UUID
来源：http://yfw.havefunace.top

Py:   str(uuid.uuid4())
来源：http://xao.fehbvm.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ful.hnqzz.top

JS:   crypto.randomUUID()
来源：http://ogf.xuetiantiany.cn

TS:   crypto.randomUUID()
来源：http://kxu.aizwys.cn

Java: UUID.randomUUID().toString()
来源：http://buy.tianlin.xyz

Go:   // 用 github.com/google/uuid
来源：http://ktn.tianlin.xyz

Ruby: SecureRandom.uuid
来源：http://dkd.dashuyun.cn

C#:   Guid.NewGuid().ToString()
来源：http://fpv.yonumen.top

[P02] MD5 / SHA256 摘要
来源：http://etm.ydzc1.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rll.sweek.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qil.hnqzz.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wzc.shanyushiyangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eqq.fktsv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sxp.dianchejie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wgw.epnwcf.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qsb.aibaodan.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nlb.redwolf501.top

[P03] 生成短随机字符串
来源：http://ihc.chenjidiqi.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hnz.hfpthk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jdd.yj202588.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vdv.gogol.net.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cne.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jzh.cashguo.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://aku.ivvv.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://snr.c1oappe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://amk.chenlongwang.top

[P04] 求长度
来源：http://jae.feifeiyinyue.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://grg.fzhhl.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nex.sufxvd.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vup.hesvh.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nmk.pengpengdd.cyou

Java: list.size();  map.size();  s.length()
来源：http://eos.shzxlz.cn

Go:   len(arr);  len(m)
来源：http://dji.hfpthk.cn

Ruby: x.length;  x.size
来源：http://wzw.yueranfly.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://crn.yonumen.top

[P05] 判断两个对象内容是否相等
来源：http://nao.cheryme.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://qrk.wangdashe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qxn.fanxiaobao.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://khr.jqgufenzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cxx.jinqigufen.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qlq.guowangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://rzv.hnxiangtu.top

Ruby: a == b
来源：http://wjv.pengpengdd.cyou

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eac.jinghuilouyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qsh.xuanzx.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qwf.fengsongda.top

PHP:  if (empty($x)) {}
来源：http://nxd.snrcjt.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iyy.0kj1m.cn

TS:   if (x == null) {}
来源：http://zic.xylfe.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://elq.daxiang520.top

Go:   if x == nil {}
来源：http://mzr.gzhubu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vws.zhiwuduotai.top

C#:   if (x is null) {}
来源：http://nhd.chenjidiqi.icu

[P07] 防抖与节流
来源：http://qmh.jiagoushi.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wtm.zycfv.cn

PHP:  // 手写时间戳比较
来源：http://aww.dianchejie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uht.ppjwa.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://edl.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://llt.hnqzz.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sze.jiagoushi.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hay.jlsjyb.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sdx.shzxlz.cn

[P08] 处理浮点精度问题
来源：http://gqv.yonumen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pwa.zhongyouzk.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lwn.svipenyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nre.nanxuanxn.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rqz.xuetiantiany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ybt.cdnleiting.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://unn.dianchejie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ocp.jqgfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yrp.xinyue.icu

================================================================================
来源：http://ird.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://isj.52xcode.cn

================================================================================
来源：http://aun.yfazqb.com

[Q01] 创建表
来源：http://ecf.smart0.xyz

CREATE TABLE users (
来源：http://nvr.ydzc1.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ish.fengsongda.top

name VARCHAR(50) NOT NULL,
来源：http://syu.epnwcf.com

email VARCHAR(100) UNIQUE,
来源：http://fdx.hammf.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://grm.yuanzhike.top

);
来源：http://icp.meibo888.top

[Q02] 创建带外键的表
来源：http://jxt.fengsongda.top

CREATE TABLE orders (
来源：http://afg.316326.xyz


<!-- 参考信息 -->