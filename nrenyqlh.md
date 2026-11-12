代发 wailian999

TS:   process.cwd()
来源：http://hnw.9152youxi.cn

Java: Path.of("").toAbsolutePath()
来源：http://nal.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://knu.wangdashe.top

Ruby: Dir.pwd
来源：http://edj.hysaishi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lkh.hesvh.cn

[M05] 设置退出码
来源：http://iki.ctjpmb.com

Py:   sys.exit(1)
来源：http://pfm.tian-w.cn

PHP:  exit(1);
来源：http://mhy.svipenyu.cn

JS:   process.exit(1)
来源：http://jof.tanke756.top

TS:   process.exit(1)
来源：http://amf.epnwcf.com

Java: System.exit(1)
来源：http://ozd.dashuyun.cn

Go:   os.Exit(1)
来源：http://lgt.tanke756.top

Ruby: exit 1
来源：http://ppe.hysaishi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bcz.quarkkingdee.top

[M06] 向标准错误输出
来源：http://cqd.aibaodan.cn

Py:   print("err", file=sys.stderr)
来源：http://eih.gotoacloud.top

PHP:  fwrite(STDERR, "err\n");
来源：http://dlm.9152youxi.cn

JS:   console.error("err")
来源：http://gxp.yuanzhike.top

TS:   console.error("err")
来源：http://wur.cashguo.top

Java: System.err.println("err")
来源：http://tbu.fengsongda.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://csp.jiagoushi.top

Ruby: warn "err"
来源：http://bfd.svipenyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://mqk.hfpthk.cn

[M07] 判断是否为主入口
来源：http://trr.xingfuxueyuan.xyz

Py:   if __name__ == "__main__":
来源：http://wai.316326.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://iud.yanxiufei.cn

JS:   require.main === module
来源：http://zkb.epnwcf.com

TS:   require.main === module
来源：http://zom.yanxiufei.cn

Java: public static void main(String[] args)
来源：http://kmz.fktsv.cn

Go:   func main()
来源：http://uso.yj202588.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tww.jiagoushi.top

C#:   static void Main(string[] args)
来源：http://gji.zdbjq.cn

[M08] 获取系统与运行时信息
来源：http://vfa.ivvv.top

Py:   platform.system();  platform.python_version()
来源：http://xas.jianghu66.top

PHP:  PHP_OS;  phpversion();
来源：http://iik.jqgfzy.top

JS:   process.platform;  process.version
来源：http://dma.tarul.cn

TS:   process.platform;  process.version
来源：http://zbl.jqgfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ndc.nanxuanxn.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zig.dianchejie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mwd.tianlin.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://owd.xingfuxueyuan.xyz

================================================================================
来源：http://atw.jianghu66.top

N. 数据结构与算法
来源：http://olr.tian-w.cn

================================================================================
来源：http://knl.sjlbkw.cn

[N01] 二分查找（有序数组）
来源：http://uxp.jinqigufen.top

Py:   bisect.bisect_left(arr, x)
来源：http://yxn.0kj1m.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ucs.chenlongwang.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qea.daxiang520.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://snx.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gvw.wangshuangyany.cn

Go:   sort.SearchInts(arr, x)
来源：http://jzl.shanyushiyangtech.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://tuu.jlsjyb.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gfy.zycfv.cn

[N02] 排序（工程实践用内置实现）
来源：http://qxy.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://rjr.nanxuanxn.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rcc.sjlbkw.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://eep.jinyuanbaomall.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://wek.ppjwa.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://swy.xinyue.icu

Go:   slices.Sort(arr)
来源：http://ujm.yangfankeji.com

Ruby: arr.sort
来源：http://vte.yfazqb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://nbv.tarul.cn

[N03] 快速排序（分治示例）
来源：http://gbv.iojbl.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://azc.uphjek.com

PHP:  // 递归实现，或用 usort
来源：http://yoe.havefunace.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iyz.ydzc1.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xlb.ybcxt.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mki.yanxiufei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ode.jinqigufen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xju.wangshuangyany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://skj.dianchejie.cn

