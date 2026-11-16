代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rqz.hysaishi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xpj.zhoulong.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://qvs.zdbjq.cn

C#:   Process.Start("ls", "-l");
来源：http://uiz.gotoacloud.top

[M04] 获取当前工作目录
来源：http://xof.tanke756.top

Py:   os.getcwd()
来源：http://zus.havefunace.top

PHP:  getcwd();
来源：http://wvn.52xcode.cn

JS:   process.cwd()
来源：http://cyy.yongpay.top

TS:   process.cwd()
来源：http://yqb.gzhubu.top

Java: Path.of("").toAbsolutePath()
来源：http://sxl.yj202588.top

Go:   os.Getwd()
来源：http://ghr.jqgfzy.top

Ruby: Dir.pwd
来源：http://xqy.pengpengdd.cyou

C#:   Directory.GetCurrentDirectory()
来源：http://rfy.jinqigfzy.top

[M05] 设置退出码
来源：http://byu.gzhubu.top

Py:   sys.exit(1)
来源：http://uun.meibo888.top

PHP:  exit(1);
来源：http://oyb.hysaishi.cn

JS:   process.exit(1)
来源：http://dkd.yj20258888.top

TS:   process.exit(1)
来源：http://yhz.hnqzz.top

Java: System.exit(1)
来源：http://lzx.vehdjk.com

Go:   os.Exit(1)
来源：http://unn.nwbrower.top

Ruby: exit 1
来源：http://jrc.zhengqikj.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jci.jinqigufen.top

[M06] 向标准错误输出
来源：http://otf.hcnkem.com

Py:   print("err", file=sys.stderr)
来源：http://rdh.kuanghao11.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mus.wangdashe.top

JS:   console.error("err")
来源：http://iln.chenzaomai.com

TS:   console.error("err")
来源：http://xtl.yj20258.top

Java: System.err.println("err")
来源：http://iwz.epnwcf.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wky.yfazqb.com

Ruby: warn "err"
来源：http://gax.jyoumei.cn

C#:   Console.Error.WriteLine("err")
来源：http://thk.daxiang520.top

[M07] 判断是否为主入口
来源：http://aqf.yfazqb.com

Py:   if __name__ == "__main__":
来源：http://lcc.shanyushiyangtech.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xqp.wangdashe.top

JS:   require.main === module
来源：http://cjs.xylfe.cn

TS:   require.main === module
来源：http://kmb.fktsv.cn

Java: public static void main(String[] args)
来源：http://ffk.sysykeji.top

Go:   func main()
来源：http://jhv.aibaodan.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nct.jinqigufen.top

C#:   static void Main(string[] args)
来源：http://gfo.vqdsnc.cn

[M08] 获取系统与运行时信息
来源：http://ruz.aizwys.cn

Py:   platform.system();  platform.python_version()
来源：http://veb.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://gwo.hammf.cn

JS:   process.platform;  process.version
来源：http://egl.yj20258888.top

TS:   process.platform;  process.version
来源：http://qlt.yanxiufei.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wqm.yongpay.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://yag.nwbrower.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://les.hywenlv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cwg.chenzaomai.com

================================================================================
来源：http://anw.zhiwuduotai.top

N. 数据结构与算法
来源：http://goc.tanke756.top

================================================================================
来源：http://rsk.ctjpmb.com

[N01] 二分查找（有序数组）
来源：http://qkx.ywan-chungtsiang.top

Py:   bisect.bisect_left(arr, x)
来源：http://teg.52xcode.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pil.fehbvm.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qxt.aizwys.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qxm.yongpay.top

Java: Arrays.binarySearch(arr, x)
来源：http://qxf.52xcode.cn

Go:   sort.SearchInts(arr, x)
来源：http://pyo.gaohongyu789.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://amj.iojbl.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sjr.hesvh.cn

[N02] 排序（工程实践用内置实现）
来源：http://akh.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://opa.hcnkem.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jyc.chenzaomai.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://olr.wangshuangyany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rrx.hywenlv.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lew.ywan-chungtsiang.top

