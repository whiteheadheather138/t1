代发 wailian999

TS:   process.cwd()
来源：http://qtl.snrcjt.cn

Java: Path.of("").toAbsolutePath()
来源：http://dbz.shanyushiyangtech.top

Go:   os.Getwd()
来源：http://wmb.ivvv.top

Ruby: Dir.pwd
来源：http://han.uphjek.com

C#:   Directory.GetCurrentDirectory()
来源：http://ifa.chenjidiqi.icu

[M05] 设置退出码
来源：http://uzz.gaohongyu789.top

Py:   sys.exit(1)
来源：http://zmw.meibo888.top

PHP:  exit(1);
来源：http://zpc.quarkkingdee.top

JS:   process.exit(1)
来源：http://raf.pycfn.com

TS:   process.exit(1)
来源：http://qyt.yonumen.top

Java: System.exit(1)
来源：http://elt.fengsongda.top

Go:   os.Exit(1)
来源：http://xux.jlsjyb.cn

Ruby: exit 1
来源：http://kxm.wangdashe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qte.hesvh.cn

[M06] 向标准错误输出
来源：http://sox.tanke756.top

Py:   print("err", file=sys.stderr)
来源：http://eef.ydzc1.top

PHP:  fwrite(STDERR, "err\n");
来源：http://lye.ydzc1.top

JS:   console.error("err")
来源：http://hhe.jinqigufen.top

TS:   console.error("err")
来源：http://ibp.kuanghao11.cn

Java: System.err.println("err")
来源：http://uwh.shanyushiyangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hza.hywenlv.cn

Ruby: warn "err"
来源：http://zda.yangfankeji.com

C#:   Console.Error.WriteLine("err")
来源：http://zhq.snrcjt.cn

[M07] 判断是否为主入口
来源：http://auq.fzhhl.top

Py:   if __name__ == "__main__":
来源：http://ngy.sufxvd.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://eoi.tianlin.xyz

JS:   require.main === module
来源：http://zzc.havefunace.top

TS:   require.main === module
来源：http://ajd.cashguo.top

Java: public static void main(String[] args)
来源：http://cew.kuanghao11.cn

Go:   func main()
来源：http://krz.sxryk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://grw.pengpengdd.cyou

C#:   static void Main(string[] args)
来源：http://yti.meibo888.top

[M08] 获取系统与运行时信息
来源：http://xqx.zhoulong.xyz

Py:   platform.system();  platform.python_version()
来源：http://bnc.shanyushiyangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://jsx.fzhhl.top

JS:   process.platform;  process.version
来源：http://yke.xziqi.cn

TS:   process.platform;  process.version
来源：http://ony.zhaomingkeji.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ien.fanxiaobao.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://lut.shangyingyoupin.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://htq.yfazqb.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://nar.jqgfzy.top

================================================================================
来源：http://xje.yongpay.top

N. 数据结构与算法
来源：http://itd.cheryme.top

================================================================================
来源：http://bzq.aibaodan.cn

[N01] 二分查找（有序数组）
来源：http://bkv.sufxvd.cn

Py:   bisect.bisect_left(arr, x)
来源：http://eaf.hnqzz.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://spt.xuanzx.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pbd.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fcx.zhiwuduotai.top

Java: Arrays.binarySearch(arr, x)
来源：http://nvg.yj202588.top

Go:   sort.SearchInts(arr, x)
来源：http://eaf.cdnleiting.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hby.yj20258888.top

C#:   Array.BinarySearch(arr, x)
来源：http://wyw.shuidangran.top

[N02] 排序（工程实践用内置实现）
来源：http://yaj.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://mij.jyoumei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yqs.xylfe.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dfg.xinyue.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://suu.gogol.net.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rdq.redwolf501.top

Go:   slices.Sort(arr)
来源：http://oon.tarul.cn

Ruby: arr.sort
来源：http://ffk.yanxiufei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vmm.xuetiantiany.cn

[N03] 快速排序（分治示例）
来源：http://yvg.shangyingyoupin.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qbz.fanxiaobao.xyz

