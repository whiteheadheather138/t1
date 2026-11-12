代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kin.chenzaomai.com

Go:   exec.Command("ls", "-l").Output()
来源：http://srz.meibo888.top

Ruby: system("ls -l");  `ls -l`
来源：http://ceh.tianlin.xyz

C#:   Process.Start("ls", "-l");
来源：http://rng.sweek.top

[M04] 获取当前工作目录
来源：http://oml.tian-w.cn

Py:   os.getcwd()
来源：http://jri.guannengcc.top

PHP:  getcwd();
来源：http://qke.fktsv.cn

JS:   process.cwd()
来源：http://kul.dashuyun.cn

TS:   process.cwd()
来源：http://lsh.guowangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://lqf.svipenyu.cn

Go:   os.Getwd()
来源：http://las.xuetiantiany.cn

Ruby: Dir.pwd
来源：http://nmj.bbcook.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yhz.aibaodan.cn

[M05] 设置退出码
来源：http://zpm.zhiwuduotai.top

Py:   sys.exit(1)
来源：http://prw.xuanzx.com

PHP:  exit(1);
来源：http://srp.cqqwz.cn

JS:   process.exit(1)
来源：http://exg.bbcook.cn

TS:   process.exit(1)
来源：http://dwk.chenzaomai.com

Java: System.exit(1)
来源：http://nlg.316326.xyz

Go:   os.Exit(1)
来源：http://znh.pengpengdd.cyou

Ruby: exit 1
来源：http://khw.meibo888.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hfg.smart0.xyz

[M06] 向标准错误输出
来源：http://nan.chenjidiqi.icu

Py:   print("err", file=sys.stderr)
来源：http://luf.yj20258888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://boz.gaohongyu789.top

JS:   console.error("err")
来源：http://yjm.fanxiaobao.xyz

TS:   console.error("err")
来源：http://evr.cdnleiting.top

Java: System.err.println("err")
来源：http://gpf.gogol.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mch.jinqigufen.top

Ruby: warn "err"
来源：http://sxw.jqgfzy.top

C#:   Console.Error.WriteLine("err")
来源：http://wuk.zdbjq.cn

[M07] 判断是否为主入口
来源：http://iyb.cheryme.top

Py:   if __name__ == "__main__":
来源：http://ssq.yongpay.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qse.xziqi.cn

JS:   require.main === module
来源：http://iqv.bjfxy.top

TS:   require.main === module
来源：http://civ.yuanzhike.top

Java: public static void main(String[] args)
来源：http://vlp.yongpay.top

Go:   func main()
来源：http://lvj.zhiwuduotai.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://prm.redwolf501.top

C#:   static void Main(string[] args)
来源：http://xfr.yuxming.cn

[M08] 获取系统与运行时信息
来源：http://tln.yueranfly.top

Py:   platform.system();  platform.python_version()
来源：http://fsm.vqdsnc.cn

PHP:  PHP_OS;  phpversion();
来源：http://ocj.zhiwuduotai.top

JS:   process.platform;  process.version
来源：http://wqi.ehwqpu.com

TS:   process.platform;  process.version
来源：http://vqn.smart0.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cxn.ivvv.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xvr.haohaochexian.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zzi.aibaodan.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zgz.tianlin.xyz

================================================================================
来源：http://exc.ybcxt.top

N. 数据结构与算法
来源：http://pjd.chenlongwang.top

================================================================================
来源：http://dij.daxiang520.top

[N01] 二分查找（有序数组）
来源：http://nge.zhengqikj.top

Py:   bisect.bisect_left(arr, x)
来源：http://lyi.ctjpmb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rie.yonumen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jtz.xuetiantiany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ifm.c1oappe.top

Java: Arrays.binarySearch(arr, x)
来源：http://zfo.mhx1999.top

Go:   sort.SearchInts(arr, x)
来源：http://kxl.ydzc1.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://xos.guannengcc.top

C#:   Array.BinarySearch(arr, x)
来源：http://plo.ppjwa.cn

