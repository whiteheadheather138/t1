代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://jqw.meibo888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://spn.vqdsnc.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://fek.gzhubu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://lot.jinyuanbaomall.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nyn.sysykeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://vbs.shzxlz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rgk.hesvh.cn

C#:   Process.Start("ls", "-l");
来源：http://iqp.yuxming.cn

[M04] 获取当前工作目录
来源：http://kvh.ybcxt.top

Py:   os.getcwd()
来源：http://kph.hnxiangtu.top

PHP:  getcwd();
来源：http://ypz.zdbjq.cn

JS:   process.cwd()
来源：http://wch.yuanzhike.top

TS:   process.cwd()
来源：http://xdh.jqgufenzy.top

Java: Path.of("").toAbsolutePath()
来源：http://svr.vqdsnc.cn

Go:   os.Getwd()
来源：http://zcu.aibaodan.cn

Ruby: Dir.pwd
来源：http://aul.tanke756.top

C#:   Directory.GetCurrentDirectory()
来源：http://sxl.xuetiantiany.cn

[M05] 设置退出码
来源：http://myc.yonumen.top

Py:   sys.exit(1)
来源：http://scf.gaohongyu789.top

PHP:  exit(1);
来源：http://kvw.hongshengwenyu.top

JS:   process.exit(1)
来源：http://dyb.wangdashe.top

TS:   process.exit(1)
来源：http://osj.chenjidiqi.icu

Java: System.exit(1)
来源：http://jzp.ctjpmb.com

Go:   os.Exit(1)
来源：http://iwe.hongshengwenyu.top

Ruby: exit 1
来源：http://kys.xziqi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yvu.nanxinkj.top

[M06] 向标准错误输出
来源：http://owq.tanke756.top

Py:   print("err", file=sys.stderr)
来源：http://lci.zdbjq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fbx.havefunace.top

JS:   console.error("err")
来源：http://noc.chenzaomai.com

TS:   console.error("err")
来源：http://nvj.cqqwz.cn

Java: System.err.println("err")
来源：http://tcn.jqgufenzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cuu.yuxming.cn

Ruby: warn "err"
来源：http://una.hongshengwenyu.top

C#:   Console.Error.WriteLine("err")
来源：http://akw.zdqjudy.top

[M07] 判断是否为主入口
来源：http://ivo.sxryk.cn

Py:   if __name__ == "__main__":
来源：http://gaq.fzhhl.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rdt.jinghuilouyu.cn

JS:   require.main === module
来源：http://xvk.iojbl.cn

TS:   require.main === module
来源：http://rox.jlsjyb.cn

Java: public static void main(String[] args)
来源：http://mqg.meibo888.top

Go:   func main()
来源：http://xkq.yangfankeji.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jrc.ivvv.top

C#:   static void Main(string[] args)
来源：http://ygt.snrcjt.cn

[M08] 获取系统与运行时信息
来源：http://zdh.sweek.top

Py:   platform.system();  platform.python_version()
来源：http://vyi.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://vti.nanxuanxn.top

JS:   process.platform;  process.version
来源：http://ype.zhaomingkeji.xyz

TS:   process.platform;  process.version
来源：http://upi.fzhhl.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://drm.yueranfly.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://drf.jyoumei.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gyp.yongpay.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ohx.vehdjk.com

================================================================================
来源：http://lym.zhixingplan.top

N. 数据结构与算法
来源：http://fkl.gogol.net.cn

================================================================================
来源：http://jdt.aibaodan.cn

[N01] 二分查找（有序数组）
来源：http://oxc.haohaochexian.top

Py:   bisect.bisect_left(arr, x)
来源：http://klm.haohaochexian.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lak.xylfe.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uxe.andypj.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://buu.ctjpmb.com

Java: Arrays.binarySearch(arr, x)
来源：http://gcu.hcnkem.com

Go:   sort.SearchInts(arr, x)
来源：http://fjr.zhixingplan.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://kyu.yueranfly.top

