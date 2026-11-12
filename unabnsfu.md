代发 wailian999

[M04] 获取当前工作目录
来源：http://qtg.hongshengwenyu.top

Py:   os.getcwd()
来源：http://pog.yonumen.top

PHP:  getcwd();
来源：http://riy.tanke756.top

JS:   process.cwd()
来源：http://cvz.epnwcf.com

TS:   process.cwd()
来源：http://uta.meibo888.top

Java: Path.of("").toAbsolutePath()
来源：http://njn.yanxiufei.cn

Go:   os.Getwd()
来源：http://gmc.316326.xyz

Ruby: Dir.pwd
来源：http://acb.hywenlv.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xbk.xinyue.icu

[M05] 设置退出码
来源：http://qea.tarul.cn

Py:   sys.exit(1)
来源：http://ukh.tanke756.top

PHP:  exit(1);
来源：http://gmh.jinqigfzy.top

JS:   process.exit(1)
来源：http://wjy.zdbjq.cn

TS:   process.exit(1)
来源：http://inj.wangdashe.top

Java: System.exit(1)
来源：http://kly.cqqwz.cn

Go:   os.Exit(1)
来源：http://sfx.chenzaomai.com

Ruby: exit 1
来源：http://bix.yvedp.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dfx.aibaodan.cn

[M06] 向标准错误输出
来源：http://bjr.cashguo.top

Py:   print("err", file=sys.stderr)
来源：http://lqa.ehwqpu.com

PHP:  fwrite(STDERR, "err\n");
来源：http://zgq.chenlongwang.top

JS:   console.error("err")
来源：http://rlv.ybcxt.top

TS:   console.error("err")
来源：http://wfa.nanxinkj.top

Java: System.err.println("err")
来源：http://gey.fzhhl.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jhu.nanxuanxn.top

Ruby: warn "err"
来源：http://sll.fzhhl.top

C#:   Console.Error.WriteLine("err")
来源：http://ajm.nanxinkj.top

[M07] 判断是否为主入口
来源：http://vsb.chenlongwang.top

Py:   if __name__ == "__main__":
来源：http://hzk.shangyingyoupin.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://muv.guowangkeji.top

JS:   require.main === module
来源：http://atq.vqdsnc.cn

TS:   require.main === module
来源：http://huv.andypj.xyz

Java: public static void main(String[] args)
来源：http://evj.guannengcc.top

Go:   func main()
来源：http://zob.cdnleiting.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dtj.jianghu66.top

C#:   static void Main(string[] args)
来源：http://kyx.tarul.cn

[M08] 获取系统与运行时信息
来源：http://hfp.wangshuangyany.cn

Py:   platform.system();  platform.python_version()
来源：http://tsh.ydjk.org.cn

PHP:  PHP_OS;  phpversion();
来源：http://nur.hfpthk.cn

JS:   process.platform;  process.version
来源：http://gnz.jinqigufen.top

TS:   process.platform;  process.version
来源：http://epe.mhx1999.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xlh.pengpengdd.cyou

Go:   runtime.GOOS;  runtime.Version()
来源：http://whh.uphjek.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vzh.hcnkem.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://nvw.hnqzz.top

================================================================================
来源：http://bew.xingfuxueyuan.xyz

N. 数据结构与算法
来源：http://rbd.shzxlz.cn

================================================================================
来源：http://efi.tian-w.cn

[N01] 二分查找（有序数组）
来源：http://eqr.yueranfly.top

Py:   bisect.bisect_left(arr, x)
来源：http://res.havefunace.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://moe.jinqigufen.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fqz.smart0.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://srx.aizwys.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fhq.nanxinkj.top

Go:   sort.SearchInts(arr, x)
来源：http://cuc.hcnkem.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://jrz.aibaodan.cn

C#:   Array.BinarySearch(arr, x)
来源：http://avi.epnwcf.com

[N02] 排序（工程实践用内置实现）
来源：http://pim.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://oux.tarul.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://eol.9152youxi.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qma.hnxiangtu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ban.iojbl.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://twu.jinqigufen.top

