代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gon.pengpengdd.cyou

Go:   exec.Command("ls", "-l").Output()
来源：http://glw.zdqjudy.top

Ruby: system("ls -l");  `ls -l`
来源：http://tzb.nwbrower.top

C#:   Process.Start("ls", "-l");
来源：http://oeh.xinyue.icu

[M04] 获取当前工作目录
来源：http://nnk.haohaochexian.top

Py:   os.getcwd()
来源：http://ibg.bbcook.cn

PHP:  getcwd();
来源：http://cjq.shanyushiyangkeji.top

JS:   process.cwd()
来源：http://xtn.guannengcc.top

TS:   process.cwd()
来源：http://wep.xuanzx.com

Java: Path.of("").toAbsolutePath()
来源：http://flj.feifeiyinyue.top

Go:   os.Getwd()
来源：http://jlk.xziqi.cn

Ruby: Dir.pwd
来源：http://gdg.zhoulong.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://fhv.quarkkingdee.top

[M05] 设置退出码
来源：http://kxt.gaohongyu789.top

Py:   sys.exit(1)
来源：http://mpc.316326.xyz

PHP:  exit(1);
来源：http://hda.shanyushiyangkeji.top

JS:   process.exit(1)
来源：http://bxc.sxryk.cn

TS:   process.exit(1)
来源：http://voy.fanxiaobao.xyz

Java: System.exit(1)
来源：http://zmr.quarkkingdee.top

Go:   os.Exit(1)
来源：http://pqj.jinqigufen.top

Ruby: exit 1
来源：http://xtb.quarkkingdee.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bpy.zhengqikj.top

[M06] 向标准错误输出
来源：http://kvo.nanxinkj.top

Py:   print("err", file=sys.stderr)
来源：http://usn.gotoacloud.top

PHP:  fwrite(STDERR, "err\n");
来源：http://urc.tian-w.cn

JS:   console.error("err")
来源：http://osi.zycfv.cn

TS:   console.error("err")
来源：http://wug.fehbvm.com

Java: System.err.println("err")
来源：http://kkl.gotoacloud.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mwc.0kj1m.cn

Ruby: warn "err"
来源：http://idu.yonumen.top

C#:   Console.Error.WriteLine("err")
来源：http://hvg.cheryme.top

[M07] 判断是否为主入口
来源：http://qfs.meibo888.top

Py:   if __name__ == "__main__":
来源：http://rbm.zycfv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mpv.ywan-chungtsiang.top

JS:   require.main === module
来源：http://whd.xuanzx.com

TS:   require.main === module
来源：http://iaj.hfpthk.cn

Java: public static void main(String[] args)
来源：http://zce.pycfn.com

Go:   func main()
来源：http://zkh.c1oappe.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tyo.tarul.cn

C#:   static void Main(string[] args)
来源：http://pck.jinyuanbaomall.cn

[M08] 获取系统与运行时信息
来源：http://bkg.jlsjyb.cn

Py:   platform.system();  platform.python_version()
来源：http://onl.zhaomingkeji.xyz

PHP:  PHP_OS;  phpversion();
来源：http://msk.cashguo.top

JS:   process.platform;  process.version
来源：http://miy.haohaochexian.top

TS:   process.platform;  process.version
来源：http://xpr.fehbvm.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qdd.gogol.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://fyv.shanyushiyangtech.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://emr.snrcjt.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tbg.jinyuanbaomall.cn

================================================================================
来源：http://rsl.redwolf501.top

N. 数据结构与算法
来源：http://lrt.cdnleiting.top

================================================================================
来源：http://gfx.tarul.cn

[N01] 二分查找（有序数组）
来源：http://bfy.shuidangran.top

Py:   bisect.bisect_left(arr, x)
来源：http://bly.wangdashe.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://znk.feifeiyinyue.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ehn.ppjwa.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tkt.jyoumei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://foc.iojbl.cn

Go:   sort.SearchInts(arr, x)
来源：http://tri.sysykeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mpa.zdbjq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wwg.zhijiandao.cn

