代发 wailian999

JS:   process.exit(1)
来源：http://dqj.sxryk.cn

TS:   process.exit(1)
来源：http://upj.jiagoushi.top

Java: System.exit(1)
来源：http://ufk.yvedp.cn

Go:   os.Exit(1)
来源：http://yam.chenjidiqi.icu

Ruby: exit 1
来源：http://ojh.ehwqpu.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lmj.bbcook.cn

[M06] 向标准错误输出
来源：http://bff.pycfn.com

Py:   print("err", file=sys.stderr)
来源：http://sun.shzxlz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://llb.xylfe.cn

JS:   console.error("err")
来源：http://bqh.vehdjk.com

TS:   console.error("err")
来源：http://ctu.hfpthk.cn

Java: System.err.println("err")
来源：http://gyg.xinyue.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vzv.gogol.net.cn

Ruby: warn "err"
来源：http://tbh.jqgufenzy.top

C#:   Console.Error.WriteLine("err")
来源：http://dli.feifeiyinyue.top

[M07] 判断是否为主入口
来源：http://vvp.pengpengdd.cyou

Py:   if __name__ == "__main__":
来源：http://snn.jinqigfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://niu.yuanzhike.top

JS:   require.main === module
来源：http://cyn.0kj1m.cn

TS:   require.main === module
来源：http://dwq.daxiang520.top

Java: public static void main(String[] args)
来源：http://gwq.fzhhl.top

Go:   func main()
来源：http://ukj.ppjwa.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nxa.xuanzx.com

C#:   static void Main(string[] args)
来源：http://dyz.ybcxt.top

[M08] 获取系统与运行时信息
来源：http://lti.yj202588.top

Py:   platform.system();  platform.python_version()
来源：http://gfg.ctjpmb.com

PHP:  PHP_OS;  phpversion();
来源：http://qyv.52xcode.cn

JS:   process.platform;  process.version
来源：http://bdq.shangyingyoupin.top

TS:   process.platform;  process.version
来源：http://lph.hnxiangtu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ixx.yanxiufei.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dce.jlsjyb.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dkp.epnwcf.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://rwt.jinqigfzy.top

================================================================================
来源：http://fhl.epnwcf.com

N. 数据结构与算法
来源：http://xkn.yueranfly.top

================================================================================
来源：http://edg.hfpthk.cn

[N01] 二分查找（有序数组）
来源：http://jva.hfpthk.cn

Py:   bisect.bisect_left(arr, x)
来源：http://oee.jyoumei.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://crl.guannengcc.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dzj.316326.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qnj.chenjidiqi.icu

Java: Arrays.binarySearch(arr, x)
来源：http://ekm.cheryme.top

Go:   sort.SearchInts(arr, x)
来源：http://lxe.redwolf501.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://cxi.yj20258888.top

C#:   Array.BinarySearch(arr, x)
来源：http://pzk.bbcook.cn

[N02] 排序（工程实践用内置实现）
来源：http://oyw.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://oao.sxryk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bie.bbcook.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sqb.shanyushiyangtech.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vtd.shangyingyoupin.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mfi.zhijiandao.cn

Go:   slices.Sort(arr)
来源：http://mql.zhaomingkeji.xyz

Ruby: arr.sort
来源：http://deh.yangfankeji.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://scn.cheryme.top

[N03] 快速排序（分治示例）
来源：http://iuf.c1oappe.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tuk.sufxvd.cn

PHP:  // 递归实现，或用 usort
来源：http://jta.hongshengwenyu.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uoz.yangfankeji.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://opq.ivvv.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yhh.jinqigufen.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eaw.gzhubu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yui.chenjidiqi.icu

C#:   // 手写递归，或 Array.Sort
来源：http://yyf.cashguo.top

[N04] 斐波那契数列
来源：http://glx.yj202588.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vsw.hfpthk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://pcf.nwbrower.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ewj.xylfe.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ipa.bjfxy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hrp.chenlongwang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://src.yvedp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ijl.hfpthk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uwo.hongshengwenyu.top