Go:   slices.Sort(arr)
来源：http://xdc.yueranfly.top

Ruby: arr.sort
来源：http://znj.yanxiufei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://pqi.shangyingyoupin.top

[N03] 快速排序（分治示例）
来源：http://jkx.hammf.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ghw.fanxiaobao.xyz

PHP:  // 递归实现，或用 usort
来源：http://tzr.hnxiangtu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://usf.fzhhl.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ffd.bjfxy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gxe.nanxinkj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kep.c1oappe.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dyl.bjfxy.top

C#:   // 手写递归，或 Array.Sort
来源：http://kft.nanxuanxn.top

[N04] 斐波那契数列
来源：http://rkp.sxryk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://llt.hfpthk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rrn.yongpay.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ahv.pycfn.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://axj.chenlongwang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gez.c1oappe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zal.hywenlv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ksz.yfazqb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oqj.aizwys.cn

[N05] 最大公约数
来源：http://vmg.fktsv.cn

Py:   math.gcd(a, b)
来源：http://mbe.sufxvd.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zpv.hcnkem.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://skg.bjfxy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://otx.hywenlv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://anf.shanyushiyangtech.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ugn.xuanzx.com

Ruby: a.gcd(b)
来源：http://vjj.havefunace.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vjr.zhaomingkeji.xyz

[N06] 判断回文字符串
来源：http://rqz.jinghuilouyu.cn

Py:   s == s[::-1]
来源：http://hcf.xziqi.cn

PHP:  $s === strrev($s);
来源：http://smf.ivvv.top

JS:   s === [...s].reverse().join("")
来源：http://qoj.vehdjk.com

TS:   s === [...s].reverse().join("")
来源：http://ket.fehbvm.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cnv.smart0.xyz

Go:   // 双指针从两端比较
来源：http://vyo.hfpthk.cn

Ruby: s == s.reverse
来源：http://jir.birdmap.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://obu.fengsongda.top

[N07] 两数之和（返回下标）
来源：http://mhk.cdnleiting.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tqd.gzhubu.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://psq.snrcjt.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://scm.xingfuxueyuan.xyz

TS:   // 手写 Map<string, number>
来源：http://pfe.yj20258888.top

Java: // 手写 HashMap
来源：http://bys.c1oappe.top

Go:   // 手写 map[int]int
来源：http://aau.316326.xyz

Ruby: // 手写 Hash
来源：http://eyt.wangshuangyany.cn

C#:   // 手写 Dictionary<int, int>
来源：http://azv.c1oappe.top

[N08] 生成全排列
来源：http://ysw.zhiwuduotai.top

Py:   itertools.permutations(arr)
来源：http://nwr.snrcjt.cn

PHP:  // 手写递归交换
来源：http://vsu.zhiwuduotai.top

JS:   // 手写回溯递归
来源：http://eml.quarkkingdee.top

TS:   // 手写回溯递归
来源：http://fiu.quarkkingdee.top

Java: // 手写回溯递归
来源：http://ibm.ydjk.org.cn

Go:   // 手写回溯递归
来源：http://sei.fktsv.cn

Ruby: arr.permutation.to_a
来源：http://trp.pycfn.com

C#:   // 手写回溯递归
来源：http://zwo.daria6918.cn

[N09] 栈与队列
来源：http://zrm.xylfe.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hpu.birdmap.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zan.zdbjq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ahm.ppjwa.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://suf.hammf.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bqm.xylfe.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yyi.haohaochexian.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lxs.yongpay.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wqg.svipenyu.cn

[N10] 链表节点定义
来源：http://ver.dashuyun.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://urn.fanxiaobao.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://ccq.316326.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://brl.bbcook.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pjw.quarkkingdee.top

Java: class Node { int v; Node next; }
来源：http://mte.hnxiangtu.top

Go:   type Node struct { V int; Next *Node }
来源：http://jtl.xylfe.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://vit.daxiang520.top

C#:   class Node { public int V; public Node? Next; }
来源：http://vnu.pengpengdd.cyou

