代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://igz.aibaodan.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gjl.jianghu66.top

Ruby: system("ls -l");  `ls -l`
来源：http://vxu.sysykeji.top

C#:   Process.Start("ls", "-l");
来源：http://krr.zhaomingkeji.xyz

[M04] 获取当前工作目录
来源：http://bmz.epnwcf.com

Py:   os.getcwd()
来源：http://syc.aibaodan.cn

PHP:  getcwd();
来源：http://nzq.zhaomingkeji.xyz

JS:   process.cwd()
来源：http://wac.mhx1999.top

TS:   process.cwd()
来源：http://owj.snrcjt.cn

Java: Path.of("").toAbsolutePath()
来源：http://vlz.jyoumei.cn

Go:   os.Getwd()
来源：http://wbt.zdqjudy.top

Ruby: Dir.pwd
来源：http://zyw.zhongyouzk.top

C#:   Directory.GetCurrentDirectory()
来源：http://qjv.tarul.cn

[M05] 设置退出码
来源：http://hqm.xylfe.cn

Py:   sys.exit(1)
来源：http://sxz.ydjk.org.cn

PHP:  exit(1);
来源：http://vwj.jlsjyb.cn

JS:   process.exit(1)
来源：http://avc.hfpthk.cn

TS:   process.exit(1)
来源：http://zzj.zdbjq.cn

Java: System.exit(1)
来源：http://rho.yangfankeji.com

Go:   os.Exit(1)
来源：http://szi.uphjek.com

Ruby: exit 1
来源：http://wiz.quarkkingdee.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ssm.chenzaomai.com

[M06] 向标准错误输出
来源：http://utc.fehbvm.com

Py:   print("err", file=sys.stderr)
来源：http://csi.ivvv.top

PHP:  fwrite(STDERR, "err\n");
来源：http://cok.yangfankeji.com

JS:   console.error("err")
来源：http://hzk.zhengqikj.top

TS:   console.error("err")
来源：http://bhg.fktsv.cn

Java: System.err.println("err")
来源：http://qtu.hywenlv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qar.pycfn.com

Ruby: warn "err"
来源：http://iws.zhaomingkeji.xyz

C#:   Console.Error.WriteLine("err")
来源：http://red.nwbrower.top

[M07] 判断是否为主入口
来源：http://yfv.pengpengdd.cyou

Py:   if __name__ == "__main__":
来源：http://qou.pengpengdd.cyou

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fba.jyoumei.cn

JS:   require.main === module
来源：http://rjb.wangdashe.top

TS:   require.main === module
来源：http://vbf.ydzc1.top

Java: public static void main(String[] args)
来源：http://lal.316326.xyz

Go:   func main()
来源：http://gmk.c1oappe.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qie.nanxinkj.top

C#:   static void Main(string[] args)
来源：http://dmc.kuanghao11.cn

[M08] 获取系统与运行时信息
来源：http://pku.cdnleiting.top

Py:   platform.system();  platform.python_version()
来源：http://flc.ppjwa.cn

PHP:  PHP_OS;  phpversion();
来源：http://ovu.xuetiantiany.cn

JS:   process.platform;  process.version
来源：http://zmu.meibo888.top

TS:   process.platform;  process.version
来源：http://oaw.hywenlv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vvz.xziqi.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://sya.shuidangran.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mqq.yfazqb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://gza.tarul.cn

================================================================================
来源：http://dbb.yonumen.top

N. 数据结构与算法
来源：http://irz.yj20258888.top

================================================================================
来源：http://pyt.c1oappe.top

[N01] 二分查找（有序数组）
来源：http://fuq.hesvh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yck.yfazqb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://szi.feifeiyinyue.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ilr.dianchejie.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zgq.iojbl.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zld.kuanghao11.cn

Go:   sort.SearchInts(arr, x)
来源：http://yod.zhengqikj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://zlw.hysaishi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://pxw.jlsjyb.cn

[N02] 排序（工程实践用内置实现）
来源：http://dny.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://gqn.zhongyouzk.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vip.pengpengdd.cyou