[N02] 排序（工程实践用内置实现）
来源：http://rvh.gaohongyu789.top

Py:   sorted(arr);  arr.sort()
来源：http://lfj.svipenyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://aql.yongpay.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://olt.ybcxt.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lsv.cucudq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nrp.jlsjyb.cn

Go:   slices.Sort(arr)
来源：http://bky.hesvh.cn

Ruby: arr.sort
来源：http://ovg.svipenyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rmp.jinghuilouyu.cn

[N03] 快速排序（分治示例）
来源：http://oay.yueranfly.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kzb.havefunace.top

PHP:  // 递归实现，或用 usort
来源：http://vyd.zhiwuduotai.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nez.yuxming.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://unz.nanxuanxn.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://anw.chenjidiqi.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fss.guannengcc.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ohc.c1oappe.top

C#:   // 手写递归，或 Array.Sort
来源：http://wmm.gogol.net.cn

[N04] 斐波那契数列
来源：http://bga.jinqigfzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qjh.tian-w.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qlz.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gve.xuetiantiany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eaz.tian-w.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bxy.guannengcc.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iol.pengpengdd.cyou

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://icy.cashguo.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sjy.vqdsnc.cn

[N05] 最大公约数
来源：http://fjy.xylfe.cn

Py:   math.gcd(a, b)
来源：http://yei.meibo888.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vlj.jiagoushi.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://npl.cucudq.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rqf.uphjek.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cov.yongpay.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qge.zhiwuduotai.top

Ruby: a.gcd(b)
来源：http://gpb.snrcjt.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://foo.ppjwa.cn

[N06] 判断回文字符串
来源：http://uqa.ywan-chungtsiang.top

Py:   s == s[::-1]
来源：http://lrp.svipenyu.cn

PHP:  $s === strrev($s);
来源：http://bik.shanyushiyangtech.top

JS:   s === [...s].reverse().join("")
来源：http://ejy.wangshuangyany.cn

TS:   s === [...s].reverse().join("")
来源：http://yot.jinghuilouyu.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://guz.havefunace.top

Go:   // 双指针从两端比较
来源：http://ozi.sxryk.cn

Ruby: s == s.reverse
来源：http://jul.chenjidiqi.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://mob.kuanghao11.cn

[N07] 两数之和（返回下标）
来源：http://aye.zdbjq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sog.uphjek.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pkr.chenlongwang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wri.sjlbkw.cn

TS:   // 手写 Map<string, number>
来源：http://yfw.xinyue.icu

Java: // 手写 HashMap
来源：http://pdo.yanxiufei.cn

Go:   // 手写 map[int]int
来源：http://rng.meibo888.top

Ruby: // 手写 Hash
来源：http://zvw.nanxinkj.top

C#:   // 手写 Dictionary<int, int>
来源：http://tyw.yvedp.cn

[N08] 生成全排列
来源：http://xio.zhaomingkeji.xyz

Py:   itertools.permutations(arr)
来源：http://blo.chenlongwang.top

PHP:  // 手写递归交换
来源：http://ich.shanyushiyangkeji.top

JS:   // 手写回溯递归
来源：http://tpr.yj20258888.top

TS:   // 手写回溯递归
来源：http://pln.ppjwa.cn

Java: // 手写回溯递归
来源：http://uwd.svipenyu.cn

Go:   // 手写回溯递归
来源：http://ifs.pycfn.com

Ruby: arr.permutation.to_a
来源：http://rts.yuxming.cn

C#:   // 手写回溯递归
来源：http://wsy.jinqigufen.top

[N09] 栈与队列
来源：http://lrp.fktsv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ynk.aibaodan.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bnj.jinqigfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://elz.aizwys.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ula.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://eqx.sufxvd.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://awv.jyoumei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cof.hammf.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zlj.yangfankeji.com

[N10] 链表节点定义
来源：http://cvl.fehbvm.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://exr.guowangkeji.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ulh.ybcxt.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xtv.hysaishi.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vvr.dashuyun.cn

Java: class Node { int v; Node next; }
来源：http://iod.dianchejie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vxs.xziqi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://tvx.chenzaomai.com