[N11] 二叉树中序遍历
来源：http://jys.chenlongwang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://joj.ivvv.top

PHP:  // 手写递归函数
来源：http://zeb.52xcode.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ibo.fktsv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lte.xziqi.cn

Java: // 手写递归
来源：http://ckj.sweek.top

Go:   // 手写递归
来源：http://qvy.bjfxy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://job.sweek.top

C#:   // 手写递归
来源：http://mab.shangyingyoupin.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jjj.shzxlz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kjk.zhijiandao.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bil.zhoulong.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lrn.jinyuanbaomall.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uvh.dashuyun.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gmw.zhiwuduotai.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://axo.0kj1m.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ysi.sweek.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kum.hnqzz.top

================================================================================
来源：http://pxd.yuxming.cn

O. 并发与异步
来源：http://vpc.fehbvm.com

================================================================================
来源：http://kgy.hywenlv.cn

[O01] 启动一个线程
来源：http://vfw.wangshuangyany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oil.jinqigufen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jbj.gaohongyu789.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kel.zhongyouzk.top

TS:   // 同 JS
来源：http://rwj.vehdjk.com

Java: new Thread(() -> f()).start()
来源：http://rzd.hnqzz.top

Go:   go f()
来源：http://dzo.gzhubu.top

Ruby: Thread.new { f }
来源：http://ptl.dianchejie.cn

C#:   Task.Run(() => F());
来源：http://isd.hcnkem.com

[O02] 使用线程池
来源：http://fun.guannengcc.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nqy.c1oappe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iri.yj202588.top

JS:   // worker_threads 线程池
来源：http://akz.pycfn.com

TS:   // worker_threads 线程池
来源：http://kma.redwolf501.top

Java: Executors.newFixedThreadPool(4)
来源：http://rvy.fzhhl.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ftt.ppjwa.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://who.fanxiaobao.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ffr.yj20258888.top

[O03] 加锁保护共享数据
来源：http://shh.epnwcf.com

Py:   with lock: shared += 1
来源：http://dcm.yuxming.cn

PHP:  // 用 flock() 做文件锁
来源：http://xhu.shuidangran.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ewb.ctjpmb.com

TS:   // 同 JS
来源：http://dbj.pycfn.com

Java: synchronized (this) { shared++; }
来源：http://ctj.dianchejie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jva.zhixingplan.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://uix.ivvv.top

C#:   lock (gate) { shared++; }
来源：http://oxz.chenlongwang.top

[O04] 定义异步函数并等待
来源：http://cja.zhongyouzk.top

Py:   async def f():⏎    await g()
来源：http://jmd.nwbrower.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uph.dashuyun.cn

JS:   async function f() { await g(); }
来源：http://uqr.guannengcc.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://iao.c1oappe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iqq.ivvv.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tij.9152youxi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://yhg.jinghuilouyu.cn

C#:   async Task F() { await G(); }
来源：http://duk.pengpengdd.cyou

[O05] 并发执行并等待全部完成
来源：http://wym.snrcjt.cn

Py:   asyncio.gather(*tasks)
来源：http://tud.epnwcf.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blc.jinqigufen.top

JS:   await Promise.all(tasks)
来源：http://gve.gaohongyu789.top

TS:   await Promise.all(tasks)
来源：http://vuy.snrcjt.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://naj.iojbl.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://stw.xinyue.icu

Ruby: threads.map(&:join)
来源：http://pfc.0kj1m.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://esd.ehwqpu.com

[O06] 使用进程池
来源：http://lng.ppjwa.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wvy.yj20258888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ddn.zhijiandao.cn

JS:   // child_process / cluster 模块
来源：http://kjy.nanxinkj.top

TS:   // child_process / cluster 模块
来源：http://tqp.yuxming.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dhl.xuanzx.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rpr.nanxuanxn.top

Ruby: // fork 块
来源：http://wfu.gotoacloud.top

C#:   Parallel.For
来源：http://iyl.zhiwuduotai.top

================================================================================
来源：http://nyn.316326.xyz

