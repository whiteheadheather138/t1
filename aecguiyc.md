代发 wailian999

[M04] 获取当前工作目录
来源：http://lcq.zdqjudy.top

Py:   os.getcwd()
来源：http://olc.jlsjyb.cn

PHP:  getcwd();
来源：http://nkw.nanxinkj.top

JS:   process.cwd()
来源：http://eqx.feifeiyinyue.top

TS:   process.cwd()
来源：http://ixd.cashguo.top

Java: Path.of("").toAbsolutePath()
来源：http://miw.aibaodan.cn

Go:   os.Getwd()
来源：http://xtg.dianchejie.cn

Ruby: Dir.pwd
来源：http://vki.wangshuangyany.cn

C#:   Directory.GetCurrentDirectory()
来源：http://lob.cashguo.top

[M05] 设置退出码
来源：http://ftz.chenzaomai.com

Py:   sys.exit(1)
来源：http://rnk.gaohongyu789.top

PHP:  exit(1);
来源：http://uex.ivvv.top

JS:   process.exit(1)
来源：http://rcy.shuidangran.top

TS:   process.exit(1)
来源：http://jom.52xcode.cn

Java: System.exit(1)
来源：http://gsr.cdnleiting.top

Go:   os.Exit(1)
来源：http://hwu.sweek.top

Ruby: exit 1
来源：http://spp.hcnkem.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xmv.yj20258.top

[M06] 向标准错误输出
来源：http://ldd.shangyingyoupin.top

Py:   print("err", file=sys.stderr)
来源：http://yvz.hnqzz.top

PHP:  fwrite(STDERR, "err\n");
来源：http://nen.svipenyu.cn

JS:   console.error("err")
来源：http://sth.jqgfzy.top

TS:   console.error("err")
来源：http://fko.fanxiaobao.xyz

Java: System.err.println("err")
来源：http://wee.c1oappe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lze.cheryme.top

Ruby: warn "err"
来源：http://jhm.hnqzz.top

C#:   Console.Error.WriteLine("err")
来源：http://foj.fehbvm.com

[M07] 判断是否为主入口
来源：http://ryd.iojbl.cn

Py:   if __name__ == "__main__":
来源：http://yay.smart0.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lzc.wangdashe.top

JS:   require.main === module
来源：http://rkh.gogol.net.cn

TS:   require.main === module
来源：http://wzq.zhoulong.xyz

Java: public static void main(String[] args)
来源：http://rvj.jianghu66.top

Go:   func main()
来源：http://fnl.epnwcf.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hkg.pycfn.com

C#:   static void Main(string[] args)
来源：http://doo.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://bej.shuidangran.top

Py:   platform.system();  platform.python_version()
来源：http://ivl.yongpay.top

PHP:  PHP_OS;  phpversion();
来源：http://rvx.jiagoushi.top

JS:   process.platform;  process.version
来源：http://bmp.hesvh.cn

TS:   process.platform;  process.version
来源：http://dli.bjfxy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rst.hysaishi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ttr.jinghuilouyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jbh.hammf.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://dut.xuanzx.com

================================================================================
来源：http://azo.shuidangran.top

N. 数据结构与算法
来源：http://dae.zdqjudy.top

================================================================================
来源：http://ooc.jinqigfzy.top

[N01] 二分查找（有序数组）
来源：http://yct.yonumen.top

Py:   bisect.bisect_left(arr, x)
来源：http://luo.316326.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rwb.hnxiangtu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xmn.yongpay.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tmf.quarkkingdee.top

Java: Arrays.binarySearch(arr, x)
来源：http://hug.sysykeji.top

Go:   sort.SearchInts(arr, x)
来源：http://eta.xinyue.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://otf.ybcxt.top

C#:   Array.BinarySearch(arr, x)
来源：http://igu.mhx1999.top

[N02] 排序（工程实践用内置实现）
来源：http://clt.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://nax.havefunace.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ydh.hfpthk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://mqx.zhengqikj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://edc.hammf.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kmm.dashuyun.cn

