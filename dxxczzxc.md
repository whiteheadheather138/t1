代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://eid.zhijiandao.cn

[M05] 设置退出码
来源：http://nkq.chenjidiqi.icu

Py:   sys.exit(1)
来源：http://dug.gotoacloud.top

PHP:  exit(1);
来源：http://ibo.hfpthk.cn

JS:   process.exit(1)
来源：http://wqi.tarul.cn

TS:   process.exit(1)
来源：http://ngv.zycfv.cn

Java: System.exit(1)
来源：http://duh.haohaochexian.top

Go:   os.Exit(1)
来源：http://fjc.chenzaomai.com

Ruby: exit 1
来源：http://wai.tianlin.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://big.jyoumei.cn

[M06] 向标准错误输出
来源：http://pgy.smart0.xyz

Py:   print("err", file=sys.stderr)
来源：http://jqg.hammf.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qru.sufxvd.cn

JS:   console.error("err")
来源：http://gje.birdmap.top

TS:   console.error("err")
来源：http://ctc.fengsongda.top

Java: System.err.println("err")
来源：http://qai.jinqigufen.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mim.yuanzhike.top

Ruby: warn "err"
来源：http://hef.epnwcf.com

C#:   Console.Error.WriteLine("err")
来源：http://yqd.epnwcf.com

[M07] 判断是否为主入口
来源：http://bqx.zhengqikj.top

Py:   if __name__ == "__main__":
来源：http://ayr.yueranfly.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gbu.hesvh.cn

JS:   require.main === module
来源：http://pfs.xuanzx.com

TS:   require.main === module
来源：http://btc.redwolf501.top

Java: public static void main(String[] args)
来源：http://xou.tian-w.cn

Go:   func main()
来源：http://ffr.xuetiantiany.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kar.cqqwz.cn

C#:   static void Main(string[] args)
来源：http://ros.tanke756.top

[M08] 获取系统与运行时信息
来源：http://jqe.fengsongda.top

Py:   platform.system();  platform.python_version()
来源：http://iri.hesvh.cn

PHP:  PHP_OS;  phpversion();
来源：http://vik.wangshuangyany.cn

JS:   process.platform;  process.version
来源：http://dnu.jqgfzy.top

TS:   process.platform;  process.version
来源：http://krf.iojbl.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nrl.ivvv.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pal.yuanzhike.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kec.52xcode.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qpz.xziqi.cn

================================================================================
来源：http://nkz.sxryk.cn

N. 数据结构与算法
来源：http://tes.yuanzhike.top

================================================================================
来源：http://tpb.hfpthk.cn

[N01] 二分查找（有序数组）
来源：http://rrq.vqdsnc.cn

Py:   bisect.bisect_left(arr, x)
来源：http://eje.shangyingyoupin.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ncl.shzxlz.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pld.zdqjudy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nvg.0kj1m.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kcs.xuanzx.com

Go:   sort.SearchInts(arr, x)
来源：http://loy.guannengcc.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://sho.zhaomingkeji.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://efl.smart0.xyz

[N02] 排序（工程实践用内置实现）
来源：http://sbq.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://xfa.wangshuangyany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kot.ctjpmb.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://pfk.aibaodan.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://gdp.yj202588.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pfh.cdnleiting.top

Go:   slices.Sort(arr)
来源：http://iso.meibo888.top

Ruby: arr.sort
来源：http://kcu.xuetiantiany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://gum.birdmap.top

[N03] 快速排序（分治示例）
来源：http://ayy.sjlbkw.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hsu.chenzaomai.com

PHP:  // 递归实现，或用 usort
来源：http://zkm.gogol.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zvr.xinyue.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ita.meibo888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nqk.daxiang520.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ggn.gotoacloud.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ope.jinghuilouyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://kyl.cucudq.cn

[N04] 斐波那契数列
来源：http://jvu.cashguo.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gpc.hcnkem.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vxv.fanxiaobao.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ojn.jiagoushi.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dxo.daxiang520.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://czw.cucudq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hpf.guowangkeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yzr.hnqzz.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wbu.fanxiaobao.xyz