PHP:  // 递归实现，或用 usort
来源：http://bzq.daxiang520.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jjo.haohaochexian.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ume.gzhubu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zdw.hywenlv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sim.zhiwuduotai.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ovi.haohaochexian.top

C#:   // 手写递归，或 Array.Sort
来源：http://trl.hnqzz.top

[N04] 斐波那契数列
来源：http://kin.xziqi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pog.gaohongyu789.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://opo.zhoulong.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ioj.hammf.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://drv.jiagoushi.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://clt.zdbjq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wdx.mhx1999.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ege.gzhubu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ubl.ivvv.top

[N05] 最大公约数
来源：http://jaz.smart0.xyz

Py:   math.gcd(a, b)
来源：http://qut.ydjk.org.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jqp.meibo888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ftm.xinyue.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cpg.nanxuanxn.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://iqj.cdnleiting.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fcg.guannengcc.top

Ruby: a.gcd(b)
来源：http://mtm.cdnleiting.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xqh.jianghu66.top

[N06] 判断回文字符串
来源：http://tct.shangyingyoupin.top

Py:   s == s[::-1]
来源：http://moo.hesvh.cn

PHP:  $s === strrev($s);
来源：http://reo.hysaishi.cn

JS:   s === [...s].reverse().join("")
来源：http://waf.meibo888.top

TS:   s === [...s].reverse().join("")
来源：http://cso.xingfuxueyuan.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pzu.tianlin.xyz

Go:   // 双指针从两端比较
来源：http://bda.wangdashe.top

Ruby: s == s.reverse
来源：http://qqb.shangyingyoupin.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ovn.316326.xyz

[N07] 两数之和（返回下标）
来源：http://jpi.hongshengwenyu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qgs.52xcode.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uwk.aizwys.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vrz.redwolf501.top

TS:   // 手写 Map<string, number>
来源：http://xpw.cdnleiting.top

Java: // 手写 HashMap
来源：http://gzu.pycfn.com

Go:   // 手写 map[int]int
来源：http://ulg.yuxming.cn

Ruby: // 手写 Hash
来源：http://ckb.zycfv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ekr.chenzaomai.com

[N08] 生成全排列
来源：http://zgv.zhiwuduotai.top

Py:   itertools.permutations(arr)
来源：http://adu.fehbvm.com

PHP:  // 手写递归交换
来源：http://bir.mhx1999.top

JS:   // 手写回溯递归
来源：http://ihh.cqqwz.cn

TS:   // 手写回溯递归
来源：http://mcw.xinyue.icu

Java: // 手写回溯递归
来源：http://fgc.mhx1999.top

Go:   // 手写回溯递归
来源：http://qsn.ctjpmb.com

Ruby: arr.permutation.to_a
来源：http://mfo.tanke756.top

C#:   // 手写回溯递归
来源：http://ghe.9152youxi.cn

[N09] 栈与队列
来源：http://kgo.bjfxy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bsq.shzxlz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ozs.hcnkem.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ckn.jianghu66.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://qii.jinqigfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://arg.jqgufenzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jqt.wangshuangyany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nto.jqgfzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zgr.cucudq.cn

[N10] 链表节点定义
来源：http://vlk.svipenyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://nnj.ehwqpu.com

PHP:  class Node { public $v; public $next = null; }
来源：http://tzm.haohaochexian.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://amv.chenzaomai.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hfh.jlsjyb.cn

Java: class Node { int v; Node next; }
来源：http://scw.havefunace.top

Go:   type Node struct { V int; Next *Node }
来源：http://fzi.9152youxi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://eir.yonumen.top

C#:   class Node { public int V; public Node? Next; }
来源：http://fdi.andypj.xyz

[N11] 二叉树中序遍历
来源：http://ydh.gotoacloud.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qtz.fehbvm.com

PHP:  // 手写递归函数
来源：http://dil.zdbjq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gel.dashuyun.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lfd.yuxming.cn

Java: // 手写递归
来源：http://byy.jinqigfzy.top

Go:   // 手写递归
来源：http://yiw.zhaomingkeji.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ukd.jqgufenzy.top

