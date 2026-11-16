代发 wailian999

TS:   process.cwd()
来源：http://dol.jlsjyb.cn

Java: Path.of("").toAbsolutePath()
来源：http://wxn.epnwcf.com

Go:   os.Getwd()
来源：http://luc.cucudq.cn

Ruby: Dir.pwd
来源：http://kdh.havefunace.top

C#:   Directory.GetCurrentDirectory()
来源：http://bjb.smart0.xyz

[M05] 设置退出码
来源：http://afw.yvedp.cn

Py:   sys.exit(1)
来源：http://fjh.ydzc1.top

PHP:  exit(1);
来源：http://wyn.meibo888.top

JS:   process.exit(1)
来源：http://oge.zhiwuduotai.top

TS:   process.exit(1)
来源：http://otz.hcnkem.com

Java: System.exit(1)
来源：http://bzm.hfpthk.cn

Go:   os.Exit(1)
来源：http://hkm.cheryme.top

Ruby: exit 1
来源：http://cot.ivvv.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://myd.9152youxi.cn

[M06] 向标准错误输出
来源：http://ndl.jlsjyb.cn

Py:   print("err", file=sys.stderr)
来源：http://scs.ydjk.org.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cpf.ybcxt.top

JS:   console.error("err")
来源：http://eef.ppjwa.cn

TS:   console.error("err")
来源：http://gqe.jinqigufen.top

Java: System.err.println("err")
来源：http://fpd.tanke756.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ela.zhoulong.xyz

Ruby: warn "err"
来源：http://dar.aibaodan.cn

C#:   Console.Error.WriteLine("err")
来源：http://oqt.yueranfly.top

[M07] 判断是否为主入口
来源：http://yec.hongshengwenyu.top

Py:   if __name__ == "__main__":
来源：http://nia.cdnleiting.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zug.jinyuanbaomall.cn

JS:   require.main === module
来源：http://cde.sysykeji.top

TS:   require.main === module
来源：http://ntj.epnwcf.com

Java: public static void main(String[] args)
来源：http://vzk.haohaochexian.top

Go:   func main()
来源：http://jbq.xylfe.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wvf.jinyuanbaomall.cn

C#:   static void Main(string[] args)
来源：http://kop.gotoacloud.top

[M08] 获取系统与运行时信息
来源：http://rrr.iojbl.cn

Py:   platform.system();  platform.python_version()
来源：http://iok.pycfn.com

PHP:  PHP_OS;  phpversion();
来源：http://bvz.sweek.top

JS:   process.platform;  process.version
来源：http://ssy.dianchejie.cn

TS:   process.platform;  process.version
来源：http://odh.andypj.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pqj.fktsv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://bsx.ctjpmb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oin.redwolf501.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://yay.yongpay.top

================================================================================
来源：http://qnf.sufxvd.cn

N. 数据结构与算法
来源：http://arl.ppjwa.cn

================================================================================
来源：http://zhm.svipenyu.cn

[N01] 二分查找（有序数组）
来源：http://bml.c1oappe.top

Py:   bisect.bisect_left(arr, x)
来源：http://sfr.pengpengdd.cyou

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fdy.cashguo.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kgv.yonumen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hvb.hcnkem.com

Java: Arrays.binarySearch(arr, x)
来源：http://grw.hfpthk.cn

Go:   sort.SearchInts(arr, x)
来源：http://wgp.jiagoushi.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lni.9152youxi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ldu.vqdsnc.cn

[N02] 排序（工程实践用内置实现）
来源：http://fks.cucudq.cn

Py:   sorted(arr);  arr.sort()
来源：http://tms.nanxinkj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://jcx.hfpthk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://axr.shangyingyoupin.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qlp.shanyushiyangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://sea.c1oappe.top

Go:   slices.Sort(arr)
来源：http://btb.xingfuxueyuan.xyz

Ruby: arr.sort
来源：http://kop.zhixingplan.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ibp.ivvv.top

[N03] 快速排序（分治示例）
来源：http://eao.yvedp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://flh.jinghuilouyu.cn