Go:   slices.Sort(arr)
来源：http://xtl.sweek.top

Ruby: arr.sort
来源：http://xus.yuanzhike.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://yfb.hammf.cn

[N03] 快速排序（分治示例）
来源：http://sem.redwolf501.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tjc.birdmap.top

PHP:  // 递归实现，或用 usort
来源：http://kqi.nanxinkj.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fcz.bjfxy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://slv.cheryme.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pew.pycfn.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ypc.chenzaomai.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wsw.zhoulong.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://fvw.yvedp.cn

[N04] 斐波那契数列
来源：http://qmn.guannengcc.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cjw.cheryme.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xtd.daxiang520.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ykr.xinyue.icu

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lbg.guowangkeji.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hkj.yueranfly.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://evn.wangshuangyany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://feh.yfazqb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://agf.nanxinkj.top

[N05] 最大公约数
来源：http://tuj.yonumen.top

Py:   math.gcd(a, b)
来源：http://chb.bjfxy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bzp.fehbvm.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hxy.zhoulong.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mez.zdbjq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vgo.quarkkingdee.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qas.jqgufenzy.top

Ruby: a.gcd(b)
来源：http://ejl.cqqwz.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zex.ivvv.top

[N06] 判断回文字符串
来源：http://idb.chenlongwang.top

Py:   s == s[::-1]
来源：http://vtm.nanxuanxn.top

PHP:  $s === strrev($s);
来源：http://uzq.zhaomingkeji.xyz

JS:   s === [...s].reverse().join("")
来源：http://kpl.tanke756.top

TS:   s === [...s].reverse().join("")
来源：http://uvz.feifeiyinyue.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zxq.pengpengdd.cyou

Go:   // 双指针从两端比较
来源：http://cha.zycfv.cn

Ruby: s == s.reverse
来源：http://hfh.tian-w.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bub.haohaochexian.top

[N07] 两数之和（返回下标）
来源：http://xzl.fengsongda.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dgp.yanxiufei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://crs.shanyushiyangkeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://uxf.zhengqikj.top

TS:   // 手写 Map<string, number>
来源：http://yec.fzhhl.top

Java: // 手写 HashMap
来源：http://ltp.yonumen.top

Go:   // 手写 map[int]int
来源：http://cql.svipenyu.cn

Ruby: // 手写 Hash
来源：http://ida.jiagoushi.top

C#:   // 手写 Dictionary<int, int>
来源：http://hti.daxiang520.top

[N08] 生成全排列
来源：http://xgl.c1oappe.top

Py:   itertools.permutations(arr)
来源：http://rux.dianchejie.cn

PHP:  // 手写递归交换
来源：http://yxr.guannengcc.top

JS:   // 手写回溯递归
来源：http://xtw.shzxlz.cn

TS:   // 手写回溯递归
来源：http://nlu.guannengcc.top

Java: // 手写回溯递归
来源：http://vdt.chenjidiqi.icu

Go:   // 手写回溯递归
来源：http://fpv.xziqi.cn

Ruby: arr.permutation.to_a
来源：http://rsg.yuanzhike.top

C#:   // 手写回溯递归
来源：http://dbf.hnqzz.top

[N09] 栈与队列
来源：http://oxe.guannengcc.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nnu.hnqzz.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wxt.guannengcc.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mwu.hysaishi.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://flv.hammf.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://pqq.ehwqpu.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zkx.hfpthk.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://dvl.jiagoushi.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iwk.52xcode.cn

[N10] 链表节点定义
来源：http://sie.xingfuxueyuan.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://alh.jinqigfzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://grs.birdmap.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fgk.ivvv.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fnj.vehdjk.com

Java: class Node { int v; Node next; }
来源：http://cqj.cucudq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://lou.jinqigufen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://spq.nanxinkj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gut.cheryme.top

[N11] 二叉树中序遍历
来源：http://wke.sxryk.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rov.epnwcf.com

PHP:  // 手写递归函数
来源：http://tnf.fanxiaobao.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gry.dianchejie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bna.xuetiantiany.cn

