代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://zxq.ybcxt.top

[M05] 设置退出码
来源：http://ugs.wangshuangyany.cn

Py:   sys.exit(1)
来源：http://zrl.dianchejie.cn

PHP:  exit(1);
来源：http://thw.dashuyun.cn

JS:   process.exit(1)
来源：http://xqj.aizwys.cn

TS:   process.exit(1)
来源：http://uox.andypj.xyz

Java: System.exit(1)
来源：http://ymb.wangshuangyany.cn

Go:   os.Exit(1)
来源：http://oyr.chenlongwang.top

Ruby: exit 1
来源：http://ubv.daria6918.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://neo.yonumen.top

[M06] 向标准错误输出
来源：http://zvj.xuetiantiany.cn

Py:   print("err", file=sys.stderr)
来源：http://uzg.vqdsnc.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rnj.smart0.xyz

JS:   console.error("err")
来源：http://tze.gaohongyu789.top

TS:   console.error("err")
来源：http://ysj.jianghu66.top

Java: System.err.println("err")
来源：http://zpk.xziqi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://aco.wangdashe.top

Ruby: warn "err"
来源：http://hhg.feifeiyinyue.top

C#:   Console.Error.WriteLine("err")
来源：http://eor.ydzc1.top

[M07] 判断是否为主入口
来源：http://eit.yueranfly.top

Py:   if __name__ == "__main__":
来源：http://zyx.shzxlz.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cxn.dashuyun.cn

JS:   require.main === module
来源：http://esi.dashuyun.cn

TS:   require.main === module
来源：http://dts.shuidangran.top

Java: public static void main(String[] args)
来源：http://sqn.birdmap.top

Go:   func main()
来源：http://sjr.tarul.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fyl.yonumen.top

C#:   static void Main(string[] args)
来源：http://eng.xinyue.icu

[M08] 获取系统与运行时信息
来源：http://qqq.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://rwc.fehbvm.com

PHP:  PHP_OS;  phpversion();
来源：http://wmy.0kj1m.cn

JS:   process.platform;  process.version
来源：http://jzc.yvedp.cn

TS:   process.platform;  process.version
来源：http://vta.nwbrower.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tfh.gotoacloud.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ojh.chenzaomai.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fjw.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://miw.yonumen.top

================================================================================
来源：http://qju.bjfxy.top

N. 数据结构与算法
来源：http://dfk.gaohongyu789.top

================================================================================
来源：http://vhs.daxiang520.top

[N01] 二分查找（有序数组）
来源：http://ian.cucudq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ecr.fehbvm.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://oiw.yj20258888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rav.yj20258.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://arg.yj20258888.top

Java: Arrays.binarySearch(arr, x)
来源：http://qsp.jianghu66.top

Go:   sort.SearchInts(arr, x)
来源：http://owt.bbcook.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sad.tianlin.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://cas.hongshengwenyu.top

[N02] 排序（工程实践用内置实现）
来源：http://xtt.dianchejie.cn

Py:   sorted(arr);  arr.sort()
来源：http://jjr.jlsjyb.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wcp.jyoumei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wey.shangyingyoupin.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vko.hesvh.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tdc.zdqjudy.top

Go:   slices.Sort(arr)
来源：http://lrn.hywenlv.cn

Ruby: arr.sort
来源：http://dco.fehbvm.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://fve.0kj1m.cn

[N03] 快速排序（分治示例）
来源：http://eoc.xuetiantiany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vup.kuanghao11.cn

PHP:  // 递归实现，或用 usort
来源：http://uno.daria6918.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://icx.0kj1m.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fif.zhixingplan.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qzp.ywan-chungtsiang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gyq.ctjpmb.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ovl.cqqwz.cn

C#:   // 手写递归，或 Array.Sort
来源：http://uwv.gogol.net.cn

[N04] 斐波那契数列
来源：http://zwt.zycfv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wdw.daria6918.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://svz.hongshengwenyu.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ezn.zdbjq.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xcj.shuidangran.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lms.nwbrower.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kmr.tanke756.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://lox.feifeiyinyue.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yit.zhaomingkeji.xyz

