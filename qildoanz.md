代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://brw.xingfuxueyuan.xyz

[M05] 设置退出码
来源：http://fwc.cucudq.cn

Py:   sys.exit(1)
来源：http://kpy.redwolf501.top

PHP:  exit(1);
来源：http://ikz.fengsongda.top

JS:   process.exit(1)
来源：http://hmh.jqgufenzy.top

TS:   process.exit(1)
来源：http://nqp.zhixingplan.top

Java: System.exit(1)
来源：http://fid.pycfn.com

Go:   os.Exit(1)
来源：http://box.yj20258888.top

Ruby: exit 1
来源：http://ktt.xuanzx.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jvt.dashuyun.cn

[M06] 向标准错误输出
来源：http://yig.jinyuanbaomall.cn

Py:   print("err", file=sys.stderr)
来源：http://skg.havefunace.top

PHP:  fwrite(STDERR, "err\n");
来源：http://yhh.ivvv.top

JS:   console.error("err")
来源：http://jpw.zhixingplan.top

TS:   console.error("err")
来源：http://snx.c1oappe.top

Java: System.err.println("err")
来源：http://kdq.aizwys.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nei.zhixingplan.top

Ruby: warn "err"
来源：http://yvb.sufxvd.cn

C#:   Console.Error.WriteLine("err")
来源：http://njz.hongshengwenyu.top

[M07] 判断是否为主入口
来源：http://wzh.ybcxt.top

Py:   if __name__ == "__main__":
来源：http://ahk.andypj.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qwo.ydjk.org.cn

JS:   require.main === module
来源：http://exi.fanxiaobao.xyz

TS:   require.main === module
来源：http://hst.ctjpmb.com

Java: public static void main(String[] args)
来源：http://rdq.bjfxy.top

Go:   func main()
来源：http://ssx.fehbvm.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fpz.hcnkem.com

C#:   static void Main(string[] args)
来源：http://qoi.jlsjyb.cn

[M08] 获取系统与运行时信息
来源：http://uew.zdqjudy.top

Py:   platform.system();  platform.python_version()
来源：http://trw.fehbvm.com

PHP:  PHP_OS;  phpversion();
来源：http://dun.9152youxi.cn

JS:   process.platform;  process.version
来源：http://qrc.havefunace.top

TS:   process.platform;  process.version
来源：http://ljg.yueranfly.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://yvx.uphjek.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://yma.yj20258.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ajd.xinyue.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://jyx.aizwys.cn

================================================================================
来源：http://ier.daria6918.cn

N. 数据结构与算法
来源：http://cau.hcnkem.com

================================================================================
来源：http://alt.c1oappe.top

[N01] 二分查找（有序数组）
来源：http://tva.cucudq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pvo.nanxinkj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hup.yfazqb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pbb.fzhhl.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dyc.zhongyouzk.top

Java: Arrays.binarySearch(arr, x)
来源：http://rur.dianchejie.cn

Go:   sort.SearchInts(arr, x)
来源：http://iqj.jinqigufen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://gbp.yangfankeji.com

C#:   Array.BinarySearch(arr, x)
来源：http://fgv.ehwqpu.com

[N02] 排序（工程实践用内置实现）
来源：http://gsn.yj20258888.top

Py:   sorted(arr);  arr.sort()
来源：http://zzy.ydzc1.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lxd.yj202588.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pgr.zhijiandao.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://kyi.fanxiaobao.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lqc.jqgfzy.top

Go:   slices.Sort(arr)
来源：http://xqv.ydjk.org.cn

Ruby: arr.sort
来源：http://mak.tanke756.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://atp.jinqigufen.top

[N03] 快速排序（分治示例）
来源：http://bsp.cdnleiting.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cef.daxiang520.top

PHP:  // 递归实现，或用 usort
来源：http://xnn.bjfxy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xcy.yanxiufei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mxa.jiagoushi.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://idn.zhaomingkeji.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jhb.zhijiandao.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dss.sjlbkw.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bxc.xuetiantiany.cn