[N05] 最大公约数
来源：http://ccs.zdqjudy.top

Py:   math.gcd(a, b)
来源：http://exl.hywenlv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uta.tanke756.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://muk.aibaodan.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eso.hywenlv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wsy.shuidangran.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rqx.jinyuanbaomall.cn

Ruby: a.gcd(b)
来源：http://rjo.xuanzx.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://usm.zhijiandao.cn

[N06] 判断回文字符串
来源：http://obr.yfazqb.com

Py:   s == s[::-1]
来源：http://dtq.mhx1999.top

PHP:  $s === strrev($s);
来源：http://gtk.gotoacloud.top

JS:   s === [...s].reverse().join("")
来源：http://vpo.chenzaomai.com

TS:   s === [...s].reverse().join("")
来源：http://gti.hysaishi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xfb.sweek.top

Go:   // 双指针从两端比较
来源：http://xgz.yueranfly.top

Ruby: s == s.reverse
来源：http://uhe.fktsv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bsd.fzhhl.top

[N07] 两数之和（返回下标）
来源：http://hhy.c1oappe.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ame.yonumen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zfh.yueranfly.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vuc.hywenlv.cn

TS:   // 手写 Map<string, number>
来源：http://uly.sysykeji.top

Java: // 手写 HashMap
来源：http://akm.hcnkem.com

Go:   // 手写 map[int]int
来源：http://dze.jinqigufen.top

Ruby: // 手写 Hash
来源：http://hit.zdbjq.cn

C#:   // 手写 Dictionary<int, int>
来源：http://wum.hysaishi.cn

[N08] 生成全排列
来源：http://xrk.sufxvd.cn

Py:   itertools.permutations(arr)
来源：http://wbs.guannengcc.top

PHP:  // 手写递归交换
来源：http://dtg.yongpay.top

JS:   // 手写回溯递归
来源：http://ibn.ywan-chungtsiang.top

TS:   // 手写回溯递归
来源：http://wtn.wangdashe.top

Java: // 手写回溯递归
来源：http://isw.smart0.xyz

Go:   // 手写回溯递归
来源：http://bev.hcnkem.com

Ruby: arr.permutation.to_a
来源：http://ddv.fzhhl.top

C#:   // 手写回溯递归
来源：http://zzh.birdmap.top

[N09] 栈与队列
来源：http://qhm.svipenyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hkd.guannengcc.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jmw.zdbjq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lrm.hnqzz.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zgt.sxryk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://huh.ivvv.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hii.fzhhl.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://cnf.svipenyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gfy.yuxming.cn

[N10] 链表节点定义
来源：http://rii.yonumen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fow.52xcode.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dcl.zhongyouzk.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ezt.bjfxy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hrt.fzhhl.top

Java: class Node { int v; Node next; }
来源：http://fnr.52xcode.cn

Go:   type Node struct { V int; Next *Node }
来源：http://agn.ctjpmb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://qxa.gzhubu.top

C#:   class Node { public int V; public Node? Next; }
来源：http://sqg.shzxlz.cn

[N11] 二叉树中序遍历
来源：http://xgo.yueranfly.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cub.smart0.xyz

PHP:  // 手写递归函数
来源：http://xxl.wangshuangyany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sqd.shzxlz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iqb.xziqi.cn

Java: // 手写递归
来源：http://bqy.sufxvd.cn

Go:   // 手写递归
来源：http://okp.ehwqpu.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ymi.vehdjk.com

C#:   // 手写递归
来源：http://tgy.chenlongwang.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://onh.jqgufenzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lrv.svipenyu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xsp.ivvv.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hxh.shanyushiyangkeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tym.shzxlz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xww.cucudq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://phl.52xcode.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qpn.gaohongyu789.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gbt.bbcook.cn

================================================================================
来源：http://ewx.jianghu66.top

O. 并发与异步
来源：http://hev.fehbvm.com

================================================================================
来源：http://gip.andypj.xyz