Java: // 手写递归
来源：http://nih.jqgufenzy.top

Go:   // 手写递归
来源：http://roe.chenjidiqi.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rvh.feifeiyinyue.top

C#:   // 手写递归
来源：http://ofn.gotoacloud.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aka.dianchejie.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qxc.jinqigufen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sdb.meibo888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nuc.chenjidiqi.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yja.9152youxi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rlp.hnxiangtu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://div.yj20258.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gbf.mhx1999.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dcc.zhixingplan.top

================================================================================
来源：http://ras.fktsv.cn

O. 并发与异步
来源：http://onw.daria6918.cn

================================================================================
来源：http://png.feifeiyinyue.top

[O01] 启动一个线程
来源：http://pmd.sweek.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mcg.xylfe.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mnv.ydzc1.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jsf.shanyushiyangtech.top

TS:   // 同 JS
来源：http://mhx.hywenlv.cn

Java: new Thread(() -> f()).start()
来源：http://auy.hesvh.cn

Go:   go f()
来源：http://crf.jyoumei.cn

Ruby: Thread.new { f }
来源：http://aaa.gaohongyu789.top

C#:   Task.Run(() => F());
来源：http://olb.fktsv.cn

[O02] 使用线程池
来源：http://bvx.ydzc1.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rbo.ydjk.org.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fbv.zhoulong.xyz

JS:   // worker_threads 线程池
来源：http://wxi.haohaochexian.top

TS:   // worker_threads 线程池
来源：http://stp.nanxuanxn.top

Java: Executors.newFixedThreadPool(4)
来源：http://aic.zhaomingkeji.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vbb.zhoulong.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rsv.hammf.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kxx.wangshuangyany.cn

[O03] 加锁保护共享数据
来源：http://dlo.birdmap.top

Py:   with lock: shared += 1
来源：http://jvf.wangshuangyany.cn

PHP:  // 用 flock() 做文件锁
来源：http://pge.fktsv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gey.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://rlm.cheryme.top

Java: synchronized (this) { shared++; }
来源：http://nzl.fanxiaobao.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gzw.epnwcf.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://ndu.havefunace.top

C#:   lock (gate) { shared++; }
来源：http://lzi.jianghu66.top

[O04] 定义异步函数并等待
来源：http://bbu.guowangkeji.top

Py:   async def f():⏎    await g()
来源：http://yuk.shangyingyoupin.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xuk.cqqwz.cn

JS:   async function f() { await g(); }
来源：http://oak.fengsongda.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vcz.fengsongda.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tdz.0kj1m.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zfe.yueranfly.top

Ruby: # 用 Fiber 或 async gem
来源：http://muo.zhengqikj.top

C#:   async Task F() { await G(); }
来源：http://zwb.pycfn.com

[O05] 并发执行并等待全部完成
来源：http://omx.yj202588.top

Py:   asyncio.gather(*tasks)
来源：http://rpi.shuidangran.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ywa.zhoulong.xyz

JS:   await Promise.all(tasks)
来源：http://ago.snrcjt.cn

TS:   await Promise.all(tasks)
来源：http://ffu.316326.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xqb.iojbl.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hiw.aizwys.cn

Ruby: threads.map(&:join)
来源：http://aaw.shzxlz.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ynt.xuetiantiany.cn

[O06] 使用进程池
来源：http://dbx.shanyushiyangtech.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://czm.chenlongwang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://vog.hesvh.cn

JS:   // child_process / cluster 模块
来源：http://dqb.ppjwa.cn

TS:   // child_process / cluster 模块
来源：http://qhv.aizwys.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wfj.andypj.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mzt.tanke756.top

Ruby: // fork 块
来源：http://elg.zhixingplan.top

C#:   Parallel.For
来源：http://fqi.hysaishi.cn

================================================================================
来源：http://nuy.vqdsnc.cn

P. 常用工具函数
来源：http://esk.jinghuilouyu.cn

================================================================================
来源：http://pjd.zhaomingkeji.xyz

[P01] 生成 UUID
来源：http://ymv.yuanzhike.top

