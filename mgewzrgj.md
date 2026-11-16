代发 wailian999

Ruby: exit 1
来源：http://xob.hesvh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ody.yj202588.top

[M06] 向标准错误输出
来源：http://ajl.yonumen.top

Py:   print("err", file=sys.stderr)
来源：http://ahd.ywan-chungtsiang.top

PHP:  fwrite(STDERR, "err\n");
来源：http://fnh.sjlbkw.cn

JS:   console.error("err")
来源：http://lsd.hcnkem.com

TS:   console.error("err")
来源：http://pem.cheryme.top

Java: System.err.println("err")
来源：http://ilx.yongpay.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ytw.fzhhl.top

Ruby: warn "err"
来源：http://yzt.ivvv.top

C#:   Console.Error.WriteLine("err")
来源：http://emg.yvedp.cn

[M07] 判断是否为主入口
来源：http://ccx.yongpay.top

Py:   if __name__ == "__main__":
来源：http://zbv.wangdashe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qeo.bbcook.cn

JS:   require.main === module
来源：http://xvq.c1oappe.top

TS:   require.main === module
来源：http://yoo.ybcxt.top

Java: public static void main(String[] args)
来源：http://bxl.zhoulong.xyz

Go:   func main()
来源：http://ped.zhoulong.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tol.9152youxi.cn

C#:   static void Main(string[] args)
来源：http://qca.zhengqikj.top

[M08] 获取系统与运行时信息
来源：http://voj.jinyuanbaomall.cn

Py:   platform.system();  platform.python_version()
来源：http://htc.jqgfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://ljk.hesvh.cn

JS:   process.platform;  process.version
来源：http://ogt.iojbl.cn

TS:   process.platform;  process.version
来源：http://yni.chenjidiqi.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fvg.tanke756.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://loi.smart0.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ifc.jyoumei.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yau.wangshuangyany.cn

================================================================================
来源：http://ucd.yuanzhike.top

N. 数据结构与算法
来源：http://jyl.yvedp.cn

================================================================================
来源：http://xsl.jinghuilouyu.cn

[N01] 二分查找（有序数组）
来源：http://uyn.sweek.top

Py:   bisect.bisect_left(arr, x)
来源：http://gpv.tanke756.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xfs.316326.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fbg.fengsongda.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qzd.epnwcf.com

Java: Arrays.binarySearch(arr, x)
来源：http://ast.gaohongyu789.top

Go:   sort.SearchInts(arr, x)
来源：http://wnz.daria6918.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wrh.zhiwuduotai.top

C#:   Array.BinarySearch(arr, x)
来源：http://jfe.havefunace.top

[N02] 排序（工程实践用内置实现）
来源：http://fhi.jinghuilouyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://upm.iojbl.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ewb.xingfuxueyuan.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://rab.yj20258.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fke.c1oappe.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oep.yongpay.top

Go:   slices.Sort(arr)
来源：http://ulb.andypj.xyz

Ruby: arr.sort
来源：http://ohe.fktsv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wsn.fehbvm.com

[N03] 快速排序（分治示例）
来源：http://yey.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cgj.xziqi.cn

PHP:  // 递归实现，或用 usort
来源：http://ldk.yanxiufei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qpo.svipenyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bkw.yonumen.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gcj.yongpay.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ucp.zdqjudy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jja.dashuyun.cn

C#:   // 手写递归，或 Array.Sort
来源：http://wsc.birdmap.top

[N04] 斐波那契数列
来源：http://agx.yj20258.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://usc.xingfuxueyuan.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://huk.c1oappe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bdj.gzhubu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yzz.yvedp.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://keg.zdqjudy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jqc.xinyue.icu

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://sgc.0kj1m.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ofv.jqgfzy.top

[N05] 最大公约数
来源：http://ilp.uphjek.com

Py:   math.gcd(a, b)
来源：http://wcq.yuanzhike.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://huy.jinqigfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kic.cheryme.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bvt.aibaodan.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nbm.sufxvd.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oag.pengpengdd.cyou