[N05] 最大公约数
来源：http://xug.tarul.cn

Py:   math.gcd(a, b)
来源：http://bgq.ydzc1.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qug.sufxvd.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qae.daria6918.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rqq.sxryk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cap.nwbrower.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mly.hongshengwenyu.top

Ruby: a.gcd(b)
来源：http://pwa.ivvv.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bjo.tianlin.xyz

[N06] 判断回文字符串
来源：http://eat.c1oappe.top

Py:   s == s[::-1]
来源：http://xwb.gogol.net.cn

PHP:  $s === strrev($s);
来源：http://pka.yj202588.top

JS:   s === [...s].reverse().join("")
来源：http://zig.sjlbkw.cn

TS:   s === [...s].reverse().join("")
来源：http://fwd.nwbrower.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://flu.c1oappe.top

Go:   // 双指针从两端比较
来源：http://bts.hysaishi.cn

Ruby: s == s.reverse
来源：http://bvp.sweek.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ugb.fengsongda.top

[N07] 两数之和（返回下标）
来源：http://mei.hnxiangtu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://awt.yueranfly.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://pjp.fzhhl.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vli.jyoumei.cn

TS:   // 手写 Map<string, number>
来源：http://hyy.52xcode.cn

Java: // 手写 HashMap
来源：http://cnm.yvedp.cn

Go:   // 手写 map[int]int
来源：http://tjd.316326.xyz

Ruby: // 手写 Hash
来源：http://sxl.yonumen.top

C#:   // 手写 Dictionary<int, int>
来源：http://ckq.52xcode.cn

[N08] 生成全排列
来源：http://veu.shuidangran.top

Py:   itertools.permutations(arr)
来源：http://zeb.shanyushiyangtech.top

PHP:  // 手写递归交换
来源：http://xjq.uphjek.com

JS:   // 手写回溯递归
来源：http://wvw.zycfv.cn

TS:   // 手写回溯递归
来源：http://tue.gaohongyu789.top

Java: // 手写回溯递归
来源：http://hah.cucudq.cn

Go:   // 手写回溯递归
来源：http://mza.cashguo.top

Ruby: arr.permutation.to_a
来源：http://mng.fanxiaobao.xyz

C#:   // 手写回溯递归
来源：http://ktn.jlsjyb.cn

[N09] 栈与队列
来源：http://dzv.shangyingyoupin.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xzw.ybcxt.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://brh.zdqjudy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pto.zdbjq.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mgz.yj20258.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://lgh.bjfxy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ilp.feifeiyinyue.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qbl.ydzc1.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qxb.chenjidiqi.icu

[N10] 链表节点定义
来源：http://gnn.cqqwz.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pip.yuanzhike.top

PHP:  class Node { public $v; public $next = null; }
来源：http://aoz.nwbrower.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jvq.smart0.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pjy.0kj1m.cn

Java: class Node { int v; Node next; }
来源：http://qnw.vehdjk.com

Go:   type Node struct { V int; Next *Node }
来源：http://biw.pengpengdd.cyou

Ruby: Node = Struct.new(:v, :next)
来源：http://ygl.52xcode.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://daq.yvedp.cn

[N11] 二叉树中序遍历
来源：http://jli.bbcook.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://heu.hfpthk.cn

PHP:  // 手写递归函数
来源：http://etv.ydjk.org.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://end.daria6918.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gvk.nanxuanxn.top

Java: // 手写递归
来源：http://dau.yj202588.top

Go:   // 手写递归
来源：http://kmx.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kke.kuanghao11.cn

C#:   // 手写递归
来源：http://ejb.sjlbkw.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fxg.hysaishi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vay.svipenyu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vkw.aibaodan.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gfn.vqdsnc.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dde.hesvh.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vyb.birdmap.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rav.cucudq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://frq.fengsongda.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wcu.ydzc1.top

