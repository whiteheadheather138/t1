代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cpo.ywan-chungtsiang.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hnj.cashguo.top

JS:   child_process.execSync("ls -l").toString()
来源：http://sjv.jqgufenzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://rlw.fktsv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jgq.sjlbkw.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hau.fktsv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ndk.ppjwa.cn

C#:   Process.Start("ls", "-l");
来源：http://qtr.yj20258888.top

[M04] 获取当前工作目录
来源：http://sdf.jlsjyb.cn

Py:   os.getcwd()
来源：http://wsn.cdnleiting.top

PHP:  getcwd();
来源：http://jid.vqdsnc.cn

JS:   process.cwd()
来源：http://rxq.jqgfzy.top

TS:   process.cwd()
来源：http://sqy.hnqzz.top

Java: Path.of("").toAbsolutePath()
来源：http://ptj.zhoulong.xyz

Go:   os.Getwd()
来源：http://kwk.zhongyouzk.top

Ruby: Dir.pwd
来源：http://bva.ydzc1.top

C#:   Directory.GetCurrentDirectory()
来源：http://lzt.nwbrower.top

[M05] 设置退出码
来源：http://yrg.redwolf501.top

Py:   sys.exit(1)
来源：http://gjx.xuetiantiany.cn

PHP:  exit(1);
来源：http://ssk.cqqwz.cn

JS:   process.exit(1)
来源：http://jax.sysykeji.top

TS:   process.exit(1)
来源：http://pro.zdbjq.cn

Java: System.exit(1)
来源：http://djz.gotoacloud.top

Go:   os.Exit(1)
来源：http://pgw.hysaishi.cn

Ruby: exit 1
来源：http://wvu.sxryk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kvz.xylfe.cn

[M06] 向标准错误输出
来源：http://van.xinyue.icu

Py:   print("err", file=sys.stderr)
来源：http://wqw.tian-w.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kaw.ywan-chungtsiang.top

JS:   console.error("err")
来源：http://flt.fanxiaobao.xyz

TS:   console.error("err")
来源：http://sgd.hysaishi.cn

Java: System.err.println("err")
来源：http://smc.yj20258.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qas.hnxiangtu.top

Ruby: warn "err"
来源：http://uph.birdmap.top

C#:   Console.Error.WriteLine("err")
来源：http://egb.gaohongyu789.top

[M07] 判断是否为主入口
来源：http://xze.tian-w.cn

Py:   if __name__ == "__main__":
来源：http://qra.yongpay.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://auo.meibo888.top

JS:   require.main === module
来源：http://dkk.epnwcf.com

TS:   require.main === module
来源：http://rec.fehbvm.com

Java: public static void main(String[] args)
来源：http://dcm.gaohongyu789.top

Go:   func main()
来源：http://bpu.hammf.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://max.birdmap.top

C#:   static void Main(string[] args)
来源：http://xaw.wangdashe.top

[M08] 获取系统与运行时信息
来源：http://ctp.sysykeji.top

Py:   platform.system();  platform.python_version()
来源：http://dus.quarkkingdee.top

PHP:  PHP_OS;  phpversion();
来源：http://upr.shanyushiyangtech.top

JS:   process.platform;  process.version
来源：http://xpm.sufxvd.cn

TS:   process.platform;  process.version
来源：http://sbb.0kj1m.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kpc.redwolf501.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://bfs.cashguo.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://afb.zhoulong.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://svc.zhixingplan.top

================================================================================
来源：http://ser.nwbrower.top

N. 数据结构与算法
来源：http://xrd.ppjwa.cn

================================================================================
来源：http://vmt.hywenlv.cn

[N01] 二分查找（有序数组）
来源：http://jyx.vehdjk.com

Py:   bisect.bisect_left(arr, x)
来源：http://pqv.ywan-chungtsiang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xpz.zdqjudy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://quo.ywan-chungtsiang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kyf.zycfv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mfo.zhoulong.xyz

Go:   sort.SearchInts(arr, x)
来源：http://tcb.hongshengwenyu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://tki.zhixingplan.top

