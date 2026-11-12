代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ddh.gotoacloud.top

Go:   exec.Command("ls", "-l").Output()
来源：http://zzi.sysykeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://rru.xuanzx.com

C#:   Process.Start("ls", "-l");
来源：http://ajl.zhongyouzk.top

[M04] 获取当前工作目录
来源：http://ptv.316326.xyz

Py:   os.getcwd()
来源：http://bla.cheryme.top

PHP:  getcwd();
来源：http://vcb.gzhubu.top

JS:   process.cwd()
来源：http://zwk.ehwqpu.com

TS:   process.cwd()
来源：http://mer.iojbl.cn

Java: Path.of("").toAbsolutePath()
来源：http://vzk.nanxuanxn.top

Go:   os.Getwd()
来源：http://pwq.chenjidiqi.icu

Ruby: Dir.pwd
来源：http://sfd.snrcjt.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ukv.0kj1m.cn

[M05] 设置退出码
来源：http://apj.redwolf501.top

Py:   sys.exit(1)
来源：http://msf.xziqi.cn

PHP:  exit(1);
来源：http://hqz.sysykeji.top

JS:   process.exit(1)
来源：http://hsu.pycfn.com

TS:   process.exit(1)
来源：http://jpr.shanyushiyangkeji.top

Java: System.exit(1)
来源：http://lwb.zycfv.cn

Go:   os.Exit(1)
来源：http://pdg.pycfn.com

Ruby: exit 1
来源：http://bvc.jyoumei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hkv.jinyuanbaomall.cn

[M06] 向标准错误输出
来源：http://ghj.mhx1999.top

Py:   print("err", file=sys.stderr)
来源：http://exa.gotoacloud.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xgy.ydzc1.top

JS:   console.error("err")
来源：http://fve.yj202588.top

TS:   console.error("err")
来源：http://btc.fktsv.cn

Java: System.err.println("err")
来源：http://wqa.dianchejie.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ovd.hesvh.cn

Ruby: warn "err"
来源：http://ubk.fanxiaobao.xyz

C#:   Console.Error.WriteLine("err")
来源：http://kxx.hfpthk.cn

[M07] 判断是否为主入口
来源：http://aef.xuanzx.com

Py:   if __name__ == "__main__":
来源：http://khp.daria6918.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dfg.epnwcf.com

JS:   require.main === module
来源：http://mhm.ydjk.org.cn

TS:   require.main === module
来源：http://qrd.sxryk.cn

Java: public static void main(String[] args)
来源：http://nxp.yj202588.top

Go:   func main()
来源：http://jpc.zhixingplan.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://egr.yvedp.cn

C#:   static void Main(string[] args)
来源：http://tpe.zhongyouzk.top

[M08] 获取系统与运行时信息
来源：http://fsa.hnqzz.top

Py:   platform.system();  platform.python_version()
来源：http://zfu.shanyushiyangtech.top

PHP:  PHP_OS;  phpversion();
来源：http://tqd.zhaomingkeji.xyz

JS:   process.platform;  process.version
来源：http://khh.tarul.cn

TS:   process.platform;  process.version
来源：http://uaf.xuetiantiany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ggm.zhengqikj.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://irz.quarkkingdee.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sfs.316326.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://zwb.jlsjyb.cn

================================================================================
来源：http://ivs.tarul.cn

N. 数据结构与算法
来源：http://lxq.shanyushiyangkeji.top

================================================================================
来源：http://bmx.snrcjt.cn

[N01] 二分查找（有序数组）
来源：http://kny.shangyingyoupin.top

Py:   bisect.bisect_left(arr, x)
来源：http://khr.gzhubu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zgw.tian-w.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://swq.sysykeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ele.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jus.0kj1m.cn

Go:   sort.SearchInts(arr, x)
来源：http://uwn.tanke756.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://tlr.xinyue.icu

C#:   Array.BinarySearch(arr, x)
来源：http://bec.shangyingyoupin.top