Go:   slices.Sort(arr)
来源：http://owd.cashguo.top

Ruby: arr.sort
来源：http://lvp.xylfe.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xbr.shuidangran.top

[N03] 快速排序（分治示例）
来源：http://czv.nanxuanxn.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rvl.ivvv.top

PHP:  // 递归实现，或用 usort
来源：http://uio.jlsjyb.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wej.sjlbkw.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ptx.jinqigfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://aqf.meibo888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jwd.jianghu66.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vgt.cashguo.top

C#:   // 手写递归，或 Array.Sort
来源：http://urr.gotoacloud.top

[N04] 斐波那契数列
来源：http://qnu.andypj.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ncg.xingfuxueyuan.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ubz.shzxlz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kqw.sjlbkw.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zmy.ivvv.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://znq.cheryme.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ttr.vqdsnc.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kvg.cucudq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wdk.nanxinkj.top

[N05] 最大公约数
来源：http://pwl.yj20258888.top

Py:   math.gcd(a, b)
来源：http://vyl.bjfxy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hhp.cucudq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mgo.ydjk.org.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mwi.chenlongwang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wip.jinqigufen.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nrg.snrcjt.cn

Ruby: a.gcd(b)
来源：http://eya.yonumen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yzw.yuanzhike.top

[N06] 判断回文字符串
来源：http://tbh.yueranfly.top

Py:   s == s[::-1]
来源：http://mcl.ctjpmb.com

PHP:  $s === strrev($s);
来源：http://lon.zhijiandao.cn

JS:   s === [...s].reverse().join("")
来源：http://mfd.hfpthk.cn

TS:   s === [...s].reverse().join("")
来源：http://uqy.sxryk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://olu.smart0.xyz

Go:   // 双指针从两端比较
来源：http://mux.zhoulong.xyz

Ruby: s == s.reverse
来源：http://axi.tian-w.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://snd.ppjwa.cn

[N07] 两数之和（返回下标）
来源：http://bra.hnqzz.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rjp.vqdsnc.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rtz.iojbl.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://hqa.yueranfly.top

TS:   // 手写 Map<string, number>
来源：http://udc.shanyushiyangtech.top

Java: // 手写 HashMap
来源：http://loa.fanxiaobao.xyz

Go:   // 手写 map[int]int
来源：http://cdh.fanxiaobao.xyz

Ruby: // 手写 Hash
来源：http://aep.svipenyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ylh.guannengcc.top

[N08] 生成全排列
来源：http://rjb.jinqigufen.top

Py:   itertools.permutations(arr)
来源：http://rqk.tian-w.cn

PHP:  // 手写递归交换
来源：http://gol.zdbjq.cn

JS:   // 手写回溯递归
来源：http://lrb.ybcxt.top

TS:   // 手写回溯递归
来源：http://ojs.tarul.cn

Java: // 手写回溯递归
来源：http://rxa.hywenlv.cn

Go:   // 手写回溯递归
来源：http://zty.gogol.net.cn

Ruby: arr.permutation.to_a
来源：http://osl.xuanzx.com

C#:   // 手写回溯递归
来源：http://ovj.nanxinkj.top

[N09] 栈与队列
来源：http://ell.shuidangran.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ohk.jiagoushi.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sym.daxiang520.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uce.ivvv.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ape.gotoacloud.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vtc.tianlin.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cqr.jqgfzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rpk.fehbvm.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eli.aibaodan.cn

[N10] 链表节点定义
来源：http://nqj.zhongyouzk.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://vka.52xcode.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://fxc.hammf.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://fiq.guannengcc.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vbg.shangyingyoupin.top

Java: class Node { int v; Node next; }
来源：http://nex.redwolf501.top

Go:   type Node struct { V int; Next *Node }
来源：http://bjb.cdnleiting.top

Ruby: Node = Struct.new(:v, :next)
来源：http://abf.ybcxt.top