P. 常用工具函数
来源：http://icg.ydjk.org.cn

================================================================================
来源：http://vew.dianchejie.cn

[P01] 生成 UUID
来源：http://tdb.yvedp.cn

Py:   str(uuid.uuid4())
来源：http://mqz.tarul.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vpx.yuxming.cn

JS:   crypto.randomUUID()
来源：http://aab.kuanghao11.cn

TS:   crypto.randomUUID()
来源：http://xeo.vqdsnc.cn

Java: UUID.randomUUID().toString()
来源：http://spm.hcnkem.com

Go:   // 用 github.com/google/uuid
来源：http://yyo.0kj1m.cn

Ruby: SecureRandom.uuid
来源：http://aze.yj20258.top

C#:   Guid.NewGuid().ToString()
来源：http://bja.daria6918.cn

[P02] MD5 / SHA256 摘要
来源：http://fkx.epnwcf.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bqq.gogol.net.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bfz.xylfe.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ajh.gzhubu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bqo.cheryme.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cfi.tarul.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tqi.daxiang520.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://svy.sweek.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rir.ppjwa.cn

[P03] 生成短随机字符串
来源：http://xdf.sysykeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mkh.ydzc1.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gdt.nwbrower.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xxp.yfazqb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wyz.nanxuanxn.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kod.0kj1m.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dox.uphjek.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://dtv.daria6918.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hyt.iojbl.cn

[P04] 求长度
来源：http://apw.yj202588.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ddo.nwbrower.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://efn.jinqigufen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://evh.sweek.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qzz.xziqi.cn

Java: list.size();  map.size();  s.length()
来源：http://jax.jinqigfzy.top

Go:   len(arr);  len(m)
来源：http://daz.jinyuanbaomall.cn

Ruby: x.length;  x.size
来源：http://rap.ywan-chungtsiang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://des.sxryk.cn

[P05] 判断两个对象内容是否相等
来源：http://scl.bbcook.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://rrz.birdmap.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://udk.hfpthk.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kwj.aizwys.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nxa.zhiwuduotai.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zqy.hammf.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bhy.jiagoushi.top

Ruby: a == b
来源：http://nlt.zhongyouzk.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dyw.yvedp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ggl.gotoacloud.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ury.nanxuanxn.top

PHP:  if (empty($x)) {}
来源：http://uxa.zhaomingkeji.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yql.9152youxi.cn

TS:   if (x == null) {}
来源：http://att.jlsjyb.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://neq.zhixingplan.top

Go:   if x == nil {}
来源：http://qju.shangyingyoupin.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mht.yj202588.top

C#:   if (x is null) {}
来源：http://cei.yj20258.top

[P07] 防抖与节流
来源：http://gsk.chenzaomai.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://czj.zhaomingkeji.xyz

PHP:  // 手写时间戳比较
来源：http://wgv.0kj1m.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://elp.yangfankeji.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nxm.vqdsnc.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tgw.cheryme.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hjb.shangyingyoupin.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://adn.gotoacloud.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wgy.guowangkeji.top

[P08] 处理浮点精度问题
来源：http://aox.zhijiandao.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://clv.gaohongyu789.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kkp.jiagoushi.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iek.daria6918.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gjx.svipenyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fdb.hysaishi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pok.yueranfly.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qng.andypj.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cyo.cqqwz.cn

================================================================================
来源：http://jay.feifeiyinyue.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kwi.9152youxi.cn

================================================================================
来源：http://mvk.yueranfly.top

[Q01] 创建表
来源：http://cla.yongpay.top

CREATE TABLE users (
来源：http://van.nwbrower.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zji.fengsongda.top

name VARCHAR(50) NOT NULL,
来源：http://qmw.gotoacloud.top

email VARCHAR(100) UNIQUE,
来源：http://lat.redwolf501.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fad.gotoacloud.top

);
来源：http://qmf.sufxvd.cn

[Q02] 创建带外键的表
来源：http://dpg.hcnkem.com

CREATE TABLE orders (
来源：http://oli.hysaishi.cn


<!-- 参考信息 -->