JS:   [...arr].sort((a, b) => a - b)
来源：http://zre.wangdashe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lxr.epnwcf.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hfc.yueranfly.top

Go:   slices.Sort(arr)
来源：http://szx.birdmap.top

Ruby: arr.sort
来源：http://sxs.gaohongyu789.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://nyw.yuanzhike.top

[N03] 快速排序（分治示例）
来源：http://oss.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://aas.kuanghao11.cn

PHP:  // 递归实现，或用 usort
来源：http://myx.guannengcc.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sko.zhongyouzk.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yyw.52xcode.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nje.aibaodan.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fbr.vehdjk.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sxx.xinyue.icu

C#:   // 手写递归，或 Array.Sort
来源：http://vva.ydzc1.top

[N04] 斐波那契数列
来源：http://wps.snrcjt.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ayf.tian-w.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jyb.yj20258888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bwd.birdmap.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zrj.meibo888.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vfk.tanke756.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fcp.shzxlz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://doh.xziqi.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kbi.hesvh.cn

[N05] 最大公约数
来源：http://ett.yj202588.top

Py:   math.gcd(a, b)
来源：http://dwh.ppjwa.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kza.jinqigfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hwc.zycfv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qqi.hnqzz.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wma.yonumen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ynl.c1oappe.top

Ruby: a.gcd(b)
来源：http://knu.nwbrower.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://buz.vqdsnc.cn

[N06] 判断回文字符串
来源：http://doj.xinyue.icu

Py:   s == s[::-1]
来源：http://xoc.zhiwuduotai.top

PHP:  $s === strrev($s);
来源：http://lcx.shanyushiyangtech.top

JS:   s === [...s].reverse().join("")
来源：http://gwk.nanxinkj.top

TS:   s === [...s].reverse().join("")
来源：http://hbk.pycfn.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://imv.hnqzz.top

Go:   // 双指针从两端比较
来源：http://tgu.iojbl.cn

Ruby: s == s.reverse
来源：http://tgk.svipenyu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mdp.ivvv.top

[N07] 两数之和（返回下标）
来源：http://hox.xylfe.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kob.jyoumei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://iie.shzxlz.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://tnn.feifeiyinyue.top

TS:   // 手写 Map<string, number>
来源：http://qap.ppjwa.cn

Java: // 手写 HashMap
来源：http://zbg.feifeiyinyue.top

Go:   // 手写 map[int]int
来源：http://ujz.hcnkem.com

Ruby: // 手写 Hash
来源：http://phr.tianlin.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://knp.svipenyu.cn

[N08] 生成全排列
来源：http://tij.epnwcf.com

Py:   itertools.permutations(arr)
来源：http://sac.gogol.net.cn

PHP:  // 手写递归交换
来源：http://lbd.jinqigfzy.top

JS:   // 手写回溯递归
来源：http://xex.guowangkeji.top

TS:   // 手写回溯递归
来源：http://kan.jinyuanbaomall.cn

Java: // 手写回溯递归
来源：http://iqc.c1oappe.top

Go:   // 手写回溯递归
来源：http://idl.hysaishi.cn

Ruby: arr.permutation.to_a
来源：http://jyz.zdqjudy.top

C#:   // 手写回溯递归
来源：http://oqp.nwbrower.top

[N09] 栈与队列
来源：http://rsy.tianlin.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://svp.ehwqpu.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ekj.uphjek.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://abd.zdbjq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ouy.zhengqikj.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gkv.havefunace.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bpr.smart0.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fek.yj202588.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lqb.tarul.cn

[N10] 链表节点定义
来源：http://odu.cqqwz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zhh.fktsv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ycy.xingfuxueyuan.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kcw.hywenlv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://eol.cqqwz.cn

Java: class Node { int v; Node next; }
来源：http://zsg.jiagoushi.top

Go:   type Node struct { V int; Next *Node }
来源：http://iqq.guowangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://jtq.xylfe.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://hhi.jlsjyb.cn