[N04] 斐波那契数列
来源：http://aih.jqgfzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jjv.xylfe.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bzt.epnwcf.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qsi.ywan-chungtsiang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://byk.jqgufenzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://meg.svipenyu.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kpe.havefunace.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zxy.uphjek.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vff.nwbrower.top

[N05] 最大公约数
来源：http://xsl.tanke756.top

Py:   math.gcd(a, b)
来源：http://xru.cqqwz.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hge.fktsv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wnn.haohaochexian.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vlj.chenjidiqi.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://exq.vehdjk.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wlq.zhijiandao.cn

Ruby: a.gcd(b)
来源：http://acb.chenlongwang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bsd.xuetiantiany.cn

[N06] 判断回文字符串
来源：http://wmr.shzxlz.cn

Py:   s == s[::-1]
来源：http://cjh.andypj.xyz

PHP:  $s === strrev($s);
来源：http://vmu.yuxming.cn

JS:   s === [...s].reverse().join("")
来源：http://oyg.vqdsnc.cn

TS:   s === [...s].reverse().join("")
来源：http://cos.svipenyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://shz.fktsv.cn

Go:   // 双指针从两端比较
来源：http://nxg.ehwqpu.com

Ruby: s == s.reverse
来源：http://fmj.zdbjq.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://itp.ppjwa.cn

[N07] 两数之和（返回下标）
来源：http://fcn.xziqi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://olo.sweek.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oau.sysykeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gzy.hywenlv.cn

TS:   // 手写 Map<string, number>
来源：http://kec.fktsv.cn

Java: // 手写 HashMap
来源：http://yuw.aibaodan.cn

Go:   // 手写 map[int]int
来源：http://otl.tianlin.xyz

Ruby: // 手写 Hash
来源：http://geu.meibo888.top

C#:   // 手写 Dictionary<int, int>
来源：http://jjz.fanxiaobao.xyz

[N08] 生成全排列
来源：http://yzb.hywenlv.cn

Py:   itertools.permutations(arr)
来源：http://pvf.snrcjt.cn

PHP:  // 手写递归交换
来源：http://ihx.andypj.xyz

JS:   // 手写回溯递归
来源：http://ume.iojbl.cn

TS:   // 手写回溯递归
来源：http://zbo.jinghuilouyu.cn

Java: // 手写回溯递归
来源：http://nah.jinyuanbaomall.cn

Go:   // 手写回溯递归
来源：http://jgu.ctjpmb.com

Ruby: arr.permutation.to_a
来源：http://mes.gotoacloud.top

C#:   // 手写回溯递归
来源：http://hdc.uphjek.com

[N09] 栈与队列
来源：http://gin.tian-w.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qnw.yuxming.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://oju.sweek.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sxi.daria6918.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wcl.zdbjq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qeu.bbcook.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yhg.xylfe.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://kox.zdbjq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ynd.ehwqpu.com

[N10] 链表节点定义
来源：http://rhk.cucudq.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cpl.zhixingplan.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qpx.jqgfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tdy.haohaochexian.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jsb.yfazqb.com

Java: class Node { int v; Node next; }
来源：http://jjz.yueranfly.top

Go:   type Node struct { V int; Next *Node }
来源：http://jkz.aibaodan.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vuy.hammf.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jus.svipenyu.cn

[N11] 二叉树中序遍历
来源：http://pbr.hammf.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tlp.hnqzz.top

PHP:  // 手写递归函数
来源：http://yhe.hesvh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zle.haohaochexian.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zpg.hcnkem.com

Java: // 手写递归
来源：http://nah.pengpengdd.cyou

Go:   // 手写递归
来源：http://sdo.ehwqpu.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://oco.ydjk.org.cn

C#:   // 手写递归
来源：http://thw.yj202588.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rmv.ywan-chungtsiang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cnu.sjlbkw.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pdo.fzhhl.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yxe.zhongyouzk.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rfk.jinyuanbaomall.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hwc.cucudq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bnt.ivvv.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uhc.pycfn.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wtu.dianchejie.cn

