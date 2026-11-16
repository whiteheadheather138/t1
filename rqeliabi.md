代发 wailian999

TS:   process.cwd()
来源：http://ijp.jqgufenzy.top

Java: Path.of("").toAbsolutePath()
来源：http://bvw.dashuyun.cn

Go:   os.Getwd()
来源：http://kre.chenzaomai.com

Ruby: Dir.pwd
来源：http://ydu.jinqigufen.top

C#:   Directory.GetCurrentDirectory()
来源：http://zyn.fengsongda.top

[M05] 设置退出码
来源：http://vly.svipenyu.cn

Py:   sys.exit(1)
来源：http://kqb.yueranfly.top

PHP:  exit(1);
来源：http://foc.nanxinkj.top

JS:   process.exit(1)
来源：http://cly.ppjwa.cn

TS:   process.exit(1)
来源：http://ugx.fanxiaobao.xyz

Java: System.exit(1)
来源：http://fkm.aizwys.cn

Go:   os.Exit(1)
来源：http://wmz.guowangkeji.top

Ruby: exit 1
来源：http://pfa.c1oappe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rtj.jinqigufen.top

[M06] 向标准错误输出
来源：http://cjc.hammf.cn

Py:   print("err", file=sys.stderr)
来源：http://kfv.quarkkingdee.top

PHP:  fwrite(STDERR, "err\n");
来源：http://yss.hesvh.cn

JS:   console.error("err")
来源：http://dmd.uphjek.com

TS:   console.error("err")
来源：http://xdt.fengsongda.top

Java: System.err.println("err")
来源：http://pps.daria6918.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tvj.jlsjyb.cn

Ruby: warn "err"
来源：http://eqr.dashuyun.cn

C#:   Console.Error.WriteLine("err")
来源：http://yjo.chenzaomai.com

[M07] 判断是否为主入口
来源：http://jmu.yongpay.top

Py:   if __name__ == "__main__":
来源：http://qid.yj20258.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bqh.yfazqb.com

JS:   require.main === module
来源：http://ikt.shzxlz.cn

TS:   require.main === module
来源：http://fqx.snrcjt.cn

Java: public static void main(String[] args)
来源：http://yof.yj20258.top

Go:   func main()
来源：http://ifd.ybcxt.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jdp.zhoulong.xyz

C#:   static void Main(string[] args)
来源：http://pck.fengsongda.top

[M08] 获取系统与运行时信息
来源：http://tex.ybcxt.top

Py:   platform.system();  platform.python_version()
来源：http://gmc.tarul.cn

PHP:  PHP_OS;  phpversion();
来源：http://sur.pycfn.com

JS:   process.platform;  process.version
来源：http://nul.shuidangran.top

TS:   process.platform;  process.version
来源：http://yzd.cdnleiting.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://evf.hywenlv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ccp.chenjidiqi.icu

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qma.aizwys.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://hfb.hesvh.cn

================================================================================
来源：http://dub.cqqwz.cn

N. 数据结构与算法
来源：http://wrz.ppjwa.cn

================================================================================
来源：http://lew.zhiwuduotai.top

[N01] 二分查找（有序数组）
来源：http://eoi.nanxinkj.top

Py:   bisect.bisect_left(arr, x)
来源：http://ztn.havefunace.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kgy.yj202588.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wrb.zdbjq.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pjr.c1oappe.top

Java: Arrays.binarySearch(arr, x)
来源：http://hve.ydjk.org.cn

Go:   sort.SearchInts(arr, x)
来源：http://iwg.daria6918.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lmd.fehbvm.com

C#:   Array.BinarySearch(arr, x)
来源：http://aqp.jinghuilouyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://bab.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://nos.yongpay.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://clh.wangshuangyany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://nal.xuanzx.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://hot.c1oappe.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rkr.yanxiufei.cn

Go:   slices.Sort(arr)
来源：http://odr.cucudq.cn

Ruby: arr.sort
来源：http://kib.yuxming.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ujl.zycfv.cn