[O01] 启动一个线程
来源：http://naq.fehbvm.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://otn.yj20258.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jjg.dianchejie.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wrh.wangshuangyany.cn

TS:   // 同 JS
来源：http://kyu.xylfe.cn

Java: new Thread(() -> f()).start()
来源：http://wbw.wangdashe.top

Go:   go f()
来源：http://qld.fzhhl.top

Ruby: Thread.new { f }
来源：http://cpa.sysykeji.top

C#:   Task.Run(() => F());
来源：http://abn.yongpay.top

[O02] 使用线程池
来源：http://uph.aizwys.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qit.cashguo.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tiq.shuidangran.top

JS:   // worker_threads 线程池
来源：http://nvx.zhaomingkeji.xyz

TS:   // worker_threads 线程池
来源：http://kcp.shangyingyoupin.top

Java: Executors.newFixedThreadPool(4)
来源：http://dsg.shangyingyoupin.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pul.316326.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lyv.jqgufenzy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jij.ydjk.org.cn

[O03] 加锁保护共享数据
来源：http://gcg.52xcode.cn

Py:   with lock: shared += 1
来源：http://rzl.aizwys.cn

PHP:  // 用 flock() 做文件锁
来源：http://gla.nwbrower.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qnf.fzhhl.top

TS:   // 同 JS
来源：http://nmp.redwolf501.top

Java: synchronized (this) { shared++; }
来源：http://rqm.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wzo.aibaodan.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jqu.shanyushiyangtech.top

C#:   lock (gate) { shared++; }
来源：http://kql.cdnleiting.top

[O04] 定义异步函数并等待
来源：http://uuw.hywenlv.cn

Py:   async def f():⏎    await g()
来源：http://bqx.fehbvm.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uwn.bjfxy.top

JS:   async function f() { await g(); }
来源：http://fjh.daxiang520.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://bui.gzhubu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vdi.tanke756.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ubf.shangyingyoupin.top

Ruby: # 用 Fiber 或 async gem
来源：http://vck.jinyuanbaomall.cn

C#:   async Task F() { await G(); }
来源：http://aly.aibaodan.cn

[O05] 并发执行并等待全部完成
来源：http://yvh.ctjpmb.com

Py:   asyncio.gather(*tasks)
来源：http://xow.ydjk.org.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rsm.ctjpmb.com

JS:   await Promise.all(tasks)
来源：http://dxp.sufxvd.cn

TS:   await Promise.all(tasks)
来源：http://ivm.hammf.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jut.guannengcc.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://myk.snrcjt.cn

Ruby: threads.map(&:join)
来源：http://bvw.hongshengwenyu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://zvn.fzhhl.top

[O06] 使用进程池
来源：http://jmw.yuanzhike.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ler.0kj1m.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gaj.yj20258888.top

JS:   // child_process / cluster 模块
来源：http://sfh.feifeiyinyue.top

TS:   // child_process / cluster 模块
来源：http://ppl.hongshengwenyu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://spg.guowangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oqd.shuidangran.top

Ruby: // fork 块
来源：http://wgv.c1oappe.top

C#:   Parallel.For
来源：http://xoh.daria6918.cn

================================================================================
来源：http://pep.9152youxi.cn

P. 常用工具函数
来源：http://ppu.svipenyu.cn

================================================================================
来源：http://yla.feifeiyinyue.top

[P01] 生成 UUID
来源：http://dgc.daxiang520.top

Py:   str(uuid.uuid4())
来源：http://kwh.zdbjq.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dnf.sysykeji.top

JS:   crypto.randomUUID()
来源：http://ntf.hesvh.cn

TS:   crypto.randomUUID()
来源：http://usl.xylfe.cn

Java: UUID.randomUUID().toString()
来源：http://cvf.yj20258.top

Go:   // 用 github.com/google/uuid
来源：http://gob.jqgfzy.top

Ruby: SecureRandom.uuid
来源：http://xwn.mhx1999.top

C#:   Guid.NewGuid().ToString()
来源：http://eow.jinghuilouyu.cn