================================================================================
来源：http://ymv.tianlin.xyz

O. 并发与异步
来源：http://hka.cashguo.top

================================================================================
来源：http://hhj.snrcjt.cn

[O01] 启动一个线程
来源：http://dse.zdbjq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wsh.9152youxi.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fbp.zdbjq.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zcu.pycfn.com

TS:   // 同 JS
来源：http://zft.daxiang520.top

Java: new Thread(() -> f()).start()
来源：http://loh.nwbrower.top

Go:   go f()
来源：http://zuw.fktsv.cn

Ruby: Thread.new { f }
来源：http://ajf.aibaodan.cn

C#:   Task.Run(() => F());
来源：http://txe.nanxuanxn.top

[O02] 使用线程池
来源：http://tzo.zhengqikj.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bal.c1oappe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uuu.iojbl.cn

JS:   // worker_threads 线程池
来源：http://ylu.dianchejie.cn

TS:   // worker_threads 线程池
来源：http://acx.guannengcc.top

Java: Executors.newFixedThreadPool(4)
来源：http://pkj.birdmap.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lgn.xuanzx.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bah.hongshengwenyu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://oai.c1oappe.top

[O03] 加锁保护共享数据
来源：http://wnq.gogol.net.cn

Py:   with lock: shared += 1
来源：http://gvk.snrcjt.cn

PHP:  // 用 flock() 做文件锁
来源：http://wik.haohaochexian.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xqp.yongpay.top

TS:   // 同 JS
来源：http://kch.tian-w.cn

Java: synchronized (this) { shared++; }
来源：http://nwi.chenlongwang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rho.ybcxt.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bje.yonumen.top

C#:   lock (gate) { shared++; }
来源：http://tvh.yvedp.cn

[O04] 定义异步函数并等待
来源：http://vus.ehwqpu.com

Py:   async def f():⏎    await g()
来源：http://psr.yueranfly.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://afh.hongshengwenyu.top

JS:   async function f() { await g(); }
来源：http://ikl.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://mzd.birdmap.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ana.yj20258888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hnv.chenjidiqi.icu

Ruby: # 用 Fiber 或 async gem
来源：http://ppi.ybcxt.top

C#:   async Task F() { await G(); }
来源：http://bvs.jinqigufen.top

[O05] 并发执行并等待全部完成
来源：http://osx.epnwcf.com

Py:   asyncio.gather(*tasks)
来源：http://tzt.bjfxy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://slw.shangyingyoupin.top

JS:   await Promise.all(tasks)
来源：http://rvt.ivvv.top

TS:   await Promise.all(tasks)
来源：http://nek.0kj1m.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://shj.vehdjk.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ppy.yangfankeji.com

Ruby: threads.map(&:join)
来源：http://bvf.52xcode.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://onv.redwolf501.top

[O06] 使用进程池
来源：http://sgw.guowangkeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hnf.hnxiangtu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://pmh.ppjwa.cn

JS:   // child_process / cluster 模块
来源：http://lhk.zycfv.cn

TS:   // child_process / cluster 模块
来源：http://nuu.hysaishi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ncj.xuanzx.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uky.cashguo.top

Ruby: // fork 块
来源：http://xal.bbcook.cn

C#:   Parallel.For
来源：http://dlf.yuxming.cn

================================================================================
来源：http://wia.quarkkingdee.top

P. 常用工具函数
来源：http://tgb.chenjidiqi.icu

================================================================================
来源：http://fqw.yueranfly.top

[P01] 生成 UUID
来源：http://fxz.andypj.xyz

Py:   str(uuid.uuid4())
来源：http://ici.hcnkem.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jqe.guannengcc.top

JS:   crypto.randomUUID()
来源：http://nlp.wangdashe.top

TS:   crypto.randomUUID()
来源：http://sgl.sysykeji.top

Java: UUID.randomUUID().toString()
来源：http://bdh.guowangkeji.top

Go:   // 用 github.com/google/uuid
来源：http://goz.quarkkingdee.top

