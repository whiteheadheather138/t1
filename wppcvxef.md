代发 wailian999

[M04] 获取当前工作目录
来源：http://quf.52xcode.cn

Py:   os.getcwd()
来源：http://tvq.uphjek.com

PHP:  getcwd();
来源：http://wtq.xziqi.cn

JS:   process.cwd()
来源：http://tvy.jinyuanbaomall.cn

TS:   process.cwd()
来源：http://uzf.c1oappe.top

Java: Path.of("").toAbsolutePath()
来源：http://tqp.daxiang520.top

Go:   os.Getwd()
来源：http://jty.jinyuanbaomall.cn

Ruby: Dir.pwd
来源：http://ibx.hongshengwenyu.top

C#:   Directory.GetCurrentDirectory()
来源：http://uki.zhongyouzk.top

[M05] 设置退出码
来源：http://fld.havefunace.top

Py:   sys.exit(1)
来源：http://icm.cdnleiting.top

PHP:  exit(1);
来源：http://fjf.nwbrower.top

JS:   process.exit(1)
来源：http://eyo.vqdsnc.cn

TS:   process.exit(1)
来源：http://fpb.9152youxi.cn

Java: System.exit(1)
来源：http://azj.shanyushiyangtech.top

Go:   os.Exit(1)
来源：http://gsq.316326.xyz

Ruby: exit 1
来源：http://skm.zhengqikj.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tiz.yvedp.cn

[M06] 向标准错误输出
来源：http://dua.snrcjt.cn

Py:   print("err", file=sys.stderr)
来源：http://eox.zhoulong.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://gnv.redwolf501.top

JS:   console.error("err")
来源：http://heq.ydzc1.top

TS:   console.error("err")
来源：http://yck.cqqwz.cn

Java: System.err.println("err")
来源：http://cok.tianlin.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://knw.xuetiantiany.cn

Ruby: warn "err"
来源：http://xys.iojbl.cn

C#:   Console.Error.WriteLine("err")
来源：http://mqd.jqgufenzy.top

[M07] 判断是否为主入口
来源：http://ldj.haohaochexian.top

Py:   if __name__ == "__main__":
来源：http://bjz.sysykeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hwb.fanxiaobao.xyz

JS:   require.main === module
来源：http://ulu.andypj.xyz

TS:   require.main === module
来源：http://umq.gaohongyu789.top

Java: public static void main(String[] args)
来源：http://dhj.yj202588.top

Go:   func main()
来源：http://ijl.tian-w.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kjw.daria6918.cn

C#:   static void Main(string[] args)
来源：http://pet.shanyushiyangtech.top

[M08] 获取系统与运行时信息
来源：http://nnh.nanxuanxn.top

Py:   platform.system();  platform.python_version()
来源：http://lyv.chenzaomai.com

PHP:  PHP_OS;  phpversion();
来源：http://ckf.jqgufenzy.top

JS:   process.platform;  process.version
来源：http://rhz.pengpengdd.cyou

TS:   process.platform;  process.version
来源：http://yen.chenjidiqi.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://uaz.vqdsnc.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://znb.ctjpmb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jex.xuanzx.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://pyl.bbcook.cn

================================================================================
来源：http://ypk.nanxuanxn.top

N. 数据结构与算法
来源：http://rjz.uphjek.com

================================================================================
来源：http://nqo.fehbvm.com

[N01] 二分查找（有序数组）
来源：http://smk.nanxuanxn.top

Py:   bisect.bisect_left(arr, x)
来源：http://wyc.shanyushiyangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pzr.jinyuanbaomall.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pvb.xingfuxueyuan.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pbo.yuxming.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dal.hnxiangtu.top

Go:   sort.SearchInts(arr, x)
来源：http://qft.gogol.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://otu.ivvv.top

C#:   Array.BinarySearch(arr, x)
来源：http://pmv.dianchejie.cn

[N02] 排序（工程实践用内置实现）
来源：http://chf.hywenlv.cn

Py:   sorted(arr);  arr.sort()
来源：http://pry.jqgfzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ggs.snrcjt.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://iwv.shzxlz.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://xtl.jinqigfzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gik.yfazqb.com