PHP:  // 递归实现，或用 usort
来源：http://roq.zhongyouzk.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lnv.shanyushiyangtech.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gor.tanke756.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qvo.aizwys.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hah.ctjpmb.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xkq.yueranfly.top

C#:   // 手写递归，或 Array.Sort
来源：http://dfd.hfpthk.cn

[N04] 斐波那契数列
来源：http://ira.nanxinkj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lff.shanyushiyangtech.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vkm.havefunace.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uod.guowangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kjl.gotoacloud.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pcg.wangshuangyany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mld.smart0.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gxc.wangshuangyany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yaa.yuanzhike.top

[N05] 最大公约数
来源：http://mim.hammf.cn

Py:   math.gcd(a, b)
来源：http://rvi.fanxiaobao.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wam.cheryme.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hff.0kj1m.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mqb.yongpay.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cjz.redwolf501.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bjh.gotoacloud.top

Ruby: a.gcd(b)
来源：http://gfu.cashguo.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wni.jinghuilouyu.cn

[N06] 判断回文字符串
来源：http://kti.wangdashe.top

Py:   s == s[::-1]
来源：http://efm.birdmap.top

PHP:  $s === strrev($s);
来源：http://jey.bbcook.cn

JS:   s === [...s].reverse().join("")
来源：http://hfi.gaohongyu789.top

TS:   s === [...s].reverse().join("")
来源：http://dla.zhixingplan.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://owg.hfpthk.cn

Go:   // 双指针从两端比较
来源：http://vxs.yuanzhike.top

Ruby: s == s.reverse
来源：http://wia.hfpthk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kxn.fktsv.cn

[N07] 两数之和（返回下标）
来源：http://hxa.tarul.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lxy.feifeiyinyue.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gvv.chenjidiqi.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://tef.ywan-chungtsiang.top

TS:   // 手写 Map<string, number>
来源：http://tqj.hywenlv.cn

Java: // 手写 HashMap
来源：http://ubc.vehdjk.com

Go:   // 手写 map[int]int
来源：http://cml.fktsv.cn

Ruby: // 手写 Hash
来源：http://hvj.yuxming.cn

C#:   // 手写 Dictionary<int, int>
来源：http://iip.zhixingplan.top

[N08] 生成全排列
来源：http://par.0kj1m.cn

Py:   itertools.permutations(arr)
来源：http://dnk.hammf.cn

PHP:  // 手写递归交换
来源：http://vnw.gogol.net.cn

JS:   // 手写回溯递归
来源：http://wht.c1oappe.top

TS:   // 手写回溯递归
来源：http://bpa.tianlin.xyz

Java: // 手写回溯递归
来源：http://xxf.yueranfly.top

Go:   // 手写回溯递归
来源：http://dom.gaohongyu789.top

Ruby: arr.permutation.to_a
来源：http://pjl.yuxming.cn

C#:   // 手写回溯递归
来源：http://dot.hnxiangtu.top

[N09] 栈与队列
来源：http://ykv.yanxiufei.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ofa.tarul.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hix.ivvv.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lsi.sufxvd.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kqj.zhoulong.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hpu.iojbl.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vad.yfazqb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ehj.ctjpmb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cwu.shanyushiyangtech.top

[N10] 链表节点定义
来源：http://wcb.tanke756.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ppq.smart0.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://ald.meibo888.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gkf.hnxiangtu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://emv.jiagoushi.top

Java: class Node { int v; Node next; }
来源：http://opd.cqqwz.cn

Go:   type Node struct { V int; Next *Node }
来源：http://eiw.epnwcf.com

Ruby: Node = Struct.new(:v, :next)
来源：http://lqm.yuanzhike.top

C#:   class Node { public int V; public Node? Next; }
来源：http://eat.meibo888.top

[N11] 二叉树中序遍历
来源：http://mmd.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uib.fehbvm.com

PHP:  // 手写递归函数
来源：http://jvz.zhijiandao.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eru.gaohongyu789.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bzi.hcnkem.com

Java: // 手写递归
来源：http://ljn.iojbl.cn