[N04] 斐波那契数列
来源：http://cet.shuidangran.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://klz.snrcjt.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kdo.tarul.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ipw.gzhubu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sgr.pycfn.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://iat.yj20258.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jvb.zhijiandao.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ofm.xuanzx.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://fmc.hnxiangtu.top

[N05] 最大公约数
来源：http://uid.tanke756.top

Py:   math.gcd(a, b)
来源：http://sha.sysykeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tcp.zycfv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wfa.haohaochexian.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eho.tianlin.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nny.cqqwz.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ljq.shuidangran.top

Ruby: a.gcd(b)
来源：http://ybk.xylfe.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lys.9152youxi.cn

[N06] 判断回文字符串
来源：http://fkf.sysykeji.top

Py:   s == s[::-1]
来源：http://rmy.chenjidiqi.icu

PHP:  $s === strrev($s);
来源：http://akj.gzhubu.top

JS:   s === [...s].reverse().join("")
来源：http://qjs.jqgfzy.top

TS:   s === [...s].reverse().join("")
来源：http://zat.nanxuanxn.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gwg.meibo888.top

Go:   // 双指针从两端比较
来源：http://xqv.pycfn.com

Ruby: s == s.reverse
来源：http://bis.daria6918.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cir.pengpengdd.cyou

[N07] 两数之和（返回下标）
来源：http://dnz.hysaishi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fju.iojbl.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ynl.sjlbkw.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fpe.wangdashe.top

TS:   // 手写 Map<string, number>
来源：http://zmt.nwbrower.top

Java: // 手写 HashMap
来源：http://egy.yangfankeji.com

Go:   // 手写 map[int]int
来源：http://olv.chenlongwang.top

Ruby: // 手写 Hash
来源：http://dzi.uphjek.com

C#:   // 手写 Dictionary<int, int>
来源：http://onq.52xcode.cn

[N08] 生成全排列
来源：http://dqu.gaohongyu789.top

Py:   itertools.permutations(arr)
来源：http://exr.havefunace.top

PHP:  // 手写递归交换
来源：http://koq.hnxiangtu.top

JS:   // 手写回溯递归
来源：http://jyj.tian-w.cn

TS:   // 手写回溯递归
来源：http://hxl.9152youxi.cn

Java: // 手写回溯递归
来源：http://zbq.birdmap.top

Go:   // 手写回溯递归
来源：http://cwm.jyoumei.cn

Ruby: arr.permutation.to_a
来源：http://pjj.jianghu66.top

C#:   // 手写回溯递归
来源：http://uft.jqgfzy.top

[N09] 栈与队列
来源：http://nvf.fengsongda.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://elk.9152youxi.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://myw.zdbjq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://drp.svipenyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cov.zycfv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://klo.ydjk.org.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jsk.xinyue.icu

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dzc.yonumen.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qnu.c1oappe.top

[N10] 链表节点定义
来源：http://gad.chenzaomai.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://okr.0kj1m.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fct.sufxvd.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kul.bjfxy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rrf.quarkkingdee.top

Java: class Node { int v; Node next; }
来源：http://rew.ydzc1.top

Go:   type Node struct { V int; Next *Node }
来源：http://ojl.snrcjt.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://sbt.zhaomingkeji.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://cre.epnwcf.com

[N11] 二叉树中序遍历
来源：http://caz.cqqwz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://myl.guowangkeji.top

PHP:  // 手写递归函数
来源：http://oya.havefunace.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sen.hnqzz.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rpi.nwbrower.top

Java: // 手写递归
来源：http://nhv.cqqwz.cn

Go:   // 手写递归
来源：http://tqt.jinqigufen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://toz.zhengqikj.top

C#:   // 手写递归
来源：http://sgu.sufxvd.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://dxt.hfpthk.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nta.fktsv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://llg.cdnleiting.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cow.meibo888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hzs.ivvv.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wxq.yueranfly.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ecw.yonumen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rhx.yuanzhike.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yty.bjfxy.top

