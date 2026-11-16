代发 wailian999

TS:   process.cwd()
来源：http://sat.yonumen.top

Java: Path.of("").toAbsolutePath()
来源：http://aby.zhengqikj.top

Go:   os.Getwd()
来源：http://bgw.vqdsnc.cn

Ruby: Dir.pwd
来源：http://hds.tianlin.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://tem.jinqigufen.top

[M05] 设置退出码
来源：http://lgr.yuxming.cn

Py:   sys.exit(1)
来源：http://sno.yanxiufei.cn

PHP:  exit(1);
来源：http://qys.yvedp.cn

JS:   process.exit(1)
来源：http://jlx.shanyushiyangkeji.top

TS:   process.exit(1)
来源：http://wqu.cqqwz.cn

Java: System.exit(1)
来源：http://clz.zhiwuduotai.top

Go:   os.Exit(1)
来源：http://gex.zhaomingkeji.xyz

Ruby: exit 1
来源：http://cgv.jinqigfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uas.mhx1999.top

[M06] 向标准错误输出
来源：http://qfm.aibaodan.cn

Py:   print("err", file=sys.stderr)
来源：http://axe.dashuyun.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://dbi.wangdashe.top

JS:   console.error("err")
来源：http://hqo.pengpengdd.cyou

TS:   console.error("err")
来源：http://tzs.gogol.net.cn

Java: System.err.println("err")
来源：http://kzo.ydzc1.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uxk.xingfuxueyuan.xyz

Ruby: warn "err"
来源：http://std.shuidangran.top

C#:   Console.Error.WriteLine("err")
来源：http://muv.jinghuilouyu.cn

[M07] 判断是否为主入口
来源：http://pbo.tian-w.cn

Py:   if __name__ == "__main__":
来源：http://jxl.jlsjyb.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dqf.jqgufenzy.top

JS:   require.main === module
来源：http://cks.guowangkeji.top

TS:   require.main === module
来源：http://lvy.xuanzx.com

Java: public static void main(String[] args)
来源：http://thx.ppjwa.cn

Go:   func main()
来源：http://gwt.jinqigufen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uwg.smart0.xyz

C#:   static void Main(string[] args)
来源：http://nfy.wangshuangyany.cn

[M08] 获取系统与运行时信息
来源：http://oaz.pengpengdd.cyou

Py:   platform.system();  platform.python_version()
来源：http://gez.tarul.cn

PHP:  PHP_OS;  phpversion();
来源：http://uua.yuxming.cn

JS:   process.platform;  process.version
来源：http://axt.316326.xyz

TS:   process.platform;  process.version
来源：http://xsp.c1oappe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xku.birdmap.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tde.fktsv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oxs.hammf.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://atw.shanyushiyangkeji.top

================================================================================
来源：http://kgk.hywenlv.cn

N. 数据结构与算法
来源：http://nus.nanxuanxn.top

================================================================================
来源：http://ryo.hongshengwenyu.top

[N01] 二分查找（有序数组）
来源：http://qzp.bjfxy.top

Py:   bisect.bisect_left(arr, x)
来源：http://oek.fzhhl.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vuw.guowangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lly.guannengcc.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ndw.birdmap.top

Java: Arrays.binarySearch(arr, x)
来源：http://prf.xylfe.cn

Go:   sort.SearchInts(arr, x)
来源：http://dzh.cheryme.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ecz.chenlongwang.top

C#:   Array.BinarySearch(arr, x)
来源：http://xxp.meibo888.top

[N02] 排序（工程实践用内置实现）
来源：http://nmd.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://epx.dianchejie.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hqc.yj202588.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xek.shzxlz.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wvz.sysykeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://reo.birdmap.top

Go:   slices.Sort(arr)
来源：http://dvc.wangdashe.top

Ruby: arr.sort
来源：http://qlg.xuanzx.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://inf.haohaochexian.top

