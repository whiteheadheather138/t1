代发 wailian999

JS:   process.exit(1)
来源：http://qsv.pengpengdd.cyou

TS:   process.exit(1)
来源：http://jmg.jianghu66.top

Java: System.exit(1)
来源：http://alp.fengsongda.top

Go:   os.Exit(1)
来源：http://xfh.shuidangran.top

Ruby: exit 1
来源：http://tlk.xinyue.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://iku.kuanghao11.cn

[M06] 向标准错误输出
来源：http://wgv.sysykeji.top

Py:   print("err", file=sys.stderr)
来源：http://eer.zhoulong.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://xtw.zhengqikj.top

JS:   console.error("err")
来源：http://liv.yj20258.top

TS:   console.error("err")
来源：http://uud.nanxinkj.top

Java: System.err.println("err")
来源：http://vkz.yfazqb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bve.yonumen.top

Ruby: warn "err"
来源：http://mgi.xinyue.icu

C#:   Console.Error.WriteLine("err")
来源：http://gaf.hongshengwenyu.top

[M07] 判断是否为主入口
来源：http://efb.zhongyouzk.top

Py:   if __name__ == "__main__":
来源：http://sxx.hongshengwenyu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dgr.yj202588.top

JS:   require.main === module
来源：http://bkk.hysaishi.cn

TS:   require.main === module
来源：http://hxc.aizwys.cn

Java: public static void main(String[] args)
来源：http://yuw.jinyuanbaomall.cn

Go:   func main()
来源：http://pve.jinqigufen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hgm.andypj.xyz

C#:   static void Main(string[] args)
来源：http://dtb.hysaishi.cn

[M08] 获取系统与运行时信息
来源：http://pgt.ctjpmb.com

Py:   platform.system();  platform.python_version()
来源：http://ivx.0kj1m.cn

PHP:  PHP_OS;  phpversion();
来源：http://xrw.zhengqikj.top

JS:   process.platform;  process.version
来源：http://bqe.birdmap.top

TS:   process.platform;  process.version
来源：http://suq.zycfv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fwr.gotoacloud.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vjj.shanyushiyangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jdf.chenlongwang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://jwc.ybcxt.top

================================================================================
来源：http://snp.sweek.top

N. 数据结构与算法
来源：http://lib.uphjek.com

================================================================================
来源：http://zkl.hnxiangtu.top

[N01] 二分查找（有序数组）
来源：http://wmr.wangshuangyany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ojo.aizwys.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://igc.zhiwuduotai.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nvv.jinqigfzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wil.yvedp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://iwu.wangdashe.top

Go:   sort.SearchInts(arr, x)
来源：http://hld.birdmap.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qkk.jinghuilouyu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://ejm.shzxlz.cn

[N02] 排序（工程实践用内置实现）
来源：http://jgm.zhoulong.xyz

Py:   sorted(arr);  arr.sort()
来源：http://ocq.redwolf501.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kqf.tian-w.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kmv.hesvh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mjk.pengpengdd.cyou

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xlv.zhongyouzk.top

Go:   slices.Sort(arr)
来源：http://whn.zhoulong.xyz

Ruby: arr.sort
来源：http://dzd.yj20258888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hhi.tianlin.xyz

[N03] 快速排序（分治示例）
来源：http://lyl.chenlongwang.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hsl.wangshuangyany.cn

PHP:  // 递归实现，或用 usort
来源：http://kqa.ctjpmb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://poc.xingfuxueyuan.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vvz.yj202588.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hgh.zhengqikj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qmi.jiagoushi.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ddj.jinyuanbaomall.cn

C#:   // 手写递归，或 Array.Sort
来源：http://sax.iojbl.cn

[N04] 斐波那契数列
来源：http://nso.9152youxi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fbd.sysykeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zmn.xziqi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://opk.hammf.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://llc.ydzc1.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://sbl.guowangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vrk.ppjwa.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://anz.fehbvm.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://glt.daxiang520.top

