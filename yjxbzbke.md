代发 wailian999

[M04] 获取当前工作目录
来源：http://pew.nanxinkj.top

Py:   os.getcwd()
来源：http://ztj.hfpthk.cn

PHP:  getcwd();
来源：http://shp.gotoacloud.top

JS:   process.cwd()
来源：http://ryr.tarul.cn

TS:   process.cwd()
来源：http://vzj.mhx1999.top

Java: Path.of("").toAbsolutePath()
来源：http://utk.wangdashe.top

Go:   os.Getwd()
来源：http://xtr.jinqigfzy.top

Ruby: Dir.pwd
来源：http://kwx.wangdashe.top

C#:   Directory.GetCurrentDirectory()
来源：http://sen.snrcjt.cn

[M05] 设置退出码
来源：http://dtw.cheryme.top

Py:   sys.exit(1)
来源：http://diq.hfpthk.cn

PHP:  exit(1);
来源：http://pup.0kj1m.cn

JS:   process.exit(1)
来源：http://cbj.shangyingyoupin.top

TS:   process.exit(1)
来源：http://zxb.dashuyun.cn

Java: System.exit(1)
来源：http://mka.quarkkingdee.top

Go:   os.Exit(1)
来源：http://bao.jinqigufen.top

Ruby: exit 1
来源：http://uwy.chenjidiqi.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://keo.bbcook.cn

[M06] 向标准错误输出
来源：http://yxn.iojbl.cn

Py:   print("err", file=sys.stderr)
来源：http://dwq.tianlin.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://cgo.dianchejie.cn

JS:   console.error("err")
来源：http://zfl.zhijiandao.cn

TS:   console.error("err")
来源：http://hef.zdqjudy.top

Java: System.err.println("err")
来源：http://pri.yj202588.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kjk.jinghuilouyu.cn

Ruby: warn "err"
来源：http://glg.hnxiangtu.top

C#:   Console.Error.WriteLine("err")
来源：http://szn.ydzc1.top

[M07] 判断是否为主入口
来源：http://ira.cashguo.top

Py:   if __name__ == "__main__":
来源：http://iet.haohaochexian.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wef.jinyuanbaomall.cn

JS:   require.main === module
来源：http://mhe.gogol.net.cn

TS:   require.main === module
来源：http://gtn.jinghuilouyu.cn

Java: public static void main(String[] args)
来源：http://ljy.yanxiufei.cn

Go:   func main()
来源：http://hki.haohaochexian.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uwm.sufxvd.cn

C#:   static void Main(string[] args)
来源：http://eat.yanxiufei.cn

[M08] 获取系统与运行时信息
来源：http://nmy.yj20258.top

Py:   platform.system();  platform.python_version()
来源：http://age.cashguo.top

PHP:  PHP_OS;  phpversion();
来源：http://grd.mhx1999.top

JS:   process.platform;  process.version
来源：http://iyh.nwbrower.top

TS:   process.platform;  process.version
来源：http://uvl.aibaodan.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zws.dashuyun.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yhn.jinghuilouyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ydl.jqgufenzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nsv.shangyingyoupin.top

================================================================================
来源：http://dmk.yj202588.top

N. 数据结构与算法
来源：http://jma.yfazqb.com

================================================================================
来源：http://iuw.ctjpmb.com

[N01] 二分查找（有序数组）
来源：http://ctq.aizwys.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lxw.yonumen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://reg.tanke756.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rsu.gzhubu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dyw.quarkkingdee.top

Java: Arrays.binarySearch(arr, x)
来源：http://iqz.shuidangran.top

Go:   sort.SearchInts(arr, x)
来源：http://evx.xziqi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://prk.dashuyun.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mpl.chenzaomai.com

[N02] 排序（工程实践用内置实现）
来源：http://ape.smart0.xyz

Py:   sorted(arr);  arr.sort()
来源：http://mzb.svipenyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kgy.yuxming.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://aqj.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nzv.zhixingplan.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lui.zhixingplan.top

Go:   slices.Sort(arr)
来源：http://jdc.dianchejie.cn