C#:   class Node { public int V; public Node? Next; }
来源：http://hng.ivvv.top

[N11] 二叉树中序遍历
来源：http://xuv.bbcook.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://eka.chenzaomai.com

PHP:  // 手写递归函数
来源：http://agx.ydjk.org.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ugq.redwolf501.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zzn.zhengqikj.top

Java: // 手写递归
来源：http://rtv.vqdsnc.cn

Go:   // 手写递归
来源：http://whe.wangshuangyany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lsy.snrcjt.cn

C#:   // 手写递归
来源：http://snx.ydjk.org.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gkg.vqdsnc.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://eua.mhx1999.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pwl.yuxming.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jqq.gogol.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dbl.yanxiufei.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ndw.yj20258888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zyl.xinyue.icu

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jrl.daxiang520.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uni.cqqwz.cn

================================================================================
来源：http://jcg.cheryme.top

O. 并发与异步
来源：http://ath.shuidangran.top

================================================================================
来源：http://kxf.ehwqpu.com

[O01] 启动一个线程
来源：http://chr.dianchejie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gpu.xziqi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lkk.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://voa.c1oappe.top

TS:   // 同 JS
来源：http://fog.ybcxt.top

Java: new Thread(() -> f()).start()
来源：http://htl.vehdjk.com

Go:   go f()
来源：http://gyj.9152youxi.cn

Ruby: Thread.new { f }
来源：http://nkp.zdqjudy.top

C#:   Task.Run(() => F());
来源：http://oiw.chenjidiqi.icu

[O02] 使用线程池
来源：http://xyb.yuxming.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bzc.zhongyouzk.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lwh.tianlin.xyz

JS:   // worker_threads 线程池
来源：http://yyp.shuidangran.top

TS:   // worker_threads 线程池
来源：http://xfa.cdnleiting.top

Java: Executors.newFixedThreadPool(4)
来源：http://xhk.zhijiandao.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hyf.haohaochexian.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tms.zhixingplan.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kqz.fehbvm.com

[O03] 加锁保护共享数据
来源：http://gow.hammf.cn

Py:   with lock: shared += 1
来源：http://klq.hnxiangtu.top

PHP:  // 用 flock() 做文件锁
来源：http://wxb.wangdashe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jvy.xuanzx.com

TS:   // 同 JS
来源：http://fox.jinyuanbaomall.cn

Java: synchronized (this) { shared++; }
来源：http://tpn.hammf.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bbm.yj202588.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://gql.chenlongwang.top

C#:   lock (gate) { shared++; }
来源：http://taa.gaohongyu789.top

[O04] 定义异步函数并等待
来源：http://kgi.cucudq.cn

Py:   async def f():⏎    await g()
来源：http://ejr.vehdjk.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jvt.aizwys.cn

JS:   async function f() { await g(); }
来源：http://gmx.daria6918.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wvj.uphjek.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vgk.guannengcc.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kkr.hysaishi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jvi.zhengqikj.top

C#:   async Task F() { await G(); }
来源：http://sup.bbcook.cn

[O05] 并发执行并等待全部完成
来源：http://wjo.havefunace.top

Py:   asyncio.gather(*tasks)
来源：http://mex.dashuyun.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vqo.ywan-chungtsiang.top

JS:   await Promise.all(tasks)
来源：http://vjv.gotoacloud.top

TS:   await Promise.all(tasks)
来源：http://lrv.hfpthk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ozq.mhx1999.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ymy.kuanghao11.cn

Ruby: threads.map(&:join)
来源：http://osq.cheryme.top

C#:   await Task.WhenAll(t1, t2)
来源：http://znq.daria6918.cn

[O06] 使用进程池
来源：http://vzf.zdbjq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xug.aibaodan.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qjf.ybcxt.top

JS:   // child_process / cluster 模块
来源：http://vfk.hesvh.cn

TS:   // child_process / cluster 模块
来源：http://jrh.tarul.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pfz.jlsjyb.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://aqa.quarkkingdee.top

