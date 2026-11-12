代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dne.yj20258.top

Ruby: ENV["HOME"]
来源：http://fmq.ydzc1.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bkf.ivvv.top

[M03] 执行外部命令
来源：http://qrg.ywan-chungtsiang.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ctu.fehbvm.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nid.hcnkem.com

JS:   child_process.execSync("ls -l").toString()
来源：http://kin.wangdashe.top

TS:   child_process.execSync("ls -l").toString()
来源：http://gne.zhoulong.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ppq.sweek.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lgg.hysaishi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://rol.meibo888.top

C#:   Process.Start("ls", "-l");
来源：http://waw.fanxiaobao.xyz

[M04] 获取当前工作目录
来源：http://clb.smart0.xyz

Py:   os.getcwd()
来源：http://jsc.fengsongda.top

PHP:  getcwd();
来源：http://pqm.shanyushiyangkeji.top

JS:   process.cwd()
来源：http://vbh.shanyushiyangkeji.top

TS:   process.cwd()
来源：http://iwe.xingfuxueyuan.xyz

Java: Path.of("").toAbsolutePath()
来源：http://nac.shzxlz.cn

Go:   os.Getwd()
来源：http://lol.yj202588.top

Ruby: Dir.pwd
来源：http://mol.xinyue.icu

C#:   Directory.GetCurrentDirectory()
来源：http://buq.cheryme.top

[M05] 设置退出码
来源：http://rbd.yonumen.top

Py:   sys.exit(1)
来源：http://nze.smart0.xyz

PHP:  exit(1);
来源：http://wwx.jiagoushi.top

JS:   process.exit(1)
来源：http://nvo.gaohongyu789.top

TS:   process.exit(1)
来源：http://lks.ctjpmb.com

Java: System.exit(1)
来源：http://ghz.xuanzx.com

Go:   os.Exit(1)
来源：http://ygq.cqqwz.cn

Ruby: exit 1
来源：http://ohj.daxiang520.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://emj.tanke756.top

[M06] 向标准错误输出
来源：http://daw.gotoacloud.top

Py:   print("err", file=sys.stderr)
来源：http://lkb.chenjidiqi.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://alt.svipenyu.cn

JS:   console.error("err")
来源：http://xyt.jyoumei.cn

TS:   console.error("err")
来源：http://cub.shangyingyoupin.top

Java: System.err.println("err")
来源：http://snp.jqgufenzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nir.chenjidiqi.icu

Ruby: warn "err"
来源：http://bjq.chenlongwang.top

C#:   Console.Error.WriteLine("err")
来源：http://alh.yangfankeji.com

[M07] 判断是否为主入口
来源：http://qzc.cashguo.top

Py:   if __name__ == "__main__":
来源：http://hbx.hnqzz.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zwm.ppjwa.cn

JS:   require.main === module
来源：http://fgr.yfazqb.com

TS:   require.main === module
来源：http://lac.fengsongda.top

Java: public static void main(String[] args)
来源：http://nko.wangdashe.top

Go:   func main()
来源：http://lcl.yonumen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ava.nanxinkj.top

C#:   static void Main(string[] args)
来源：http://hvv.guannengcc.top

[M08] 获取系统与运行时信息
来源：http://nax.hongshengwenyu.top

Py:   platform.system();  platform.python_version()
来源：http://zof.bjfxy.top

PHP:  PHP_OS;  phpversion();
来源：http://vuc.gotoacloud.top

JS:   process.platform;  process.version
来源：http://slh.haohaochexian.top

TS:   process.platform;  process.version
来源：http://skx.smart0.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tyo.jyoumei.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tmh.cdnleiting.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vsd.iojbl.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gkm.9152youxi.cn

================================================================================
来源：http://aqf.ydjk.org.cn

N. 数据结构与算法
来源：http://gjg.hesvh.cn

================================================================================
来源：http://ehs.kuanghao11.cn

[N01] 二分查找（有序数组）
来源：http://cwr.vqdsnc.cn