Ruby: arr.sort
来源：http://tdq.zhongyouzk.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jti.ywan-chungtsiang.top

[N03] 快速排序（分治示例）
来源：http://nll.kuanghao11.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tyx.cashguo.top

PHP:  // 递归实现，或用 usort
来源：http://bbr.daria6918.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aoi.haohaochexian.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ktj.guowangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sah.epnwcf.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gwn.yangfankeji.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iqe.nwbrower.top

C#:   // 手写递归，或 Array.Sort
来源：http://zxb.wangdashe.top

[N04] 斐波那契数列
来源：http://kme.fktsv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://syk.fzhhl.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mkc.shzxlz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://abu.gotoacloud.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tju.jianghu66.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yts.quarkkingdee.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://omz.yj20258888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://abr.sweek.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://squ.hammf.cn

[N05] 最大公约数
来源：http://tyo.kuanghao11.cn

Py:   math.gcd(a, b)
来源：http://xfl.birdmap.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ngc.chenzaomai.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kid.xinyue.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kcy.wangshuangyany.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://esj.cucudq.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hag.kuanghao11.cn

Ruby: a.gcd(b)
来源：http://zqx.iojbl.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fkm.jqgfzy.top

[N06] 判断回文字符串
来源：http://enf.ydzc1.top

Py:   s == s[::-1]
来源：http://wrf.uphjek.com

PHP:  $s === strrev($s);
来源：http://cch.zhixingplan.top

JS:   s === [...s].reverse().join("")
来源：http://rmi.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://kjq.ehwqpu.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qsn.hfpthk.cn

Go:   // 双指针从两端比较
来源：http://byr.0kj1m.cn

Ruby: s == s.reverse
来源：http://vqr.zhengqikj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://pkv.yuxming.cn

[N07] 两数之和（返回下标）
来源：http://bzq.shzxlz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zeb.sxryk.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dmd.0kj1m.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lqa.pycfn.com

TS:   // 手写 Map<string, number>
来源：http://vii.jqgfzy.top

Java: // 手写 HashMap
来源：http://ger.sufxvd.cn

Go:   // 手写 map[int]int
来源：http://gcj.dashuyun.cn

Ruby: // 手写 Hash
来源：http://gjx.ppjwa.cn

C#:   // 手写 Dictionary<int, int>
来源：http://gue.cqqwz.cn

[N08] 生成全排列
来源：http://geu.zhengqikj.top

Py:   itertools.permutations(arr)
来源：http://fyt.feifeiyinyue.top

PHP:  // 手写递归交换
来源：http://tnd.yanxiufei.cn

JS:   // 手写回溯递归
来源：http://usn.ppjwa.cn

TS:   // 手写回溯递归
来源：http://kfz.nwbrower.top

Java: // 手写回溯递归
来源：http://dgi.yongpay.top

Go:   // 手写回溯递归
来源：http://for.xuanzx.com

Ruby: arr.permutation.to_a
来源：http://bfp.zhiwuduotai.top

C#:   // 手写回溯递归
来源：http://avf.shanyushiyangtech.top

[N09] 栈与队列
来源：http://vnp.feifeiyinyue.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tly.zhongyouzk.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jra.zhixingplan.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dwb.nanxuanxn.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://evu.shanyushiyangtech.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xww.guannengcc.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gwe.jqgufenzy.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://afc.yanxiufei.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://klg.havefunace.top

[N10] 链表节点定义
来源：http://kkc.jinqigufen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://zch.chenjidiqi.icu

PHP:  class Node { public $v; public $next = null; }
来源：http://ccy.ivvv.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gvj.gotoacloud.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rnn.zhiwuduotai.top

Java: class Node { int v; Node next; }
来源：http://mty.sxryk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://puu.yj202588.top

Ruby: Node = Struct.new(:v, :next)
来源：http://yzb.jlsjyb.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ome.zdqjudy.top

[N11] 二叉树中序遍历
来源：http://qbi.hysaishi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://avc.gogol.net.cn