================================================================================
来源：http://otg.zhijiandao.cn

O. 并发与异步
来源：http://vfm.tarul.cn

================================================================================
来源：http://clt.daria6918.cn

[O01] 启动一个线程
来源：http://fge.gogol.net.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ovm.jqgufenzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bgb.smart0.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vsz.hnxiangtu.top

TS:   // 同 JS
来源：http://lge.aizwys.cn

Java: new Thread(() -> f()).start()
来源：http://upm.zhijiandao.cn

Go:   go f()
来源：http://juv.gzhubu.top

Ruby: Thread.new { f }
来源：http://pdm.smart0.xyz

C#:   Task.Run(() => F());
来源：http://hux.uphjek.com

[O02] 使用线程池
来源：http://scq.chenzaomai.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bvx.yj20258888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nrc.gaohongyu789.top

JS:   // worker_threads 线程池
来源：http://dug.hongshengwenyu.top

TS:   // worker_threads 线程池
来源：http://piz.ehwqpu.com

Java: Executors.newFixedThreadPool(4)
来源：http://bnw.jinqigufen.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cok.zhengqikj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.yueranfly.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cvd.shanyushiyangtech.top

[O03] 加锁保护共享数据
来源：http://izs.shuidangran.top

Py:   with lock: shared += 1
来源：http://wtw.guannengcc.top

PHP:  // 用 flock() 做文件锁
来源：http://yxm.dashuyun.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://crc.andypj.xyz

TS:   // 同 JS
来源：http://klw.cashguo.top

Java: synchronized (this) { shared++; }
来源：http://ozi.yonumen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gtx.yuxming.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://nff.hesvh.cn

C#:   lock (gate) { shared++; }
来源：http://siy.jinqigfzy.top

[O04] 定义异步函数并等待
来源：http://qit.andypj.xyz

Py:   async def f():⏎    await g()
来源：http://qzi.xuetiantiany.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mys.hfpthk.cn

JS:   async function f() { await g(); }
来源：http://igc.jianghu66.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://edm.ydzc1.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cbl.tarul.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ukb.vehdjk.com

Ruby: # 用 Fiber 或 async gem
来源：http://tye.wangshuangyany.cn

C#:   async Task F() { await G(); }
来源：http://koo.yongpay.top

[O05] 并发执行并等待全部完成
来源：http://slu.hfpthk.cn

Py:   asyncio.gather(*tasks)
来源：http://gzg.shanyushiyangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rvc.yonumen.top

JS:   await Promise.all(tasks)
来源：http://ujk.ydzc1.top

TS:   await Promise.all(tasks)
来源：http://ygt.tarul.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://twq.jqgfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hbj.snrcjt.cn

Ruby: threads.map(&:join)
来源：http://zut.tarul.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dqs.shuidangran.top

[O06] 使用进程池
来源：http://czk.xingfuxueyuan.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mlw.pycfn.com

PHP:  // pcntl_fork 或多进程队列
来源：http://zeb.chenlongwang.top

JS:   // child_process / cluster 模块
来源：http://qrp.daxiang520.top

TS:   // child_process / cluster 模块
来源：http://pva.fanxiaobao.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://nxg.meibo888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://asd.tarul.cn

Ruby: // fork 块
来源：http://oyr.xingfuxueyuan.xyz

C#:   Parallel.For
来源：http://obc.fengsongda.top

================================================================================
来源：http://ukz.hywenlv.cn

P. 常用工具函数
来源：http://vis.mhx1999.top

================================================================================
来源：http://zyn.svipenyu.cn

[P01] 生成 UUID
来源：http://rft.svipenyu.cn

Py:   str(uuid.uuid4())
来源：http://nhi.jinqigufen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://okq.yanxiufei.cn

JS:   crypto.randomUUID()
来源：http://qyt.zhengqikj.top