[N03] 快速排序（分治示例）
来源：http://wju.zhengqikj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vzo.hywenlv.cn

PHP:  // 递归实现，或用 usort
来源：http://clp.sxryk.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yiq.hywenlv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nkr.hesvh.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nmo.cqqwz.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tux.cucudq.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fqf.birdmap.top

C#:   // 手写递归，或 Array.Sort
来源：http://nya.gzhubu.top

[N04] 斐波那契数列
来源：http://fvv.guannengcc.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gjc.jiagoushi.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://sik.shanyushiyangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qmf.tanke756.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zzy.cheryme.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xhz.ppjwa.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://twy.bbcook.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jjo.cheryme.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qbq.nwbrower.top

[N05] 最大公约数
来源：http://cqy.jiagoushi.top

Py:   math.gcd(a, b)
来源：http://cog.pengpengdd.cyou

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mkl.yj20258.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dvn.zhengqikj.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wfy.ehwqpu.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ago.bjfxy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fea.xziqi.cn

Ruby: a.gcd(b)
来源：http://ezr.chenzaomai.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://czb.pycfn.com

[N06] 判断回文字符串
来源：http://kos.shangyingyoupin.top

Py:   s == s[::-1]
来源：http://old.zdbjq.cn

PHP:  $s === strrev($s);
来源：http://fpc.shanyushiyangkeji.top

JS:   s === [...s].reverse().join("")
来源：http://ipa.dianchejie.cn

TS:   s === [...s].reverse().join("")
来源：http://mim.yanxiufei.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://azj.uphjek.com

Go:   // 双指针从两端比较
来源：http://xch.hcnkem.com

Ruby: s == s.reverse
来源：http://wre.yuxming.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hwh.jqgfzy.top

[N07] 两数之和（返回下标）
来源：http://lki.yangfankeji.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ggz.wangdashe.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ceb.vehdjk.com

JS:   // 手写 Map：map.set(v, i)
来源：http://bky.haohaochexian.top

TS:   // 手写 Map<string, number>
来源：http://wmg.c1oappe.top

Java: // 手写 HashMap
来源：http://wjl.shanyushiyangtech.top

Go:   // 手写 map[int]int
来源：http://yjk.shanyushiyangtech.top

Ruby: // 手写 Hash
来源：http://knb.jlsjyb.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ant.gzhubu.top

[N08] 生成全排列
来源：http://dme.uphjek.com

Py:   itertools.permutations(arr)
来源：http://glh.shanyushiyangkeji.top

PHP:  // 手写递归交换
来源：http://yqw.chenjidiqi.icu

JS:   // 手写回溯递归
来源：http://kyv.xinyue.icu

TS:   // 手写回溯递归
来源：http://ibj.sxryk.cn

Java: // 手写回溯递归
来源：http://fsd.xingfuxueyuan.xyz

Go:   // 手写回溯递归
来源：http://iwn.fzhhl.top

Ruby: arr.permutation.to_a
来源：http://dwt.jqgfzy.top

C#:   // 手写回溯递归
来源：http://wel.yvedp.cn

[N09] 栈与队列
来源：http://rxd.dianchejie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ayn.ydzc1.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ezu.shanyushiyangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qco.yonumen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yio.zhengqikj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zkw.shangyingyoupin.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bxo.wangdashe.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://czn.andypj.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ssw.pengpengdd.cyou

[N10] 链表节点定义
来源：http://eaf.jinqigfzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ohx.daria6918.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ysk.jinghuilouyu.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tro.hysaishi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pro.zhijiandao.cn

Java: class Node { int v; Node next; }
来源：http://xtz.hesvh.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lxw.chenjidiqi.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://fjd.gogol.net.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ljj.quarkkingdee.top

[N11] 二叉树中序遍历
来源：http://hah.cdnleiting.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zbb.yj20258.top

PHP:  // 手写递归函数
来源：http://ofl.aizwys.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sbh.feifeiyinyue.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hvr.feifeiyinyue.top

Java: // 手写递归
来源：http://nrr.cashguo.top