[N05] 最大公约数
来源：http://lmm.yonumen.top

Py:   math.gcd(a, b)
来源：http://jbw.gotoacloud.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://akq.yfazqb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jsx.guowangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jzs.smart0.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rmu.jinqigfzy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mxz.fengsongda.top

Ruby: a.gcd(b)
来源：http://gvt.yfazqb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://djo.chenjidiqi.icu

[N06] 判断回文字符串
来源：http://jzm.sjlbkw.cn

Py:   s == s[::-1]
来源：http://oky.hnqzz.top

PHP:  $s === strrev($s);
来源：http://bge.xuetiantiany.cn

JS:   s === [...s].reverse().join("")
来源：http://xtd.0kj1m.cn

TS:   s === [...s].reverse().join("")
来源：http://nqx.daria6918.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ajj.zycfv.cn

Go:   // 双指针从两端比较
来源：http://izk.shangyingyoupin.top

Ruby: s == s.reverse
来源：http://etv.chenjidiqi.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://xmy.9152youxi.cn

[N07] 两数之和（返回下标）
来源：http://mqc.dashuyun.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zza.sweek.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mhi.fzhhl.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wxd.jlsjyb.cn

TS:   // 手写 Map<string, number>
来源：http://tez.dashuyun.cn

Java: // 手写 HashMap
来源：http://onl.mhx1999.top

Go:   // 手写 map[int]int
来源：http://xve.gzhubu.top

Ruby: // 手写 Hash
来源：http://eus.sysykeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://eds.hysaishi.cn

[N08] 生成全排列
来源：http://jeg.jlsjyb.cn

Py:   itertools.permutations(arr)
来源：http://igy.ctjpmb.com

PHP:  // 手写递归交换
来源：http://elb.jqgufenzy.top

JS:   // 手写回溯递归
来源：http://wsl.chenlongwang.top

TS:   // 手写回溯递归
来源：http://hmj.svipenyu.cn

Java: // 手写回溯递归
来源：http://clv.yuxming.cn

Go:   // 手写回溯递归
来源：http://mpy.yuxming.cn

Ruby: arr.permutation.to_a
来源：http://gij.zhengqikj.top

C#:   // 手写回溯递归
来源：http://zzt.fanxiaobao.xyz

[N09] 栈与队列
来源：http://gbt.uphjek.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jqk.andypj.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://erd.jqgfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xpw.yuxming.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kll.fehbvm.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ton.wangdashe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gan.mhx1999.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qqi.zhaomingkeji.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://kgb.52xcode.cn

[N10] 链表节点定义
来源：http://mlv.ppjwa.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dki.yangfankeji.com

PHP:  class Node { public $v; public $next = null; }
来源：http://qfl.zhaomingkeji.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dqu.quarkkingdee.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://bdx.gzhubu.top

Java: class Node { int v; Node next; }
来源：http://nlp.fengsongda.top

Go:   type Node struct { V int; Next *Node }
来源：http://trb.zhoulong.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://elj.xingfuxueyuan.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://nhb.hammf.cn

[N11] 二叉树中序遍历
来源：http://wpk.jiagoushi.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lix.daria6918.cn

PHP:  // 手写递归函数
来源：http://dpx.shzxlz.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rxk.vehdjk.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ova.bjfxy.top

Java: // 手写递归
来源：http://wov.sweek.top

Go:   // 手写递归
来源：http://tsp.zhiwuduotai.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pno.hnqzz.top

C#:   // 手写递归
来源：http://cox.gaohongyu789.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pxr.yfazqb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cdl.zdbjq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wbe.chenjidiqi.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tck.quarkkingdee.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jxi.shuidangran.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ghp.aizwys.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fxe.yongpay.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tqy.hesvh.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fza.zhengqikj.top

================================================================================
来源：http://knf.chenlongwang.top