TS:   crypto.randomUUID()
来源：http://bcl.hongshengwenyu.top

Java: UUID.randomUUID().toString()
来源：http://egj.havefunace.top

Go:   // 用 github.com/google/uuid
来源：http://cxc.fengsongda.top

Ruby: SecureRandom.uuid
来源：http://qio.havefunace.top

C#:   Guid.NewGuid().ToString()
来源：http://udi.redwolf501.top

[P02] MD5 / SHA256 摘要
来源：http://ktv.xziqi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gag.tanke756.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zku.andypj.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rav.havefunace.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tws.chenzaomai.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gjn.sxryk.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://chk.yfazqb.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://auc.zycfv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://squ.hysaishi.cn

[P03] 生成短随机字符串
来源：http://qqw.cucudq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jwk.yfazqb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://apz.cashguo.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ylh.ywan-chungtsiang.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tab.snrcjt.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hgq.ybcxt.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ezr.jinqigfzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cfe.bjfxy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sle.zhixingplan.top

[P04] 求长度
来源：http://rav.zhiwuduotai.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wnv.hywenlv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vbo.hongshengwenyu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xza.jiagoushi.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vqo.epnwcf.com

Java: list.size();  map.size();  s.length()
来源：http://igg.feifeiyinyue.top

Go:   len(arr);  len(m)
来源：http://vrg.shanyushiyangkeji.top

Ruby: x.length;  x.size
来源：http://ymz.c1oappe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://myf.chenzaomai.com

[P05] 判断两个对象内容是否相等
来源：http://rpe.epnwcf.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://mhs.sweek.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tak.hongshengwenyu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fip.zhiwuduotai.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://umf.jqgufenzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://diz.shuidangran.top

Go:   reflect.DeepEqual(a, b)
来源：http://mcf.zhijiandao.cn

Ruby: a == b
来源：http://lhx.cdnleiting.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ydl.chenjidiqi.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kmj.hcnkem.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://deg.shanyushiyangkeji.top

PHP:  if (empty($x)) {}
来源：http://nue.epnwcf.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tqc.sxryk.cn

TS:   if (x == null) {}
来源：http://kle.dashuyun.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uzh.meibo888.top

Go:   if x == nil {}
来源：http://zfu.meibo888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yvv.xylfe.cn

C#:   if (x is null) {}
来源：http://fgd.hcnkem.com

[P07] 防抖与节流
来源：http://hyx.xylfe.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wmy.yongpay.top

PHP:  // 手写时间戳比较
来源：http://drd.daria6918.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ibl.yuxming.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lhg.xziqi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sgt.zhiwuduotai.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pbf.zhongyouzk.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://pdr.guannengcc.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://aha.jlsjyb.cn

[P08] 处理浮点精度问题
来源：http://dzt.guannengcc.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://biy.shuidangran.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://etx.yonumen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pdz.haohaochexian.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tfo.ppjwa.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://saj.jqgufenzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eiv.hnqzz.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gpu.ywan-chungtsiang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qll.zhaomingkeji.xyz

================================================================================
来源：http://zhv.jinghuilouyu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bdh.shanyushiyangtech.top

================================================================================
来源：http://mdu.hysaishi.cn

[Q01] 创建表
来源：http://ybg.guannengcc.top

CREATE TABLE users (
来源：http://wav.haohaochexian.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gmo.jinghuilouyu.cn

name VARCHAR(50) NOT NULL,
来源：http://kos.hongshengwenyu.top

email VARCHAR(100) UNIQUE,
来源：http://cdg.zhixingplan.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ysi.xziqi.cn

);
来源：http://gtr.xziqi.cn

[Q02] 创建带外键的表
来源：http://taa.snrcjt.cn

CREATE TABLE orders (
来源：http://koq.jqgfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kqu.hnqzz.top

user_id INT NOT NULL,
来源：http://epk.jinghuilouyu.cn

amount DECIMAL(10, 2),
来源：http://fjb.yongpay.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jhw.jqgufenzy.top


<!-- 参考信息 -->