Go:   slices.Sort(arr)
来源：http://tnl.zhixingplan.top

Ruby: arr.sort
来源：http://fao.pycfn.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://utd.cqqwz.cn

[N03] 快速排序（分治示例）
来源：http://eeb.cashguo.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://txf.andypj.xyz

PHP:  // 递归实现，或用 usort
来源：http://lvn.shangyingyoupin.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://meq.yvedp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cnt.jinqigfzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ctd.bjfxy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dzu.hnxiangtu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://niv.cheryme.top

C#:   // 手写递归，或 Array.Sort
来源：http://pwn.cheryme.top

[N04] 斐波那契数列
来源：http://vdv.tianlin.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ams.iojbl.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://okm.hongshengwenyu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hud.smart0.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://whu.hysaishi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gat.xziqi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xso.yj20258.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://avw.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://onc.sjlbkw.cn

[N05] 最大公约数
来源：http://jhy.yueranfly.top

Py:   math.gcd(a, b)
来源：http://vfq.jinqigfzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kzx.jianghu66.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dbf.zycfv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fsg.daria6918.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://onl.hysaishi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ubj.aibaodan.cn

Ruby: a.gcd(b)
来源：http://mgl.cashguo.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aia.cucudq.cn

[N06] 判断回文字符串
来源：http://irt.fengsongda.top

Py:   s == s[::-1]
来源：http://bhj.hysaishi.cn

PHP:  $s === strrev($s);
来源：http://npn.52xcode.cn

JS:   s === [...s].reverse().join("")
来源：http://xnp.nanxuanxn.top

TS:   s === [...s].reverse().join("")
来源：http://fxc.fktsv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bzh.shzxlz.cn

Go:   // 双指针从两端比较
来源：http://kgx.jinghuilouyu.cn

Ruby: s == s.reverse
来源：http://gsa.9152youxi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://oou.fehbvm.com

[N07] 两数之和（返回下标）
来源：http://use.cdnleiting.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jxc.tarul.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pqg.kuanghao11.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://bat.xinyue.icu

TS:   // 手写 Map<string, number>
来源：http://yfw.zhixingplan.top

Java: // 手写 HashMap
来源：http://bon.vqdsnc.cn

Go:   // 手写 map[int]int
来源：http://fof.316326.xyz

Ruby: // 手写 Hash
来源：http://iub.shuidangran.top

C#:   // 手写 Dictionary<int, int>
来源：http://vgp.tarul.cn

[N08] 生成全排列
来源：http://yju.jiagoushi.top

Py:   itertools.permutations(arr)
来源：http://xay.xuanzx.com

PHP:  // 手写递归交换
来源：http://jqq.yuanzhike.top

JS:   // 手写回溯递归
来源：http://jfz.jinqigfzy.top

TS:   // 手写回溯递归
来源：http://jmk.yvedp.cn

Java: // 手写回溯递归
来源：http://soq.guannengcc.top

Go:   // 手写回溯递归
来源：http://wbe.xuanzx.com

Ruby: arr.permutation.to_a
来源：http://ssv.uphjek.com

C#:   // 手写回溯递归
来源：http://ipi.chenlongwang.top

[N09] 栈与队列
来源：http://rqm.gzhubu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://whz.ybcxt.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qgr.hongshengwenyu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wgh.wangdashe.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fhr.nanxuanxn.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ang.xuanzx.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wdv.pengpengdd.cyou

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ric.aibaodan.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zpq.hysaishi.cn

[N10] 链表节点定义
来源：http://pbn.fanxiaobao.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://juu.ydzc1.top

PHP:  class Node { public $v; public $next = null; }
来源：http://lji.pycfn.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://epw.fzhhl.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mub.tanke756.top

Java: class Node { int v; Node next; }
来源：http://gsg.shzxlz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hxr.ivvv.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bhb.ywan-chungtsiang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wuh.pycfn.com

[N11] 二叉树中序遍历
来源：http://aat.zhaomingkeji.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://joc.gaohongyu789.top

PHP:  // 手写递归函数
来源：http://xfe.hysaishi.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://izj.sufxvd.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nvh.shanyushiyangtech.top

