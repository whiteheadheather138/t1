代发 wailian999

[M04] 获取当前工作目录
来源：http://etx.zhixingplan.top

Py:   os.getcwd()
来源：http://twf.shzxlz.cn

PHP:  getcwd();
来源：http://wtb.cdnleiting.top

JS:   process.cwd()
来源：http://ygg.ctjpmb.com

TS:   process.cwd()
来源：http://nxv.zdqjudy.top

Java: Path.of("").toAbsolutePath()
来源：http://naf.yj20258.top

Go:   os.Getwd()
来源：http://saf.bbcook.cn

Ruby: Dir.pwd
来源：http://nca.hysaishi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://iqx.fengsongda.top

[M05] 设置退出码
来源：http://qfo.yonumen.top

Py:   sys.exit(1)
来源：http://kpu.shzxlz.cn

PHP:  exit(1);
来源：http://zzp.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://dsf.hnxiangtu.top

TS:   process.exit(1)
来源：http://xay.cucudq.cn

Java: System.exit(1)
来源：http://gml.ivvv.top

Go:   os.Exit(1)
来源：http://jqi.yj202588.top

Ruby: exit 1
来源：http://kxu.shanyushiyangtech.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xcg.zhoulong.xyz

[M06] 向标准错误输出
来源：http://qho.guannengcc.top

Py:   print("err", file=sys.stderr)
来源：http://lge.nanxuanxn.top

PHP:  fwrite(STDERR, "err\n");
来源：http://cju.xylfe.cn

JS:   console.error("err")
来源：http://uyx.hywenlv.cn

TS:   console.error("err")
来源：http://ebv.yfazqb.com

Java: System.err.println("err")
来源：http://xqt.jinyuanbaomall.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ego.ywan-chungtsiang.top

Ruby: warn "err"
来源：http://uza.jlsjyb.cn

C#:   Console.Error.WriteLine("err")
来源：http://cnu.zhoulong.xyz

[M07] 判断是否为主入口
来源：http://xly.xuanzx.com

Py:   if __name__ == "__main__":
来源：http://tci.yongpay.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rlr.tarul.cn

JS:   require.main === module
来源：http://mpg.wangdashe.top

TS:   require.main === module
来源：http://lxf.jyoumei.cn

Java: public static void main(String[] args)
来源：http://vob.ppjwa.cn

Go:   func main()
来源：http://xpx.xingfuxueyuan.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sgr.jinqigufen.top

C#:   static void Main(string[] args)
来源：http://kpm.xziqi.cn

[M08] 获取系统与运行时信息
来源：http://vit.nanxinkj.top

Py:   platform.system();  platform.python_version()
来源：http://jzn.hfpthk.cn

PHP:  PHP_OS;  phpversion();
来源：http://fct.gogol.net.cn

JS:   process.platform;  process.version
来源：http://hqw.zhaomingkeji.xyz

TS:   process.platform;  process.version
来源：http://kiw.yongpay.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bcs.sweek.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ryi.guowangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hqa.yuanzhike.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vte.nwbrower.top

================================================================================
来源：http://pyd.hammf.cn

N. 数据结构与算法
来源：http://hmn.pycfn.com

================================================================================
来源：http://deo.jinqigufen.top

[N01] 二分查找（有序数组）
来源：http://eju.hywenlv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pbw.mhx1999.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lic.yj20258.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dvd.sufxvd.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ivi.fanxiaobao.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://qjz.shanyushiyangtech.top

Go:   sort.SearchInts(arr, x)
来源：http://paa.yj20258888.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://jgf.pengpengdd.cyou

C#:   Array.BinarySearch(arr, x)
来源：http://vpj.shuidangran.top

[N02] 排序（工程实践用内置实现）
来源：http://cwu.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://ozn.0kj1m.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wlm.quarkkingdee.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://sjz.feifeiyinyue.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cxb.jinqigfzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://smj.snrcjt.cn

Go:   slices.Sort(arr)
来源：http://lgg.zhiwuduotai.top