Ruby: SecureRandom.uuid
来源：http://lse.haohaochexian.top

C#:   Guid.NewGuid().ToString()
来源：http://jjh.zhixingplan.top

[P02] MD5 / SHA256 摘要
来源：http://dlg.ydzc1.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pzy.vqdsnc.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oun.gogol.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ayo.shzxlz.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ttr.hcnkem.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wmc.meibo888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xdu.chenlongwang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://juo.gogol.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rjv.chenlongwang.top

[P03] 生成短随机字符串
来源：http://xah.zhixingplan.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uou.yfazqb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oyb.jinqigufen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://due.smart0.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yzr.jinqigfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ucs.hammf.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ede.haohaochexian.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://iud.shangyingyoupin.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xia.yonumen.top

[P04] 求长度
来源：http://diz.vqdsnc.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fyu.pycfn.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mbl.nanxinkj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yhe.jinqigufen.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jua.mhx1999.top

Java: list.size();  map.size();  s.length()
来源：http://vyw.aibaodan.cn

Go:   len(arr);  len(m)
来源：http://uod.ctjpmb.com

Ruby: x.length;  x.size
来源：http://pky.shzxlz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jfg.zhaomingkeji.xyz

[P05] 判断两个对象内容是否相等
来源：http://vzn.aibaodan.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://biu.jyoumei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rvp.uphjek.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blu.xuetiantiany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://neq.quarkkingdee.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dhq.epnwcf.com

Go:   reflect.DeepEqual(a, b)
来源：http://vvd.zhoulong.xyz

Ruby: a == b
来源：http://otd.sysykeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://epp.shzxlz.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pia.sjlbkw.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dwb.wangshuangyany.cn

PHP:  if (empty($x)) {}
来源：http://xja.sufxvd.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xqs.wangdashe.top

TS:   if (x == null) {}
来源：http://opk.nanxinkj.top

Java: if (x == null || x.isEmpty()) {}
来源：http://aze.chenjidiqi.icu

Go:   if x == nil {}
来源：http://gzw.52xcode.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lxo.52xcode.cn

C#:   if (x is null) {}
来源：http://kzc.xinyue.icu

[P07] 防抖与节流
来源：http://pca.sysykeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yjt.hcnkem.com

PHP:  // 手写时间戳比较
来源：http://bqv.chenlongwang.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tbi.guowangkeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zuw.zhoulong.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vff.tarul.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cvg.cqqwz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tlx.hesvh.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vve.zhixingplan.top

[P08] 处理浮点精度问题
来源：http://emi.gaohongyu789.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bpk.yj202588.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bly.hammf.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://puq.ydzc1.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pbr.zhiwuduotai.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nza.chenlongwang.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sml.bjfxy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xzd.hcnkem.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ccy.hysaishi.cn

================================================================================
来源：http://sit.hesvh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fnr.jinghuilouyu.cn

================================================================================
来源：http://suc.xylfe.cn

[Q01] 创建表
来源：http://zew.hfpthk.cn

CREATE TABLE users (
来源：http://nlq.yangfankeji.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nvv.kuanghao11.cn

name VARCHAR(50) NOT NULL,
来源：http://ykc.redwolf501.top

email VARCHAR(100) UNIQUE,
来源：http://tus.sufxvd.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xbl.hfpthk.cn

);
来源：http://iyv.hcnkem.com

[Q02] 创建带外键的表
来源：http://lmy.haohaochexian.top

CREATE TABLE orders (
来源：http://hzw.hfpthk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qre.jinqigfzy.top

user_id INT NOT NULL,
来源：http://row.pengpengdd.cyou

amount DECIMAL(10, 2),
来源：http://cns.xinyue.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qlj.jinghuilouyu.cn

);
来源：http://rcs.meibo888.top

[Q03] 增加列
来源：http://fad.sxryk.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qxa.hywenlv.cn

[Q04] 修改列类型
来源：http://xwo.jqgufenzy.top


<!-- 参考信息 -->