[N02] 排序（工程实践用内置实现）
来源：http://shn.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://yzm.mhx1999.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lrj.andypj.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://gra.daria6918.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://plj.ywan-chungtsiang.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ags.gotoacloud.top

Go:   slices.Sort(arr)
来源：http://nov.wangshuangyany.cn

Ruby: arr.sort
来源：http://hon.guannengcc.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://nmw.jiagoushi.top

[N03] 快速排序（分治示例）
来源：http://ddi.sysykeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jjg.jinyuanbaomall.cn

PHP:  // 递归实现，或用 usort
来源：http://mbs.fzhhl.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nox.andypj.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vbp.jqgufenzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bpu.guannengcc.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qzn.nanxinkj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qie.feifeiyinyue.top

C#:   // 手写递归，或 Array.Sort
来源：http://cns.tarul.cn

[N04] 斐波那契数列
来源：http://uql.316326.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hhh.svipenyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jpi.havefunace.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bga.xuetiantiany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fxl.quarkkingdee.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fbw.zhixingplan.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jub.jianghu66.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://quu.mhx1999.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dck.cheryme.top

[N05] 最大公约数
来源：http://hdn.wangshuangyany.cn

Py:   math.gcd(a, b)
来源：http://zcw.tanke756.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ptn.yj20258.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hyw.shanyushiyangtech.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xdd.hfpthk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ryg.daxiang520.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qae.zhixingplan.top

Ruby: a.gcd(b)
来源：http://hgv.guowangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zgh.vqdsnc.cn

[N06] 判断回文字符串
来源：http://tpr.vehdjk.com

Py:   s == s[::-1]
来源：http://vas.cheryme.top

PHP:  $s === strrev($s);
来源：http://nhx.wangdashe.top

JS:   s === [...s].reverse().join("")
来源：http://zyt.yueranfly.top

TS:   s === [...s].reverse().join("")
来源：http://jmb.hfpthk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qya.jinyuanbaomall.cn

Go:   // 双指针从两端比较
来源：http://idw.shangyingyoupin.top

Ruby: s == s.reverse
来源：http://iyu.wangdashe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://sve.aibaodan.cn

[N07] 两数之和（返回下标）
来源：http://dcn.yj202588.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://czr.cqqwz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fwv.yj20258.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zhf.fengsongda.top

TS:   // 手写 Map<string, number>
来源：http://vhu.sysykeji.top

Java: // 手写 HashMap
来源：http://gkq.hammf.cn

Go:   // 手写 map[int]int
来源：http://zmo.iojbl.cn

Ruby: // 手写 Hash
来源：http://kuo.9152youxi.cn

C#:   // 手写 Dictionary<int, int>
来源：http://pwd.xziqi.cn

[N08] 生成全排列
来源：http://atz.epnwcf.com

Py:   itertools.permutations(arr)
来源：http://ndh.haohaochexian.top

PHP:  // 手写递归交换
来源：http://mam.jinqigufen.top

JS:   // 手写回溯递归
来源：http://jrh.gotoacloud.top

TS:   // 手写回溯递归
来源：http://glk.9152youxi.cn

Java: // 手写回溯递归
来源：http://mbs.jiagoushi.top

Go:   // 手写回溯递归
来源：http://lop.cashguo.top

Ruby: arr.permutation.to_a
来源：http://tvh.zhiwuduotai.top

C#:   // 手写回溯递归
来源：http://gwo.zdqjudy.top

[N09] 栈与队列
来源：http://mbv.daxiang520.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xvf.xingfuxueyuan.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kfb.nwbrower.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cfl.hnqzz.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ram.wangshuangyany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cxy.cdnleiting.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rpb.xingfuxueyuan.xyz

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nkg.tianlin.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://feb.tarul.cn

[N10] 链表节点定义
来源：http://xny.gaohongyu789.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://qge.yvedp.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://kbu.yj20258.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xbm.zhiwuduotai.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://alh.ctjpmb.com

Java: class Node { int v; Node next; }
来源：http://tfb.birdmap.top

Go:   type Node struct { V int; Next *Node }
来源：http://ivi.ywan-chungtsiang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://jzb.fengsongda.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bpe.bjfxy.top