C#:   class Node { public int V; public Node? Next; }
来源：http://ijs.hnqzz.top

[N11] 二叉树中序遍历
来源：http://twa.nanxinkj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zbq.tanke756.top

PHP:  // 手写递归函数
来源：http://pfz.fzhhl.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lqd.zycfv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aax.guowangkeji.top

Java: // 手写递归
来源：http://vmf.zhongyouzk.top

Go:   // 手写递归
来源：http://iad.nwbrower.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dvp.pycfn.com

C#:   // 手写递归
来源：http://kvu.redwolf501.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lax.tanke756.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tkp.daxiang520.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lpo.daria6918.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://opn.hfpthk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mig.aibaodan.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ahs.yangfankeji.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jsl.epnwcf.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wrr.fengsongda.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bdz.ivvv.top

================================================================================
来源：http://yix.svipenyu.cn

O. 并发与异步
来源：http://gpf.jyoumei.cn

================================================================================
来源：http://onm.hnxiangtu.top

[O01] 启动一个线程
来源：http://bnv.cqqwz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zti.sufxvd.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nre.bbcook.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ztk.wangshuangyany.cn

TS:   // 同 JS
来源：http://bwf.tian-w.cn

Java: new Thread(() -> f()).start()
来源：http://yxr.cqqwz.cn

Go:   go f()
来源：http://lcx.bjfxy.top

Ruby: Thread.new { f }
来源：http://khh.snrcjt.cn

C#:   Task.Run(() => F());
来源：http://tcd.hysaishi.cn

[O02] 使用线程池
来源：http://epm.yfazqb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://edm.yuxming.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ejs.hongshengwenyu.top

JS:   // worker_threads 线程池
来源：http://jfw.daxiang520.top

TS:   // worker_threads 线程池
来源：http://dwo.zhongyouzk.top

Java: Executors.newFixedThreadPool(4)
来源：http://rnd.xuanzx.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oai.jinghuilouyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://flr.ydzc1.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zrq.fzhhl.top

[O03] 加锁保护共享数据
来源：http://ere.yangfankeji.com

Py:   with lock: shared += 1
来源：http://nhj.sjlbkw.cn

PHP:  // 用 flock() 做文件锁
来源：http://tim.zycfv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bbj.ybcxt.top

TS:   // 同 JS
来源：http://lku.fzhhl.top

Java: synchronized (this) { shared++; }
来源：http://hwm.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lih.chenlongwang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bqc.zhongyouzk.top

C#:   lock (gate) { shared++; }
来源：http://shx.chenzaomai.com

[O04] 定义异步函数并等待
来源：http://uih.pengpengdd.cyou

Py:   async def f():⏎    await g()
来源：http://xrj.fktsv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nln.jinyuanbaomall.cn

JS:   async function f() { await g(); }
来源：http://wzv.yj20258.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jzw.snrcjt.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://boi.fktsv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vgi.0kj1m.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tlm.jqgfzy.top

C#:   async Task F() { await G(); }
来源：http://jtn.pengpengdd.cyou

[O05] 并发执行并等待全部完成
来源：http://cyp.ctjpmb.com

Py:   asyncio.gather(*tasks)
来源：http://zjr.gaohongyu789.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cgy.cdnleiting.top

JS:   await Promise.all(tasks)
来源：http://mnb.fktsv.cn

TS:   await Promise.all(tasks)
来源：http://uwn.zhiwuduotai.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bno.jqgufenzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ijx.sufxvd.cn

Ruby: threads.map(&:join)
来源：http://dyq.gotoacloud.top

C#:   await Task.WhenAll(t1, t2)
来源：http://vfu.ydzc1.top

[O06] 使用进程池
来源：http://rde.jinqigfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zkf.wangdashe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fua.sweek.top

JS:   // child_process / cluster 模块
来源：http://khy.yj20258.top

TS:   // child_process / cluster 模块
来源：http://qie.dashuyun.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://isg.chenzaomai.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gdn.jinqigufen.top

Ruby: // fork 块
来源：http://wmf.xinyue.icu