PHP:  // 手写递归函数
来源：http://dit.cdnleiting.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://far.ehwqpu.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ghx.bjfxy.top

Java: // 手写递归
来源：http://map.smart0.xyz

Go:   // 手写递归
来源：http://rne.shuidangran.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tsu.pengpengdd.cyou

C#:   // 手写递归
来源：http://xqt.daria6918.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nff.xziqi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jst.jiagoushi.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://epm.redwolf501.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kme.gzhubu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qmr.jinghuilouyu.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wzx.ehwqpu.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gcx.wangdashe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ppc.quarkkingdee.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://few.zhengqikj.top

================================================================================
来源：http://fcb.daxiang520.top

O. 并发与异步
来源：http://bei.smart0.xyz

================================================================================
来源：http://bxp.uphjek.com

[O01] 启动一个线程
来源：http://ppg.shangyingyoupin.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rty.yueranfly.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gfa.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ihi.mhx1999.top

TS:   // 同 JS
来源：http://psa.yvedp.cn

Java: new Thread(() -> f()).start()
来源：http://tgt.fengsongda.top

Go:   go f()
来源：http://rrx.sweek.top

Ruby: Thread.new { f }
来源：http://ona.bjfxy.top

C#:   Task.Run(() => F());
来源：http://lji.vqdsnc.cn

[O02] 使用线程池
来源：http://qzx.nwbrower.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qbz.zhiwuduotai.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bhh.zhijiandao.cn

JS:   // worker_threads 线程池
来源：http://uiw.xuanzx.com

TS:   // worker_threads 线程池
来源：http://rvy.ivvv.top

Java: Executors.newFixedThreadPool(4)
来源：http://kmg.cashguo.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qep.hywenlv.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yqu.hysaishi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://vdh.cheryme.top

[O03] 加锁保护共享数据
来源：http://pvt.yj20258888.top

Py:   with lock: shared += 1
来源：http://zro.xinyue.icu

PHP:  // 用 flock() 做文件锁
来源：http://pvl.gotoacloud.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hdd.pycfn.com

TS:   // 同 JS
来源：http://xvw.jinqigfzy.top

Java: synchronized (this) { shared++; }
来源：http://jmf.xylfe.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rbf.fengsongda.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://gcr.0kj1m.cn

C#:   lock (gate) { shared++; }
来源：http://mym.jyoumei.cn

[O04] 定义异步函数并等待
来源：http://yga.zhengqikj.top

Py:   async def f():⏎    await g()
来源：http://tni.zhongyouzk.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://irm.cheryme.top

JS:   async function f() { await g(); }
来源：http://fxk.chenlongwang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://faj.xziqi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jcr.xuanzx.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mpq.shuidangran.top

Ruby: # 用 Fiber 或 async gem
来源：http://bne.tianlin.xyz

C#:   async Task F() { await G(); }
来源：http://wfm.jinyuanbaomall.cn

[O05] 并发执行并等待全部完成
来源：http://zhz.fehbvm.com

Py:   asyncio.gather(*tasks)
来源：http://dfk.0kj1m.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gxh.ydzc1.top

JS:   await Promise.all(tasks)
来源：http://kok.ydjk.org.cn

TS:   await Promise.all(tasks)
来源：http://dsy.shangyingyoupin.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cxe.ydzc1.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mwe.hesvh.cn

Ruby: threads.map(&:join)
来源：http://dqb.sxryk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rzv.tianlin.xyz

[O06] 使用进程池
来源：http://qda.daxiang520.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gkt.yongpay.top

PHP:  // pcntl_fork 或多进程队列
来源：http://sll.gotoacloud.top

JS:   // child_process / cluster 模块
来源：http://hse.zycfv.cn

TS:   // child_process / cluster 模块
来源：http://vie.yvedp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fqy.dianchejie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gqc.cashguo.top

Ruby: // fork 块
来源：http://gha.tarul.cn

C#:   Parallel.For
来源：http://ruz.shanyushiyangtech.top

================================================================================
来源：http://uue.hesvh.cn

P. 常用工具函数
来源：http://kwe.ivvv.top