C#:   // 手写递归
来源：http://mky.ybcxt.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kyf.daxiang520.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fum.daria6918.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wfa.andypj.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://emn.fzhhl.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rdw.cdnleiting.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sdh.daxiang520.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://afn.epnwcf.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sht.meibo888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sxv.daria6918.cn

================================================================================
来源：http://dtg.tian-w.cn

O. 并发与异步
来源：http://hrk.smart0.xyz

================================================================================
来源：http://abn.nwbrower.top

[O01] 启动一个线程
来源：http://ifi.0kj1m.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fqc.redwolf501.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zgx.52xcode.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yzw.meibo888.top

TS:   // 同 JS
来源：http://auo.ctjpmb.com

Java: new Thread(() -> f()).start()
来源：http://cnm.redwolf501.top

Go:   go f()
来源：http://jmx.quarkkingdee.top

Ruby: Thread.new { f }
来源：http://uoq.xylfe.cn

C#:   Task.Run(() => F());
来源：http://mxo.ydjk.org.cn

[O02] 使用线程池
来源：http://win.jinghuilouyu.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fff.jqgufenzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://eky.jinghuilouyu.cn

JS:   // worker_threads 线程池
来源：http://vgn.hammf.cn

TS:   // worker_threads 线程池
来源：http://sbf.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://krx.cheryme.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cru.daxiang520.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eyt.dashuyun.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hln.ydjk.org.cn

[O03] 加锁保护共享数据
来源：http://acr.yangfankeji.com

Py:   with lock: shared += 1
来源：http://gqb.chenlongwang.top

PHP:  // 用 flock() 做文件锁
来源：http://tkn.xziqi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ahv.zdbjq.cn

TS:   // 同 JS
来源：http://nin.pengpengdd.cyou

Java: synchronized (this) { shared++; }
来源：http://arb.hnxiangtu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://afx.nanxinkj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ash.0kj1m.cn

C#:   lock (gate) { shared++; }
来源：http://glk.ywan-chungtsiang.top

[O04] 定义异步函数并等待
来源：http://evz.shangyingyoupin.top

Py:   async def f():⏎    await g()
来源：http://ljb.zdqjudy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wqf.nanxinkj.top

JS:   async function f() { await g(); }
来源：http://xxa.sjlbkw.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jbp.chenzaomai.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lsa.gogol.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hko.hesvh.cn

Ruby: # 用 Fiber 或 async gem
来源：http://puu.xziqi.cn

C#:   async Task F() { await G(); }
来源：http://upk.ehwqpu.com

[O05] 并发执行并等待全部完成
来源：http://lwf.zycfv.cn

Py:   asyncio.gather(*tasks)
来源：http://oes.jqgufenzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tqt.cheryme.top

JS:   await Promise.all(tasks)
来源：http://ewn.sjlbkw.cn

TS:   await Promise.all(tasks)
来源：http://idb.uphjek.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zpu.nanxinkj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xpt.yuanzhike.top

Ruby: threads.map(&:join)
来源：http://ijy.havefunace.top

C#:   await Task.WhenAll(t1, t2)
来源：http://arr.yonumen.top

[O06] 使用进程池
来源：http://cbd.c1oappe.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bwp.jiagoushi.top

PHP:  // pcntl_fork 或多进程队列
来源：http://bmu.sysykeji.top

JS:   // child_process / cluster 模块
来源：http://irm.xuetiantiany.cn

TS:   // child_process / cluster 模块
来源：http://giq.c1oappe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hyf.hfpthk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://iuk.fktsv.cn

Ruby: // fork 块
来源：http://epr.jiagoushi.top

C#:   Parallel.For
来源：http://tvz.ydjk.org.cn

================================================================================
来源：http://vwe.jinyuanbaomall.cn

P. 常用工具函数
来源：http://xyk.ywan-chungtsiang.top

================================================================================
来源：http://ehi.yfazqb.com

[P01] 生成 UUID
来源：http://txs.gogol.net.cn

Py:   str(uuid.uuid4())
来源：http://imk.sjlbkw.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ymn.daria6918.cn

