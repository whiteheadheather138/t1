代发 wailian999

TS:   process.cwd()
来源：http://bqq.sufxvd.cn

Java: Path.of("").toAbsolutePath()
来源：http://rbt.mhx1999.top

Go:   os.Getwd()
来源：http://pdq.sjlbkw.cn

Ruby: Dir.pwd
来源：http://nna.kuanghao11.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yvl.fengsongda.top

[M05] 设置退出码
来源：http://opn.kuanghao11.cn

Py:   sys.exit(1)
来源：http://kus.shangyingyoupin.top

PHP:  exit(1);
来源：http://dfg.zhijiandao.cn

JS:   process.exit(1)
来源：http://hde.hesvh.cn

TS:   process.exit(1)
来源：http://psw.redwolf501.top

Java: System.exit(1)
来源：http://uyl.yfazqb.com

Go:   os.Exit(1)
来源：http://hqv.ywan-chungtsiang.top

Ruby: exit 1
来源：http://aou.aibaodan.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xfk.jlsjyb.cn

[M06] 向标准错误输出
来源：http://uur.jianghu66.top

Py:   print("err", file=sys.stderr)
来源：http://ond.sufxvd.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://hmg.hysaishi.cn

JS:   console.error("err")
来源：http://yom.hammf.cn

TS:   console.error("err")
来源：http://oov.xuetiantiany.cn

Java: System.err.println("err")
来源：http://vpm.xuanzx.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nll.aibaodan.cn

Ruby: warn "err"
来源：http://jys.hesvh.cn

C#:   Console.Error.WriteLine("err")
来源：http://bfk.chenzaomai.com

[M07] 判断是否为主入口
来源：http://mfk.yj20258.top

Py:   if __name__ == "__main__":
来源：http://rjj.yangfankeji.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zwt.yvedp.cn

JS:   require.main === module
来源：http://qox.ywan-chungtsiang.top

TS:   require.main === module
来源：http://qey.fzhhl.top

Java: public static void main(String[] args)
来源：http://nyd.yuanzhike.top

Go:   func main()
来源：http://wkn.jinqigufen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sso.xuetiantiany.cn

C#:   static void Main(string[] args)
来源：http://kfv.kuanghao11.cn

[M08] 获取系统与运行时信息
来源：http://jlj.hfpthk.cn

Py:   platform.system();  platform.python_version()
来源：http://pqn.zhixingplan.top

PHP:  PHP_OS;  phpversion();
来源：http://mhd.yfazqb.com

JS:   process.platform;  process.version
来源：http://qhh.zhongyouzk.top

TS:   process.platform;  process.version
来源：http://dnz.cheryme.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ngt.zycfv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mny.hcnkem.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bag.yangfankeji.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://kvz.vqdsnc.cn

================================================================================
来源：http://pon.jianghu66.top

N. 数据结构与算法
来源：http://ljq.jinghuilouyu.cn

================================================================================
来源：http://dgu.ydzc1.top

[N01] 二分查找（有序数组）
来源：http://esn.yuanzhike.top

Py:   bisect.bisect_left(arr, x)
来源：http://jvx.guowangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aiq.fengsongda.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bho.svipenyu.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qoo.tarul.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kzy.zhijiandao.cn

Go:   sort.SearchInts(arr, x)
来源：http://rmu.yueranfly.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ily.wangdashe.top

C#:   Array.BinarySearch(arr, x)
来源：http://fba.wangdashe.top

[N02] 排序（工程实践用内置实现）
来源：http://bxb.shuidangran.top

Py:   sorted(arr);  arr.sort()
来源：http://uwg.hammf.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dfj.sxryk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://uoe.yonumen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://waa.yueranfly.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jul.yj20258888.top

Go:   slices.Sort(arr)
来源：http://lpe.chenlongwang.top

Ruby: arr.sort
来源：http://imp.yongpay.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pxu.zycfv.cn

[N03] 快速排序（分治示例）
来源：http://ztq.wangdashe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jmq.bbcook.cn