Go:   // 手写递归
来源：http://gdu.hfpthk.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ael.jinqigfzy.top

C#:   // 手写递归
来源：http://rar.yj20258888.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pau.shanyushiyangtech.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://avg.andypj.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hzy.cheryme.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ybb.c1oappe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://azp.ybcxt.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rra.aibaodan.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kve.yongpay.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hya.yvedp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bun.mhx1999.top

================================================================================
来源：http://tsm.xuanzx.com

O. 并发与异步
来源：http://wmt.vehdjk.com

================================================================================
来源：http://hmd.cdnleiting.top

[O01] 启动一个线程
来源：http://ayc.xylfe.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xoe.tianlin.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lbb.ydzc1.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sen.zhixingplan.top

TS:   // 同 JS
来源：http://oqp.zhixingplan.top

Java: new Thread(() -> f()).start()
来源：http://ekc.andypj.xyz

Go:   go f()
来源：http://zxp.cdnleiting.top

Ruby: Thread.new { f }
来源：http://apb.c1oappe.top

C#:   Task.Run(() => F());
来源：http://rae.hfpthk.cn

[O02] 使用线程池
来源：http://cmv.jianghu66.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yqw.xuetiantiany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bet.hysaishi.cn

JS:   // worker_threads 线程池
来源：http://ivf.shanyushiyangtech.top

TS:   // worker_threads 线程池
来源：http://sfn.andypj.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://sea.epnwcf.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mkc.nanxuanxn.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xpc.yanxiufei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mko.jinqigufen.top

[O03] 加锁保护共享数据
来源：http://mez.fktsv.cn

Py:   with lock: shared += 1
来源：http://hda.wangdashe.top

PHP:  // 用 flock() 做文件锁
来源：http://baq.quarkkingdee.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ifp.ydjk.org.cn

TS:   // 同 JS
来源：http://wms.xinyue.icu

Java: synchronized (this) { shared++; }
来源：http://gzh.shuidangran.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nuu.gaohongyu789.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ysj.ybcxt.top

C#:   lock (gate) { shared++; }
来源：http://rfc.gotoacloud.top

[O04] 定义异步函数并等待
来源：http://xbl.kuanghao11.cn

Py:   async def f():⏎    await g()
来源：http://ldv.yanxiufei.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ypt.zdqjudy.top

JS:   async function f() { await g(); }
来源：http://ich.jianghu66.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://axi.zdbjq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yns.zdbjq.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eyg.ivvv.top

Ruby: # 用 Fiber 或 async gem
来源：http://rvj.zhongyouzk.top

C#:   async Task F() { await G(); }
来源：http://www.chenzaomai.com

[O05] 并发执行并等待全部完成
来源：http://nmc.fzhhl.top

Py:   asyncio.gather(*tasks)
来源：http://dbs.sufxvd.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ndv.tanke756.top

JS:   await Promise.all(tasks)
来源：http://wzy.jinqigfzy.top

TS:   await Promise.all(tasks)
来源：http://lrs.jinqigufen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hzp.chenlongwang.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://udt.hnqzz.top

Ruby: threads.map(&:join)
来源：http://vaz.bbcook.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qsq.aizwys.cn

[O06] 使用进程池
来源：http://hax.sxryk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jbq.gogol.net.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zeg.xingfuxueyuan.xyz

JS:   // child_process / cluster 模块
来源：http://uie.fzhhl.top

TS:   // child_process / cluster 模块
来源：http://sle.nanxuanxn.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://swh.hnqzz.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ahx.sxryk.cn

Ruby: // fork 块
来源：http://gtl.yj20258888.top

C#:   Parallel.For
来源：http://otq.ctjpmb.com

================================================================================
来源：http://lpu.yongpay.top

P. 常用工具函数
来源：http://cez.cashguo.top

================================================================================
来源：http://llv.ehwqpu.com

[P01] 生成 UUID
来源：http://jts.nanxuanxn.top

Py:   str(uuid.uuid4())
来源：http://dvt.zhaomingkeji.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wul.ivvv.top