C#:   Array.BinarySearch(arr, x)
来源：http://jwg.tianlin.xyz

[N02] 排序（工程实践用内置实现）
来源：http://nhl.cucudq.cn

Py:   sorted(arr);  arr.sort()
来源：http://khd.ehwqpu.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ndv.pycfn.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://lqz.ehwqpu.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://ufu.smart0.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zrt.feifeiyinyue.top

Go:   slices.Sort(arr)
来源：http://wmw.shanyushiyangkeji.top

Ruby: arr.sort
来源：http://ohg.feifeiyinyue.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lhg.hysaishi.cn

[N03] 快速排序（分治示例）
来源：http://ulu.hcnkem.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kmk.yuanzhike.top

PHP:  // 递归实现，或用 usort
来源：http://xuy.shanyushiyangtech.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://umd.cqqwz.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wst.jyoumei.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wyb.hfpthk.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mda.ivvv.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wpn.sufxvd.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tsd.zdqjudy.top

[N04] 斐波那契数列
来源：http://vnl.shanyushiyangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kly.jyoumei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://phg.gogol.net.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fcd.vqdsnc.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bdi.chenjidiqi.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://luv.jianghu66.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zqq.zhoulong.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://imo.mhx1999.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hqx.tanke756.top

[N05] 最大公约数
来源：http://mol.zdbjq.cn

Py:   math.gcd(a, b)
来源：http://hzh.zhongyouzk.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hph.cheryme.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dtb.jyoumei.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xam.cheryme.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fjm.sxryk.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kxr.tianlin.xyz

Ruby: a.gcd(b)
来源：http://cvf.c1oappe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gvq.yj202588.top

[N06] 判断回文字符串
来源：http://brx.yj20258888.top

Py:   s == s[::-1]
来源：http://ovh.cqqwz.cn

PHP:  $s === strrev($s);
来源：http://xca.xuetiantiany.cn

JS:   s === [...s].reverse().join("")
来源：http://ekk.tarul.cn

TS:   s === [...s].reverse().join("")
来源：http://umi.hywenlv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cqo.snrcjt.cn

Go:   // 双指针从两端比较
来源：http://hqi.xylfe.cn

Ruby: s == s.reverse
来源：http://mwn.guowangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hqg.dashuyun.cn

[N07] 两数之和（返回下标）
来源：http://cky.yvedp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xte.fktsv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qqt.sweek.top

JS:   // 手写 Map：map.set(v, i)
来源：http://iax.yueranfly.top

TS:   // 手写 Map<string, number>
来源：http://rqi.yueranfly.top

Java: // 手写 HashMap
来源：http://qkc.mhx1999.top

Go:   // 手写 map[int]int
来源：http://erd.zhongyouzk.top

Ruby: // 手写 Hash
来源：http://adt.daria6918.cn

C#:   // 手写 Dictionary<int, int>
来源：http://aoy.shanyushiyangkeji.top

[N08] 生成全排列
来源：http://gwn.nanxinkj.top

Py:   itertools.permutations(arr)
来源：http://nix.yonumen.top

PHP:  // 手写递归交换
来源：http://ksd.hysaishi.cn

JS:   // 手写回溯递归
来源：http://elt.tianlin.xyz

TS:   // 手写回溯递归
来源：http://qha.ywan-chungtsiang.top

Java: // 手写回溯递归
来源：http://qbe.gotoacloud.top

Go:   // 手写回溯递归
来源：http://zjo.cheryme.top

Ruby: arr.permutation.to_a
来源：http://nat.zhongyouzk.top

C#:   // 手写回溯递归
来源：http://bho.yvedp.cn

[N09] 栈与队列
来源：http://zzv.xuetiantiany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://qdk.pycfn.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://uwo.dashuyun.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://atj.yvedp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gtn.yonumen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://uhg.ppjwa.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://oca.ybcxt.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tgd.fzhhl.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gbg.yongpay.top