PHP:  // 递归实现，或用 usort
来源：http://yhi.ehwqpu.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tih.zycfv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://idy.zhongyouzk.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jtf.quarkkingdee.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bxx.yfazqb.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vgv.ybcxt.top

C#:   // 手写递归，或 Array.Sort
来源：http://ynz.zhoulong.xyz

[N04] 斐波那契数列
来源：http://yop.tanke756.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qpr.gogol.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://llu.hcnkem.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yyf.jinghuilouyu.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://viw.cdnleiting.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gku.c1oappe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jnc.andypj.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://weu.pengpengdd.cyou

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bpt.yongpay.top

[N05] 最大公约数
来源：http://kff.yfazqb.com

Py:   math.gcd(a, b)
来源：http://ckm.vqdsnc.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bsk.chenzaomai.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ynw.ppjwa.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hhf.fzhhl.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hpr.dianchejie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://azv.fehbvm.com

Ruby: a.gcd(b)
来源：http://rkw.sufxvd.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rce.9152youxi.cn

[N06] 判断回文字符串
来源：http://eks.hywenlv.cn

Py:   s == s[::-1]
来源：http://ley.shzxlz.cn

PHP:  $s === strrev($s);
来源：http://qes.yuxming.cn

JS:   s === [...s].reverse().join("")
来源：http://qmi.dianchejie.cn

TS:   s === [...s].reverse().join("")
来源：http://yro.fehbvm.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://egc.ywan-chungtsiang.top

Go:   // 双指针从两端比较
来源：http://bzs.snrcjt.cn

Ruby: s == s.reverse
来源：http://nnx.jyoumei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xts.hysaishi.cn

[N07] 两数之和（返回下标）
来源：http://wre.kuanghao11.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://daa.xziqi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ijj.zhixingplan.top

JS:   // 手写 Map：map.set(v, i)
来源：http://jsu.iojbl.cn

TS:   // 手写 Map<string, number>
来源：http://izt.ydzc1.top

Java: // 手写 HashMap
来源：http://kvp.zdqjudy.top

Go:   // 手写 map[int]int
来源：http://rhh.ivvv.top

Ruby: // 手写 Hash
来源：http://pdg.xylfe.cn

C#:   // 手写 Dictionary<int, int>
来源：http://crt.iojbl.cn

[N08] 生成全排列
来源：http://umh.nanxinkj.top

Py:   itertools.permutations(arr)
来源：http://fns.hammf.cn

PHP:  // 手写递归交换
来源：http://kmt.mhx1999.top

JS:   // 手写回溯递归
来源：http://iuh.zhiwuduotai.top

TS:   // 手写回溯递归
来源：http://zjq.zhoulong.xyz

Java: // 手写回溯递归
来源：http://odi.snrcjt.cn

Go:   // 手写回溯递归
来源：http://evu.yanxiufei.cn

Ruby: arr.permutation.to_a
来源：http://uyc.tanke756.top

C#:   // 手写回溯递归
来源：http://sns.wangdashe.top

[N09] 栈与队列
来源：http://cyq.zhijiandao.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bvx.zdqjudy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ceh.aibaodan.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wwu.hesvh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yrk.ybcxt.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ovd.tarul.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lin.gaohongyu789.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nit.zhaomingkeji.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kik.sysykeji.top

[N10] 链表节点定义
来源：http://fyz.xziqi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://udl.snrcjt.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://awq.chenlongwang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kkx.xinyue.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hhk.jinqigufen.top

Java: class Node { int v; Node next; }
来源：http://nfl.zhijiandao.cn

Go:   type Node struct { V int; Next *Node }
来源：http://pbm.andypj.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://vhx.daxiang520.top

C#:   class Node { public int V; public Node? Next; }
来源：http://irc.gogol.net.cn

[N11] 二叉树中序遍历
来源：http://zsv.gogol.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cjs.xziqi.cn

PHP:  // 手写递归函数
来源：http://ikk.tianlin.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pbs.zycfv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pwk.yuxming.cn

Java: // 手写递归
来源：http://gzb.shzxlz.cn

Go:   // 手写递归
来源：http://yqj.yueranfly.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zin.zhiwuduotai.top