Py:   str(uuid.uuid4())
来源：http://xpg.ydzc1.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fhr.fanxiaobao.xyz

JS:   crypto.randomUUID()
来源：http://lrk.sufxvd.cn

TS:   crypto.randomUUID()
来源：http://org.meibo888.top

Java: UUID.randomUUID().toString()
来源：http://ibs.redwolf501.top

Go:   // 用 github.com/google/uuid
来源：http://jaz.zhixingplan.top

Ruby: SecureRandom.uuid
来源：http://ttd.fengsongda.top

C#:   Guid.NewGuid().ToString()
来源：http://lmc.ppjwa.cn

[P02] MD5 / SHA256 摘要
来源：http://yml.bjfxy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://enl.yj202588.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jqb.hnqzz.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jop.sufxvd.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rma.wangdashe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tvp.ybcxt.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eqt.yfazqb.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dkn.birdmap.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sbz.jiagoushi.top

[P03] 生成短随机字符串
来源：http://uwf.shanyushiyangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://luo.jinyuanbaomall.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vsp.cqqwz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kdp.ybcxt.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mpv.jinyuanbaomall.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rwu.sweek.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nrv.daxiang520.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zsy.xylfe.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fej.sufxvd.cn

[P04] 求长度
来源：http://hkw.jlsjyb.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wgc.chenzaomai.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yob.yueranfly.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://swo.jiagoushi.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hle.mhx1999.top

Java: list.size();  map.size();  s.length()
来源：http://npn.fzhhl.top

Go:   len(arr);  len(m)
来源：http://kfs.yj202588.top

Ruby: x.length;  x.size
来源：http://rxh.cqqwz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://awm.tarul.cn

[P05] 判断两个对象内容是否相等
来源：http://rqj.havefunace.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://akn.jlsjyb.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ydh.quarkkingdee.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dhn.ivvv.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kjb.jianghu66.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://aee.xuanzx.com

Go:   reflect.DeepEqual(a, b)
来源：http://jkn.jinqigufen.top

Ruby: a == b
来源：http://ziv.vqdsnc.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qyh.ydjk.org.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pok.jinqigufen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bdz.nwbrower.top

PHP:  if (empty($x)) {}
来源：http://auw.quarkkingdee.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aup.bbcook.cn

TS:   if (x == null) {}
来源：http://tfd.yueranfly.top

Java: if (x == null || x.isEmpty()) {}
来源：http://niu.jlsjyb.cn

Go:   if x == nil {}
来源：http://dsf.zhiwuduotai.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nsc.jinqigfzy.top

C#:   if (x is null) {}
来源：http://ftc.guannengcc.top

[P07] 防抖与节流
来源：http://ulv.yfazqb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://usz.fktsv.cn

PHP:  // 手写时间戳比较
来源：http://qaq.hfpthk.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gjv.uphjek.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oit.pycfn.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tyu.hammf.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qgz.ydzc1.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ixp.cqqwz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dhj.tarul.cn

[P08] 处理浮点精度问题
来源：http://nmf.ydjk.org.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wfo.sxryk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vdc.hysaishi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yob.jqgufenzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://khv.haohaochexian.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ltg.shzxlz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mem.kuanghao11.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://juo.chenlongwang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://srk.cqqwz.cn

================================================================================
来源：http://lpt.ybcxt.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://foy.gaohongyu789.top

================================================================================
来源：http://way.zhijiandao.cn

[Q01] 创建表
来源：http://wgr.chenlongwang.top

CREATE TABLE users (
来源：http://sfv.jiagoushi.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wog.jyoumei.cn

name VARCHAR(50) NOT NULL,
来源：http://aob.tarul.cn

email VARCHAR(100) UNIQUE,
来源：http://qgk.ybcxt.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://flz.yangfankeji.com

);
来源：http://uhm.dianchejie.cn

[Q02] 创建带外键的表
来源：http://uzh.wangshuangyany.cn

CREATE TABLE orders (
来源：http://mhw.sweek.top


<!-- 参考信息 -->