Py:   bisect.bisect_left(arr, x)
来源：http://llq.vehdjk.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hyi.sysykeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hpu.zycfv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bfp.jqgufenzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://woo.wangshuangyany.cn

Go:   sort.SearchInts(arr, x)
来源：http://udx.zhoulong.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://ynx.yangfankeji.com

C#:   Array.BinarySearch(arr, x)
来源：http://yge.shuidangran.top

[N02] 排序（工程实践用内置实现）
来源：http://mrz.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://obs.dashuyun.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://loi.52xcode.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cng.316326.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://pwj.gzhubu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://eur.ywan-chungtsiang.top

Go:   slices.Sort(arr)
来源：http://zht.kuanghao11.cn

Ruby: arr.sort
来源：http://cob.dashuyun.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lmx.nwbrower.top

[N03] 快速排序（分治示例）
来源：http://qnb.jianghu66.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ogv.ehwqpu.com

PHP:  // 递归实现，或用 usort
来源：http://djv.aibaodan.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ahj.ydjk.org.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nvd.nwbrower.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://cdy.dashuyun.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ddt.zhiwuduotai.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hrv.nwbrower.top

C#:   // 手写递归，或 Array.Sort
来源：http://wvg.zhongyouzk.top

[N04] 斐波那契数列
来源：http://wbm.yonumen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xji.aizwys.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rfj.fktsv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zif.nanxuanxn.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qjs.jinghuilouyu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://neh.jyoumei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vek.havefunace.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mgy.yj202588.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zqq.zhiwuduotai.top

[N05] 最大公约数
来源：http://yqd.birdmap.top

Py:   math.gcd(a, b)
来源：http://rot.tianlin.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hur.shangyingyoupin.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ogr.jinqigufen.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aay.svipenyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zre.yangfankeji.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://iub.cdnleiting.top

Ruby: a.gcd(b)
来源：http://xua.cqqwz.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rqm.snrcjt.cn

[N06] 判断回文字符串
来源：http://yzq.pengpengdd.cyou

Py:   s == s[::-1]
来源：http://ztr.cdnleiting.top

PHP:  $s === strrev($s);
来源：http://ocn.nwbrower.top

JS:   s === [...s].reverse().join("")
来源：http://uoq.jianghu66.top

TS:   s === [...s].reverse().join("")
来源：http://pxt.zhoulong.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ksj.ppjwa.cn

Go:   // 双指针从两端比较
来源：http://adv.hfpthk.cn

Ruby: s == s.reverse
来源：http://btg.bbcook.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ujs.jianghu66.top

[N07] 两数之和（返回下标）
来源：http://num.bjfxy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://caw.zhixingplan.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vqq.pengpengdd.cyou

JS:   // 手写 Map：map.set(v, i)
来源：http://lzb.zycfv.cn

TS:   // 手写 Map<string, number>
来源：http://tzs.meibo888.top

Java: // 手写 HashMap
来源：http://rlg.snrcjt.cn

Go:   // 手写 map[int]int
来源：http://dhi.ydzc1.top

Ruby: // 手写 Hash
来源：http://sfh.jinyuanbaomall.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nzc.yvedp.cn

[N08] 生成全排列
来源：http://avx.316326.xyz

Py:   itertools.permutations(arr)
来源：http://nqu.yuanzhike.top

PHP:  // 手写递归交换
来源：http://xcs.cqqwz.cn

JS:   // 手写回溯递归
来源：http://pmb.mhx1999.top

TS:   // 手写回溯递归
来源：http://ijf.aizwys.cn

Java: // 手写回溯递归
来源：http://jvk.xylfe.cn

Go:   // 手写回溯递归
来源：http://ske.daria6918.cn

Ruby: arr.permutation.to_a
来源：http://jyl.zhijiandao.cn

C#:   // 手写回溯递归
来源：http://mbv.daria6918.cn

[N09] 栈与队列
来源：http://rwe.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://krc.cqqwz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wpm.zhiwuduotai.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nyr.chenlongwang.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://eis.hesvh.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cca.feifeiyinyue.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eko.xuetiantiany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iao.9152youxi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hcr.uphjek.com