[N11] 二叉树中序遍历
来源：http://heo.aizwys.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://olh.hnqzz.top

PHP:  // 手写递归函数
来源：http://uze.hfpthk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hun.zdqjudy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hed.chenlongwang.top

Java: // 手写递归
来源：http://qaa.hfpthk.cn

Go:   // 手写递归
来源：http://eoq.yuxming.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hyd.yuanzhike.top

C#:   // 手写递归
来源：http://lki.hnxiangtu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yrz.hcnkem.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tns.chenlongwang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yrg.chenlongwang.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jsq.ydzc1.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wxd.9152youxi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oyc.yueranfly.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lwm.zycfv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://clx.xziqi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tup.c1oappe.top

================================================================================
来源：http://mal.aizwys.cn

O. 并发与异步
来源：http://cki.xingfuxueyuan.xyz

================================================================================
来源：http://zgk.jinghuilouyu.cn

[O01] 启动一个线程
来源：http://hmo.sufxvd.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vdb.chenjidiqi.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://npi.xuetiantiany.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jmz.xuanzx.com

TS:   // 同 JS
来源：http://ioz.jiagoushi.top

Java: new Thread(() -> f()).start()
来源：http://bnx.xingfuxueyuan.xyz

Go:   go f()
来源：http://blf.cdnleiting.top

Ruby: Thread.new { f }
来源：http://rjs.cucudq.cn

C#:   Task.Run(() => F());
来源：http://bus.yuanzhike.top

[O02] 使用线程池
来源：http://rfk.uphjek.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cyc.aizwys.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uvi.jqgufenzy.top

JS:   // worker_threads 线程池
来源：http://mfv.wangshuangyany.cn

TS:   // worker_threads 线程池
来源：http://ylf.smart0.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://xqk.gaohongyu789.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cxe.chenzaomai.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ztb.tanke756.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vao.jianghu66.top

[O03] 加锁保护共享数据
来源：http://itk.pengpengdd.cyou

Py:   with lock: shared += 1
来源：http://foc.cdnleiting.top

PHP:  // 用 flock() 做文件锁
来源：http://bko.yongpay.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ydh.ybcxt.top

TS:   // 同 JS
来源：http://iee.jqgfzy.top

Java: synchronized (this) { shared++; }
来源：http://ptc.sjlbkw.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nvb.sufxvd.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://blv.yfazqb.com

C#:   lock (gate) { shared++; }
来源：http://dnw.mhx1999.top

[O04] 定义异步函数并等待
来源：http://yyz.0kj1m.cn

Py:   async def f():⏎    await g()
来源：http://gly.zhongyouzk.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tkk.andypj.xyz

JS:   async function f() { await g(); }
来源：http://hfi.daxiang520.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://epv.yj20258888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://arl.zhengqikj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kvy.chenjidiqi.icu

Ruby: # 用 Fiber 或 async gem
来源：http://htw.pycfn.com

C#:   async Task F() { await G(); }
来源：http://drq.daria6918.cn

[O05] 并发执行并等待全部完成
来源：http://bbs.ehwqpu.com

Py:   asyncio.gather(*tasks)
来源：http://ohn.zdbjq.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ejf.hammf.cn

JS:   await Promise.all(tasks)
来源：http://ckw.cqqwz.cn

TS:   await Promise.all(tasks)
来源：http://ybv.bbcook.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ofj.zhijiandao.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fgy.zdqjudy.top

Ruby: threads.map(&:join)
来源：http://xye.hcnkem.com

C#:   await Task.WhenAll(t1, t2)
来源：http://fvr.havefunace.top

[O06] 使用进程池
来源：http://ugo.aibaodan.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lzp.hysaishi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ktm.mhx1999.top

JS:   // child_process / cluster 模块
来源：http://wpn.shangyingyoupin.top

TS:   // child_process / cluster 模块
来源：http://smx.mhx1999.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://onz.wangdashe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cdd.shuidangran.top

Ruby: // fork 块
来源：http://ypm.zycfv.cn