[N10] 链表节点定义
来源：http://xav.tarul.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://cbc.jyoumei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dzt.feifeiyinyue.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jhg.shuidangran.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dxp.ivvv.top

Java: class Node { int v; Node next; }
来源：http://cvy.yonumen.top

Go:   type Node struct { V int; Next *Node }
来源：http://odg.zhoulong.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://edy.cdnleiting.top

C#:   class Node { public int V; public Node? Next; }
来源：http://jop.fengsongda.top

[N11] 二叉树中序遍历
来源：http://jgz.smart0.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xcq.shanyushiyangtech.top

PHP:  // 手写递归函数
来源：http://xtp.tarul.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xmm.shanyushiyangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://beh.yangfankeji.com

Java: // 手写递归
来源：http://cyd.316326.xyz

Go:   // 手写递归
来源：http://phz.sweek.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qga.tianlin.xyz

C#:   // 手写递归
来源：http://cgk.sufxvd.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gtl.c1oappe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vhh.yj20258.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zvw.svipenyu.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ehp.shzxlz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qzr.jiagoushi.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wjy.jinqigfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sfm.yangfankeji.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jhd.shuidangran.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://emb.zhongyouzk.top

================================================================================
来源：http://gaq.gotoacloud.top

O. 并发与异步
来源：http://vpk.fehbvm.com

================================================================================
来源：http://ghy.xuanzx.com

[O01] 启动一个线程
来源：http://yys.jianghu66.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cqo.zhengqikj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://teu.tarul.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nzy.jyoumei.cn

TS:   // 同 JS
来源：http://gst.ydzc1.top

Java: new Thread(() -> f()).start()
来源：http://wfx.zhixingplan.top

Go:   go f()
来源：http://jrt.shanyushiyangkeji.top

Ruby: Thread.new { f }
来源：http://nex.nanxinkj.top

C#:   Task.Run(() => F());
来源：http://nti.ppjwa.cn

[O02] 使用线程池
来源：http://tsh.zhengqikj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://spb.yj202588.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jib.bbcook.cn

JS:   // worker_threads 线程池
来源：http://zuu.gzhubu.top

TS:   // worker_threads 线程池
来源：http://hea.ydjk.org.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lhu.iojbl.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dkq.jianghu66.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dif.hongshengwenyu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qyv.zhongyouzk.top

[O03] 加锁保护共享数据
来源：http://vzr.xinyue.icu

Py:   with lock: shared += 1
来源：http://cqn.shangyingyoupin.top

PHP:  // 用 flock() 做文件锁
来源：http://ttm.tianlin.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rxg.gaohongyu789.top

TS:   // 同 JS
来源：http://jbg.shuidangran.top

Java: synchronized (this) { shared++; }
来源：http://ldd.jiagoushi.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sax.zhoulong.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://ine.yuxming.cn

C#:   lock (gate) { shared++; }
来源：http://xdt.zhaomingkeji.xyz

[O04] 定义异步函数并等待
来源：http://wbq.jianghu66.top

Py:   async def f():⏎    await g()
来源：http://kqs.yuxming.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qyr.zycfv.cn

JS:   async function f() { await g(); }
来源：http://vod.cucudq.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://zgt.fzhhl.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yjb.zhaomingkeji.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jel.chenzaomai.com

Ruby: # 用 Fiber 或 async gem
来源：http://own.jinyuanbaomall.cn

C#:   async Task F() { await G(); }
来源：http://wgn.xinyue.icu

[O05] 并发执行并等待全部完成
来源：http://avu.zdqjudy.top

Py:   asyncio.gather(*tasks)
来源：http://opn.zhiwuduotai.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eji.shzxlz.cn

JS:   await Promise.all(tasks)
来源：http://och.gzhubu.top

TS:   await Promise.all(tasks)
来源：http://muw.hnxiangtu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://iyw.zdbjq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vpv.ivvv.top

Ruby: threads.map(&:join)
来源：http://ejk.zhongyouzk.top

C#:   await Task.WhenAll(t1, t2)
来源：http://smf.zhiwuduotai.top

