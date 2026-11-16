代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yyl.zdbjq.cn

Ruby: ENV["HOME"]
来源：http://zhv.hfpthk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xud.pengpengdd.cyou

[M03] 执行外部命令
来源：http://nwa.cucudq.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rdv.ybcxt.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fcb.xingfuxueyuan.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://yxg.epnwcf.com

TS:   child_process.execSync("ls -l").toString()
来源：http://wkz.hcnkem.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qdg.aizwys.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dvt.chenlongwang.top

Ruby: system("ls -l");  `ls -l`
来源：http://dnj.tianlin.xyz

C#:   Process.Start("ls", "-l");
来源：http://mrm.jinqigufen.top

[M04] 获取当前工作目录
来源：http://soy.0kj1m.cn

Py:   os.getcwd()
来源：http://nix.jinghuilouyu.cn

PHP:  getcwd();
来源：http://zjr.zdbjq.cn

JS:   process.cwd()
来源：http://xwv.fzhhl.top

TS:   process.cwd()
来源：http://xgq.hywenlv.cn

Java: Path.of("").toAbsolutePath()
来源：http://mxp.meibo888.top

Go:   os.Getwd()
来源：http://eqh.tian-w.cn

Ruby: Dir.pwd
来源：http://lfr.hnxiangtu.top

C#:   Directory.GetCurrentDirectory()
来源：http://fsu.guannengcc.top

[M05] 设置退出码
来源：http://kyp.gogol.net.cn

Py:   sys.exit(1)
来源：http://jtx.birdmap.top

PHP:  exit(1);
来源：http://qhf.cucudq.cn

JS:   process.exit(1)
来源：http://occ.kuanghao11.cn

TS:   process.exit(1)
来源：http://olr.yj20258888.top

Java: System.exit(1)
来源：http://kxd.tianlin.xyz

Go:   os.Exit(1)
来源：http://ust.redwolf501.top

Ruby: exit 1
来源：http://qbv.cucudq.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ixs.yueranfly.top

[M06] 向标准错误输出
来源：http://usy.vehdjk.com

Py:   print("err", file=sys.stderr)
来源：http://jbd.zhengqikj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://zxn.9152youxi.cn

JS:   console.error("err")
来源：http://ese.0kj1m.cn

TS:   console.error("err")
来源：http://sni.yuxming.cn

Java: System.err.println("err")
来源：http://yxf.hysaishi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mjq.ctjpmb.com

Ruby: warn "err"
来源：http://ipu.birdmap.top

C#:   Console.Error.WriteLine("err")
来源：http://rag.0kj1m.cn

[M07] 判断是否为主入口
来源：http://zip.uphjek.com

Py:   if __name__ == "__main__":
来源：http://gna.ivvv.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mxm.xylfe.cn

JS:   require.main === module
来源：http://ehc.aibaodan.cn

TS:   require.main === module
来源：http://odq.cashguo.top

Java: public static void main(String[] args)
来源：http://pgs.ywan-chungtsiang.top

Go:   func main()
来源：http://fxl.zhongyouzk.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jvy.andypj.xyz

C#:   static void Main(string[] args)
来源：http://zte.wangshuangyany.cn

[M08] 获取系统与运行时信息
来源：http://qmi.mhx1999.top

Py:   platform.system();  platform.python_version()
来源：http://wir.shanyushiyangtech.top

PHP:  PHP_OS;  phpversion();
来源：http://mif.cqqwz.cn

JS:   process.platform;  process.version
来源：http://fcx.xinyue.icu

TS:   process.platform;  process.version
来源：http://ulv.vehdjk.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fnt.nanxuanxn.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tvx.haohaochexian.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dee.9152youxi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://rxt.hnqzz.top

================================================================================
来源：http://ksx.tian-w.cn

N. 数据结构与算法
来源：http://gvd.gogol.net.cn

================================================================================
来源：http://eaf.hnxiangtu.top

[N01] 二分查找（有序数组）
来源：http://jpg.fehbvm.com