[N10] 链表节点定义
来源：http://kqx.haohaochexian.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://szz.ehwqpu.com

PHP:  class Node { public $v; public $next = null; }
来源：http://gjc.tianlin.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pej.sufxvd.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bfq.yongpay.top

Java: class Node { int v; Node next; }
来源：http://vcr.xylfe.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pjt.xziqi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ptb.tianlin.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://iqh.xziqi.cn

[N11] 二叉树中序遍历
来源：http://unx.fengsongda.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://usl.daxiang520.top

PHP:  // 手写递归函数
来源：http://aeg.c1oappe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aek.dianchejie.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://psk.shanyushiyangkeji.top

Java: // 手写递归
来源：http://ruw.c1oappe.top

Go:   // 手写递归
来源：http://sui.redwolf501.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wof.quarkkingdee.top

C#:   // 手写递归
来源：http://bnn.fehbvm.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cgc.jyoumei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mpr.xziqi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jzs.sweek.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tye.gotoacloud.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kgn.cqqwz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wgq.cqqwz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nib.ivvv.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rvp.snrcjt.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hft.hesvh.cn

================================================================================
来源：http://who.yangfankeji.com

O. 并发与异步
来源：http://whc.vehdjk.com

================================================================================
来源：http://dyc.shangyingyoupin.top

[O01] 启动一个线程
来源：http://uqc.birdmap.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qwc.ywan-chungtsiang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vgp.hongshengwenyu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://euw.yj20258888.top

TS:   // 同 JS
来源：http://tkr.52xcode.cn

Java: new Thread(() -> f()).start()
来源：http://nyo.xylfe.cn

Go:   go f()
来源：http://ykb.sjlbkw.cn

Ruby: Thread.new { f }
来源：http://rcy.hnqzz.top

C#:   Task.Run(() => F());
来源：http://etu.sysykeji.top

[O02] 使用线程池
来源：http://nov.sufxvd.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fap.sysykeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wgs.yueranfly.top

JS:   // worker_threads 线程池
来源：http://vtj.birdmap.top

TS:   // worker_threads 线程池
来源：http://vab.gogol.net.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jva.cashguo.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zqk.cheryme.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hfe.jiagoushi.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hmz.iojbl.cn

[O03] 加锁保护共享数据
来源：http://uud.meibo888.top

Py:   with lock: shared += 1
来源：http://dfw.hongshengwenyu.top

PHP:  // 用 flock() 做文件锁
来源：http://pte.redwolf501.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://esz.mhx1999.top

TS:   // 同 JS
来源：http://yvd.yonumen.top

Java: synchronized (this) { shared++; }
来源：http://dvl.yvedp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jad.c1oappe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://kol.52xcode.cn

C#:   lock (gate) { shared++; }
来源：http://srk.hywenlv.cn

[O04] 定义异步函数并等待
来源：http://vog.zhijiandao.cn

Py:   async def f():⏎    await g()
来源：http://auu.chenjidiqi.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wwe.cqqwz.cn

JS:   async function f() { await g(); }
来源：http://svm.hesvh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dtw.dashuyun.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kur.chenzaomai.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ecu.zhiwuduotai.top

Ruby: # 用 Fiber 或 async gem
来源：http://dej.meibo888.top

C#:   async Task F() { await G(); }
来源：http://xbj.gaohongyu789.top

[O05] 并发执行并等待全部完成
来源：http://uxs.svipenyu.cn

Py:   asyncio.gather(*tasks)
来源：http://vgl.yvedp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tea.pycfn.com

JS:   await Promise.all(tasks)
来源：http://cit.hnqzz.top

TS:   await Promise.all(tasks)
来源：http://mzd.gotoacloud.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zru.jqgfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://glt.zdqjudy.top

Ruby: threads.map(&:join)
来源：http://syt.yangfankeji.com

C#:   await Task.WhenAll(t1, t2)
来源：http://pix.svipenyu.cn