JS:   crypto.randomUUID()
来源：http://ytb.gotoacloud.top

TS:   crypto.randomUUID()
来源：http://fty.sxryk.cn

Java: UUID.randomUUID().toString()
来源：http://bwn.zhongyouzk.top

Go:   // 用 github.com/google/uuid
来源：http://gqw.yanxiufei.cn

Ruby: SecureRandom.uuid
来源：http://ikb.jinqigfzy.top

C#:   Guid.NewGuid().ToString()
来源：http://tie.sweek.top

[P02] MD5 / SHA256 摘要
来源：http://rwk.cheryme.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://acy.yj202588.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://uyu.bbcook.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zav.epnwcf.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bfh.52xcode.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lkx.kuanghao11.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://odx.yuxming.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iug.bbcook.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fcn.0kj1m.cn

[P03] 生成短随机字符串
来源：http://qde.fzhhl.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kku.sysykeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ycf.kuanghao11.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ixp.yongpay.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wbr.jianghu66.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pws.zhixingplan.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hzp.mhx1999.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://agv.shanyushiyangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jkk.ctjpmb.com

[P04] 求长度
来源：http://wev.feifeiyinyue.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jwo.jinyuanbaomall.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kki.birdmap.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://czq.bbcook.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vba.zhiwuduotai.top

Java: list.size();  map.size();  s.length()
来源：http://auq.ivvv.top

Go:   len(arr);  len(m)
来源：http://gdy.316326.xyz

Ruby: x.length;  x.size
来源：http://ubp.snrcjt.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cfv.yj20258888.top

[P05] 判断两个对象内容是否相等
来源：http://yqc.hammf.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rnp.pengpengdd.cyou

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lne.xingfuxueyuan.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qqw.hcnkem.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fzh.sufxvd.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zzz.52xcode.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kfy.ehwqpu.com

Ruby: a == b
来源：http://wbm.gzhubu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uxc.snrcjt.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qkw.ydzc1.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pvo.zhixingplan.top

PHP:  if (empty($x)) {}
来源：http://mjb.andypj.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aip.yanxiufei.cn

TS:   if (x == null) {}
来源：http://hgw.sysykeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://gbz.dianchejie.cn

Go:   if x == nil {}
来源：http://bsq.dianchejie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dby.dashuyun.cn

C#:   if (x is null) {}
来源：http://smv.tarul.cn

[P07] 防抖与节流
来源：http://lyt.fengsongda.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ulc.redwolf501.top

PHP:  // 手写时间戳比较
来源：http://xjq.jinyuanbaomall.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hyi.cqqwz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wsq.cashguo.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ywh.ydjk.org.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uft.quarkkingdee.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://svg.zhixingplan.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mmm.yuxming.cn

[P08] 处理浮点精度问题
来源：http://bde.xylfe.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jxv.hesvh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vex.kuanghao11.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hke.yongpay.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uae.aibaodan.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ntb.jlsjyb.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fvr.yvedp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xaw.jyoumei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jpe.sweek.top

================================================================================
来源：http://npt.jqgfzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ybh.feifeiyinyue.top

================================================================================
来源：http://yyu.gotoacloud.top

[Q01] 创建表
来源：http://avv.zhoulong.xyz

CREATE TABLE users (
来源：http://rnk.jinqigfzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bch.xylfe.cn

name VARCHAR(50) NOT NULL,
来源：http://egh.shuidangran.top

email VARCHAR(100) UNIQUE,
来源：http://jgj.zhiwuduotai.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kfq.jlsjyb.cn

);
来源：http://ayu.pengpengdd.cyou

[Q02] 创建带外键的表
来源：http://nqy.jinyuanbaomall.cn

CREATE TABLE orders (
来源：http://azp.cashguo.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lvu.cheryme.top

user_id INT NOT NULL,
来源：http://arf.ydzc1.top

amount DECIMAL(10, 2),
来源：http://pyy.xylfe.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xuh.hammf.cn


<!-- 参考信息 -->