[N02] 排序（工程实践用内置实现）
来源：http://obl.hysaishi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ugi.yongpay.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pwd.zhoulong.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://cgg.fzhhl.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dfm.ybcxt.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qdx.hfpthk.cn

Go:   slices.Sort(arr)
来源：http://wzf.smart0.xyz

Ruby: arr.sort
来源：http://mxr.hammf.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wzt.birdmap.top

[N03] 快速排序（分治示例）
来源：http://mie.9152youxi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cov.shzxlz.cn

PHP:  // 递归实现，或用 usort
来源：http://bwf.jlsjyb.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://puy.jinghuilouyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tws.jqgufenzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bdd.zycfv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zlu.guowangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mox.zhijiandao.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bfd.gotoacloud.top

[N04] 斐波那契数列
来源：http://iqn.redwolf501.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kig.pycfn.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pyl.nwbrower.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mru.hcnkem.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sji.yonumen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://aqx.hammf.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ynl.svipenyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tgu.cashguo.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uwe.aibaodan.cn

[N05] 最大公约数
来源：http://ibg.mhx1999.top

Py:   math.gcd(a, b)
来源：http://lci.birdmap.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rco.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://foz.dashuyun.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hqh.gogol.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://plf.gogol.net.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cmu.ywan-chungtsiang.top

Ruby: a.gcd(b)
来源：http://qfj.sjlbkw.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cie.jinqigufen.top

[N06] 判断回文字符串
来源：http://tsz.jinghuilouyu.cn

Py:   s == s[::-1]
来源：http://szc.yuxming.cn

PHP:  $s === strrev($s);
来源：http://xxe.meibo888.top

JS:   s === [...s].reverse().join("")
来源：http://txj.zhixingplan.top

TS:   s === [...s].reverse().join("")
来源：http://xnd.jianghu66.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kjt.andypj.xyz

Go:   // 双指针从两端比较
来源：http://xne.nanxinkj.top

Ruby: s == s.reverse
来源：http://pbr.tarul.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ezr.shangyingyoupin.top

[N07] 两数之和（返回下标）
来源：http://tbr.yvedp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xgr.yuxming.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ein.mhx1999.top

JS:   // 手写 Map：map.set(v, i)
来源：http://qtc.ivvv.top

TS:   // 手写 Map<string, number>
来源：http://usr.hammf.cn

Java: // 手写 HashMap
来源：http://nin.vqdsnc.cn

Go:   // 手写 map[int]int
来源：http://lev.zycfv.cn

Ruby: // 手写 Hash
来源：http://izg.zhaomingkeji.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://ajv.gaohongyu789.top

[N08] 生成全排列
来源：http://xjo.havefunace.top

Py:   itertools.permutations(arr)
来源：http://pxi.jinyuanbaomall.cn

PHP:  // 手写递归交换
来源：http://nxt.tianlin.xyz

JS:   // 手写回溯递归
来源：http://rck.guannengcc.top

TS:   // 手写回溯递归
来源：http://fij.aizwys.cn

Java: // 手写回溯递归
来源：http://yxq.jinqigfzy.top

Go:   // 手写回溯递归
来源：http://nvj.gogol.net.cn

Ruby: arr.permutation.to_a
来源：http://ozh.yuxming.cn

C#:   // 手写回溯递归
来源：http://wtf.dianchejie.cn

[N09] 栈与队列
来源：http://ikt.zhixingplan.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vsz.andypj.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ywo.zhixingplan.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jrz.52xcode.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://nku.redwolf501.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qog.jyoumei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://nov.yonumen.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://way.yongpay.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wsl.haohaochexian.top

[N10] 链表节点定义
来源：http://nho.bjfxy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://rzn.daria6918.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://nth.ybcxt.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lbs.sxryk.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hrn.pycfn.com

Java: class Node { int v; Node next; }
来源：http://jty.xuetiantiany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://szd.zhaomingkeji.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://gal.ctjpmb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://zec.jyoumei.cn

[N11] 二叉树中序遍历
来源：http://ino.vqdsnc.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kuv.sjlbkw.cn

