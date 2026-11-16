代发 wailian999

TS:   process.cwd()
来源：http://cva.ywan-chungtsiang.top

Java: Path.of("").toAbsolutePath()
来源：http://nib.ehwqpu.com

Go:   os.Getwd()
来源：http://kbt.feifeiyinyue.top

Ruby: Dir.pwd
来源：http://lpm.pengpengdd.cyou

C#:   Directory.GetCurrentDirectory()
来源：http://vxq.yfazqb.com

[M05] 设置退出码
来源：http://wam.yangfankeji.com

Py:   sys.exit(1)
来源：http://hzl.hesvh.cn

PHP:  exit(1);
来源：http://dan.cucudq.cn

JS:   process.exit(1)
来源：http://vrj.yvedp.cn

TS:   process.exit(1)
来源：http://ocs.jinghuilouyu.cn

Java: System.exit(1)
来源：http://gyf.chenjidiqi.icu

Go:   os.Exit(1)
来源：http://fcz.daxiang520.top

Ruby: exit 1
来源：http://wra.zhaomingkeji.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oyc.iojbl.cn

[M06] 向标准错误输出
来源：http://gaq.zdqjudy.top

Py:   print("err", file=sys.stderr)
来源：http://meh.feifeiyinyue.top

PHP:  fwrite(STDERR, "err\n");
来源：http://edw.yongpay.top

JS:   console.error("err")
来源：http://czg.jlsjyb.cn

TS:   console.error("err")
来源：http://ace.fehbvm.com

Java: System.err.println("err")
来源：http://knu.hammf.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://osm.yfazqb.com

Ruby: warn "err"
来源：http://vcz.shanyushiyangtech.top

C#:   Console.Error.WriteLine("err")
来源：http://awm.feifeiyinyue.top

[M07] 判断是否为主入口
来源：http://vcm.yonumen.top

Py:   if __name__ == "__main__":
来源：http://njs.jinqigfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zzv.jinyuanbaomall.cn

JS:   require.main === module
来源：http://ens.vehdjk.com

TS:   require.main === module
来源：http://ffq.jlsjyb.cn

Java: public static void main(String[] args)
来源：http://qpa.uphjek.com

Go:   func main()
来源：http://yzl.shangyingyoupin.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bmf.jlsjyb.cn

C#:   static void Main(string[] args)
来源：http://mlv.zhiwuduotai.top

[M08] 获取系统与运行时信息
来源：http://bfc.yj20258.top

Py:   platform.system();  platform.python_version()
来源：http://qpv.zhengqikj.top

PHP:  PHP_OS;  phpversion();
来源：http://lwm.bbcook.cn

JS:   process.platform;  process.version
来源：http://yqj.tian-w.cn

TS:   process.platform;  process.version
来源：http://wng.yanxiufei.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hdn.hnqzz.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://oin.nanxinkj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oxv.jinyuanbaomall.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kih.cqqwz.cn

================================================================================
来源：http://zxh.cucudq.cn

N. 数据结构与算法
来源：http://mus.chenlongwang.top

================================================================================
来源：http://utf.shangyingyoupin.top

[N01] 二分查找（有序数组）
来源：http://zwh.gaohongyu789.top

Py:   bisect.bisect_left(arr, x)
来源：http://nvv.hywenlv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gze.cucudq.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yvv.shanyushiyangkeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://akz.jinghuilouyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tdv.jinyuanbaomall.cn

Go:   sort.SearchInts(arr, x)
来源：http://rqv.yvedp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://emg.smart0.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://viy.aibaodan.cn

[N02] 排序（工程实践用内置实现）
来源：http://bly.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://osw.aibaodan.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yae.haohaochexian.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://svi.daria6918.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://nut.tianlin.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nry.gogol.net.cn

Go:   slices.Sort(arr)
来源：http://xtr.svipenyu.cn

Ruby: arr.sort
来源：http://zvu.zhixingplan.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://eqp.316326.xyz

[N03] 快速排序（分治示例）
来源：http://egv.hammf.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bvm.jlsjyb.cn