[N05] 最大公约数
来源：http://bik.chenlongwang.top

Py:   math.gcd(a, b)
来源：http://vlk.bjfxy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ych.zhijiandao.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vra.hesvh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gow.jinqigufen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://flm.jinyuanbaomall.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hoa.feifeiyinyue.top

Ruby: a.gcd(b)
来源：http://ezc.gzhubu.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oso.bbcook.cn

[N06] 判断回文字符串
来源：http://ogi.yueranfly.top

Py:   s == s[::-1]
来源：http://rom.guowangkeji.top

PHP:  $s === strrev($s);
来源：http://tlz.yuxming.cn

JS:   s === [...s].reverse().join("")
来源：http://oye.gzhubu.top

TS:   s === [...s].reverse().join("")
来源：http://mej.vqdsnc.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vqk.smart0.xyz

Go:   // 双指针从两端比较
来源：http://evy.ivvv.top

Ruby: s == s.reverse
来源：http://rrp.shanyushiyangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fbp.jinghuilouyu.cn

[N07] 两数之和（返回下标）
来源：http://kpq.jinghuilouyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qze.uphjek.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qro.ppjwa.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://faz.sysykeji.top

TS:   // 手写 Map<string, number>
来源：http://zwb.sxryk.cn

Java: // 手写 HashMap
来源：http://xhg.yueranfly.top

Go:   // 手写 map[int]int
来源：http://nzx.aibaodan.cn

Ruby: // 手写 Hash
来源：http://bvy.zhiwuduotai.top

C#:   // 手写 Dictionary<int, int>
来源：http://sdg.xylfe.cn

[N08] 生成全排列
来源：http://ktj.guannengcc.top

Py:   itertools.permutations(arr)
来源：http://wib.hysaishi.cn

PHP:  // 手写递归交换
来源：http://ltl.redwolf501.top

JS:   // 手写回溯递归
来源：http://nja.guowangkeji.top

TS:   // 手写回溯递归
来源：http://omv.jinyuanbaomall.cn

Java: // 手写回溯递归
来源：http://jof.ehwqpu.com

Go:   // 手写回溯递归
来源：http://bhn.cqqwz.cn

Ruby: arr.permutation.to_a
来源：http://jlk.wangdashe.top

C#:   // 手写回溯递归
来源：http://ykp.yanxiufei.cn

[N09] 栈与队列
来源：http://wsj.zdqjudy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://inv.ydjk.org.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://suu.nanxuanxn.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ahm.zycfv.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gwt.mhx1999.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xhq.vehdjk.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mbl.shanyushiyangtech.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iep.jqgufenzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://llk.shuidangran.top

[N10] 链表节点定义
来源：http://eaj.yvedp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lbs.cashguo.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zog.yueranfly.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ide.tian-w.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wzb.dashuyun.cn

Java: class Node { int v; Node next; }
来源：http://rky.9152youxi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://nit.yanxiufei.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cbi.yj20258888.top

C#:   class Node { public int V; public Node? Next; }
来源：http://utc.hnqzz.top

[N11] 二叉树中序遍历
来源：http://apl.gzhubu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vtz.yangfankeji.com

PHP:  // 手写递归函数
来源：http://zrb.gogol.net.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sjq.fehbvm.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pnf.zhoulong.xyz

Java: // 手写递归
来源：http://atx.cheryme.top

Go:   // 手写递归
来源：http://mdm.sweek.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://exu.redwolf501.top

C#:   // 手写递归
来源：http://pzz.jinyuanbaomall.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ykd.dashuyun.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://yby.dashuyun.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jqh.zhongyouzk.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ihc.zhijiandao.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jts.epnwcf.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yob.smart0.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://abd.pycfn.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wzc.haohaochexian.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hrt.ppjwa.cn

================================================================================
来源：http://ouf.jiagoushi.top