[N03] 快速排序（分治示例）
来源：http://xwi.sxryk.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qfs.shanyushiyangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://nyz.tianlin.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://naq.bbcook.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://evz.xziqi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cft.zhijiandao.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xub.tanke756.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xlj.dashuyun.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tbf.sweek.top

[N04] 斐波那契数列
来源：http://xsm.hesvh.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fdc.316326.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ikc.vehdjk.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ftg.hcnkem.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fgk.316326.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://off.xuanzx.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://abr.svipenyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ewm.gogol.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yfx.yj20258888.top

[N05] 最大公约数
来源：http://gfv.yanxiufei.cn

Py:   math.gcd(a, b)
来源：http://alh.dianchejie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://udg.xuetiantiany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hir.vehdjk.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://juu.ydjk.org.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://dku.redwolf501.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://izv.pycfn.com

Ruby: a.gcd(b)
来源：http://bne.hnxiangtu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://css.yvedp.cn

[N06] 判断回文字符串
来源：http://hkw.yj20258888.top

Py:   s == s[::-1]
来源：http://hhk.jianghu66.top

PHP:  $s === strrev($s);
来源：http://rqx.andypj.xyz

JS:   s === [...s].reverse().join("")
来源：http://zha.hcnkem.com

TS:   s === [...s].reverse().join("")
来源：http://pwa.ydjk.org.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ifk.yongpay.top

Go:   // 双指针从两端比较
来源：http://oxu.cucudq.cn

Ruby: s == s.reverse
来源：http://srz.pengpengdd.cyou

C#:   s == new string(s.Reverse().ToArray())
来源：http://rlz.gogol.net.cn

[N07] 两数之和（返回下标）
来源：http://pqb.birdmap.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hxf.yj20258.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fjb.sweek.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jqa.ydjk.org.cn

TS:   // 手写 Map<string, number>
来源：http://xhg.cucudq.cn

Java: // 手写 HashMap
来源：http://nbl.dashuyun.cn

Go:   // 手写 map[int]int
来源：http://ijn.xziqi.cn

Ruby: // 手写 Hash
来源：http://uye.epnwcf.com

C#:   // 手写 Dictionary<int, int>
来源：http://hhq.0kj1m.cn

[N08] 生成全排列
来源：http://qyb.hcnkem.com

Py:   itertools.permutations(arr)
来源：http://bxt.tianlin.xyz

PHP:  // 手写递归交换
来源：http://bmf.pycfn.com

JS:   // 手写回溯递归
来源：http://fnx.jinqigufen.top

TS:   // 手写回溯递归
来源：http://kcz.yuxming.cn

Java: // 手写回溯递归
来源：http://svj.nanxinkj.top

Go:   // 手写回溯递归
来源：http://xgz.hnxiangtu.top

Ruby: arr.permutation.to_a
来源：http://fcj.zhijiandao.cn

C#:   // 手写回溯递归
来源：http://hqt.zycfv.cn

[N09] 栈与队列
来源：http://tcv.pengpengdd.cyou

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://utu.birdmap.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nvy.hcnkem.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://taz.dashuyun.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://spn.shuidangran.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://eec.jiagoushi.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tpu.cdnleiting.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qpd.ehwqpu.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rik.hysaishi.cn

[N10] 链表节点定义
来源：http://voa.yuxming.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://geb.9152youxi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://omv.wangshuangyany.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tft.chenzaomai.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://stt.yonumen.top

Java: class Node { int v; Node next; }
来源：http://pvn.hnxiangtu.top

Go:   type Node struct { V int; Next *Node }
来源：http://tna.ywan-chungtsiang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://btz.ivvv.top

C#:   class Node { public int V; public Node? Next; }
来源：http://usb.xinyue.icu

[N11] 二叉树中序遍历
来源：http://uta.nwbrower.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mph.daria6918.cn

PHP:  // 手写递归函数
来源：http://knl.shanyushiyangtech.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ewe.fanxiaobao.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pbf.fktsv.cn

Java: // 手写递归
来源：http://ztl.zhijiandao.cn

Go:   // 手写递归
来源：http://yzf.bbcook.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://clc.ctjpmb.com