Ruby: // fork 块
来源：http://suq.meibo888.top

C#:   Parallel.For
来源：http://kxn.jinqigufen.top

================================================================================
来源：http://oum.aibaodan.cn

P. 常用工具函数
来源：http://mkg.ydzc1.top

================================================================================
来源：http://axr.hammf.cn

[P01] 生成 UUID
来源：http://qgw.andypj.xyz

Py:   str(uuid.uuid4())
来源：http://wud.tanke756.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://stz.feifeiyinyue.top

JS:   crypto.randomUUID()
来源：http://xvr.ppjwa.cn

TS:   crypto.randomUUID()
来源：http://mec.fengsongda.top

Java: UUID.randomUUID().toString()
来源：http://fdw.redwolf501.top

Go:   // 用 github.com/google/uuid
来源：http://imw.ehwqpu.com

Ruby: SecureRandom.uuid
来源：http://jvt.sweek.top

C#:   Guid.NewGuid().ToString()
来源：http://zzx.meibo888.top

[P02] MD5 / SHA256 摘要
来源：http://oqn.cucudq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mni.yfazqb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://zwq.gogol.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ioe.jiagoushi.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://skw.dashuyun.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ejn.pengpengdd.cyou

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hxa.chenjidiqi.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kyu.0kj1m.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iva.hcnkem.com

[P03] 生成短随机字符串
来源：http://qqc.yj20258.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ljw.ivvv.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bqc.haohaochexian.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jkw.haohaochexian.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cum.smart0.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://owp.bjfxy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wnv.xinyue.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://zkh.fktsv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xno.zhoulong.xyz

[P04] 求长度
来源：http://euz.shuidangran.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://quz.wangdashe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wtd.haohaochexian.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wwg.cucudq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mcz.hammf.cn

Java: list.size();  map.size();  s.length()
来源：http://toi.guannengcc.top

Go:   len(arr);  len(m)
来源：http://oyd.yonumen.top

Ruby: x.length;  x.size
来源：http://pkp.316326.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://lme.yuanzhike.top

[P05] 判断两个对象内容是否相等
来源：http://pir.hcnkem.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://cio.hongshengwenyu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://srm.fengsongda.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fwd.ydjk.org.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jen.yj202588.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qbj.316326.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://aso.xinyue.icu

Ruby: a == b
来源：http://vse.gotoacloud.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wcp.shzxlz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wxv.xinyue.icu

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tkk.bbcook.cn

PHP:  if (empty($x)) {}
来源：http://mli.jiagoushi.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hft.zhijiandao.cn

TS:   if (x == null) {}
来源：http://den.tianlin.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://ccl.c1oappe.top

Go:   if x == nil {}
来源：http://bmk.nanxuanxn.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xxd.jinghuilouyu.cn

C#:   if (x is null) {}
来源：http://gjt.yfazqb.com

[P07] 防抖与节流
来源：http://dfx.sufxvd.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gkq.gzhubu.top

PHP:  // 手写时间戳比较
来源：http://tqj.tian-w.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lqd.nwbrower.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bnt.iojbl.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rum.tianlin.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xrw.wangshuangyany.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nwz.zhijiandao.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gju.xziqi.cn

[P08] 处理浮点精度问题
来源：http://vxw.yfazqb.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ptx.quarkkingdee.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zyf.daria6918.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dgq.52xcode.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ebt.dianchejie.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rxf.cucudq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mzd.nanxinkj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://atv.hysaishi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ivr.zdbjq.cn

================================================================================
来源：http://jqb.xingfuxueyuan.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tzt.dianchejie.cn

================================================================================
来源：http://wgi.cheryme.top

[Q01] 创建表
来源：http://sye.bjfxy.top

CREATE TABLE users (
来源：http://vbc.fktsv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jxi.havefunace.top

name VARCHAR(50) NOT NULL,
来源：http://owg.sufxvd.cn

email VARCHAR(100) UNIQUE,
来源：http://hiw.pycfn.com


<!-- 参考信息 -->