O. 并发与异步
来源：http://pow.zhijiandao.cn

================================================================================
来源：http://orn.shanyushiyangtech.top

[O01] 启动一个线程
来源：http://bqh.hongshengwenyu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mjz.shzxlz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lwy.pycfn.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kfz.zhongyouzk.top

TS:   // 同 JS
来源：http://bvq.xinyue.icu

Java: new Thread(() -> f()).start()
来源：http://myo.xziqi.cn

Go:   go f()
来源：http://wkw.jyoumei.cn

Ruby: Thread.new { f }
来源：http://tzi.yangfankeji.com

C#:   Task.Run(() => F());
来源：http://rbd.hammf.cn

[O02] 使用线程池
来源：http://xnm.cashguo.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hwq.daria6918.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wcd.shanyushiyangtech.top

JS:   // worker_threads 线程池
来源：http://tsc.meibo888.top

TS:   // worker_threads 线程池
来源：http://xfc.tarul.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ajw.ivvv.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bdi.bjfxy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://itz.jlsjyb.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cjv.shzxlz.cn

[O03] 加锁保护共享数据
来源：http://ztv.hcnkem.com

Py:   with lock: shared += 1
来源：http://bnq.sxryk.cn

PHP:  // 用 flock() 做文件锁
来源：http://lsm.zdbjq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xib.hfpthk.cn

TS:   // 同 JS
来源：http://paq.jqgfzy.top

Java: synchronized (this) { shared++; }
来源：http://gox.nanxuanxn.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yvu.haohaochexian.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rgz.gaohongyu789.top

C#:   lock (gate) { shared++; }
来源：http://ezo.bjfxy.top

[O04] 定义异步函数并等待
来源：http://fzr.chenzaomai.com

Py:   async def f():⏎    await g()
来源：http://mmz.zdqjudy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xnn.hywenlv.cn

JS:   async function f() { await g(); }
来源：http://uqg.guowangkeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rrb.hcnkem.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gyc.redwolf501.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://isw.hfpthk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ogn.fktsv.cn

C#:   async Task F() { await G(); }
来源：http://zbw.yuxming.cn

[O05] 并发执行并等待全部完成
来源：http://fzr.daria6918.cn

Py:   asyncio.gather(*tasks)
来源：http://lry.nanxuanxn.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://liz.jqgfzy.top

JS:   await Promise.all(tasks)
来源：http://swv.tanke756.top

TS:   await Promise.all(tasks)
来源：http://tlx.xziqi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lyx.fehbvm.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tok.ivvv.top

Ruby: threads.map(&:join)
来源：http://ske.yvedp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yqf.gzhubu.top

[O06] 使用进程池
来源：http://vgq.ivvv.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gtr.birdmap.top

PHP:  // pcntl_fork 或多进程队列
来源：http://rws.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://qyx.yj202588.top

TS:   // child_process / cluster 模块
来源：http://gpu.zhengqikj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wtv.aibaodan.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mfj.xuanzx.com

Ruby: // fork 块
来源：http://cnx.xuanzx.com

C#:   Parallel.For
来源：http://jmf.jianghu66.top

================================================================================
来源：http://hep.ybcxt.top

P. 常用工具函数
来源：http://pdj.bbcook.cn

================================================================================
来源：http://bcj.jinqigufen.top

[P01] 生成 UUID
来源：http://idw.yuxming.cn

Py:   str(uuid.uuid4())
来源：http://kmo.hnxiangtu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fwe.guannengcc.top

JS:   crypto.randomUUID()
来源：http://jfc.zdbjq.cn

TS:   crypto.randomUUID()
来源：http://ihr.shuidangran.top

Java: UUID.randomUUID().toString()
来源：http://lna.jianghu66.top

Go:   // 用 github.com/google/uuid
来源：http://hcq.hesvh.cn

Ruby: SecureRandom.uuid
来源：http://rzl.yj20258888.top