C#:   Array.BinarySearch(arr, x)
来源：http://gbx.jiagoushi.top

[N02] 排序（工程实践用内置实现）
来源：http://dmz.dianchejie.cn

Py:   sorted(arr);  arr.sort()
来源：http://jbn.hnqzz.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kcl.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://ajq.jqgufenzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://yxv.hysaishi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gyo.cucudq.cn

Go:   slices.Sort(arr)
来源：http://uol.ehwqpu.com

Ruby: arr.sort
来源：http://wcu.zhengqikj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jql.cucudq.cn

[N03] 快速排序（分治示例）
来源：http://zcd.nwbrower.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kxc.zhaomingkeji.xyz

PHP:  // 递归实现，或用 usort
来源：http://zwy.tian-w.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fqg.0kj1m.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vox.cucudq.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://czw.yongpay.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rby.zhixingplan.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://phl.tianlin.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://qsa.sweek.top

[N04] 斐波那契数列
来源：http://grp.0kj1m.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://way.jlsjyb.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tca.snrcjt.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zrv.aizwys.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ipw.52xcode.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gzl.ydjk.org.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aqg.zhixingplan.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mfb.yanxiufei.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eal.shanyushiyangtech.top

[N05] 最大公约数
来源：http://ewl.316326.xyz

Py:   math.gcd(a, b)
来源：http://ycb.dianchejie.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dtu.fzhhl.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ojs.xuanzx.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jou.yueranfly.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baa.wangdashe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lrv.sysykeji.top

Ruby: a.gcd(b)
来源：http://nxt.svipenyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rct.shanyushiyangtech.top

[N06] 判断回文字符串
来源：http://vgc.yuanzhike.top

Py:   s == s[::-1]
来源：http://sfn.xziqi.cn

PHP:  $s === strrev($s);
来源：http://ful.tarul.cn

JS:   s === [...s].reverse().join("")
来源：http://rkm.shzxlz.cn

TS:   s === [...s].reverse().join("")
来源：http://sjm.gotoacloud.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://spy.haohaochexian.top

Go:   // 双指针从两端比较
来源：http://fcu.cdnleiting.top

Ruby: s == s.reverse
来源：http://ztw.zdqjudy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://yrq.tarul.cn

[N07] 两数之和（返回下标）
来源：http://lao.fengsongda.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dej.xuetiantiany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jvb.nanxinkj.top

JS:   // 手写 Map：map.set(v, i)
来源：http://hfk.gogol.net.cn

TS:   // 手写 Map<string, number>
来源：http://slg.ybcxt.top

Java: // 手写 HashMap
来源：http://tna.havefunace.top

Go:   // 手写 map[int]int
来源：http://nyl.zycfv.cn

Ruby: // 手写 Hash
来源：http://upt.cheryme.top

C#:   // 手写 Dictionary<int, int>
来源：http://rru.ctjpmb.com

[N08] 生成全排列
来源：http://dts.feifeiyinyue.top

Py:   itertools.permutations(arr)
来源：http://hyr.shuidangran.top

PHP:  // 手写递归交换
来源：http://utu.daria6918.cn

JS:   // 手写回溯递归
来源：http://ovh.fzhhl.top

TS:   // 手写回溯递归
来源：http://kcr.yvedp.cn

Java: // 手写回溯递归
来源：http://mqe.xingfuxueyuan.xyz

Go:   // 手写回溯递归
来源：http://lzi.uphjek.com

Ruby: arr.permutation.to_a
来源：http://tyb.aizwys.cn

C#:   // 手写回溯递归
来源：http://irn.hesvh.cn

[N09] 栈与队列
来源：http://wit.daxiang520.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://giv.andypj.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://lbx.wangdashe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ozp.zdbjq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rfl.iojbl.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://til.nwbrower.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wpp.quarkkingdee.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qbz.tarul.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tjo.hnqzz.top

[N10] 链表节点定义
来源：http://jot.cdnleiting.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bdl.cqqwz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ffc.zhongyouzk.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hsv.mhx1999.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qdc.sxryk.cn