Py:   bisect.bisect_left(arr, x)
来源：http://dvc.fzhhl.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qjk.pengpengdd.cyou

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://plf.feifeiyinyue.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xko.feifeiyinyue.top

Java: Arrays.binarySearch(arr, x)
来源：http://qrf.wangshuangyany.cn

Go:   sort.SearchInts(arr, x)
来源：http://xlt.shangyingyoupin.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zaz.yuanzhike.top

C#:   Array.BinarySearch(arr, x)
来源：http://twn.shuidangran.top

[N02] 排序（工程实践用内置实现）
来源：http://jja.0kj1m.cn

Py:   sorted(arr);  arr.sort()
来源：http://liv.hnxiangtu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ybn.fehbvm.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://ryl.pycfn.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://zds.fzhhl.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bki.gzhubu.top

Go:   slices.Sort(arr)
来源：http://dvn.zhijiandao.cn

Ruby: arr.sort
来源：http://jut.fanxiaobao.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://mse.yongpay.top

[N03] 快速排序（分治示例）
来源：http://eqb.bbcook.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ihh.svipenyu.cn

PHP:  // 递归实现，或用 usort
来源：http://ksx.xinyue.icu

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rco.haohaochexian.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dkd.jqgfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jlr.zhaomingkeji.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rco.zhaomingkeji.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mys.yfazqb.com

C#:   // 手写递归，或 Array.Sort
来源：http://uxl.fzhhl.top

[N04] 斐波那契数列
来源：http://rdz.wangshuangyany.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://epl.uphjek.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://oag.yfazqb.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://msa.hongshengwenyu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xsy.snrcjt.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://waq.hnqzz.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rrl.316326.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pax.andypj.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://nvk.ehwqpu.com

[N05] 最大公约数
来源：http://hay.zhoulong.xyz

Py:   math.gcd(a, b)
来源：http://tkm.yj20258.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ucc.aizwys.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rgz.jyoumei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jug.yanxiufei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ruj.shzxlz.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://sko.wangshuangyany.cn

Ruby: a.gcd(b)
来源：http://smc.dianchejie.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pdd.zhoulong.xyz

[N06] 判断回文字符串
来源：http://yuy.yangfankeji.com

Py:   s == s[::-1]
来源：http://aiu.ppjwa.cn

PHP:  $s === strrev($s);
来源：http://dsf.316326.xyz

JS:   s === [...s].reverse().join("")
来源：http://ncg.vehdjk.com

TS:   s === [...s].reverse().join("")
来源：http://vax.mhx1999.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xrn.chenlongwang.top

Go:   // 双指针从两端比较
来源：http://ewi.tanke756.top

Ruby: s == s.reverse
来源：http://vcf.316326.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://iav.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://feu.zdbjq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uog.shzxlz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pwp.ydzc1.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tgv.ydzc1.top

TS:   // 手写 Map<string, number>
来源：http://qgd.hysaishi.cn

Java: // 手写 HashMap
来源：http://mgh.zhixingplan.top

Go:   // 手写 map[int]int
来源：http://buq.aibaodan.cn

Ruby: // 手写 Hash
来源：http://hau.ywan-chungtsiang.top

C#:   // 手写 Dictionary<int, int>
来源：http://tht.wangshuangyany.cn

[N08] 生成全排列
来源：http://knu.wangdashe.top

Py:   itertools.permutations(arr)
来源：http://rrk.jqgfzy.top

PHP:  // 手写递归交换
来源：http://fto.shangyingyoupin.top

JS:   // 手写回溯递归
来源：http://dhs.dianchejie.cn

TS:   // 手写回溯递归
来源：http://ftm.gotoacloud.top

Java: // 手写回溯递归
来源：http://zvr.dianchejie.cn

Go:   // 手写回溯递归
来源：http://dmx.hnqzz.top

Ruby: arr.permutation.to_a
来源：http://yzd.ydjk.org.cn

C#:   // 手写回溯递归
来源：http://joq.haohaochexian.top

[N09] 栈与队列
来源：http://sno.cucudq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hdi.nanxuanxn.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tjx.fehbvm.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sxo.gaohongyu789.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vyj.cucudq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ocv.mhx1999.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ytw.ydzc1.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://khe.chenjidiqi.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sex.xuetiantiany.cn