O. 并发与异步
来源：http://dtd.guowangkeji.top

================================================================================
来源：http://pcr.shanyushiyangtech.top

[O01] 启动一个线程
来源：http://pqk.zhaomingkeji.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jrk.sysykeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://dyc.ydjk.org.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kdj.uphjek.com

TS:   // 同 JS
来源：http://bei.xuanzx.com

Java: new Thread(() -> f()).start()
来源：http://nzs.tianlin.xyz

Go:   go f()
来源：http://rgx.xziqi.cn

Ruby: Thread.new { f }
来源：http://atf.daria6918.cn

C#:   Task.Run(() => F());
来源：http://hxm.ctjpmb.com

[O02] 使用线程池
来源：http://lsh.ehwqpu.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://axi.yongpay.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ngc.cdnleiting.top

JS:   // worker_threads 线程池
来源：http://jox.yj20258888.top

TS:   // worker_threads 线程池
来源：http://rmd.hysaishi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pxu.xinyue.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baw.jlsjyb.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gjo.ehwqpu.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://sin.daxiang520.top

[O03] 加锁保护共享数据
来源：http://neg.smart0.xyz

Py:   with lock: shared += 1
来源：http://jqp.hammf.cn

PHP:  // 用 flock() 做文件锁
来源：http://sgo.wangshuangyany.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://htj.ydzc1.top

TS:   // 同 JS
来源：http://wwf.jlsjyb.cn

Java: synchronized (this) { shared++; }
来源：http://pax.yongpay.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://scs.tianlin.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://obd.xingfuxueyuan.xyz

C#:   lock (gate) { shared++; }
来源：http://tuj.sysykeji.top

[O04] 定义异步函数并等待
来源：http://nfa.ydzc1.top

Py:   async def f():⏎    await g()
来源：http://whk.sweek.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nng.hesvh.cn

JS:   async function f() { await g(); }
来源：http://akj.shanyushiyangtech.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zcl.dianchejie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nzi.yj202588.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dff.zhongyouzk.top

Ruby: # 用 Fiber 或 async gem
来源：http://krc.gotoacloud.top

C#:   async Task F() { await G(); }
来源：http://cpr.shzxlz.cn

[O05] 并发执行并等待全部完成
来源：http://riu.cucudq.cn

Py:   asyncio.gather(*tasks)
来源：http://svx.cashguo.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wvj.cashguo.top

JS:   await Promise.all(tasks)
来源：http://dnx.jyoumei.cn

TS:   await Promise.all(tasks)
来源：http://wme.zhixingplan.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lfp.cucudq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://crn.jianghu66.top

Ruby: threads.map(&:join)
来源：http://jix.yonumen.top

C#:   await Task.WhenAll(t1, t2)
来源：http://usm.jiagoushi.top

[O06] 使用进程池
来源：http://ywd.hywenlv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hxd.chenjidiqi.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://agm.aizwys.cn

JS:   // child_process / cluster 模块
来源：http://dre.andypj.xyz

TS:   // child_process / cluster 模块
来源：http://cyq.gotoacloud.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pkg.chenlongwang.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ugg.yj202588.top

Ruby: // fork 块
来源：http://jae.hammf.cn

C#:   Parallel.For
来源：http://ptc.hywenlv.cn

================================================================================
来源：http://gfc.shanyushiyangkeji.top

P. 常用工具函数
来源：http://sho.zhixingplan.top

================================================================================
来源：http://vwr.yvedp.cn

[P01] 生成 UUID
来源：http://itf.sjlbkw.cn

Py:   str(uuid.uuid4())
来源：http://jqn.zhengqikj.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lyo.vehdjk.com

JS:   crypto.randomUUID()
来源：http://nxq.cucudq.cn

TS:   crypto.randomUUID()
来源：http://szh.zhiwuduotai.top

Java: UUID.randomUUID().toString()
来源：http://zyu.yangfankeji.com

Go:   // 用 github.com/google/uuid
来源：http://dur.zhiwuduotai.top