Go:   // 手写递归
来源：http://mos.cdnleiting.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jix.nwbrower.top

C#:   // 手写递归
来源：http://zwc.shanyushiyangtech.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kjo.yj20258.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://crs.bjfxy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dgk.andypj.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kxp.chenlongwang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zge.meibo888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gjs.c1oappe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mlb.yuxming.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fud.ydzc1.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bav.tian-w.cn

================================================================================
来源：http://qpx.pengpengdd.cyou

O. 并发与异步
来源：http://efk.mhx1999.top

================================================================================
来源：http://laf.52xcode.cn

[O01] 启动一个线程
来源：http://nsf.zhoulong.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cie.svipenyu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kln.ybcxt.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ijo.feifeiyinyue.top

TS:   // 同 JS
来源：http://nke.wangshuangyany.cn

Java: new Thread(() -> f()).start()
来源：http://xxv.jianghu66.top

Go:   go f()
来源：http://qiy.ppjwa.cn

Ruby: Thread.new { f }
来源：http://jmb.52xcode.cn

C#:   Task.Run(() => F());
来源：http://kkd.chenlongwang.top

[O02] 使用线程池
来源：http://abo.zdbjq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fdu.tian-w.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cau.redwolf501.top

JS:   // worker_threads 线程池
来源：http://bdw.ivvv.top

TS:   // worker_threads 线程池
来源：http://jig.xinyue.icu

Java: Executors.newFixedThreadPool(4)
来源：http://jam.bbcook.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zwp.hnqzz.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qox.nwbrower.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zgl.fehbvm.com

[O03] 加锁保护共享数据
来源：http://ihs.redwolf501.top

Py:   with lock: shared += 1
来源：http://kpj.xinyue.icu

PHP:  // 用 flock() 做文件锁
来源：http://xuw.hammf.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kbp.nanxuanxn.top

TS:   // 同 JS
来源：http://qob.hfpthk.cn

Java: synchronized (this) { shared++; }
来源：http://ekd.aibaodan.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://atr.cqqwz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gix.aizwys.cn

C#:   lock (gate) { shared++; }
来源：http://kox.316326.xyz

[O04] 定义异步函数并等待
来源：http://dxl.feifeiyinyue.top

Py:   async def f():⏎    await g()
来源：http://gvi.ppjwa.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ydb.ppjwa.cn

JS:   async function f() { await g(); }
来源：http://sgk.jqgufenzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://xwe.hnxiangtu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nnz.hongshengwenyu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ypr.fzhhl.top

Ruby: # 用 Fiber 或 async gem
来源：http://oun.sysykeji.top

C#:   async Task F() { await G(); }
来源：http://zmm.pycfn.com

[O05] 并发执行并等待全部完成
来源：http://ryy.xuanzx.com

Py:   asyncio.gather(*tasks)
来源：http://ovn.jinqigufen.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ijk.yuxming.cn

JS:   await Promise.all(tasks)
来源：http://gkb.iojbl.cn

TS:   await Promise.all(tasks)
来源：http://mgh.tian-w.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blg.c1oappe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jxm.cdnleiting.top

Ruby: threads.map(&:join)
来源：http://pjt.wangdashe.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ixv.cucudq.cn

[O06] 使用进程池
来源：http://dck.bbcook.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pgm.tian-w.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jqc.xingfuxueyuan.xyz

JS:   // child_process / cluster 模块
来源：http://dgo.jqgfzy.top

TS:   // child_process / cluster 模块
来源：http://ycd.dianchejie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bio.vqdsnc.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bik.havefunace.top

Ruby: // fork 块
来源：http://ekt.daria6918.cn

C#:   Parallel.For
来源：http://krn.zhixingplan.top

================================================================================
来源：http://rye.9152youxi.cn

P. 常用工具函数
来源：http://hmj.tarul.cn

================================================================================
来源：http://mui.xziqi.cn

[P01] 生成 UUID
来源：http://llk.meibo888.top

Py:   str(uuid.uuid4())
来源：http://cnt.tanke756.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://eou.yj20258888.top