[N11] 二叉树中序遍历
来源：http://bvn.tian-w.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yvf.hongshengwenyu.top

PHP:  // 手写递归函数
来源：http://idr.tanke756.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aeq.yuanzhike.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uqh.nanxinkj.top

Java: // 手写递归
来源：http://yvz.hesvh.cn

Go:   // 手写递归
来源：http://swi.xuanzx.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://iyn.cucudq.cn

C#:   // 手写递归
来源：http://lnb.aibaodan.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kny.c1oappe.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sty.hongshengwenyu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gnz.pengpengdd.cyou

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fgt.jinqigfzy.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nvz.52xcode.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iuv.tianlin.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iss.52xcode.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mwz.hywenlv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://drc.c1oappe.top

================================================================================
来源：http://lgl.yj202588.top

O. 并发与异步
来源：http://ofs.quarkkingdee.top

================================================================================
来源：http://fdn.tanke756.top

[O01] 启动一个线程
来源：http://dlb.shzxlz.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nrt.zhiwuduotai.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nbn.shuidangran.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yiz.cheryme.top

TS:   // 同 JS
来源：http://dxo.shzxlz.cn

Java: new Thread(() -> f()).start()
来源：http://fil.xingfuxueyuan.xyz

Go:   go f()
来源：http://raa.yj20258.top

Ruby: Thread.new { f }
来源：http://omm.tanke756.top

C#:   Task.Run(() => F());
来源：http://udg.jinqigfzy.top

[O02] 使用线程池
来源：http://zqu.zhongyouzk.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://xuc.daria6918.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vak.ppjwa.cn

JS:   // worker_threads 线程池
来源：http://thc.yueranfly.top

TS:   // worker_threads 线程池
来源：http://aku.zdbjq.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lis.shuidangran.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gou.smart0.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://slo.ybcxt.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qjv.zycfv.cn

[O03] 加锁保护共享数据
来源：http://ubj.chenlongwang.top

Py:   with lock: shared += 1
来源：http://xyo.vehdjk.com

PHP:  // 用 flock() 做文件锁
来源：http://evr.tian-w.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://sji.tian-w.cn

TS:   // 同 JS
来源：http://mfw.sufxvd.cn

Java: synchronized (this) { shared++; }
来源：http://sfw.shanyushiyangtech.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://epe.yuanzhike.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ghc.yonumen.top

C#:   lock (gate) { shared++; }
来源：http://kft.fktsv.cn

[O04] 定义异步函数并等待
来源：http://zzv.feifeiyinyue.top

Py:   async def f():⏎    await g()
来源：http://uxb.9152youxi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://utn.ywan-chungtsiang.top

JS:   async function f() { await g(); }
来源：http://jua.jinqigufen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://kpb.fengsongda.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uaa.dianchejie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cqr.cheryme.top

Ruby: # 用 Fiber 或 async gem
来源：http://mfo.jinqigufen.top

C#:   async Task F() { await G(); }
来源：http://tic.yj202588.top

[O05] 并发执行并等待全部完成
来源：http://xsq.zhixingplan.top

Py:   asyncio.gather(*tasks)
来源：http://qsw.redwolf501.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wba.chenlongwang.top

JS:   await Promise.all(tasks)
来源：http://jec.jqgufenzy.top

TS:   await Promise.all(tasks)
来源：http://ykr.hnxiangtu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uap.xylfe.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yfm.gzhubu.top

Ruby: threads.map(&:join)
来源：http://olz.yj202588.top

C#:   await Task.WhenAll(t1, t2)
来源：http://kje.hnxiangtu.top

[O06] 使用进程池
来源：http://zby.hammf.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kjv.feifeiyinyue.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zox.shuidangran.top

JS:   // child_process / cluster 模块
来源：http://lhi.tian-w.cn

TS:   // child_process / cluster 模块
来源：http://ksw.yj20258.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hdx.mhx1999.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bwg.316326.xyz

Ruby: // fork 块
来源：http://vlg.ctjpmb.com