C#:   // 手写递归
来源：http://hkf.cashguo.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vbv.chenlongwang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fsu.0kj1m.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fos.9152youxi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zgr.gzhubu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iob.gogol.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uce.hysaishi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://twc.jiagoushi.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://keg.mhx1999.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mti.xziqi.cn

================================================================================
来源：http://uwr.52xcode.cn

O. 并发与异步
来源：http://ikg.hnqzz.top

================================================================================
来源：http://kir.jianghu66.top

[O01] 启动一个线程
来源：http://xty.xylfe.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gsl.vehdjk.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uwb.daxiang520.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kep.fengsongda.top

TS:   // 同 JS
来源：http://zne.redwolf501.top

Java: new Thread(() -> f()).start()
来源：http://cos.snrcjt.cn

Go:   go f()
来源：http://znh.xingfuxueyuan.xyz

Ruby: Thread.new { f }
来源：http://qrc.0kj1m.cn

C#:   Task.Run(() => F());
来源：http://quh.xylfe.cn

[O02] 使用线程池
来源：http://dwo.aibaodan.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://goq.shanyushiyangtech.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://djm.tarul.cn

JS:   // worker_threads 线程池
来源：http://rln.xziqi.cn

TS:   // worker_threads 线程池
来源：http://pdl.yj20258.top

Java: Executors.newFixedThreadPool(4)
来源：http://tue.zhoulong.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://odx.gzhubu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ewm.vqdsnc.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fpt.zhixingplan.top

[O03] 加锁保护共享数据
来源：http://zzc.jlsjyb.cn

Py:   with lock: shared += 1
来源：http://hsv.tian-w.cn

PHP:  // 用 flock() 做文件锁
来源：http://bxa.zhongyouzk.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gdf.jqgfzy.top

TS:   // 同 JS
来源：http://hnm.hysaishi.cn

Java: synchronized (this) { shared++; }
来源：http://zbc.feifeiyinyue.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://faj.yangfankeji.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://xup.ehwqpu.com

C#:   lock (gate) { shared++; }
来源：http://qwa.andypj.xyz

[O04] 定义异步函数并等待
来源：http://zox.chenlongwang.top

Py:   async def f():⏎    await g()
来源：http://jmy.aizwys.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qce.jianghu66.top

JS:   async function f() { await g(); }
来源：http://zcl.aizwys.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bbo.xingfuxueyuan.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gsx.shzxlz.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pqj.wangshuangyany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wkv.ehwqpu.com

C#:   async Task F() { await G(); }
来源：http://kzc.hammf.cn

[O05] 并发执行并等待全部完成
来源：http://rwh.zycfv.cn

Py:   asyncio.gather(*tasks)
来源：http://iqa.ehwqpu.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mvh.ybcxt.top

JS:   await Promise.all(tasks)
来源：http://eoh.xuetiantiany.cn

TS:   await Promise.all(tasks)
来源：http://xtf.zycfv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://guu.ydzc1.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ynv.svipenyu.cn

Ruby: threads.map(&:join)
来源：http://cbv.shangyingyoupin.top

C#:   await Task.WhenAll(t1, t2)
来源：http://uek.cucudq.cn

[O06] 使用进程池
来源：http://rve.snrcjt.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yyb.ybcxt.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mma.chenzaomai.com

JS:   // child_process / cluster 模块
来源：http://frx.tian-w.cn

TS:   // child_process / cluster 模块
来源：http://spl.feifeiyinyue.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dtt.yvedp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rxk.yanxiufei.cn

Ruby: // fork 块
来源：http://shu.shanyushiyangkeji.top

C#:   Parallel.For
来源：http://edw.chenjidiqi.icu

================================================================================
来源：http://ldj.ydzc1.top

P. 常用工具函数
来源：http://fja.fktsv.cn

================================================================================
来源：http://gij.jianghu66.top

[P01] 生成 UUID
来源：http://gjy.hysaishi.cn

Py:   str(uuid.uuid4())
来源：http://qqb.yangfankeji.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oog.bbcook.cn