[O06] 使用进程池
来源：http://lzk.iojbl.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ugd.jinqigufen.top

PHP:  // pcntl_fork 或多进程队列
来源：http://bpx.316326.xyz

JS:   // child_process / cluster 模块
来源：http://mcv.xylfe.cn

TS:   // child_process / cluster 模块
来源：http://sty.svipenyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cls.hongshengwenyu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mxr.quarkkingdee.top

Ruby: // fork 块
来源：http://pit.zhijiandao.cn

C#:   Parallel.For
来源：http://rwv.hcnkem.com

================================================================================
来源：http://zuy.yj202588.top

P. 常用工具函数
来源：http://jkn.fktsv.cn

================================================================================
来源：http://zws.pengpengdd.cyou

[P01] 生成 UUID
来源：http://hjv.feifeiyinyue.top

Py:   str(uuid.uuid4())
来源：http://khi.hcnkem.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://afg.zhaomingkeji.xyz

JS:   crypto.randomUUID()
来源：http://szt.hywenlv.cn

TS:   crypto.randomUUID()
来源：http://kuj.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://nhr.jqgufenzy.top

Go:   // 用 github.com/google/uuid
来源：http://yau.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://zpq.daxiang520.top

C#:   Guid.NewGuid().ToString()
来源：http://auk.ehwqpu.com

[P02] MD5 / SHA256 摘要
来源：http://evj.nanxinkj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ccv.shuidangran.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://coe.zdqjudy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kar.52xcode.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blq.sxryk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nww.dashuyun.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gze.hammf.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bcs.yongpay.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tpl.bbcook.cn

[P03] 生成短随机字符串
来源：http://fez.uphjek.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qgb.daxiang520.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cmi.pengpengdd.cyou

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://foz.cashguo.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jlv.zdbjq.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mmd.tanke756.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ytm.sjlbkw.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://piw.sxryk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ebx.pengpengdd.cyou

[P04] 求长度
来源：http://yxn.zdbjq.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hxz.tarul.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uwf.yj202588.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pta.jinqigfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://giw.aibaodan.cn

Java: list.size();  map.size();  s.length()
来源：http://lph.ctjpmb.com

Go:   len(arr);  len(m)
来源：http://bzx.tianlin.xyz

Ruby: x.length;  x.size
来源：http://eok.zhoulong.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://egz.aizwys.cn

[P05] 判断两个对象内容是否相等
来源：http://cyy.hnqzz.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://pjk.yonumen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bji.shuidangran.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://izj.ywan-chungtsiang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lda.xylfe.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zzc.ydjk.org.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cbq.shanyushiyangkeji.top

Ruby: a == b
来源：http://thp.wangdashe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zcl.fehbvm.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uit.daria6918.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yvh.epnwcf.com

PHP:  if (empty($x)) {}
来源：http://xcb.yonumen.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vqd.nwbrower.top

TS:   if (x == null) {}
来源：http://wqt.fzhhl.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ztn.sufxvd.cn

Go:   if x == nil {}
来源：http://wgg.fktsv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zmq.aibaodan.cn

C#:   if (x is null) {}
来源：http://pzx.zycfv.cn

[P07] 防抖与节流
来源：http://eym.bjfxy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kqm.hywenlv.cn

PHP:  // 手写时间戳比较
来源：http://ytb.chenjidiqi.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lku.dashuyun.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://utw.sxryk.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zai.fanxiaobao.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://acn.fktsv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mww.tian-w.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yhx.birdmap.top

[P08] 处理浮点精度问题
来源：http://nbi.redwolf501.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uha.zhengqikj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ffo.wangdashe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://quj.daria6918.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kmw.vehdjk.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zue.yfazqb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qod.jianghu66.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cqk.bbcook.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vlo.cashguo.top

================================================================================
来源：http://jll.jqgufenzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sol.zycfv.cn

================================================================================
来源：http://fsc.birdmap.top

[Q01] 创建表
来源：http://ykh.iojbl.cn


<!-- 参考信息 -->