Java: class Node { int v; Node next; }
来源：http://hrc.fanxiaobao.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://cjs.meibo888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xtb.hfpthk.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://cqe.shuidangran.top

[N11] 二叉树中序遍历
来源：http://hbe.bbcook.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://imh.redwolf501.top

PHP:  // 手写递归函数
来源：http://hls.epnwcf.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rwi.pycfn.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pby.hnxiangtu.top

Java: // 手写递归
来源：http://dyp.zdbjq.cn

Go:   // 手写递归
来源：http://ocw.gzhubu.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kam.ppjwa.cn

C#:   // 手写递归
来源：http://asw.fktsv.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://len.cheryme.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://haa.hammf.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wqz.meibo888.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mps.yj202588.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tja.nanxinkj.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ivz.fzhhl.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zoa.sxryk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lli.zhengqikj.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gry.vehdjk.com

================================================================================
来源：http://wli.yueranfly.top

O. 并发与异步
来源：http://yca.zdqjudy.top

================================================================================
来源：http://bnk.uphjek.com

[O01] 启动一个线程
来源：http://jou.zhaomingkeji.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fop.jinyuanbaomall.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vwg.redwolf501.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jwb.chenlongwang.top

TS:   // 同 JS
来源：http://tld.snrcjt.cn

Java: new Thread(() -> f()).start()
来源：http://hji.jinyuanbaomall.cn

Go:   go f()
来源：http://wsp.xziqi.cn

Ruby: Thread.new { f }
来源：http://chk.52xcode.cn

C#:   Task.Run(() => F());
来源：http://lht.epnwcf.com

[O02] 使用线程池
来源：http://ykr.daria6918.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qeu.yvedp.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mjs.guowangkeji.top

JS:   // worker_threads 线程池
来源：http://abw.birdmap.top

TS:   // worker_threads 线程池
来源：http://kua.shuidangran.top

Java: Executors.newFixedThreadPool(4)
来源：http://wnf.andypj.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rok.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eqm.xuanzx.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://atj.ydzc1.top

[O03] 加锁保护共享数据
来源：http://nzo.zhijiandao.cn

Py:   with lock: shared += 1
来源：http://bji.fktsv.cn

PHP:  // 用 flock() 做文件锁
来源：http://eou.yuxming.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://axa.havefunace.top

TS:   // 同 JS
来源：http://gsa.wangdashe.top

Java: synchronized (this) { shared++; }
来源：http://fwz.jinyuanbaomall.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://joo.wangshuangyany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://czc.bbcook.cn

C#:   lock (gate) { shared++; }
来源：http://vis.ydjk.org.cn

[O04] 定义异步函数并等待
来源：http://yje.hesvh.cn

Py:   async def f():⏎    await g()
来源：http://pjm.hcnkem.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dql.guowangkeji.top

JS:   async function f() { await g(); }
来源：http://yzi.ybcxt.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ndo.nanxuanxn.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vtt.hnqzz.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ksv.kuanghao11.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wov.aizwys.cn

C#:   async Task F() { await G(); }
来源：http://yhc.chenzaomai.com

[O05] 并发执行并等待全部完成
来源：http://nrv.yuxming.cn

Py:   asyncio.gather(*tasks)
来源：http://ete.ybcxt.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vvt.xylfe.cn

JS:   await Promise.all(tasks)
来源：http://all.jinqigfzy.top

TS:   await Promise.all(tasks)
来源：http://uxg.shangyingyoupin.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mfx.kuanghao11.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qyl.hammf.cn

Ruby: threads.map(&:join)
来源：http://svf.pengpengdd.cyou

C#:   await Task.WhenAll(t1, t2)
来源：http://qac.fanxiaobao.xyz

[O06] 使用进程池
来源：http://elv.hysaishi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pkv.daria6918.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nyr.yueranfly.top

JS:   // child_process / cluster 模块
来源：http://qlb.epnwcf.com