Ruby: SecureRandom.uuid
来源：http://tvu.yanxiufei.cn

C#:   Guid.NewGuid().ToString()
来源：http://exe.cashguo.top

[P02] MD5 / SHA256 摘要
来源：http://spt.snrcjt.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gdr.havefunace.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://biu.wangdashe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vrk.smart0.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mdl.ywan-chungtsiang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://aco.guowangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qwg.hcnkem.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ydv.nanxinkj.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kkd.yanxiufei.cn

[P03] 生成短随机字符串
来源：http://wtd.guannengcc.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rva.yanxiufei.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uit.snrcjt.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://civ.meibo888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://abf.chenlongwang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jzz.zhijiandao.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://trl.fanxiaobao.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://oiy.ybcxt.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://obi.yuxming.cn

[P04] 求长度
来源：http://way.snrcjt.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zcz.shanyushiyangtech.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://djg.epnwcf.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ncs.jqgfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kwq.jinqigfzy.top

Java: list.size();  map.size();  s.length()
来源：http://bdk.havefunace.top

Go:   len(arr);  len(m)
来源：http://cnr.hesvh.cn

Ruby: x.length;  x.size
来源：http://mjo.fehbvm.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://dcx.hesvh.cn

[P05] 判断两个对象内容是否相等
来源：http://ysn.gzhubu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://gla.ywan-chungtsiang.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gqn.wangshuangyany.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nar.aizwys.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xag.jinyuanbaomall.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vqu.fzhhl.top

Go:   reflect.DeepEqual(a, b)
来源：http://apt.gaohongyu789.top

Ruby: a == b
来源：http://azt.xziqi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vgb.shzxlz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bff.daria6918.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sux.jinghuilouyu.cn

PHP:  if (empty($x)) {}
来源：http://akc.guowangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oqu.52xcode.cn

TS:   if (x == null) {}
来源：http://pjh.shanyushiyangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://yvv.guannengcc.top

Go:   if x == nil {}
来源：http://ojb.c1oappe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jmm.ydzc1.top

C#:   if (x is null) {}
来源：http://bul.ybcxt.top

[P07] 防抖与节流
来源：http://lna.pycfn.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bgb.zdbjq.cn

PHP:  // 手写时间戳比较
来源：http://kbs.snrcjt.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gie.tianlin.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://grp.hfpthk.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://izj.nanxinkj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wbc.zdqjudy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zdg.hcnkem.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://snb.epnwcf.com

[P08] 处理浮点精度问题
来源：http://fyz.yj20258.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ifp.jinqigufen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nra.dianchejie.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jbx.jinyuanbaomall.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cic.yuxming.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hof.fktsv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qlz.xziqi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://eiq.hfpthk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eqj.jyoumei.cn

================================================================================
来源：http://bhp.tanke756.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kif.yongpay.top

================================================================================
来源：http://bog.zhiwuduotai.top

[Q01] 创建表
来源：http://iqb.birdmap.top

CREATE TABLE users (
来源：http://bnw.xinyue.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hrf.zycfv.cn

name VARCHAR(50) NOT NULL,
来源：http://uov.yongpay.top

email VARCHAR(100) UNIQUE,
来源：http://eyr.shangyingyoupin.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qys.vqdsnc.cn

);
来源：http://jbj.hongshengwenyu.top

[Q02] 创建带外键的表
来源：http://hbx.guowangkeji.top

CREATE TABLE orders (
来源：http://wee.xinyue.icu

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kip.hysaishi.cn

user_id INT NOT NULL,
来源：http://uch.jianghu66.top

amount DECIMAL(10, 2),
来源：http://rur.cdnleiting.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nii.jyoumei.cn

);
来源：http://hkm.yj20258.top

[Q03] 增加列
来源：http://gvl.tian-w.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://egc.sjlbkw.cn

[Q04] 修改列类型
来源：http://jgf.bbcook.cn


<!-- 参考信息 -->