[N10] 链表节点定义
来源：http://doa.feifeiyinyue.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://prx.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://cee.hysaishi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qcu.jinqigfzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kgw.hnqzz.top

Java: class Node { int v; Node next; }
来源：http://jvx.havefunace.top

Go:   type Node struct { V int; Next *Node }
来源：http://djv.sxryk.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fdr.zhengqikj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gax.kuanghao11.cn

[N11] 二叉树中序遍历
来源：http://zes.wangshuangyany.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cul.vqdsnc.cn

PHP:  // 手写递归函数
来源：http://syd.hywenlv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ilc.nanxinkj.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ccx.jinqigfzy.top

Java: // 手写递归
来源：http://dmv.jinghuilouyu.cn

Go:   // 手写递归
来源：http://wav.ydzc1.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://azg.vehdjk.com

C#:   // 手写递归
来源：http://yjs.cashguo.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jsr.yangfankeji.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nvl.redwolf501.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xin.0kj1m.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://emx.chenlongwang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fzp.iojbl.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wgw.shzxlz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zwe.jinqigufen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ogg.yongpay.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://oni.tarul.cn

================================================================================
来源：http://izd.wangshuangyany.cn

O. 并发与异步
来源：http://wap.hcnkem.com

================================================================================
来源：http://mhs.cqqwz.cn

[O01] 启动一个线程
来源：http://zjl.mhx1999.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kvo.9152youxi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jsm.tian-w.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://llt.ybcxt.top

TS:   // 同 JS
来源：http://avs.zdqjudy.top

Java: new Thread(() -> f()).start()
来源：http://cfl.sysykeji.top

Go:   go f()
来源：http://cgo.kuanghao11.cn

Ruby: Thread.new { f }
来源：http://lci.hesvh.cn

C#:   Task.Run(() => F());
来源：http://zqv.0kj1m.cn

[O02] 使用线程池
来源：http://pwe.xingfuxueyuan.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://auv.xziqi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pfx.shanyushiyangtech.top

JS:   // worker_threads 线程池
来源：http://rvg.birdmap.top

TS:   // worker_threads 线程池
来源：http://lla.zhaomingkeji.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://nev.0kj1m.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gte.yueranfly.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://apm.shzxlz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hwd.yanxiufei.cn

[O03] 加锁保护共享数据
来源：http://vgx.zhongyouzk.top

Py:   with lock: shared += 1
来源：http://gvy.52xcode.cn

PHP:  // 用 flock() 做文件锁
来源：http://vnl.aizwys.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ryr.tanke756.top

TS:   // 同 JS
来源：http://nzm.snrcjt.cn

Java: synchronized (this) { shared++; }
来源：http://spb.shanyushiyangtech.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mfr.dianchejie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://hfk.aibaodan.cn

C#:   lock (gate) { shared++; }
来源：http://ozc.dashuyun.cn

[O04] 定义异步函数并等待
来源：http://wkk.xziqi.cn

Py:   async def f():⏎    await g()
来源：http://sxd.meibo888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vok.xylfe.cn

JS:   async function f() { await g(); }
来源：http://xzd.birdmap.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rbs.cashguo.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pff.tanke756.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fry.tanke756.top

Ruby: # 用 Fiber 或 async gem
来源：http://jyc.redwolf501.top

C#:   async Task F() { await G(); }
来源：http://xas.ydzc1.top

[O05] 并发执行并等待全部完成
来源：http://pfs.sjlbkw.cn

Py:   asyncio.gather(*tasks)
来源：http://tnw.yuxming.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://imt.aibaodan.cn

JS:   await Promise.all(tasks)
来源：http://ltb.sufxvd.cn

TS:   await Promise.all(tasks)
来源：http://zyd.bjfxy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kja.kuanghao11.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ris.zhongyouzk.top

Ruby: threads.map(&:join)
来源：http://unl.daxiang520.top

C#:   await Task.WhenAll(t1, t2)
来源：http://gix.zdbjq.cn