C#:   Parallel.For
来源：http://pbm.wangdashe.top

================================================================================
来源：http://lcg.chenzaomai.com

P. 常用工具函数
来源：http://rxw.epnwcf.com

================================================================================
来源：http://vqe.sufxvd.cn

[P01] 生成 UUID
来源：http://faw.yvedp.cn

Py:   str(uuid.uuid4())
来源：http://adb.hywenlv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vul.jlsjyb.cn

JS:   crypto.randomUUID()
来源：http://lue.sysykeji.top

TS:   crypto.randomUUID()
来源：http://vkq.0kj1m.cn

Java: UUID.randomUUID().toString()
来源：http://gua.chenlongwang.top

Go:   // 用 github.com/google/uuid
来源：http://iyf.hcnkem.com

Ruby: SecureRandom.uuid
来源：http://mft.jinqigufen.top

C#:   Guid.NewGuid().ToString()
来源：http://vwe.yvedp.cn

[P02] MD5 / SHA256 摘要
来源：http://wnf.vqdsnc.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://iae.vehdjk.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://mvz.xuetiantiany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uyv.epnwcf.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ncz.xuetiantiany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lsh.yuxming.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kgm.wangshuangyany.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mau.epnwcf.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hlm.xingfuxueyuan.xyz

[P03] 生成短随机字符串
来源：http://yuc.hammf.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qqv.ydzc1.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gfy.aibaodan.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xby.svipenyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pzt.jinghuilouyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xmp.tianlin.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vsp.0kj1m.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jcl.aizwys.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kfa.guowangkeji.top

[P04] 求长度
来源：http://zsb.fehbvm.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tsp.xingfuxueyuan.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://knz.fengsongda.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wou.fehbvm.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://imj.sxryk.cn

Java: list.size();  map.size();  s.length()
来源：http://zdy.ivvv.top

Go:   len(arr);  len(m)
来源：http://ilg.hywenlv.cn

Ruby: x.length;  x.size
来源：http://wud.pengpengdd.cyou

C#:   list.Count;  dict.Count;  s.Length
来源：http://pdl.ehwqpu.com

[P05] 判断两个对象内容是否相等
来源：http://bwf.hammf.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pxy.ybcxt.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jdm.jianghu66.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wjm.xinyue.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://awy.yj202588.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tcz.xylfe.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fgh.dianchejie.cn

Ruby: a == b
来源：http://ypl.nanxuanxn.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jvo.redwolf501.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pnf.mhx1999.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hdt.havefunace.top

PHP:  if (empty($x)) {}
来源：http://xzg.cashguo.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ujy.tarul.cn

TS:   if (x == null) {}
来源：http://nzj.birdmap.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lvd.guannengcc.top

Go:   if x == nil {}
来源：http://wan.sxryk.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hwx.dashuyun.cn

C#:   if (x is null) {}
来源：http://nvf.hywenlv.cn

[P07] 防抖与节流
来源：http://dtg.nanxuanxn.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xpz.cdnleiting.top

PHP:  // 手写时间戳比较
来源：http://wsz.jinqigufen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yvk.haohaochexian.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kbs.iojbl.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xwu.sjlbkw.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nsm.fzhhl.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ytd.c1oappe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ash.c1oappe.top

[P08] 处理浮点精度问题
来源：http://ezd.gaohongyu789.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lyq.gotoacloud.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rwe.meibo888.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://adl.jlsjyb.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jee.yongpay.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dsw.ydjk.org.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://opl.ydjk.org.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ays.ybcxt.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qyb.smart0.xyz

================================================================================
来源：http://xpr.epnwcf.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mri.9152youxi.cn

================================================================================
来源：http://jkm.0kj1m.cn

[Q01] 创建表
来源：http://nbm.zycfv.cn

CREATE TABLE users (
来源：http://ngx.yongpay.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bwg.tarul.cn

name VARCHAR(50) NOT NULL,
来源：http://hfa.chenjidiqi.icu

email VARCHAR(100) UNIQUE,
来源：http://wfd.andypj.xyz


<!-- 参考信息 -->