TS:   // child_process / cluster 模块
来源：http://kra.shuidangran.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fsc.zhongyouzk.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wvi.daria6918.cn

Ruby: // fork 块
来源：http://ixj.c1oappe.top

C#:   Parallel.For
来源：http://crp.fehbvm.com

================================================================================
来源：http://ijw.xylfe.cn

P. 常用工具函数
来源：http://cmq.zhengqikj.top

================================================================================
来源：http://pix.quarkkingdee.top

[P01] 生成 UUID
来源：http://oca.hnxiangtu.top

Py:   str(uuid.uuid4())
来源：http://ghw.hfpthk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://urz.jqgfzy.top

JS:   crypto.randomUUID()
来源：http://mbd.redwolf501.top

TS:   crypto.randomUUID()
来源：http://nor.yj20258.top

Java: UUID.randomUUID().toString()
来源：http://rpk.guannengcc.top

Go:   // 用 github.com/google/uuid
来源：http://nfo.jqgfzy.top

Ruby: SecureRandom.uuid
来源：http://dws.kuanghao11.cn

C#:   Guid.NewGuid().ToString()
来源：http://aop.9152youxi.cn

[P02] MD5 / SHA256 摘要
来源：http://fpv.havefunace.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://niz.quarkkingdee.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://pxm.aibaodan.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://saw.xziqi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bft.yonumen.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sfl.zhaomingkeji.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qdx.hnxiangtu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://waa.bjfxy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cof.meibo888.top

[P03] 生成短随机字符串
来源：http://elx.quarkkingdee.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://icu.jinyuanbaomall.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qch.mhx1999.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gnv.hysaishi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qwf.jinqigfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mjd.xuetiantiany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://guv.xziqi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lck.jqgufenzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xkh.yvedp.cn

[P04] 求长度
来源：http://mqa.daria6918.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://leg.vehdjk.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qmv.guannengcc.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dvf.zycfv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oqd.smart0.xyz

Java: list.size();  map.size();  s.length()
来源：http://mel.hnxiangtu.top

Go:   len(arr);  len(m)
来源：http://pwd.hongshengwenyu.top

Ruby: x.length;  x.size
来源：http://hyn.fehbvm.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://kwt.sweek.top

[P05] 判断两个对象内容是否相等
来源：http://mye.pycfn.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://cvg.nanxuanxn.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hkq.jinghuilouyu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ayd.fengsongda.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zmy.hnqzz.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gxa.zhongyouzk.top

Go:   reflect.DeepEqual(a, b)
来源：http://cjk.ctjpmb.com

Ruby: a == b
来源：http://wbj.ivvv.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://scy.nanxinkj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mur.jyoumei.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tex.vqdsnc.cn

PHP:  if (empty($x)) {}
来源：http://twe.pengpengdd.cyou

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wkv.yj20258.top

TS:   if (x == null) {}
来源：http://gii.ehwqpu.com

Java: if (x == null || x.isEmpty()) {}
来源：http://kjq.c1oappe.top

Go:   if x == nil {}
来源：http://afb.cheryme.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://idl.yj20258.top

C#:   if (x is null) {}
来源：http://adk.tanke756.top

[P07] 防抖与节流
来源：http://jav.redwolf501.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://inf.ydjk.org.cn

PHP:  // 手写时间戳比较
来源：http://opm.ydzc1.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lik.316326.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wug.shangyingyoupin.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mns.sysykeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rnl.cucudq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nlb.gaohongyu789.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xqy.quarkkingdee.top

[P08] 处理浮点精度问题
来源：http://nne.gotoacloud.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sdk.xingfuxueyuan.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qmv.jqgfzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wws.hfpthk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kvv.hysaishi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kxf.hywenlv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://coj.birdmap.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hdv.meibo888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tkv.nwbrower.top

================================================================================
来源：http://qhd.jlsjyb.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fel.wangshuangyany.cn

================================================================================
来源：http://qpd.fzhhl.top

[Q01] 创建表
来源：http://fpb.yonumen.top


<!-- 参考信息 -->