C#:   // 手写递归
来源：http://dwr.fehbvm.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xcz.hongshengwenyu.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nmg.xuetiantiany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://nix.bbcook.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qfa.zhoulong.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dpe.svipenyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oag.chenjidiqi.icu

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://inm.hnxiangtu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lmq.zhoulong.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hnq.nanxuanxn.top

================================================================================
来源：http://hvs.ydzc1.top

O. 并发与异步
来源：http://wfd.pycfn.com

================================================================================
来源：http://kra.sxryk.cn

[O01] 启动一个线程
来源：http://uvo.hesvh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fpu.ehwqpu.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eah.uphjek.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://bca.shangyingyoupin.top

TS:   // 同 JS
来源：http://kcg.xziqi.cn

Java: new Thread(() -> f()).start()
来源：http://oxd.gotoacloud.top

Go:   go f()
来源：http://cqz.gzhubu.top

Ruby: Thread.new { f }
来源：http://drt.hongshengwenyu.top

C#:   Task.Run(() => F());
来源：http://ico.fehbvm.com

[O02] 使用线程池
来源：http://ven.smart0.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ozo.sxryk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qll.wangdashe.top

JS:   // worker_threads 线程池
来源：http://bfm.fengsongda.top

TS:   // worker_threads 线程池
来源：http://jij.sufxvd.cn

Java: Executors.newFixedThreadPool(4)
来源：http://uyk.guannengcc.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://jcw.cdnleiting.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://glo.shanyushiyangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wpf.daxiang520.top

[O03] 加锁保护共享数据
来源：http://fyt.tianlin.xyz

Py:   with lock: shared += 1
来源：http://tfc.nwbrower.top

PHP:  // 用 flock() 做文件锁
来源：http://grz.bjfxy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rbd.sufxvd.cn

TS:   // 同 JS
来源：http://oba.jinqigufen.top

Java: synchronized (this) { shared++; }
来源：http://rlz.daria6918.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gns.hcnkem.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://ifl.aizwys.cn

C#:   lock (gate) { shared++; }
来源：http://scg.sufxvd.cn

[O04] 定义异步函数并等待
来源：http://ssu.yongpay.top

Py:   async def f():⏎    await g()
来源：http://ylo.hfpthk.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dld.zdbjq.cn

JS:   async function f() { await g(); }
来源：http://shc.ehwqpu.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://edf.zdbjq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cwz.tanke756.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zlk.jyoumei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kbk.chenzaomai.com

C#:   async Task F() { await G(); }
来源：http://eqs.sjlbkw.cn

[O05] 并发执行并等待全部完成
来源：http://yob.dashuyun.cn

Py:   asyncio.gather(*tasks)
来源：http://jlh.nwbrower.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rsj.epnwcf.com

JS:   await Promise.all(tasks)
来源：http://pwf.ctjpmb.com

TS:   await Promise.all(tasks)
来源：http://par.tian-w.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://msc.iojbl.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dlq.pycfn.com

Ruby: threads.map(&:join)
来源：http://qrf.zhongyouzk.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ylf.c1oappe.top

[O06] 使用进程池
来源：http://hgw.jianghu66.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://udh.shangyingyoupin.top

PHP:  // pcntl_fork 或多进程队列
来源：http://dqu.zhixingplan.top

JS:   // child_process / cluster 模块
来源：http://kcy.9152youxi.cn

TS:   // child_process / cluster 模块
来源：http://mft.shanyushiyangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lyn.ivvv.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qua.yonumen.top

Ruby: // fork 块
来源：http://pel.yfazqb.com

C#:   Parallel.For
来源：http://lwy.bjfxy.top

================================================================================
来源：http://qaq.bbcook.cn

P. 常用工具函数
来源：http://rrv.yueranfly.top

================================================================================
来源：http://rnw.zhongyouzk.top

[P01] 生成 UUID
来源：http://nfd.dashuyun.cn

Py:   str(uuid.uuid4())
来源：http://zfb.wangshuangyany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://byk.nanxuanxn.top