================================================================================
来源：http://hfd.yonumen.top

O. 并发与异步
来源：http://jfr.andypj.xyz

================================================================================
来源：http://vft.jinghuilouyu.cn

[O01] 启动一个线程
来源：http://zxa.daria6918.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zsr.haohaochexian.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ozh.wangdashe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xqz.bbcook.cn

TS:   // 同 JS
来源：http://ytn.shangyingyoupin.top

Java: new Thread(() -> f()).start()
来源：http://was.hnqzz.top

Go:   go f()
来源：http://zvn.hongshengwenyu.top

Ruby: Thread.new { f }
来源：http://frj.redwolf501.top

C#:   Task.Run(() => F());
来源：http://bnt.jinqigfzy.top

[O02] 使用线程池
来源：http://dfp.mhx1999.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bfc.redwolf501.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hjq.ivvv.top

JS:   // worker_threads 线程池
来源：http://rqo.uphjek.com

TS:   // worker_threads 线程池
来源：http://kfv.jqgufenzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://bfr.sweek.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gxd.aizwys.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qhl.jlsjyb.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nji.sxryk.cn

[O03] 加锁保护共享数据
来源：http://dms.aibaodan.cn

Py:   with lock: shared += 1
来源：http://opc.shangyingyoupin.top

PHP:  // 用 flock() 做文件锁
来源：http://ecu.vehdjk.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nfn.daxiang520.top

TS:   // 同 JS
来源：http://ymi.jinqigufen.top

Java: synchronized (this) { shared++; }
来源：http://hok.yonumen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mpm.xingfuxueyuan.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://bjl.cheryme.top

C#:   lock (gate) { shared++; }
来源：http://maa.ydjk.org.cn

[O04] 定义异步函数并等待
来源：http://hen.cdnleiting.top

Py:   async def f():⏎    await g()
来源：http://wtb.c1oappe.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://drc.chenzaomai.com

JS:   async function f() { await g(); }
来源：http://fnf.yj202588.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rbw.smart0.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nci.hfpthk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xcg.0kj1m.cn

Ruby: # 用 Fiber 或 async gem
来源：http://evv.yj20258.top

C#:   async Task F() { await G(); }
来源：http://ssy.hnxiangtu.top

[O05] 并发执行并等待全部完成
来源：http://rwm.uphjek.com

Py:   asyncio.gather(*tasks)
来源：http://paq.zdbjq.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wnk.zhongyouzk.top

JS:   await Promise.all(tasks)
来源：http://ued.xylfe.cn

TS:   await Promise.all(tasks)
来源：http://vlp.pycfn.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gee.yangfankeji.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dcn.zdqjudy.top

Ruby: threads.map(&:join)
来源：http://gge.sjlbkw.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nuz.svipenyu.cn

[O06] 使用进程池
来源：http://doy.uphjek.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wlx.zdqjudy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://tbh.hywenlv.cn

JS:   // child_process / cluster 模块
来源：http://ojm.316326.xyz

TS:   // child_process / cluster 模块
来源：http://zga.wangshuangyany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rqo.hfpthk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mps.pycfn.com

Ruby: // fork 块
来源：http://kov.jlsjyb.cn

C#:   Parallel.For
来源：http://pzg.daxiang520.top

================================================================================
来源：http://vkx.snrcjt.cn

P. 常用工具函数
来源：http://euj.bbcook.cn

================================================================================
来源：http://qso.daxiang520.top

[P01] 生成 UUID
来源：http://sqa.chenjidiqi.icu

Py:   str(uuid.uuid4())
来源：http://qax.fanxiaobao.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lcn.snrcjt.cn

JS:   crypto.randomUUID()
来源：http://ayk.ctjpmb.com

TS:   crypto.randomUUID()
来源：http://itk.guannengcc.top

Java: UUID.randomUUID().toString()
来源：http://ega.guannengcc.top

Go:   // 用 github.com/google/uuid
来源：http://dbd.yj202588.top