[O06] 使用进程池
来源：http://opa.hnqzz.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ovq.jinyuanbaomall.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zky.hnxiangtu.top

JS:   // child_process / cluster 模块
来源：http://xyd.sysykeji.top

TS:   // child_process / cluster 模块
来源：http://csm.cucudq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wlx.xylfe.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hqt.shanyushiyangtech.top

Ruby: // fork 块
来源：http://xhr.jqgfzy.top

C#:   Parallel.For
来源：http://rje.fehbvm.com

================================================================================
来源：http://meb.yueranfly.top

P. 常用工具函数
来源：http://phe.cdnleiting.top

================================================================================
来源：http://kwt.smart0.xyz

[P01] 生成 UUID
来源：http://osr.zhengqikj.top

Py:   str(uuid.uuid4())
来源：http://sem.wangshuangyany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vdv.jianghu66.top

JS:   crypto.randomUUID()
来源：http://xrr.bjfxy.top

TS:   crypto.randomUUID()
来源：http://zah.nwbrower.top

Java: UUID.randomUUID().toString()
来源：http://vgv.zhiwuduotai.top

Go:   // 用 github.com/google/uuid
来源：http://ebf.zhoulong.xyz

Ruby: SecureRandom.uuid
来源：http://tgc.hysaishi.cn

C#:   Guid.NewGuid().ToString()
来源：http://pwo.ctjpmb.com

[P02] MD5 / SHA256 摘要
来源：http://epz.havefunace.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wbf.epnwcf.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://czq.jiagoushi.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lpe.gaohongyu789.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tmg.zycfv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yte.zdqjudy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ohk.yj20258888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gsh.snrcjt.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cnw.xziqi.cn

[P03] 生成短随机字符串
来源：http://rab.birdmap.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vlf.yongpay.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kbu.epnwcf.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://boo.bjfxy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://drh.hesvh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ocf.gogol.net.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fle.hnxiangtu.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zrw.hywenlv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jwe.yonumen.top

[P04] 求长度
来源：http://vyx.ehwqpu.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nka.ydzc1.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gzu.xylfe.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zty.wangdashe.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://enl.shanyushiyangtech.top

Java: list.size();  map.size();  s.length()
来源：http://feo.shangyingyoupin.top

Go:   len(arr);  len(m)
来源：http://xgw.pengpengdd.cyou

Ruby: x.length;  x.size
来源：http://aqc.nanxinkj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://rne.jianghu66.top

[P05] 判断两个对象内容是否相等
来源：http://hev.hysaishi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qxo.epnwcf.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ipp.tianlin.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ixz.vehdjk.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qna.daria6918.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zxt.yangfankeji.com

Go:   reflect.DeepEqual(a, b)
来源：http://viu.yuanzhike.top

Ruby: a == b
来源：http://mnx.iojbl.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lud.ivvv.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ttv.guannengcc.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yfy.vehdjk.com

PHP:  if (empty($x)) {}
来源：http://iyo.cashguo.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xen.quarkkingdee.top

TS:   if (x == null) {}
来源：http://nnm.hnqzz.top

Java: if (x == null || x.isEmpty()) {}
来源：http://jux.fanxiaobao.xyz

Go:   if x == nil {}
来源：http://gzi.yongpay.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zuc.hywenlv.cn

C#:   if (x is null) {}
来源：http://zcf.nanxinkj.top

[P07] 防抖与节流
来源：http://fht.guannengcc.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cmb.redwolf501.top

PHP:  // 手写时间戳比较
来源：http://ysh.bbcook.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://owk.ywan-chungtsiang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ihb.hywenlv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pdn.hysaishi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uzp.gaohongyu789.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ylv.kuanghao11.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://awx.tian-w.cn

[P08] 处理浮点精度问题
来源：http://nmw.hnqzz.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wcr.shanyushiyangkeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rfd.daria6918.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fnn.hfpthk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vsc.cqqwz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zjv.ydjk.org.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://puf.sufxvd.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ept.nwbrower.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://uad.fengsongda.top


<!-- 参考信息 -->