PHP:  // 手写递归函数
来源：http://uah.xingfuxueyuan.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://prs.fktsv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tdb.yuxming.cn

Java: // 手写递归
来源：http://hvy.zhongyouzk.top

Go:   // 手写递归
来源：http://rjk.yonumen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://rsc.zhijiandao.cn

C#:   // 手写递归
来源：http://lei.daria6918.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jxf.0kj1m.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zwf.ivvv.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xgx.guowangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bsu.yj20258.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rej.vehdjk.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vac.bjfxy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zqv.ywan-chungtsiang.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lng.nanxuanxn.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jox.tarul.cn

================================================================================
来源：http://lsr.bjfxy.top

O. 并发与异步
来源：http://jze.gogol.net.cn

================================================================================
来源：http://nzb.dianchejie.cn

[O01] 启动一个线程
来源：http://osi.meibo888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cci.cucudq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hbc.zhijiandao.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sfh.chenlongwang.top

TS:   // 同 JS
来源：http://agh.epnwcf.com

Java: new Thread(() -> f()).start()
来源：http://nyf.jqgfzy.top

Go:   go f()
来源：http://ehi.yueranfly.top

Ruby: Thread.new { f }
来源：http://ikd.zhongyouzk.top

C#:   Task.Run(() => F());
来源：http://ykk.tian-w.cn

[O02] 使用线程池
来源：http://ora.zdbjq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://piw.chenjidiqi.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tah.shzxlz.cn

JS:   // worker_threads 线程池
来源：http://pct.c1oappe.top

TS:   // worker_threads 线程池
来源：http://hbj.guowangkeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://sxj.jianghu66.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dmu.fzhhl.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qvs.wangshuangyany.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bjm.jqgfzy.top

[O03] 加锁保护共享数据
来源：http://zrx.shangyingyoupin.top

Py:   with lock: shared += 1
来源：http://naj.epnwcf.com

PHP:  // 用 flock() 做文件锁
来源：http://naa.kuanghao11.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hgi.yj20258.top

TS:   // 同 JS
来源：http://boa.ehwqpu.com

Java: synchronized (this) { shared++; }
来源：http://vqw.havefunace.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xdn.smart0.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://vqg.vehdjk.com

C#:   lock (gate) { shared++; }
来源：http://wij.xingfuxueyuan.xyz

[O04] 定义异步函数并等待
来源：http://qka.cashguo.top

Py:   async def f():⏎    await g()
来源：http://khe.zhiwuduotai.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://efh.zdqjudy.top

JS:   async function f() { await g(); }
来源：http://yel.chenjidiqi.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://afv.chenjidiqi.icu

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cbs.zycfv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tvx.svipenyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kpd.ywan-chungtsiang.top

C#:   async Task F() { await G(); }
来源：http://czd.yonumen.top

[O05] 并发执行并等待全部完成
来源：http://ekl.fengsongda.top

Py:   asyncio.gather(*tasks)
来源：http://yvn.mhx1999.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jhb.nanxuanxn.top

JS:   await Promise.all(tasks)
来源：http://ujf.yonumen.top

TS:   await Promise.all(tasks)
来源：http://hyl.tanke756.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ryv.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://elm.xuanzx.com

Ruby: threads.map(&:join)
来源：http://lai.aizwys.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://epq.shzxlz.cn

[O06] 使用进程池
来源：http://rcl.havefunace.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://erl.zhoulong.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://rfs.jiagoushi.top

JS:   // child_process / cluster 模块
来源：http://zni.bjfxy.top

TS:   // child_process / cluster 模块
来源：http://yxb.bjfxy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qpw.yueranfly.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jvu.wangshuangyany.cn

Ruby: // fork 块
来源：http://kew.tanke756.top

C#:   Parallel.For
来源：http://qek.zycfv.cn

================================================================================
来源：http://wwu.daxiang520.top

P. 常用工具函数
来源：http://wbd.zhongyouzk.top

================================================================================
来源：http://yoa.hcnkem.com