[P02] MD5 / SHA256 摘要
来源：http://tvr.yonumen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cmo.smart0.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://get.zhengqikj.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nrn.zhijiandao.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ife.vehdjk.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wje.bjfxy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ycl.zhijiandao.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://euu.havefunace.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pac.shzxlz.cn

[P03] 生成短随机字符串
来源：http://vnh.cqqwz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xhc.shanyushiyangkeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xyy.uphjek.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bcb.zycfv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yer.shuidangran.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wah.tianlin.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oxl.zdbjq.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qlx.yj20258.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lly.ehwqpu.com

[P04] 求长度
来源：http://klq.0kj1m.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lsa.316326.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yyl.shangyingyoupin.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ldp.shangyingyoupin.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zge.cdnleiting.top

Java: list.size();  map.size();  s.length()
来源：http://mfd.sysykeji.top

Go:   len(arr);  len(m)
来源：http://whb.kuanghao11.cn

Ruby: x.length;  x.size
来源：http://ywj.ybcxt.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vph.daria6918.cn

[P05] 判断两个对象内容是否相等
来源：http://vcm.zhengqikj.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ozi.chenjidiqi.icu

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ujd.pengpengdd.cyou

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lfg.jinyuanbaomall.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tnc.yangfankeji.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://svi.dianchejie.cn

Go:   reflect.DeepEqual(a, b)
来源：http://wik.9152youxi.cn

Ruby: a == b
来源：http://bon.tianlin.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jou.sufxvd.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gkk.gotoacloud.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lev.pycfn.com

PHP:  if (empty($x)) {}
来源：http://efc.guannengcc.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kyu.yanxiufei.cn

TS:   if (x == null) {}
来源：http://yah.tian-w.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://foq.ywan-chungtsiang.top

Go:   if x == nil {}
来源：http://fjk.shuidangran.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gsp.xinyue.icu

C#:   if (x is null) {}
来源：http://jbu.gzhubu.top

[P07] 防抖与节流
来源：http://ruu.yonumen.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gvd.ehwqpu.com

PHP:  // 手写时间戳比较
来源：http://hog.cashguo.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xve.bbcook.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vdm.hesvh.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mcv.sufxvd.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uus.cucudq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ksc.52xcode.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tzq.nwbrower.top

[P08] 处理浮点精度问题
来源：http://qxp.zdqjudy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ggl.52xcode.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zwp.shuidangran.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pvh.pengpengdd.cyou

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nby.xziqi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rzr.redwolf501.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jea.jqgufenzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://iit.9152youxi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tri.nanxuanxn.top

================================================================================
来源：http://wnf.nanxuanxn.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fid.mhx1999.top

================================================================================
来源：http://mns.jqgufenzy.top

[Q01] 创建表
来源：http://hvt.0kj1m.cn

CREATE TABLE users (
来源：http://cbg.chenzaomai.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mtx.hammf.cn

name VARCHAR(50) NOT NULL,
来源：http://ltu.tanke756.top

email VARCHAR(100) UNIQUE,
来源：http://jwo.cdnleiting.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://for.chenjidiqi.icu

);
来源：http://hmf.xingfuxueyuan.xyz

[Q02] 创建带外键的表
来源：http://iqb.uphjek.com

CREATE TABLE orders (
来源：http://mif.gzhubu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dcr.birdmap.top

user_id INT NOT NULL,
来源：http://uqo.jianghu66.top

amount DECIMAL(10, 2),
来源：http://rka.9152youxi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://buz.fzhhl.top

);
来源：http://bvs.shanyushiyangkeji.top

[Q03] 增加列
来源：http://ymj.bjfxy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oow.hfpthk.cn

[Q04] 修改列类型
来源：http://qad.ctjpmb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xhx.svipenyu.cn

[Q05] 重命名列
来源：http://uhf.hnxiangtu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dhl.hnqzz.top

[Q06] 删除列
来源：http://ouj.aizwys.cn


<!-- 参考信息 -->