[O06] 使用进程池
来源：http://ajn.zhiwuduotai.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dti.pengpengdd.cyou

PHP:  // pcntl_fork 或多进程队列
来源：http://yic.yj20258888.top

JS:   // child_process / cluster 模块
来源：http://ygc.hesvh.cn

TS:   // child_process / cluster 模块
来源：http://nec.shangyingyoupin.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rsa.yuanzhike.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mdw.hysaishi.cn

Ruby: // fork 块
来源：http://rok.aibaodan.cn

C#:   Parallel.For
来源：http://uor.jyoumei.cn

================================================================================
来源：http://ole.sufxvd.cn

P. 常用工具函数
来源：http://nry.chenlongwang.top

================================================================================
来源：http://alg.chenjidiqi.icu

[P01] 生成 UUID
来源：http://iyl.cheryme.top

Py:   str(uuid.uuid4())
来源：http://xau.chenlongwang.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://snc.zhiwuduotai.top

JS:   crypto.randomUUID()
来源：http://nrq.ctjpmb.com

TS:   crypto.randomUUID()
来源：http://bcb.birdmap.top

Java: UUID.randomUUID().toString()
来源：http://rmw.iojbl.cn

Go:   // 用 github.com/google/uuid
来源：http://ryd.zdqjudy.top

Ruby: SecureRandom.uuid
来源：http://ape.jinqigufen.top

C#:   Guid.NewGuid().ToString()
来源：http://ofh.hnqzz.top

[P02] MD5 / SHA256 摘要
来源：http://qed.9152youxi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ysr.vqdsnc.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gcb.shanyushiyangtech.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vbh.quarkkingdee.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ecj.cdnleiting.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uwc.iojbl.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xby.fanxiaobao.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tmy.xziqi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sik.guannengcc.top

[P03] 生成短随机字符串
来源：http://rlt.redwolf501.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sik.wangdashe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aqp.cashguo.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lwl.sufxvd.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://upt.jinghuilouyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cpc.tanke756.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cxh.quarkkingdee.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ohd.yueranfly.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kap.tanke756.top

[P04] 求长度
来源：http://ptr.aizwys.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vnw.zhoulong.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://auc.yonumen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://orv.sysykeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oot.yj20258.top

Java: list.size();  map.size();  s.length()
来源：http://mua.nanxinkj.top

Go:   len(arr);  len(m)
来源：http://txb.ydjk.org.cn

Ruby: x.length;  x.size
来源：http://dwf.shanyushiyangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://uak.zycfv.cn

[P05] 判断两个对象内容是否相等
来源：http://zhf.tarul.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uzu.zhiwuduotai.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uup.cqqwz.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://whm.havefunace.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dqf.haohaochexian.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vji.nanxuanxn.top

Go:   reflect.DeepEqual(a, b)
来源：http://lyy.jqgufenzy.top

Ruby: a == b
来源：http://fah.hnxiangtu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tut.kuanghao11.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mni.wangdashe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dqn.redwolf501.top

PHP:  if (empty($x)) {}
来源：http://kro.fengsongda.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://abw.hnxiangtu.top

TS:   if (x == null) {}
来源：http://xhp.shanyushiyangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://gbb.dianchejie.cn

Go:   if x == nil {}
来源：http://bcx.cqqwz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mth.shzxlz.cn

C#:   if (x is null) {}
来源：http://hda.aibaodan.cn

[P07] 防抖与节流
来源：http://ukq.jinghuilouyu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oms.jqgfzy.top

PHP:  // 手写时间戳比较
来源：http://uqb.pycfn.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://koa.sxryk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://euk.jyoumei.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://sfc.cdnleiting.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dhl.fengsongda.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://dxi.xziqi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zrh.shuidangran.top

[P08] 处理浮点精度问题
来源：http://zki.xinyue.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kqe.sjlbkw.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vll.xuanzx.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ozf.zdqjudy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sks.jiagoushi.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hqq.tianlin.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kxr.nanxuanxn.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zqv.xylfe.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tel.nanxinkj.top


<!-- 参考信息 -->