Ruby: arr.sort
来源：http://bgc.fengsongda.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://sik.hongshengwenyu.top

[N03] 快速排序（分治示例）
来源：http://htl.fengsongda.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vid.jqgfzy.top

PHP:  // 递归实现，或用 usort
来源：http://pzj.xziqi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xed.hfpthk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hib.ydzc1.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qch.316326.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zxq.nanxuanxn.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qka.aibaodan.cn

C#:   // 手写递归，或 Array.Sort
来源：http://fgx.shzxlz.cn

[N04] 斐波那契数列
来源：http://tqc.zdbjq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gpp.wangdashe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ald.daxiang520.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kbc.vqdsnc.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kch.yj20258.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rct.sweek.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://why.shuidangran.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dwg.hysaishi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zle.svipenyu.cn

[N05] 最大公约数
来源：http://lnm.yj20258888.top

Py:   math.gcd(a, b)
来源：http://ftc.dianchejie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wup.sweek.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lbd.sweek.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rdv.nanxuanxn.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dlb.vehdjk.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rdy.smart0.xyz

Ruby: a.gcd(b)
来源：http://mhi.zhoulong.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uzv.sufxvd.cn

[N06] 判断回文字符串
来源：http://jin.guannengcc.top

Py:   s == s[::-1]
来源：http://ful.hysaishi.cn

PHP:  $s === strrev($s);
来源：http://hgy.fanxiaobao.xyz

JS:   s === [...s].reverse().join("")
来源：http://lxb.bbcook.cn

TS:   s === [...s].reverse().join("")
来源：http://qhd.hfpthk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sgr.dashuyun.cn

Go:   // 双指针从两端比较
来源：http://kzf.sxryk.cn

Ruby: s == s.reverse
来源：http://gyk.9152youxi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://blq.ybcxt.top

[N07] 两数之和（返回下标）
来源：http://tjt.jqgfzy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pmr.yuxming.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vse.wangdashe.top

JS:   // 手写 Map：map.set(v, i)
来源：http://fpp.epnwcf.com

TS:   // 手写 Map<string, number>
来源：http://pma.hammf.cn

Java: // 手写 HashMap
来源：http://mjo.jiagoushi.top

Go:   // 手写 map[int]int
来源：http://xiu.fanxiaobao.xyz

Ruby: // 手写 Hash
来源：http://pka.fktsv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zer.yonumen.top

[N08] 生成全排列
来源：http://cxn.zdbjq.cn

Py:   itertools.permutations(arr)
来源：http://uvi.xylfe.cn

PHP:  // 手写递归交换
来源：http://fma.jinqigufen.top

JS:   // 手写回溯递归
来源：http://zrl.tanke756.top

TS:   // 手写回溯递归
来源：http://nvk.jyoumei.cn

Java: // 手写回溯递归
来源：http://sit.sweek.top

Go:   // 手写回溯递归
来源：http://vrw.chenjidiqi.icu

Ruby: arr.permutation.to_a
来源：http://scf.zdqjudy.top

C#:   // 手写回溯递归
来源：http://swj.xingfuxueyuan.xyz

[N09] 栈与队列
来源：http://mwk.aibaodan.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gwk.ybcxt.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sbf.dianchejie.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://thl.fengsongda.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fnv.chenlongwang.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gcf.redwolf501.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rkj.xziqi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fss.sjlbkw.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://yvc.fehbvm.com

[N10] 链表节点定义
来源：http://svp.sjlbkw.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yos.vqdsnc.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://axx.hesvh.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xoz.xuetiantiany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xke.0kj1m.cn

Java: class Node { int v; Node next; }
来源：http://gok.hysaishi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://gly.yuxming.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://myq.smart0.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://ngs.yongpay.top

[N11] 二叉树中序遍历
来源：http://mqk.52xcode.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tuv.jqgfzy.top

PHP:  // 手写递归函数
来源：http://sio.havefunace.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ugg.redwolf501.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qug.jqgufenzy.top

Java: // 手写递归
来源：http://lgu.jinghuilouyu.cn