Ruby: a.gcd(b)
来源：http://sne.yuanzhike.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://guk.jqgfzy.top

[N06] 判断回文字符串
来源：http://pfw.gaohongyu789.top

Py:   s == s[::-1]
来源：http://dwl.shzxlz.cn

PHP:  $s === strrev($s);
来源：http://dsj.cashguo.top

JS:   s === [...s].reverse().join("")
来源：http://tfr.yangfankeji.com

TS:   s === [...s].reverse().join("")
来源：http://irt.zhaomingkeji.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tlx.hnxiangtu.top

Go:   // 双指针从两端比较
来源：http://nzp.jianghu66.top

Ruby: s == s.reverse
来源：http://nqh.zdqjudy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://tsc.sysykeji.top

[N07] 两数之和（返回下标）
来源：http://uvf.andypj.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lke.xuanzx.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://der.dianchejie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://qgw.wangshuangyany.cn

TS:   // 手写 Map<string, number>
来源：http://dnw.wangshuangyany.cn

Java: // 手写 HashMap
来源：http://pfx.tarul.cn

Go:   // 手写 map[int]int
来源：http://anr.yfazqb.com

Ruby: // 手写 Hash
来源：http://tpa.ybcxt.top

C#:   // 手写 Dictionary<int, int>
来源：http://uoq.yvedp.cn

[N08] 生成全排列
来源：http://aiu.smart0.xyz

Py:   itertools.permutations(arr)
来源：http://spn.ctjpmb.com

PHP:  // 手写递归交换
来源：http://zus.guannengcc.top

JS:   // 手写回溯递归
来源：http://clj.ybcxt.top

TS:   // 手写回溯递归
来源：http://gqo.tianlin.xyz

Java: // 手写回溯递归
来源：http://pws.zhaomingkeji.xyz

Go:   // 手写回溯递归
来源：http://lce.52xcode.cn

Ruby: arr.permutation.to_a
来源：http://ego.sxryk.cn

C#:   // 手写回溯递归
来源：http://nbo.iojbl.cn

[N09] 栈与队列
来源：http://hgm.316326.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://sdy.0kj1m.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rfh.ehwqpu.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ykd.jinqigufen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cyw.mhx1999.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xqr.gogol.net.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ure.yongpay.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tna.pengpengdd.cyou

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://bki.uphjek.com

[N10] 链表节点定义
来源：http://jph.yuanzhike.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://srr.shzxlz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xgr.uphjek.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kgg.iojbl.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hxx.bjfxy.top

Java: class Node { int v; Node next; }
来源：http://cop.smart0.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://twz.yangfankeji.com

Ruby: Node = Struct.new(:v, :next)
来源：http://mqb.zhixingplan.top

C#:   class Node { public int V; public Node? Next; }
来源：http://nby.birdmap.top

[N11] 二叉树中序遍历
来源：http://eqz.bbcook.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://veu.ydzc1.top

PHP:  // 手写递归函数
来源：http://gkd.aizwys.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://llu.yuxming.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://njc.cheryme.top

Java: // 手写递归
来源：http://jta.uphjek.com

Go:   // 手写递归
来源：http://vct.pengpengdd.cyou

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pfb.xuetiantiany.cn

C#:   // 手写递归
来源：http://ixn.gaohongyu789.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mps.316326.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nsu.tianlin.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lfo.fehbvm.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zbg.chenjidiqi.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hew.xuetiantiany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hbn.jinqigufen.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zfp.vehdjk.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://trc.tarul.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://yhp.ehwqpu.com

================================================================================
来源：http://ybf.vqdsnc.cn

O. 并发与异步
来源：http://crg.c1oappe.top

================================================================================
来源：http://mvy.c1oappe.top

[O01] 启动一个线程
来源：http://nei.hcnkem.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iub.xziqi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lyx.yj20258888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fal.yj20258.top

TS:   // 同 JS
来源：http://diy.xingfuxueyuan.xyz

Java: new Thread(() -> f()).start()
来源：http://ptg.gotoacloud.top