JS:   crypto.randomUUID()
来源：http://baj.hcnkem.com

TS:   crypto.randomUUID()
来源：http://eae.yanxiufei.cn

Java: UUID.randomUUID().toString()
来源：http://nns.iojbl.cn

Go:   // 用 github.com/google/uuid
来源：http://hfl.gaohongyu789.top

Ruby: SecureRandom.uuid
来源：http://dig.xinyue.icu

C#:   Guid.NewGuid().ToString()
来源：http://qet.0kj1m.cn

[P02] MD5 / SHA256 摘要
来源：http://vim.yonumen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bzd.bjfxy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ghd.haohaochexian.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mnz.ppjwa.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lqr.hysaishi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lec.xuanzx.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pip.yfazqb.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zaf.xylfe.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gud.hammf.cn

[P03] 生成短随机字符串
来源：http://hgq.hysaishi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://eoq.ywan-chungtsiang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nhs.chenjidiqi.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://khy.daxiang520.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://llp.zhengqikj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://imm.xingfuxueyuan.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vju.shanyushiyangtech.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tjd.uphjek.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://owk.9152youxi.cn

[P04] 求长度
来源：http://rpk.jinqigufen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cne.xingfuxueyuan.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cfi.hammf.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pld.hammf.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dcq.yfazqb.com

Java: list.size();  map.size();  s.length()
来源：http://hhf.smart0.xyz

Go:   len(arr);  len(m)
来源：http://cpf.hcnkem.com

Ruby: x.length;  x.size
来源：http://ddf.hammf.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ync.feifeiyinyue.top

[P05] 判断两个对象内容是否相等
来源：http://brp.chenlongwang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nxd.chenjidiqi.icu

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dme.xziqi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hmx.chenjidiqi.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://smx.iojbl.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gck.mhx1999.top

Go:   reflect.DeepEqual(a, b)
来源：http://cex.shuidangran.top

Ruby: a == b
来源：http://gtd.birdmap.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fqa.zhaomingkeji.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kga.shanyushiyangkeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vzt.hfpthk.cn

PHP:  if (empty($x)) {}
来源：http://lag.52xcode.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hwb.cashguo.top

TS:   if (x == null) {}
来源：http://dpx.hesvh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mkd.zhoulong.xyz

Go:   if x == nil {}
来源：http://slr.dianchejie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ils.jiagoushi.top

C#:   if (x is null) {}
来源：http://cge.yj20258888.top

[P07] 防抖与节流
来源：http://vcf.jinqigfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gcp.yj20258.top

PHP:  // 手写时间戳比较
来源：http://zlq.jinqigfzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nss.meibo888.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://neq.vehdjk.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jya.meibo888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ipj.ppjwa.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://hio.nanxuanxn.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fih.aibaodan.cn

[P08] 处理浮点精度问题
来源：http://urn.yj20258.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uwb.epnwcf.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fia.nanxinkj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dpc.kuanghao11.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xnj.jyoumei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://inx.zhixingplan.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xuq.cucudq.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cff.ydzc1.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kyh.gzhubu.top

================================================================================
来源：http://smr.hnxiangtu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://buh.hammf.cn

================================================================================
来源：http://iht.sysykeji.top

[Q01] 创建表
来源：http://emr.kuanghao11.cn

CREATE TABLE users (
来源：http://als.zycfv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ybc.sxryk.cn

name VARCHAR(50) NOT NULL,
来源：http://wpd.sxryk.cn

email VARCHAR(100) UNIQUE,
来源：http://hgz.kuanghao11.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://opq.cqqwz.cn

);
来源：http://hnz.vqdsnc.cn

[Q02] 创建带外键的表
来源：http://djz.ehwqpu.com

CREATE TABLE orders (
来源：http://agq.yongpay.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mdw.shanyushiyangkeji.top

user_id INT NOT NULL,
来源：http://dpg.316326.xyz

amount DECIMAL(10, 2),
来源：http://cht.ydzc1.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mch.316326.xyz


<!-- 参考信息 -->