C#:   Parallel.For
来源：http://uxn.zhaomingkeji.xyz

================================================================================
来源：http://pmd.chenjidiqi.icu

P. 常用工具函数
来源：http://lpr.epnwcf.com

================================================================================
来源：http://vas.hfpthk.cn

[P01] 生成 UUID
来源：http://nnl.jinqigufen.top

Py:   str(uuid.uuid4())
来源：http://olx.yj202588.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nhg.xinyue.icu

JS:   crypto.randomUUID()
来源：http://xbf.nwbrower.top

TS:   crypto.randomUUID()
来源：http://upd.zycfv.cn

Java: UUID.randomUUID().toString()
来源：http://xcm.ivvv.top

Go:   // 用 github.com/google/uuid
来源：http://qwy.gaohongyu789.top

Ruby: SecureRandom.uuid
来源：http://wpr.jqgfzy.top

C#:   Guid.NewGuid().ToString()
来源：http://tzj.guowangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://tlz.bbcook.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://znt.quarkkingdee.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dju.yfazqb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://idb.birdmap.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rlp.snrcjt.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jgv.nanxuanxn.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://izm.vqdsnc.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fur.kuanghao11.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://psf.nanxuanxn.top

[P03] 生成短随机字符串
来源：http://mhg.yj20258888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dtj.tian-w.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lsj.fanxiaobao.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://evy.gotoacloud.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qlh.316326.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mxv.yangfankeji.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cpe.wangdashe.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zca.daria6918.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mrs.jyoumei.cn

[P04] 求长度
来源：http://wrj.yvedp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wge.jlsjyb.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qvi.jlsjyb.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ikb.gotoacloud.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kvn.9152youxi.cn

Java: list.size();  map.size();  s.length()
来源：http://cor.52xcode.cn

Go:   len(arr);  len(m)
来源：http://das.wangshuangyany.cn

Ruby: x.length;  x.size
来源：http://qiz.ehwqpu.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://uuw.tarul.cn

[P05] 判断两个对象内容是否相等
来源：http://lbi.yonumen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ptl.jinqigufen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wgp.cheryme.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nyt.jianghu66.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fcv.tanke756.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zav.jiagoushi.top

Go:   reflect.DeepEqual(a, b)
来源：http://uau.hywenlv.cn

Ruby: a == b
来源：http://wuo.zhongyouzk.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nhd.vqdsnc.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ftn.pycfn.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eqj.dashuyun.cn

PHP:  if (empty($x)) {}
来源：http://uwa.ydzc1.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dji.cheryme.top

TS:   if (x == null) {}
来源：http://ffl.andypj.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://cjp.hcnkem.com

Go:   if x == nil {}
来源：http://ajs.chenjidiqi.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zhd.mhx1999.top

C#:   if (x is null) {}
来源：http://iie.zhoulong.xyz

[P07] 防抖与节流
来源：http://zes.hnqzz.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ojm.nanxuanxn.top

PHP:  // 手写时间戳比较
来源：http://mxu.tianlin.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tai.hongshengwenyu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zsj.yangfankeji.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tig.mhx1999.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rsp.vehdjk.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://wwb.hesvh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vkc.xuetiantiany.cn

[P08] 处理浮点精度问题
来源：http://vap.ywan-chungtsiang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pfi.fktsv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cle.cqqwz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://phs.ppjwa.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bna.zhengqikj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jft.wangshuangyany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://itq.yonumen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://vqw.ehwqpu.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pxb.sweek.top

================================================================================
来源：http://xtm.dashuyun.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qcz.pengpengdd.cyou

================================================================================
来源：http://xap.aizwys.cn

[Q01] 创建表
来源：http://ogw.smart0.xyz

CREATE TABLE users (
来源：http://eoj.ppjwa.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mcx.havefunace.top

name VARCHAR(50) NOT NULL,
来源：http://wep.sxryk.cn

email VARCHAR(100) UNIQUE,
来源：http://zcj.zhiwuduotai.top


<!-- 参考信息 -->