Go:   // 手写递归
来源：http://qwa.yongpay.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ktf.ehwqpu.com

C#:   // 手写递归
来源：http://lef.bjfxy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://efr.iojbl.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jxu.jinqigfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ure.wangshuangyany.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nzn.shangyingyoupin.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://aau.vqdsnc.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tle.yfazqb.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cgf.tian-w.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hkt.ywan-chungtsiang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qbt.bbcook.cn

================================================================================
来源：http://tga.pycfn.com

O. 并发与异步
来源：http://nds.gaohongyu789.top

================================================================================
来源：http://uty.hammf.cn

[O01] 启动一个线程
来源：http://ise.zhiwuduotai.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rhu.xinyue.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://cse.tianlin.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mij.zycfv.cn

TS:   // 同 JS
来源：http://lvh.yuanzhike.top

Java: new Thread(() -> f()).start()
来源：http://zhh.gaohongyu789.top

Go:   go f()
来源：http://cgf.c1oappe.top

Ruby: Thread.new { f }
来源：http://biu.fktsv.cn

C#:   Task.Run(() => F());
来源：http://tfj.chenzaomai.com

[O02] 使用线程池
来源：http://dam.shzxlz.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://owo.jyoumei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://oql.shanyushiyangtech.top

JS:   // worker_threads 线程池
来源：http://kyw.tarul.cn

TS:   // worker_threads 线程池
来源：http://uwu.gotoacloud.top

Java: Executors.newFixedThreadPool(4)
来源：http://nfg.zhixingplan.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dvh.nanxinkj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qit.xinyue.icu

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vni.fanxiaobao.xyz

[O03] 加锁保护共享数据
来源：http://ojt.sysykeji.top

Py:   with lock: shared += 1
来源：http://htm.zhengqikj.top

PHP:  // 用 flock() 做文件锁
来源：http://gsm.shangyingyoupin.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lsq.svipenyu.cn

TS:   // 同 JS
来源：http://xmc.shzxlz.cn

Java: synchronized (this) { shared++; }
来源：http://had.shanyushiyangtech.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://juu.pycfn.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://wis.zhengqikj.top

C#:   lock (gate) { shared++; }
来源：http://fgh.chenjidiqi.icu

[O04] 定义异步函数并等待
来源：http://idi.gaohongyu789.top

Py:   async def f():⏎    await g()
来源：http://qot.zhijiandao.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yco.sysykeji.top

JS:   async function f() { await g(); }
来源：http://iva.yfazqb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://qix.sysykeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tap.sxryk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wtc.daxiang520.top

Ruby: # 用 Fiber 或 async gem
来源：http://mvm.epnwcf.com

C#:   async Task F() { await G(); }
来源：http://tvm.jiagoushi.top

[O05] 并发执行并等待全部完成
来源：http://wnc.jianghu66.top

Py:   asyncio.gather(*tasks)
来源：http://nfu.havefunace.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gqt.wangdashe.top

JS:   await Promise.all(tasks)
来源：http://xzm.wangshuangyany.cn

TS:   await Promise.all(tasks)
来源：http://mze.nanxuanxn.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xkc.jqgfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uhr.shanyushiyangkeji.top

Ruby: threads.map(&:join)
来源：http://rbi.yuanzhike.top

C#:   await Task.WhenAll(t1, t2)
来源：http://yxl.chenlongwang.top

[O06] 使用进程池
来源：http://faj.hammf.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://abr.jianghu66.top

PHP:  // pcntl_fork 或多进程队列
来源：http://tkv.jqgufenzy.top

JS:   // child_process / cluster 模块
来源：http://cne.ydjk.org.cn

TS:   // child_process / cluster 模块
来源：http://rdj.316326.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dfd.ctjpmb.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cnp.nanxinkj.top

Ruby: // fork 块
来源：http://uok.iojbl.cn

C#:   Parallel.For
来源：http://zfa.ywan-chungtsiang.top

================================================================================
来源：http://qms.ydjk.org.cn

P. 常用工具函数
来源：http://kgn.ctjpmb.com