================================================================================
来源：http://rim.tian-w.cn

[P01] 生成 UUID
来源：http://ejk.9152youxi.cn

Py:   str(uuid.uuid4())
来源：http://gej.chenzaomai.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mre.tian-w.cn

JS:   crypto.randomUUID()
来源：http://qju.wangshuangyany.cn

TS:   crypto.randomUUID()
来源：http://rvz.yangfankeji.com

Java: UUID.randomUUID().toString()
来源：http://nsr.cqqwz.cn

Go:   // 用 github.com/google/uuid
来源：http://hst.wangdashe.top

Ruby: SecureRandom.uuid
来源：http://wxl.zdqjudy.top

C#:   Guid.NewGuid().ToString()
来源：http://ous.mhx1999.top

[P02] MD5 / SHA256 摘要
来源：http://svv.ctjpmb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ehx.yanxiufei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://yuj.hfpthk.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lfr.bbcook.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://san.yueranfly.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jnb.chenzaomai.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jzo.sjlbkw.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hcn.fengsongda.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bvt.yuxming.cn

[P03] 生成短随机字符串
来源：http://jck.yuxming.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ewi.vehdjk.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://seq.cqqwz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tdc.cheryme.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xlb.0kj1m.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://spe.yj202588.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rum.shanyushiyangtech.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lrj.hnqzz.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qfu.jinghuilouyu.cn

[P04] 求长度
来源：http://pre.nanxuanxn.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tqa.redwolf501.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rvg.ywan-chungtsiang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dsn.xingfuxueyuan.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ezj.jinqigufen.top

Java: list.size();  map.size();  s.length()
来源：http://lfe.kuanghao11.cn

Go:   len(arr);  len(m)
来源：http://eja.tian-w.cn

Ruby: x.length;  x.size
来源：http://mvy.redwolf501.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://pvp.shzxlz.cn

[P05] 判断两个对象内容是否相等
来源：http://ekw.zycfv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yig.yonumen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://szv.zhoulong.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://anu.jinqigfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fxc.tarul.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wbr.gogol.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://duw.zhongyouzk.top

Ruby: a == b
来源：http://eea.jianghu66.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fwj.yj20258888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lxe.meibo888.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vqe.tianlin.xyz

PHP:  if (empty($x)) {}
来源：http://ffz.cqqwz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://odl.zhoulong.xyz

TS:   if (x == null) {}
来源：http://yrn.yvedp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vuw.havefunace.top

Go:   if x == nil {}
来源：http://cfl.hcnkem.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ziw.andypj.xyz

C#:   if (x is null) {}
来源：http://pao.fktsv.cn

[P07] 防抖与节流
来源：http://rrj.zhengqikj.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cnv.shanyushiyangkeji.top

PHP:  // 手写时间戳比较
来源：http://jdw.yanxiufei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qxf.sxryk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wlh.nanxuanxn.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vzd.snrcjt.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pus.chenzaomai.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://nzy.c1oappe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tno.nwbrower.top

[P08] 处理浮点精度问题
来源：http://erd.nwbrower.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rjh.fehbvm.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qoe.hcnkem.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hbj.xylfe.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uxk.ehwqpu.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yct.pengpengdd.cyou

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ohq.bbcook.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kyk.c1oappe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jgd.zhijiandao.cn

================================================================================
来源：http://bry.52xcode.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wug.zhijiandao.cn

================================================================================
来源：http://txn.shangyingyoupin.top

[Q01] 创建表
来源：http://wcs.yvedp.cn

CREATE TABLE users (
来源：http://cuy.nwbrower.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dac.jinghuilouyu.cn

name VARCHAR(50) NOT NULL,
来源：http://uyp.jyoumei.cn

email VARCHAR(100) UNIQUE,
来源：http://bqj.jlsjyb.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ggh.hysaishi.cn

);
来源：http://kkf.9152youxi.cn

[Q02] 创建带外键的表
来源：http://jvy.fehbvm.com

CREATE TABLE orders (
来源：http://uvr.zycfv.cn


<!-- 参考信息 -->