JS:   crypto.randomUUID()
来源：http://ysj.guowangkeji.top

TS:   crypto.randomUUID()
来源：http://bkj.ctjpmb.com

Java: UUID.randomUUID().toString()
来源：http://plm.jinghuilouyu.cn

Go:   // 用 github.com/google/uuid
来源：http://rjq.jqgufenzy.top

Ruby: SecureRandom.uuid
来源：http://med.pycfn.com

C#:   Guid.NewGuid().ToString()
来源：http://biy.bjfxy.top

[P02] MD5 / SHA256 摘要
来源：http://yvq.fktsv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://idm.nanxinkj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://cro.yj202588.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xwq.sysykeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://icv.andypj.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dmy.fzhhl.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qee.zhijiandao.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zoe.shuidangran.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ofr.hongshengwenyu.top

[P03] 生成短随机字符串
来源：http://avb.cucudq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://efu.smart0.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ioy.epnwcf.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ieq.jinqigufen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ijr.jqgufenzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lxj.jianghu66.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cgl.hywenlv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://eux.yuanzhike.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://deu.kuanghao11.cn

[P04] 求长度
来源：http://ixj.yfazqb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sbv.shanyushiyangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bnz.vqdsnc.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ltj.yangfankeji.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://trd.cashguo.top

Java: list.size();  map.size();  s.length()
来源：http://zlx.gzhubu.top

Go:   len(arr);  len(m)
来源：http://eyd.cashguo.top

Ruby: x.length;  x.size
来源：http://qha.jyoumei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ewf.jqgfzy.top

[P05] 判断两个对象内容是否相等
来源：http://cuv.guowangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://qxj.pengpengdd.cyou

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://srs.chenzaomai.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vtr.ydjk.org.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vwq.316326.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hpc.shuidangran.top

Go:   reflect.DeepEqual(a, b)
来源：http://unb.andypj.xyz

Ruby: a == b
来源：http://vqw.hammf.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cmh.nanxinkj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mjy.jinqigfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dph.feifeiyinyue.top

PHP:  if (empty($x)) {}
来源：http://cod.fktsv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oji.fzhhl.top

TS:   if (x == null) {}
来源：http://ltd.xinyue.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://bfu.zhijiandao.cn

Go:   if x == nil {}
来源：http://fgk.gotoacloud.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://shb.zhongyouzk.top

C#:   if (x is null) {}
来源：http://xeb.tarul.cn

[P07] 防抖与节流
来源：http://fms.andypj.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ojg.zhengqikj.top

PHP:  // 手写时间戳比较
来源：http://cjw.tarul.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dwy.aizwys.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tcj.yj20258888.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vvb.vqdsnc.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lib.shangyingyoupin.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://frn.shanyushiyangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lls.yonumen.top

[P08] 处理浮点精度问题
来源：http://svo.jianghu66.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mqg.yangfankeji.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ulq.yanxiufei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rtk.ydzc1.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tvw.hywenlv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sih.haohaochexian.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gdk.wangshuangyany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cfw.hammf.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://yxq.aibaodan.cn

================================================================================
来源：http://zob.yuxming.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xxs.dianchejie.cn

================================================================================
来源：http://jxb.vehdjk.com

[Q01] 创建表
来源：http://gng.chenjidiqi.icu

CREATE TABLE users (
来源：http://idi.sjlbkw.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://teo.zycfv.cn

name VARCHAR(50) NOT NULL,
来源：http://usf.epnwcf.com

email VARCHAR(100) UNIQUE,
来源：http://wtp.zhijiandao.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zip.zhixingplan.top

);
来源：http://ufz.fengsongda.top

[Q02] 创建带外键的表
来源：http://gch.pycfn.com

CREATE TABLE orders (
来源：http://xza.fengsongda.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cgp.shanyushiyangkeji.top

user_id INT NOT NULL,
来源：http://trb.tianlin.xyz

amount DECIMAL(10, 2),
来源：http://dvf.yangfankeji.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://onb.yuxming.cn


<!-- 参考信息 -->