[P01] 生成 UUID
来源：http://qhv.shanyushiyangkeji.top

Py:   str(uuid.uuid4())
来源：http://jgk.cashguo.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://asd.jiagoushi.top

JS:   crypto.randomUUID()
来源：http://xsu.uphjek.com

TS:   crypto.randomUUID()
来源：http://jkb.zhoulong.xyz

Java: UUID.randomUUID().toString()
来源：http://tku.ehwqpu.com

Go:   // 用 github.com/google/uuid
来源：http://ltr.wangdashe.top

Ruby: SecureRandom.uuid
来源：http://atd.hnqzz.top

C#:   Guid.NewGuid().ToString()
来源：http://xpt.jqgufenzy.top

[P02] MD5 / SHA256 摘要
来源：http://lwn.aizwys.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aby.jyoumei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://zmd.yuxming.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rur.yangfankeji.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bhp.andypj.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xln.birdmap.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://phx.nanxinkj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lyb.ybcxt.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uot.hesvh.cn

[P03] 生成短随机字符串
来源：http://pby.ybcxt.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vih.jqgufenzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://efr.redwolf501.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://skw.sufxvd.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uak.bjfxy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nvi.nanxinkj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://txf.yuanzhike.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://kmg.xuetiantiany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qpv.iojbl.cn

[P04] 求长度
来源：http://tog.cqqwz.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sqa.shanyushiyangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mow.jinqigufen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://phy.zhiwuduotai.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fys.sjlbkw.cn

Java: list.size();  map.size();  s.length()
来源：http://hye.gogol.net.cn

Go:   len(arr);  len(m)
来源：http://npm.jlsjyb.cn

Ruby: x.length;  x.size
来源：http://ptc.pengpengdd.cyou

C#:   list.Count;  dict.Count;  s.Length
来源：http://gft.yvedp.cn

[P05] 判断两个对象内容是否相等
来源：http://bbk.chenjidiqi.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://jvw.aibaodan.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lkc.yonumen.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oup.yuxming.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://imn.chenjidiqi.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://whq.jinyuanbaomall.cn

Go:   reflect.DeepEqual(a, b)
来源：http://zuf.yanxiufei.cn

Ruby: a == b
来源：http://gkk.gzhubu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lzm.kuanghao11.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nxm.sweek.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yaq.zycfv.cn

PHP:  if (empty($x)) {}
来源：http://hte.jinghuilouyu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aep.wangshuangyany.cn

TS:   if (x == null) {}
来源：http://cup.c1oappe.top

Java: if (x == null || x.isEmpty()) {}
来源：http://tnv.ehwqpu.com

Go:   if x == nil {}
来源：http://era.ctjpmb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://snk.vqdsnc.cn

C#:   if (x is null) {}
来源：http://vge.jqgufenzy.top

[P07] 防抖与节流
来源：http://gte.zhoulong.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vkv.zdbjq.cn

PHP:  // 手写时间戳比较
来源：http://alv.yuxming.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zxz.daria6918.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yyh.sweek.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://isl.hongshengwenyu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pzu.fanxiaobao.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://uow.mhx1999.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dhs.jiagoushi.top

[P08] 处理浮点精度问题
来源：http://dmo.sjlbkw.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://awz.hnqzz.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vvn.jyoumei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ewk.jqgfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mtn.cdnleiting.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wwx.xingfuxueyuan.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zie.yonumen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rje.quarkkingdee.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lzs.chenjidiqi.icu

================================================================================
来源：http://lrl.kuanghao11.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tsw.52xcode.cn

================================================================================
来源：http://aqb.chenzaomai.com

[Q01] 创建表
来源：http://pko.jinqigufen.top

CREATE TABLE users (
来源：http://bpd.jinghuilouyu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://asg.xinyue.icu

name VARCHAR(50) NOT NULL,
来源：http://nso.dianchejie.cn

email VARCHAR(100) UNIQUE,
来源：http://oqr.xuetiantiany.cn


<!-- 参考信息 -->