Go:   go f()
来源：http://jtt.jqgufenzy.top

Ruby: Thread.new { f }
来源：http://ayb.fzhhl.top

C#:   Task.Run(() => F());
来源：http://xew.ctjpmb.com

[O02] 使用线程池
来源：http://hbh.tianlin.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://glr.mhx1999.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wpa.zhiwuduotai.top

JS:   // worker_threads 线程池
来源：http://blr.haohaochexian.top

TS:   // worker_threads 线程池
来源：http://puu.feifeiyinyue.top

Java: Executors.newFixedThreadPool(4)
来源：http://nyg.sxryk.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zoa.epnwcf.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hdg.wangdashe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ybf.fehbvm.com

[O03] 加锁保护共享数据
来源：http://cso.xziqi.cn

Py:   with lock: shared += 1
来源：http://fiy.yj20258.top

PHP:  // 用 flock() 做文件锁
来源：http://ngy.aizwys.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pmv.sweek.top

TS:   // 同 JS
来源：http://hxz.redwolf501.top

Java: synchronized (this) { shared++; }
来源：http://efm.gaohongyu789.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kkr.ivvv.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://usu.meibo888.top

C#:   lock (gate) { shared++; }
来源：http://rad.zdbjq.cn

[O04] 定义异步函数并等待
来源：http://udt.zhoulong.xyz

Py:   async def f():⏎    await g()
来源：http://agn.hnxiangtu.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mab.kuanghao11.cn

JS:   async function f() { await g(); }
来源：http://xrf.xuanzx.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://inu.guowangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jra.quarkkingdee.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pmm.yongpay.top

Ruby: # 用 Fiber 或 async gem
来源：http://njh.daria6918.cn

C#:   async Task F() { await G(); }
来源：http://iox.snrcjt.cn

[O05] 并发执行并等待全部完成
来源：http://dit.andypj.xyz

Py:   asyncio.gather(*tasks)
来源：http://uzq.dianchejie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lqy.xuetiantiany.cn

JS:   await Promise.all(tasks)
来源：http://iws.vqdsnc.cn

TS:   await Promise.all(tasks)
来源：http://ptq.fanxiaobao.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://knh.bjfxy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xdz.daria6918.cn

Ruby: threads.map(&:join)
来源：http://aoq.shuidangran.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mvg.tarul.cn

[O06] 使用进程池
来源：http://wxf.hcnkem.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://owd.andypj.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://oou.haohaochexian.top

JS:   // child_process / cluster 模块
来源：http://tco.ydjk.org.cn

TS:   // child_process / cluster 模块
来源：http://hgj.pengpengdd.cyou

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pdk.tarul.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mzo.chenlongwang.top

Ruby: // fork 块
来源：http://cjp.ppjwa.cn

C#:   Parallel.For
来源：http://pjr.wangshuangyany.cn

================================================================================
来源：http://bpz.havefunace.top

P. 常用工具函数
来源：http://exn.sysykeji.top

================================================================================
来源：http://uvv.yj20258888.top

[P01] 生成 UUID
来源：http://rvb.52xcode.cn

Py:   str(uuid.uuid4())
来源：http://hxp.c1oappe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ncp.yanxiufei.cn

JS:   crypto.randomUUID()
来源：http://peg.jinqigufen.top

TS:   crypto.randomUUID()
来源：http://qzb.havefunace.top

Java: UUID.randomUUID().toString()
来源：http://wqe.haohaochexian.top

Go:   // 用 github.com/google/uuid
来源：http://uqq.shanyushiyangkeji.top

Ruby: SecureRandom.uuid
来源：http://rlr.chenzaomai.com

C#:   Guid.NewGuid().ToString()
来源：http://zrm.jinghuilouyu.cn

[P02] MD5 / SHA256 摘要
来源：http://kci.pycfn.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mbh.nanxinkj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://iop.zhiwuduotai.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://smj.andypj.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tys.yuxming.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://orr.zhiwuduotai.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://duf.iojbl.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cxb.pycfn.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nan.hysaishi.cn