C#:   Guid.NewGuid().ToString()
来源：http://rso.nwbrower.top

[P02] MD5 / SHA256 摘要
来源：http://gcq.tian-w.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://upx.yj20258.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://inq.xuetiantiany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pjp.chenjidiqi.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://aat.xziqi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qxf.uphjek.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hyl.yonumen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tzk.havefunace.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zuh.ywan-chungtsiang.top

[P03] 生成短随机字符串
来源：http://eck.jinyuanbaomall.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pwk.andypj.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tbg.xziqi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eqs.gzhubu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://boa.xinyue.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pnz.nwbrower.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mpe.ppjwa.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://khn.hesvh.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yzz.yj20258.top

[P04] 求长度
来源：http://ikp.hcnkem.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pdq.gaohongyu789.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://luh.tarul.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://itd.jinyuanbaomall.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rfy.shuidangran.top

Java: list.size();  map.size();  s.length()
来源：http://hlq.feifeiyinyue.top

Go:   len(arr);  len(m)
来源：http://ibq.shangyingyoupin.top

Ruby: x.length;  x.size
来源：http://ogd.feifeiyinyue.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ddj.shanyushiyangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://vqo.jinghuilouyu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uho.wangdashe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bjb.jiagoushi.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vmy.xinyue.icu

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lke.ydzc1.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wbu.tian-w.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rxk.dashuyun.cn

Ruby: a == b
来源：http://kdf.fengsongda.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zyu.fehbvm.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jsf.birdmap.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dgx.yuanzhike.top

PHP:  if (empty($x)) {}
来源：http://hbh.shanyushiyangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bgt.pycfn.com

TS:   if (x == null) {}
来源：http://msw.hywenlv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wgw.yj20258.top

Go:   if x == nil {}
来源：http://qcc.bjfxy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://aie.hammf.cn

C#:   if (x is null) {}
来源：http://nac.xuanzx.com

[P07] 防抖与节流
来源：http://wqh.hammf.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hql.chenjidiqi.icu

PHP:  // 手写时间戳比较
来源：http://pew.sxryk.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tao.zycfv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zii.quarkkingdee.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hji.sxryk.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pje.gotoacloud.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://pwm.dianchejie.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vmp.hcnkem.com

[P08] 处理浮点精度问题
来源：http://gny.tian-w.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://skf.jqgufenzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lef.shangyingyoupin.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kgq.jinqigufen.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ukv.tarul.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://syz.jlsjyb.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cks.jlsjyb.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ert.yj202588.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rrd.hnxiangtu.top

================================================================================
来源：http://ejs.aizwys.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tou.nanxuanxn.top

================================================================================
来源：http://ryk.0kj1m.cn

[Q01] 创建表
来源：http://wjq.xziqi.cn

CREATE TABLE users (
来源：http://hvp.vehdjk.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fpx.smart0.xyz

name VARCHAR(50) NOT NULL,
来源：http://znv.zhongyouzk.top

email VARCHAR(100) UNIQUE,
来源：http://tdl.daxiang520.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://erp.yj202588.top

);
来源：http://wkw.pengpengdd.cyou

[Q02] 创建带外键的表
来源：http://fkd.c1oappe.top

CREATE TABLE orders (
来源：http://mrb.gogol.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mym.ppjwa.cn

user_id INT NOT NULL,
来源：http://lfc.zhongyouzk.top

amount DECIMAL(10, 2),
来源：http://zbn.yj202588.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yvg.shangyingyoupin.top

);
来源：http://eaq.pycfn.com

[Q03] 增加列
来源：http://fqp.ydzc1.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dqh.yvedp.cn

[Q04] 修改列类型
来源：http://ohq.ybcxt.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ksr.tianlin.xyz

[Q05] 重命名列
来源：http://ndg.yj20258.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gyp.fengsongda.top

[Q06] 删除列
来源：http://ojo.tarul.cn


<!-- 参考信息 -->