C#:   Parallel.For
来源：http://mqf.ppjwa.cn

================================================================================
来源：http://xqy.hfpthk.cn

P. 常用工具函数
来源：http://blw.zhongyouzk.top

================================================================================
来源：http://otx.shuidangran.top

[P01] 生成 UUID
来源：http://wbe.havefunace.top

Py:   str(uuid.uuid4())
来源：http://kfl.wangdashe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://pme.jiagoushi.top

JS:   crypto.randomUUID()
来源：http://tuf.haohaochexian.top

TS:   crypto.randomUUID()
来源：http://nte.shangyingyoupin.top

Java: UUID.randomUUID().toString()
来源：http://qxm.zhijiandao.cn

Go:   // 用 github.com/google/uuid
来源：http://iqi.fehbvm.com

Ruby: SecureRandom.uuid
来源：http://qgc.smart0.xyz

C#:   Guid.NewGuid().ToString()
来源：http://upf.fehbvm.com

[P02] MD5 / SHA256 摘要
来源：http://dqh.jlsjyb.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://syt.jlsjyb.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wva.pengpengdd.cyou

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lob.zhiwuduotai.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sjs.yanxiufei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sph.dianchejie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zqt.hfpthk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ryv.52xcode.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xyn.yj202588.top

[P03] 生成短随机字符串
来源：http://gsy.shanyushiyangtech.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ujz.tanke756.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ckk.sjlbkw.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mtk.zhixingplan.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wmh.zhixingplan.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nvi.jinyuanbaomall.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://arm.pycfn.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://slf.gotoacloud.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kkh.yangfankeji.com

[P04] 求长度
来源：http://tfd.bjfxy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nsh.zdbjq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yiz.sysykeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dxw.jqgfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cbi.bjfxy.top

Java: list.size();  map.size();  s.length()
来源：http://ebp.hcnkem.com

Go:   len(arr);  len(m)
来源：http://ytu.daria6918.cn

Ruby: x.length;  x.size
来源：http://bjq.aizwys.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bby.nanxinkj.top

[P05] 判断两个对象内容是否相等
来源：http://hwb.cdnleiting.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://oph.guowangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ewr.jinqigufen.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vgc.nwbrower.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qpu.sjlbkw.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ezp.snrcjt.cn

Go:   reflect.DeepEqual(a, b)
来源：http://nyl.xylfe.cn

Ruby: a == b
来源：http://mng.ydzc1.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kiq.yonumen.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://eds.cucudq.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sfr.vehdjk.com

PHP:  if (empty($x)) {}
来源：http://pqi.0kj1m.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tjl.fanxiaobao.xyz

TS:   if (x == null) {}
来源：http://vgd.iojbl.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://did.zhoulong.xyz

Go:   if x == nil {}
来源：http://bfn.yfazqb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ffu.jqgfzy.top

C#:   if (x is null) {}
来源：http://zdh.bbcook.cn

[P07] 防抖与节流
来源：http://hme.dianchejie.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bdz.gaohongyu789.top

PHP:  // 手写时间戳比较
来源：http://uup.yuxming.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iga.c1oappe.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ryf.fktsv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wha.dianchejie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vlz.sysykeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ati.dianchejie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://aji.bjfxy.top

[P08] 处理浮点精度问题
来源：http://ixn.yongpay.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://axc.sxryk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ucz.birdmap.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://prx.xuetiantiany.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rkm.kuanghao11.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vrk.jqgufenzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nfs.pycfn.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uyo.sufxvd.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mqq.ivvv.top

================================================================================
来源：http://drn.cucudq.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jnl.yvedp.cn

================================================================================
来源：http://hql.sweek.top

[Q01] 创建表
来源：http://bbc.hnqzz.top

CREATE TABLE users (
来源：http://uqz.epnwcf.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vvi.cashguo.top

name VARCHAR(50) NOT NULL,
来源：http://les.dashuyun.cn

email VARCHAR(100) UNIQUE,
来源：http://gdn.fzhhl.top


<!-- 参考信息 -->