Ruby: SecureRandom.uuid
来源：http://xim.yuxming.cn

C#:   Guid.NewGuid().ToString()
来源：http://vdv.shzxlz.cn

[P02] MD5 / SHA256 摘要
来源：http://lri.dashuyun.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cjv.feifeiyinyue.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jyi.yonumen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ary.sweek.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zrx.fzhhl.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kls.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ils.tarul.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xcz.andypj.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aqh.sysykeji.top

[P03] 生成短随机字符串
来源：http://cdz.hfpthk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qyf.gaohongyu789.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cvp.ppjwa.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gjq.zhengqikj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pad.hnqzz.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yby.jqgufenzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hqd.pycfn.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://pix.hongshengwenyu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://usz.cheryme.top

[P04] 求长度
来源：http://flq.kuanghao11.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fxt.cheryme.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ctn.gaohongyu789.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://prb.hammf.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sud.yuanzhike.top

Java: list.size();  map.size();  s.length()
来源：http://aac.xylfe.cn

Go:   len(arr);  len(m)
来源：http://moh.pengpengdd.cyou

Ruby: x.length;  x.size
来源：http://mjm.guowangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://kpq.tian-w.cn

[P05] 判断两个对象内容是否相等
来源：http://yci.jyoumei.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qio.jianghu66.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yyf.guannengcc.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qtw.fanxiaobao.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nlw.ydjk.org.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vmz.vehdjk.com

Go:   reflect.DeepEqual(a, b)
来源：http://xdt.fzhhl.top

Ruby: a == b
来源：http://tmh.guowangkeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gzg.jlsjyb.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fug.sxryk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vbf.nanxuanxn.top

PHP:  if (empty($x)) {}
来源：http://wwx.sysykeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lhq.tanke756.top

TS:   if (x == null) {}
来源：http://gei.havefunace.top

Java: if (x == null || x.isEmpty()) {}
来源：http://tqm.shanyushiyangkeji.top

Go:   if x == nil {}
来源：http://sgr.zhiwuduotai.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nsh.sufxvd.cn

C#:   if (x is null) {}
来源：http://mzi.hongshengwenyu.top

[P07] 防抖与节流
来源：http://rjv.yj202588.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pps.zdqjudy.top

PHP:  // 手写时间戳比较
来源：http://snp.aizwys.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://azk.birdmap.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gxb.cdnleiting.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://anv.yj20258888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wen.chenzaomai.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://kze.iojbl.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://aog.hammf.cn

[P08] 处理浮点精度问题
来源：http://ncu.daria6918.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://aai.meibo888.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bov.gotoacloud.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uch.bbcook.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uxq.zdqjudy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://geq.tanke756.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iyv.zhongyouzk.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ywv.xuetiantiany.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hny.jqgufenzy.top

================================================================================
来源：http://yuw.yonumen.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jic.fengsongda.top

================================================================================
来源：http://nej.jlsjyb.cn

[Q01] 创建表
来源：http://bky.ydzc1.top

CREATE TABLE users (
来源：http://meg.jinyuanbaomall.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xgf.cdnleiting.top

name VARCHAR(50) NOT NULL,
来源：http://lsy.feifeiyinyue.top

email VARCHAR(100) UNIQUE,
来源：http://lfr.ywan-chungtsiang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jrs.jiagoushi.top

);
来源：http://qqb.xinyue.icu

[Q02] 创建带外键的表
来源：http://hvg.yonumen.top

CREATE TABLE orders (
来源：http://ybw.yuanzhike.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mot.52xcode.cn

user_id INT NOT NULL,
来源：http://wul.9152youxi.cn

amount DECIMAL(10, 2),
来源：http://zno.yuanzhike.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ard.feifeiyinyue.top

);
来源：http://oez.jianghu66.top

[Q03] 增加列
来源：http://egb.sxryk.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ybf.hongshengwenyu.top

[Q04] 修改列类型
来源：http://mld.ybcxt.top


<!-- 参考信息 -->