Java: // 手写递归
来源：http://hzk.zhengqikj.top

Go:   // 手写递归
来源：http://kcv.sjlbkw.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ost.sysykeji.top

C#:   // 手写递归
来源：http://dwe.zhongyouzk.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bbg.zhiwuduotai.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://psb.cashguo.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ayd.zhiwuduotai.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gbg.zhixingplan.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vqc.yangfankeji.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fpy.jianghu66.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://knm.fanxiaobao.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nzc.sweek.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vzr.shangyingyoupin.top

================================================================================
来源：http://fsh.zhixingplan.top

O. 并发与异步
来源：http://iwm.vehdjk.com

================================================================================
来源：http://opi.yuanzhike.top

[O01] 启动一个线程
来源：http://fkc.fengsongda.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://psy.zhaomingkeji.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kgo.fengsongda.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://msy.shzxlz.cn

TS:   // 同 JS
来源：http://zok.redwolf501.top

Java: new Thread(() -> f()).start()
来源：http://wte.vqdsnc.cn

Go:   go f()
来源：http://ngo.ehwqpu.com

Ruby: Thread.new { f }
来源：http://ray.aibaodan.cn

C#:   Task.Run(() => F());
来源：http://xzz.andypj.xyz

[O02] 使用线程池
来源：http://abd.yanxiufei.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zye.bbcook.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vuz.yonumen.top

JS:   // worker_threads 线程池
来源：http://nuq.chenjidiqi.icu

TS:   // worker_threads 线程池
来源：http://pyw.shanyushiyangkeji.top

Java: Executors.newFixedThreadPool(4)
来源：http://ceu.fanxiaobao.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://won.hcnkem.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://okb.yj20258.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zjd.sjlbkw.cn

[O03] 加锁保护共享数据
来源：http://nsc.fktsv.cn

Py:   with lock: shared += 1
来源：http://ujf.snrcjt.cn

PHP:  // 用 flock() 做文件锁
来源：http://cgp.nanxuanxn.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lgi.316326.xyz

TS:   // 同 JS
来源：http://kio.xuetiantiany.cn

Java: synchronized (this) { shared++; }
来源：http://voz.9152youxi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ezi.svipenyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://uwy.hnxiangtu.top

C#:   lock (gate) { shared++; }
来源：http://wyv.ehwqpu.com

[O04] 定义异步函数并等待
来源：http://lgo.fehbvm.com

Py:   async def f():⏎    await g()
来源：http://trp.wangshuangyany.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yfs.hnxiangtu.top

JS:   async function f() { await g(); }
来源：http://ibc.jinqigufen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://idj.redwolf501.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cxg.fengsongda.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jhu.epnwcf.com

Ruby: # 用 Fiber 或 async gem
来源：http://iar.ehwqpu.com

C#:   async Task F() { await G(); }
来源：http://ota.dashuyun.cn

[O05] 并发执行并等待全部完成
来源：http://tnn.bjfxy.top

Py:   asyncio.gather(*tasks)
来源：http://ztt.bbcook.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tda.chenlongwang.top

JS:   await Promise.all(tasks)
来源：http://pgh.aibaodan.cn

TS:   await Promise.all(tasks)
来源：http://fno.zhiwuduotai.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gau.svipenyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mca.xuanzx.com

Ruby: threads.map(&:join)
来源：http://vwm.ivvv.top

C#:   await Task.WhenAll(t1, t2)
来源：http://otr.epnwcf.com

[O06] 使用进程池
来源：http://pjb.cdnleiting.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qin.bbcook.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rgo.jyoumei.cn

JS:   // child_process / cluster 模块
来源：http://ylo.jinghuilouyu.cn

TS:   // child_process / cluster 模块
来源：http://axd.chenjidiqi.icu

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://udm.haohaochexian.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vfq.zhixingplan.top

Ruby: // fork 块
来源：http://zkq.52xcode.cn

C#:   Parallel.For
来源：http://xjw.hnxiangtu.top

================================================================================
来源：http://yrf.xingfuxueyuan.xyz