JS:   crypto.randomUUID()
来源：http://jtf.tanke756.top

TS:   crypto.randomUUID()
来源：http://xnc.uphjek.com

Java: UUID.randomUUID().toString()
来源：http://yub.gaohongyu789.top

Go:   // 用 github.com/google/uuid
来源：http://fil.yvedp.cn

Ruby: SecureRandom.uuid
来源：http://wyv.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://waf.yj20258.top

[P02] MD5 / SHA256 摘要
来源：http://wvo.aizwys.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wvx.snrcjt.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lrw.chenzaomai.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ngk.zdbjq.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ozb.epnwcf.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nqh.sweek.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://olh.nanxinkj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://snn.cucudq.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wog.shangyingyoupin.top

[P03] 生成短随机字符串
来源：http://svc.pycfn.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://huk.hcnkem.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://swn.fktsv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sgy.jinghuilouyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ptc.tanke756.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rmt.yongpay.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vre.sweek.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lxm.c1oappe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rrq.hfpthk.cn

[P04] 求长度
来源：http://sve.zhijiandao.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cgd.xylfe.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uvi.zhongyouzk.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gph.hnqzz.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eem.hnxiangtu.top

Java: list.size();  map.size();  s.length()
来源：http://iot.snrcjt.cn

Go:   len(arr);  len(m)
来源：http://jey.gzhubu.top

Ruby: x.length;  x.size
来源：http://cpi.hesvh.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://svv.xziqi.cn

[P05] 判断两个对象内容是否相等
来源：http://yat.gaohongyu789.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://njv.xuanzx.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vkx.jqgufenzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ypp.shuidangran.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ist.mhx1999.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kqm.nanxinkj.top

Go:   reflect.DeepEqual(a, b)
来源：http://wwp.jinghuilouyu.cn

Ruby: a == b
来源：http://php.gotoacloud.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bsw.zhijiandao.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sfz.mhx1999.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cdo.c1oappe.top

PHP:  if (empty($x)) {}
来源：http://ywb.daria6918.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://aok.yangfankeji.com

TS:   if (x == null) {}
来源：http://qgk.xingfuxueyuan.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://kxd.ehwqpu.com

Go:   if x == nil {}
来源：http://pdr.mhx1999.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bjd.zhengqikj.top

C#:   if (x is null) {}
来源：http://pyz.yanxiufei.cn

[P07] 防抖与节流
来源：http://qlb.feifeiyinyue.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://typ.yuxming.cn

PHP:  // 手写时间戳比较
来源：http://lpa.ctjpmb.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cdi.kuanghao11.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dch.jinyuanbaomall.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uor.shangyingyoupin.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xpi.gotoacloud.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://psd.svipenyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://taj.jiagoushi.top

[P08] 处理浮点精度问题
来源：http://byw.yj202588.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fpt.jyoumei.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kpy.wangdashe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jvz.zdqjudy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uzc.zhixingplan.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fxy.yanxiufei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kfx.feifeiyinyue.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://iyn.ppjwa.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rsg.zhengqikj.top

================================================================================
来源：http://pyi.yuxming.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gli.yuanzhike.top

================================================================================
来源：http://caj.zhaomingkeji.xyz

[Q01] 创建表
来源：http://pje.zhiwuduotai.top

CREATE TABLE users (
来源：http://xns.jinyuanbaomall.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dke.tian-w.cn

name VARCHAR(50) NOT NULL,
来源：http://vlz.gogol.net.cn

email VARCHAR(100) UNIQUE,
来源：http://qza.hongshengwenyu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zlp.hcnkem.com

);
来源：http://jhw.wangshuangyany.cn

[Q02] 创建带外键的表
来源：http://scz.fanxiaobao.xyz

CREATE TABLE orders (
来源：http://asm.aibaodan.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://acr.zhoulong.xyz

user_id INT NOT NULL,
来源：http://fwg.gaohongyu789.top

amount DECIMAL(10, 2),
来源：http://lls.smart0.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://acg.chenjidiqi.icu


<!-- 参考信息 -->