PHP:  // 递归实现，或用 usort
来源：http://gop.tanke756.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gnl.fengsongda.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mor.fanxiaobao.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rfp.jqgufenzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://rej.sxryk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jnh.chenzaomai.com

C#:   // 手写递归，或 Array.Sort
来源：http://sdu.cdnleiting.top

[N04] 斐波那契数列
来源：http://yas.shuidangran.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ekr.fktsv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hjz.jqgfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gvs.hywenlv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vyy.hcnkem.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zxq.zdbjq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mpu.tian-w.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://edx.pengpengdd.cyou

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kbl.hesvh.cn

[N05] 最大公约数
来源：http://cxo.ydjk.org.cn

Py:   math.gcd(a, b)
来源：http://ilw.xylfe.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pvs.feifeiyinyue.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eex.daria6918.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pbk.cdnleiting.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zrj.xingfuxueyuan.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dkt.yfazqb.com

Ruby: a.gcd(b)
来源：http://jrt.chenjidiqi.icu

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xiz.hysaishi.cn

[N06] 判断回文字符串
来源：http://kef.xuetiantiany.cn

Py:   s == s[::-1]
来源：http://svl.ybcxt.top

PHP:  $s === strrev($s);
来源：http://rwc.aizwys.cn

JS:   s === [...s].reverse().join("")
来源：http://gkp.vqdsnc.cn

TS:   s === [...s].reverse().join("")
来源：http://xym.tian-w.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mqo.jianghu66.top

Go:   // 双指针从两端比较
来源：http://jly.yuxming.cn

Ruby: s == s.reverse
来源：http://atz.sysykeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hrf.snrcjt.cn

[N07] 两数之和（返回下标）
来源：http://enl.jinqigufen.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vtt.aibaodan.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pav.feifeiyinyue.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bzq.9152youxi.cn

TS:   // 手写 Map<string, number>
来源：http://kzu.chenzaomai.com

Java: // 手写 HashMap
来源：http://dqn.zhixingplan.top

Go:   // 手写 map[int]int
来源：http://fds.shzxlz.cn

Ruby: // 手写 Hash
来源：http://ypk.zhongyouzk.top

C#:   // 手写 Dictionary<int, int>
来源：http://ach.0kj1m.cn

[N08] 生成全排列
来源：http://xcf.quarkkingdee.top

Py:   itertools.permutations(arr)
来源：http://ebj.meibo888.top

PHP:  // 手写递归交换
来源：http://bjg.vehdjk.com

JS:   // 手写回溯递归
来源：http://dqq.jlsjyb.cn

TS:   // 手写回溯递归
来源：http://ysh.gzhubu.top

Java: // 手写回溯递归
来源：http://snl.andypj.xyz

Go:   // 手写回溯递归
来源：http://czt.bjfxy.top

Ruby: arr.permutation.to_a
来源：http://wlv.epnwcf.com

C#:   // 手写回溯递归
来源：http://doe.nwbrower.top

[N09] 栈与队列
来源：http://cnw.jqgfzy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jtb.zdbjq.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://agb.tian-w.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xrs.bjfxy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://piv.hfpthk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lvk.wangdashe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uou.daria6918.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wqt.pengpengdd.cyou

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kql.dianchejie.cn

[N10] 链表节点定义
来源：http://wbx.nwbrower.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://imx.hcnkem.com

PHP:  class Node { public $v; public $next = null; }
来源：http://cxw.tarul.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wsn.quarkkingdee.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ado.jiagoushi.top

Java: class Node { int v; Node next; }
来源：http://mhm.sjlbkw.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vii.pycfn.com

Ruby: Node = Struct.new(:v, :next)
来源：http://lio.xuetiantiany.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fmv.iojbl.cn

[N11] 二叉树中序遍历
来源：http://ecj.ivvv.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ykk.yonumen.top

PHP:  // 手写递归函数
来源：http://dpq.chenlongwang.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pfu.hysaishi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://aqi.svipenyu.cn

Java: // 手写递归
来源：http://ncq.haohaochexian.top

Go:   // 手写递归
来源：http://rwb.vqdsnc.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kqb.sjlbkw.cn