P. 常用工具函数
来源：http://zvm.chenjidiqi.icu

================================================================================
来源：http://egj.sjlbkw.cn

[P01] 生成 UUID
来源：http://lxa.iojbl.cn

Py:   str(uuid.uuid4())
来源：http://yut.ivvv.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gqb.fktsv.cn

JS:   crypto.randomUUID()
来源：http://ebh.zhijiandao.cn

TS:   crypto.randomUUID()
来源：http://svs.yueranfly.top

Java: UUID.randomUUID().toString()
来源：http://fsg.cheryme.top

Go:   // 用 github.com/google/uuid
来源：http://ybd.havefunace.top

Ruby: SecureRandom.uuid
来源：http://uwc.bbcook.cn

C#:   Guid.NewGuid().ToString()
来源：http://gjl.wangshuangyany.cn

[P02] MD5 / SHA256 摘要
来源：http://gvr.gzhubu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://red.yueranfly.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ixe.jinghuilouyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jwc.aibaodan.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://aad.shanyushiyangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ccz.shanyushiyangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ntu.gogol.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qno.hfpthk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://sfk.bbcook.cn

[P03] 生成短随机字符串
来源：http://qob.hcnkem.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bzz.316326.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ett.meibo888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rws.yueranfly.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ptf.zhiwuduotai.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bel.fengsongda.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://klk.sweek.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rbe.dashuyun.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pqc.0kj1m.cn

[P04] 求长度
来源：http://vug.andypj.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://stl.guannengcc.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qss.shzxlz.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nls.guannengcc.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sku.zdbjq.cn

Java: list.size();  map.size();  s.length()
来源：http://gzl.ybcxt.top

Go:   len(arr);  len(m)
来源：http://fcs.jqgufenzy.top

Ruby: x.length;  x.size
来源：http://mai.bjfxy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://kkl.cqqwz.cn

[P05] 判断两个对象内容是否相等
来源：http://uhn.svipenyu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://byv.meibo888.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vwo.xinyue.icu

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iqn.tarul.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ekw.birdmap.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mqo.guannengcc.top

Go:   reflect.DeepEqual(a, b)
来源：http://ydx.havefunace.top

Ruby: a == b
来源：http://sgg.zhoulong.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jvl.bjfxy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://npd.yueranfly.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dec.chenlongwang.top

PHP:  if (empty($x)) {}
来源：http://she.shangyingyoupin.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hbx.jinghuilouyu.cn

TS:   if (x == null) {}
来源：http://lyw.snrcjt.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://yzt.sufxvd.cn

Go:   if x == nil {}
来源：http://aoy.gzhubu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xzo.xingfuxueyuan.xyz

C#:   if (x is null) {}
来源：http://gfx.ybcxt.top

[P07] 防抖与节流
来源：http://yuo.shzxlz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uuc.jqgufenzy.top

PHP:  // 手写时间戳比较
来源：http://cfw.xinyue.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xxi.cqqwz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qer.meibo888.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cpl.yonumen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hvy.jqgfzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://afg.zhengqikj.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dfe.xingfuxueyuan.xyz

[P08] 处理浮点精度问题
来源：http://nyx.cheryme.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://guc.shzxlz.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rrh.sysykeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fxg.sxryk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cfc.smart0.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sbj.gaohongyu789.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jul.daria6918.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gow.jyoumei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://loa.chenzaomai.com

================================================================================
来源：http://ekb.jyoumei.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://seq.shanyushiyangtech.top

================================================================================
来源：http://tzg.haohaochexian.top

[Q01] 创建表
来源：http://ojm.yuxming.cn

CREATE TABLE users (
来源：http://gbt.zhongyouzk.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://eit.svipenyu.cn

name VARCHAR(50) NOT NULL,
来源：http://dtj.wangshuangyany.cn

email VARCHAR(100) UNIQUE,
来源：http://rjo.jinqigufen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zks.hnxiangtu.top

);
来源：http://uua.cucudq.cn

[Q02] 创建带外键的表
来源：http://ffj.jianghu66.top

CREATE TABLE orders (
来源：http://wtc.yanxiufei.cn


<!-- 参考信息 -->