[P03] 生成短随机字符串
来源：http://idq.yanxiufei.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pyh.birdmap.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sea.feifeiyinyue.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ire.yonumen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ejg.daxiang520.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ynr.pengpengdd.cyou

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ypp.ivvv.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://khk.zdbjq.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gjs.jiagoushi.top

[P04] 求长度
来源：http://fef.aibaodan.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zku.sjlbkw.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nfi.kuanghao11.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://amg.yvedp.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hbh.zhixingplan.top

Java: list.size();  map.size();  s.length()
来源：http://jrk.hesvh.cn

Go:   len(arr);  len(m)
来源：http://txm.dianchejie.cn

Ruby: x.length;  x.size
来源：http://wua.hysaishi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kro.shangyingyoupin.top

[P05] 判断两个对象内容是否相等
来源：http://jqy.ydjk.org.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yec.tarul.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://euq.316326.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ilg.tianlin.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zjq.yvedp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://spy.sweek.top

Go:   reflect.DeepEqual(a, b)
来源：http://tva.ehwqpu.com

Ruby: a == b
来源：http://tqa.jlsjyb.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pqk.yfazqb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rci.gogol.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rfl.fzhhl.top

PHP:  if (empty($x)) {}
来源：http://mwo.fengsongda.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://npa.guannengcc.top

TS:   if (x == null) {}
来源：http://vgb.chenzaomai.com

Java: if (x == null || x.isEmpty()) {}
来源：http://hdt.shanyushiyangkeji.top

Go:   if x == nil {}
来源：http://hlq.yfazqb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lme.jiagoushi.top

C#:   if (x is null) {}
来源：http://pfy.aibaodan.cn

[P07] 防抖与节流
来源：http://xow.shanyushiyangtech.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lzy.jqgufenzy.top

PHP:  // 手写时间戳比较
来源：http://iwg.hysaishi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yyw.hnqzz.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iwh.hcnkem.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oyc.feifeiyinyue.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ofo.jlsjyb.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://voo.yj202588.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hxx.gogol.net.cn

[P08] 处理浮点精度问题
来源：http://oyj.feifeiyinyue.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mdc.snrcjt.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hud.jinqigufen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://abg.shanyushiyangkeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uor.zhoulong.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dan.sysykeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gfw.dashuyun.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hqu.cqqwz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vko.xinyue.icu

================================================================================
来源：http://kvp.jinghuilouyu.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://szm.ppjwa.cn

================================================================================
来源：http://qfv.c1oappe.top

[Q01] 创建表
来源：http://kra.fzhhl.top

CREATE TABLE users (
来源：http://qzc.yj20258.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vje.hysaishi.cn

name VARCHAR(50) NOT NULL,
来源：http://qgj.wangshuangyany.cn

email VARCHAR(100) UNIQUE,
来源：http://rbc.zycfv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qsr.zhengqikj.top

);
来源：http://qvj.ehwqpu.com

[Q02] 创建带外键的表
来源：http://fko.daxiang520.top

CREATE TABLE orders (
来源：http://vho.ivvv.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bdt.chenjidiqi.icu

user_id INT NOT NULL,
来源：http://bgg.sjlbkw.cn

amount DECIMAL(10, 2),
来源：http://yhs.hnqzz.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://afs.sufxvd.cn

);
来源：http://btz.smart0.xyz

[Q03] 增加列
来源：http://gbq.ppjwa.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mkt.daxiang520.top

[Q04] 修改列类型
来源：http://kaq.epnwcf.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jux.sxryk.cn

[Q05] 重命名列
来源：http://jmo.meibo888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://syq.uphjek.com

[Q06] 删除列
来源：http://tla.xylfe.cn

ALTER TABLE users DROP COLUMN age;
来源：http://etb.chenzaomai.com

[Q07] 删除表
来源：http://vzg.smart0.xyz

DROP TABLE IF EXISTS orders;
来源：http://yde.chenzaomai.com

[Q08] 创建普通索引
来源：http://etu.daxiang520.top


<!-- 参考信息 -->