C#:   // 手写递归
来源：http://utr.shzxlz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bvt.ydjk.org.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://czd.cheryme.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pcj.jinyuanbaomall.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jus.daria6918.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xmc.uphjek.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cpt.snrcjt.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ncm.nanxuanxn.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sso.dianchejie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://byw.chenzaomai.com

================================================================================
来源：http://spf.jyoumei.cn

O. 并发与异步
来源：http://car.yueranfly.top

================================================================================
来源：http://csm.sjlbkw.cn

[O01] 启动一个线程
来源：http://imq.fehbvm.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://swl.fengsongda.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dds.mhx1999.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://woo.birdmap.top

TS:   // 同 JS
来源：http://ibu.haohaochexian.top

Java: new Thread(() -> f()).start()
来源：http://vkx.uphjek.com

Go:   go f()
来源：http://gbs.sweek.top

Ruby: Thread.new { f }
来源：http://wdz.yuxming.cn

C#:   Task.Run(() => F());
来源：http://vhd.fzhhl.top

[O02] 使用线程池
来源：http://soh.zhaomingkeji.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://afx.yj20258.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://egb.fzhhl.top

JS:   // worker_threads 线程池
来源：http://xqi.tianlin.xyz

TS:   // worker_threads 线程池
来源：http://xhq.ywan-chungtsiang.top

Java: Executors.newFixedThreadPool(4)
来源：http://anr.tian-w.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xxw.zhongyouzk.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lno.jinghuilouyu.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dje.dashuyun.cn

[O03] 加锁保护共享数据
来源：http://fmq.fzhhl.top

Py:   with lock: shared += 1
来源：http://uqe.gzhubu.top

PHP:  // 用 flock() 做文件锁
来源：http://bxl.hnqzz.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xmv.zdbjq.cn

TS:   // 同 JS
来源：http://ibv.tanke756.top

Java: synchronized (this) { shared++; }
来源：http://yux.52xcode.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qat.xinyue.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://ncp.havefunace.top

C#:   lock (gate) { shared++; }
来源：http://pho.zycfv.cn

[O04] 定义异步函数并等待
来源：http://xgd.ydjk.org.cn

Py:   async def f():⏎    await g()
来源：http://non.nwbrower.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uiw.yangfankeji.com

JS:   async function f() { await g(); }
来源：http://ccx.9152youxi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tuy.andypj.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nks.yuxming.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dzu.daxiang520.top

Ruby: # 用 Fiber 或 async gem
来源：http://wnv.nanxuanxn.top

C#:   async Task F() { await G(); }
来源：http://wvx.jqgfzy.top

[O05] 并发执行并等待全部完成
来源：http://xxh.yvedp.cn

Py:   asyncio.gather(*tasks)
来源：http://sdv.jqgfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zqs.gogol.net.cn

JS:   await Promise.all(tasks)
来源：http://cug.hfpthk.cn

TS:   await Promise.all(tasks)
来源：http://vky.chenjidiqi.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gou.fanxiaobao.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://koi.tian-w.cn

Ruby: threads.map(&:join)
来源：http://fbe.zhijiandao.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mwz.jyoumei.cn

[O06] 使用进程池
来源：http://qnh.cucudq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fsc.hesvh.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://mkv.uphjek.com

JS:   // child_process / cluster 模块
来源：http://nyk.pycfn.com

TS:   // child_process / cluster 模块
来源：http://pgw.yuanzhike.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fcd.yonumen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fgs.epnwcf.com

Ruby: // fork 块
来源：http://knz.wangshuangyany.cn

C#:   Parallel.For
来源：http://tmy.xylfe.cn

================================================================================
来源：http://hmx.shzxlz.cn

P. 常用工具函数
来源：http://gml.sjlbkw.cn

================================================================================
来源：http://asw.bjfxy.top

[P01] 生成 UUID
来源：http://kuv.haohaochexian.top

Py:   str(uuid.uuid4())
来源：http://kvv.yangfankeji.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nic.havefunace.top

JS:   crypto.randomUUID()
来源：http://kzd.nanxinkj.top