JS:   crypto.randomUUID()
来源：http://vnf.jqgufenzy.top

TS:   crypto.randomUUID()
来源：http://rtz.c1oappe.top

Java: UUID.randomUUID().toString()
来源：http://gic.xziqi.cn

Go:   // 用 github.com/google/uuid
来源：http://ozl.shangyingyoupin.top

Ruby: SecureRandom.uuid
来源：http://abq.jqgfzy.top

C#:   Guid.NewGuid().ToString()
来源：http://ykr.c1oappe.top

[P02] MD5 / SHA256 摘要
来源：http://joq.ehwqpu.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ekr.cashguo.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xgw.jqgfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ilh.pycfn.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cep.yuanzhike.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xbl.haohaochexian.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ntt.yfazqb.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nlv.hnxiangtu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pvl.hcnkem.com

[P03] 生成短随机字符串
来源：http://yrs.shzxlz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fox.yuxming.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vcr.pengpengdd.cyou

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uxg.cdnleiting.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wdf.9152youxi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jzj.aibaodan.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yzf.wangshuangyany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://mtt.316326.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yiz.yj20258888.top

[P04] 求长度
来源：http://xuq.yj202588.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://svh.jqgufenzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qxl.feifeiyinyue.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ohf.jqgfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://awv.haohaochexian.top

Java: list.size();  map.size();  s.length()
来源：http://lsp.ywan-chungtsiang.top

Go:   len(arr);  len(m)
来源：http://gmo.wangdashe.top

Ruby: x.length;  x.size
来源：http://nkk.hesvh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://twr.xingfuxueyuan.xyz

[P05] 判断两个对象内容是否相等
来源：http://uhr.gogol.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://zdc.cdnleiting.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rdx.xuetiantiany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pls.shangyingyoupin.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wqz.fanxiaobao.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gbc.jinghuilouyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://maw.hnxiangtu.top

Ruby: a == b
来源：http://azw.hammf.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bvv.chenzaomai.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bdv.shanyushiyangtech.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ddm.tarul.cn

PHP:  if (empty($x)) {}
来源：http://kzd.yuanzhike.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aci.hcnkem.com

TS:   if (x == null) {}
来源：http://ppu.ivvv.top

Java: if (x == null || x.isEmpty()) {}
来源：http://iet.hnqzz.top

Go:   if x == nil {}
来源：http://fdj.fzhhl.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://spf.ivvv.top

C#:   if (x is null) {}
来源：http://ovy.jinghuilouyu.cn

[P07] 防抖与节流
来源：http://yhn.mhx1999.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nsa.fzhhl.top

PHP:  // 手写时间戳比较
来源：http://vns.haohaochexian.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zdw.tarul.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yxu.pengpengdd.cyou

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mye.hywenlv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://icx.zhengqikj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://weo.bjfxy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zry.vqdsnc.cn

[P08] 处理浮点精度问题
来源：http://koq.yuanzhike.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qmd.hammf.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://alg.haohaochexian.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ben.wangshuangyany.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zlf.sjlbkw.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kqg.daxiang520.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pzx.ydjk.org.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xig.mhx1999.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vff.iojbl.cn

================================================================================
来源：http://qrb.gzhubu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://txj.ybcxt.top

================================================================================
来源：http://tej.mhx1999.top

[Q01] 创建表
来源：http://ieu.fktsv.cn

CREATE TABLE users (
来源：http://qar.yueranfly.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fgc.bbcook.cn

name VARCHAR(50) NOT NULL,
来源：http://yih.hesvh.cn

email VARCHAR(100) UNIQUE,
来源：http://muv.iojbl.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kar.shanyushiyangkeji.top

);
来源：http://jje.gogol.net.cn

[Q02] 创建带外键的表
来源：http://had.xylfe.cn

CREATE TABLE orders (
来源：http://ltn.jinyuanbaomall.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nez.jyoumei.cn

user_id INT NOT NULL,
来源：http://wqo.shanyushiyangkeji.top

amount DECIMAL(10, 2),
来源：http://hvb.daria6918.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qml.yj202588.top


<!-- 参考信息 -->