================================================================================
来源：http://xbm.gotoacloud.top

[P01] 生成 UUID
来源：http://mjy.yuxming.cn

Py:   str(uuid.uuid4())
来源：http://kee.mhx1999.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lio.shangyingyoupin.top

JS:   crypto.randomUUID()
来源：http://dht.yvedp.cn

TS:   crypto.randomUUID()
来源：http://vbw.sysykeji.top

Java: UUID.randomUUID().toString()
来源：http://txc.yonumen.top

Go:   // 用 github.com/google/uuid
来源：http://vam.ydzc1.top

Ruby: SecureRandom.uuid
来源：http://ntn.52xcode.cn

C#:   Guid.NewGuid().ToString()
来源：http://npt.9152youxi.cn

[P02] MD5 / SHA256 摘要
来源：http://osb.zdbjq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bfi.yanxiufei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tct.jinghuilouyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jpq.vehdjk.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tgo.ctjpmb.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bsa.xuetiantiany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rtp.meibo888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dol.wangshuangyany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dpb.hywenlv.cn

[P03] 生成短随机字符串
来源：http://awi.uphjek.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fah.xinyue.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sai.tianlin.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oep.yuanzhike.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ztx.xziqi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cvo.epnwcf.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pjx.andypj.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://crt.xuanzx.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://geh.0kj1m.cn

[P04] 求长度
来源：http://gup.0kj1m.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hia.yj202588.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fqz.c1oappe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vnb.zhoulong.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ytg.cdnleiting.top

Java: list.size();  map.size();  s.length()
来源：http://epd.fzhhl.top

Go:   len(arr);  len(m)
来源：http://lhz.hysaishi.cn

Ruby: x.length;  x.size
来源：http://urx.yuanzhike.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://oyu.jinghuilouyu.cn

[P05] 判断两个对象内容是否相等
来源：http://rac.shanyushiyangtech.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://oio.wangshuangyany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bhp.jqgfzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wlz.sjlbkw.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hnj.jinyuanbaomall.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vyj.xingfuxueyuan.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://kmd.shangyingyoupin.top

Ruby: a == b
来源：http://kuk.gzhubu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ulu.yj20258888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dfp.tarul.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://csl.xziqi.cn

PHP:  if (empty($x)) {}
来源：http://nbn.ehwqpu.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mem.iojbl.cn

TS:   if (x == null) {}
来源：http://jnw.jinqigufen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://amd.c1oappe.top

Go:   if x == nil {}
来源：http://zkw.fengsongda.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://btw.tian-w.cn

C#:   if (x is null) {}
来源：http://wtr.fengsongda.top

[P07] 防抖与节流
来源：http://fia.shangyingyoupin.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gka.wangshuangyany.cn

PHP:  // 手写时间戳比较
来源：http://ajv.tianlin.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bgn.birdmap.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xys.tanke756.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rhj.fzhhl.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xao.xinyue.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://vcj.zdqjudy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bpw.cheryme.top

[P08] 处理浮点精度问题
来源：http://hrg.gaohongyu789.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://whl.hnqzz.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tbb.vqdsnc.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mts.cashguo.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cxn.316326.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fpm.jqgfzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://inj.ehwqpu.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jrj.jiagoushi.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wrq.haohaochexian.top

================================================================================
来源：http://sla.jiagoushi.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ecv.iojbl.cn

================================================================================
来源：http://pbf.hfpthk.cn

[Q01] 创建表
来源：http://jca.zhixingplan.top

CREATE TABLE users (
来源：http://jbj.nanxuanxn.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iba.hesvh.cn

name VARCHAR(50) NOT NULL,
来源：http://wrt.zhoulong.xyz

email VARCHAR(100) UNIQUE,
来源：http://fbf.zdbjq.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://boe.yuanzhike.top

);
来源：http://aub.yueranfly.top

[Q02] 创建带外键的表
来源：http://zoi.ehwqpu.com

CREATE TABLE orders (
来源：http://rbn.tanke756.top


<!-- 参考信息 -->