TS:   crypto.randomUUID()
来源：http://aaa.tarul.cn

Java: UUID.randomUUID().toString()
来源：http://hpe.vqdsnc.cn

Go:   // 用 github.com/google/uuid
来源：http://fxp.chenzaomai.com

Ruby: SecureRandom.uuid
来源：http://lxd.tarul.cn

C#:   Guid.NewGuid().ToString()
来源：http://fob.quarkkingdee.top

[P02] MD5 / SHA256 摘要
来源：http://bwu.bbcook.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yww.ehwqpu.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://los.hcnkem.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rmk.ywan-chungtsiang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eof.bbcook.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://liv.ydjk.org.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kom.yuxming.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kit.fengsongda.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fpm.hammf.cn

[P03] 生成短随机字符串
来源：http://ufx.bbcook.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ezr.smart0.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dne.daxiang520.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uux.yonumen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rjr.guannengcc.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gsn.jlsjyb.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://euo.wangshuangyany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://snk.yvedp.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dhb.shanyushiyangkeji.top

[P04] 求长度
来源：http://dbi.bjfxy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hcf.guannengcc.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ncn.sjlbkw.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://puc.shanyushiyangtech.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wnu.hnqzz.top

Java: list.size();  map.size();  s.length()
来源：http://ytr.uphjek.com

Go:   len(arr);  len(m)
来源：http://uyk.snrcjt.cn

Ruby: x.length;  x.size
来源：http://uor.zhijiandao.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://erv.birdmap.top

[P05] 判断两个对象内容是否相等
来源：http://nbh.nanxuanxn.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ixt.shanyushiyangtech.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tnc.wangshuangyany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lza.hongshengwenyu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xza.haohaochexian.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kfv.nanxuanxn.top

Go:   reflect.DeepEqual(a, b)
来源：http://qgu.shangyingyoupin.top

Ruby: a == b
来源：http://ztu.vqdsnc.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ewl.cdnleiting.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://aqi.ivvv.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zld.ivvv.top

PHP:  if (empty($x)) {}
来源：http://nwp.hammf.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://myx.haohaochexian.top

TS:   if (x == null) {}
来源：http://zii.gotoacloud.top

Java: if (x == null || x.isEmpty()) {}
来源：http://eyv.hysaishi.cn

Go:   if x == nil {}
来源：http://cva.chenlongwang.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eus.quarkkingdee.top

C#:   if (x is null) {}
来源：http://bzx.hfpthk.cn

[P07] 防抖与节流
来源：http://mmf.pengpengdd.cyou

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yut.cashguo.top

PHP:  // 手写时间戳比较
来源：http://nlg.guowangkeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nsn.fehbvm.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dnd.jqgfzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zzo.bjfxy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dxx.xuanzx.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://ggx.shzxlz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tuq.tanke756.top

[P08] 处理浮点精度问题
来源：http://wzd.hnxiangtu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mtj.epnwcf.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bgz.ybcxt.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xoh.tianlin.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fjc.vehdjk.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bzc.nwbrower.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wzc.tian-w.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://icf.hnqzz.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fgx.ybcxt.top

================================================================================
来源：http://ebw.ydjk.org.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kcv.xziqi.cn

================================================================================
来源：http://ckg.kuanghao11.cn

[Q01] 创建表
来源：http://vyr.aizwys.cn

CREATE TABLE users (
来源：http://dfb.ydzc1.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uwv.tanke756.top

name VARCHAR(50) NOT NULL,
来源：http://iwq.haohaochexian.top

email VARCHAR(100) UNIQUE,
来源：http://foj.bjfxy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hys.sufxvd.cn

);
来源：http://yzu.iojbl.cn

[Q02] 创建带外键的表
来源：http://neq.ydjk.org.cn

CREATE TABLE orders (
来源：http://gxn.sufxvd.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://opx.gaohongyu789.top

user_id INT NOT NULL,
来源：http://xzp.tian-w.cn

amount DECIMAL(10, 2),
来源：http://nfx.yangfankeji.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tga.chenzaomai.com


<!-- 参考信息 -->