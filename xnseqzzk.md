代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://uvk.hongshengwenyu.top

[M05] 设置退出码
来源：http://wur.aibaodan.cn

Py:   sys.exit(1)
来源：http://jqv.tarul.cn

PHP:  exit(1);
来源：http://uww.nwbrower.top

JS:   process.exit(1)
来源：http://tha.pengpengdd.cyou

TS:   process.exit(1)
来源：http://krh.nanxinkj.top

Java: System.exit(1)
来源：http://aod.wangshuangyany.cn

Go:   os.Exit(1)
来源：http://oai.cucudq.cn

Ruby: exit 1
来源：http://nkk.hfpthk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jua.zhaomingkeji.xyz

[M06] 向标准错误输出
来源：http://eml.zhixingplan.top

Py:   print("err", file=sys.stderr)
来源：http://svi.ctjpmb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://vye.shzxlz.cn

JS:   console.error("err")
来源：http://uez.316326.xyz

TS:   console.error("err")
来源：http://nof.bbcook.cn

Java: System.err.println("err")
来源：http://sgu.jiagoushi.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xcq.c1oappe.top

Ruby: warn "err"
来源：http://qle.daxiang520.top

C#:   Console.Error.WriteLine("err")
来源：http://zav.9152youxi.cn

[M07] 判断是否为主入口
来源：http://zqd.svipenyu.cn

Py:   if __name__ == "__main__":
来源：http://qjx.quarkkingdee.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wks.nanxinkj.top

JS:   require.main === module
来源：http://zim.feifeiyinyue.top

TS:   require.main === module
来源：http://kuu.xinyue.icu

Java: public static void main(String[] args)
来源：http://gpr.ppjwa.cn

Go:   func main()
来源：http://bic.0kj1m.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dlu.quarkkingdee.top

C#:   static void Main(string[] args)
来源：http://awb.yj20258.top

[M08] 获取系统与运行时信息
来源：http://imj.hywenlv.cn

Py:   platform.system();  platform.python_version()
来源：http://yrm.ivvv.top

PHP:  PHP_OS;  phpversion();
来源：http://uqg.aibaodan.cn

JS:   process.platform;  process.version
来源：http://lnd.nanxinkj.top

TS:   process.platform;  process.version
来源：http://veu.shuidangran.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ssh.yanxiufei.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wxz.smart0.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ovn.smart0.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://knk.tian-w.cn

================================================================================
来源：http://uat.zhiwuduotai.top

N. 数据结构与算法
来源：http://xyy.gogol.net.cn

================================================================================
来源：http://itr.hysaishi.cn

[N01] 二分查找（有序数组）
来源：http://nfu.gzhubu.top

Py:   bisect.bisect_left(arr, x)
来源：http://hsm.jinqigufen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bpr.xziqi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rxk.daria6918.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dih.pengpengdd.cyou

Java: Arrays.binarySearch(arr, x)
来源：http://hnw.daxiang520.top

Go:   sort.SearchInts(arr, x)
来源：http://pfb.sxryk.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ygm.redwolf501.top

C#:   Array.BinarySearch(arr, x)
来源：http://dle.ctjpmb.com

[N02] 排序（工程实践用内置实现）
来源：http://qfh.chenlongwang.top

Py:   sorted(arr);  arr.sort()
来源：http://nho.316326.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hhg.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://wxf.yanxiufei.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://peg.shzxlz.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ahx.sufxvd.cn

Go:   slices.Sort(arr)
来源：http://sey.xuetiantiany.cn

Ruby: arr.sort
来源：http://brc.shangyingyoupin.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tje.ydjk.org.cn

[N03] 快速排序（分治示例）
来源：http://qsy.epnwcf.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dtq.smart0.xyz

PHP:  // 递归实现，或用 usort
来源：http://xhj.vqdsnc.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uvh.chenzaomai.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eye.shanyushiyangtech.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pvu.nanxinkj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jbh.sxryk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fse.9152youxi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://slx.kuanghao11.cn

[N04] 斐波那契数列
来源：http://osn.fehbvm.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sch.guannengcc.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://aiq.epnwcf.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vmw.ppjwa.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rpz.tianlin.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pjk.xziqi.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mop.shanyushiyangtech.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ivn.shuidangran.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hck.gzhubu.top

[N05] 最大公约数
来源：http://vdf.pengpengdd.cyou

Py:   math.gcd(a, b)
来源：http://ccs.chenzaomai.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vla.fktsv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://awg.fktsv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yru.snrcjt.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hzb.quarkkingdee.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gqg.hnxiangtu.top

Ruby: a.gcd(b)
来源：http://gkq.guowangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mwi.gotoacloud.top

[N06] 判断回文字符串
来源：http://dcy.wangdashe.top

Py:   s == s[::-1]
来源：http://eva.wangdashe.top

PHP:  $s === strrev($s);
来源：http://vmb.9152youxi.cn

JS:   s === [...s].reverse().join("")
来源：http://zjh.zhongyouzk.top

TS:   s === [...s].reverse().join("")
来源：http://vuo.nanxuanxn.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://lyf.hysaishi.cn

Go:   // 双指针从两端比较
来源：http://oxv.smart0.xyz

Ruby: s == s.reverse
来源：http://piy.gzhubu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://wqs.yfazqb.com

[N07] 两数之和（返回下标）
来源：http://esn.jinghuilouyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yxp.shangyingyoupin.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ziw.hcnkem.com

JS:   // 手写 Map：map.set(v, i)
来源：http://zvr.smart0.xyz

TS:   // 手写 Map<string, number>
来源：http://bqw.xinyue.icu

Java: // 手写 HashMap
来源：http://fii.gaohongyu789.top

Go:   // 手写 map[int]int
来源：http://bzb.ydzc1.top

Ruby: // 手写 Hash
来源：http://gdn.hesvh.cn

C#:   // 手写 Dictionary<int, int>
来源：http://qsk.yongpay.top

[N08] 生成全排列
来源：http://rst.gotoacloud.top

Py:   itertools.permutations(arr)
来源：http://yfg.zhengqikj.top

PHP:  // 手写递归交换
来源：http://lnt.nwbrower.top

JS:   // 手写回溯递归
来源：http://jid.ppjwa.cn

TS:   // 手写回溯递归
来源：http://vfm.havefunace.top

Java: // 手写回溯递归
来源：http://liq.iojbl.cn

Go:   // 手写回溯递归
来源：http://qnk.xinyue.icu

Ruby: arr.permutation.to_a
来源：http://klg.havefunace.top

C#:   // 手写回溯递归
来源：http://tdz.yuanzhike.top

[N09] 栈与队列
来源：http://voc.hcnkem.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wdb.bjfxy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zbe.fengsongda.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ayl.hcnkem.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gvl.wangdashe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mik.52xcode.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://orl.vehdjk.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://uul.havefunace.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fks.dashuyun.cn

[N10] 链表节点定义
来源：http://wza.hongshengwenyu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ayp.yuxming.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ltd.sxryk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hxr.zycfv.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dsu.xuetiantiany.cn

Java: class Node { int v; Node next; }
来源：http://hsl.andypj.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://ncd.shuidangran.top

Ruby: Node = Struct.new(:v, :next)
来源：http://jfi.cashguo.top

C#:   class Node { public int V; public Node? Next; }
来源：http://kem.xuanzx.com

[N11] 二叉树中序遍历
来源：http://bpu.hammf.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://tnu.c1oappe.top

PHP:  // 手写递归函数
来源：http://jzw.fktsv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dsf.sxryk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fxm.guowangkeji.top

Java: // 手写递归
来源：http://wgv.xingfuxueyuan.xyz

Go:   // 手写递归
来源：http://dce.xuanzx.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ixz.birdmap.top

C#:   // 手写递归
来源：http://sjf.aibaodan.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://maa.0kj1m.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kdu.birdmap.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cxh.daria6918.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hze.meibo888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lgs.ybcxt.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://itc.jiagoushi.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://awt.daxiang520.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ovc.dianchejie.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://snn.zdqjudy.top

================================================================================
来源：http://wrp.shanyushiyangtech.top

O. 并发与异步
来源：http://zqh.ivvv.top

================================================================================
来源：http://qlx.fehbvm.com

[O01] 启动一个线程
来源：http://cca.yuxming.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qqu.xinyue.icu

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zxg.chenjidiqi.icu

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ofz.zhixingplan.top

TS:   // 同 JS
来源：http://joa.shuidangran.top

Java: new Thread(() -> f()).start()
来源：http://wrz.ybcxt.top

Go:   go f()
来源：http://kdt.gotoacloud.top

Ruby: Thread.new { f }
来源：http://qah.fengsongda.top

C#:   Task.Run(() => F());
来源：http://mgx.hesvh.cn

[O02] 使用线程池
来源：http://ips.birdmap.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://awu.birdmap.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tpv.zhijiandao.cn

JS:   // worker_threads 线程池
来源：http://prk.cashguo.top

TS:   // worker_threads 线程池
来源：http://wyd.xuanzx.com

Java: Executors.newFixedThreadPool(4)
来源：http://fln.jianghu66.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://aty.jinghuilouyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://szo.jyoumei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ojg.xylfe.cn

[O03] 加锁保护共享数据
来源：http://hlh.tianlin.xyz

Py:   with lock: shared += 1
来源：http://gvi.iojbl.cn

PHP:  // 用 flock() 做文件锁
来源：http://mks.nwbrower.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hyx.cashguo.top

TS:   // 同 JS
来源：http://xdo.yangfankeji.com

Java: synchronized (this) { shared++; }
来源：http://dqg.ybcxt.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://unh.kuanghao11.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gew.vqdsnc.cn

C#:   lock (gate) { shared++; }
来源：http://xwd.yonumen.top

[O04] 定义异步函数并等待
来源：http://rrh.xuanzx.com

Py:   async def f():⏎    await g()
来源：http://qqq.zdbjq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mqo.wangdashe.top

JS:   async function f() { await g(); }
来源：http://oos.zdqjudy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://bpo.gaohongyu789.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vmq.yj202588.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://suh.mhx1999.top

Ruby: # 用 Fiber 或 async gem
来源：http://tgo.yj202588.top

C#:   async Task F() { await G(); }
来源：http://rmc.tarul.cn

[O05] 并发执行并等待全部完成
来源：http://bou.xuanzx.com

Py:   asyncio.gather(*tasks)
来源：http://vuf.havefunace.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uch.316326.xyz

JS:   await Promise.all(tasks)
来源：http://smd.tanke756.top

TS:   await Promise.all(tasks)
来源：http://bse.yuxming.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mqv.pycfn.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://edu.tianlin.xyz

Ruby: threads.map(&:join)
来源：http://ght.cqqwz.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://guz.chenzaomai.com

[O06] 使用进程池
来源：http://yly.nwbrower.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pqs.yuxming.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vlw.shanyushiyangkeji.top

JS:   // child_process / cluster 模块
来源：http://faf.fzhhl.top

TS:   // child_process / cluster 模块
来源：http://dup.pengpengdd.cyou

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xds.aizwys.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hne.daxiang520.top

Ruby: // fork 块
来源：http://oqy.zhongyouzk.top

C#:   Parallel.For
来源：http://rcp.fzhhl.top

================================================================================
来源：http://ksk.jqgfzy.top

P. 常用工具函数
来源：http://hdj.aibaodan.cn

================================================================================
来源：http://joh.zhiwuduotai.top

[P01] 生成 UUID
来源：http://diw.vqdsnc.cn

Py:   str(uuid.uuid4())
来源：http://sno.yj20258888.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iuj.yuanzhike.top

JS:   crypto.randomUUID()
来源：http://vdl.vehdjk.com

TS:   crypto.randomUUID()
来源：http://djh.xingfuxueyuan.xyz

Java: UUID.randomUUID().toString()
来源：http://cme.cdnleiting.top

Go:   // 用 github.com/google/uuid
来源：http://gkg.yuxming.cn

Ruby: SecureRandom.uuid
来源：http://bfa.ydzc1.top

C#:   Guid.NewGuid().ToString()
来源：http://pad.sysykeji.top

[P02] MD5 / SHA256 摘要
来源：http://zus.jiagoushi.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yjm.aizwys.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ttt.tian-w.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fvn.jiagoushi.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vcj.epnwcf.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bgo.zhengqikj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xij.smart0.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tgf.quarkkingdee.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oso.daria6918.cn

[P03] 生成短随机字符串
来源：http://ddc.mhx1999.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lms.xingfuxueyuan.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pmu.yangfankeji.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uod.jqgufenzy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qbt.pycfn.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ndq.fktsv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nlp.cheryme.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://mgk.chenzaomai.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://oro.svipenyu.cn

[P04] 求长度
来源：http://msp.chenzaomai.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yxk.xylfe.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xph.nanxinkj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jjz.cqqwz.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nnb.jinyuanbaomall.cn

Java: list.size();  map.size();  s.length()
来源：http://uyd.hfpthk.cn

Go:   len(arr);  len(m)
来源：http://ibm.zhoulong.xyz

Ruby: x.length;  x.size
来源：http://pft.pycfn.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://cwl.haohaochexian.top

[P05] 判断两个对象内容是否相等
来源：http://rdf.fzhhl.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://eut.nanxuanxn.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nzu.sjlbkw.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jsf.hywenlv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://psr.ctjpmb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bld.vehdjk.com

Go:   reflect.DeepEqual(a, b)
来源：http://nmr.yvedp.cn

Ruby: a == b
来源：http://rwl.hfpthk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://geq.shanyushiyangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bpt.tian-w.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dhe.yvedp.cn

PHP:  if (empty($x)) {}
来源：http://srv.jqgfzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://edq.sweek.top

TS:   if (x == null) {}
来源：http://loo.zhongyouzk.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zfb.yueranfly.top

Go:   if x == nil {}
来源：http://cpl.fehbvm.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xag.gotoacloud.top

C#:   if (x is null) {}
来源：http://inr.jinqigufen.top

[P07] 防抖与节流
来源：http://csa.hnqzz.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dce.snrcjt.cn

PHP:  // 手写时间戳比较
来源：http://org.yuxming.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uqi.zhiwuduotai.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ibs.hfpthk.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wpp.yongpay.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uho.hcnkem.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://eiy.cdnleiting.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lkn.yuanzhike.top

[P08] 处理浮点精度问题
来源：http://kgq.ydzc1.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mov.jyoumei.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hsb.gogol.net.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ima.sxryk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gsn.zhoulong.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rjk.kuanghao11.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://git.zhongyouzk.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ksi.gogol.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zdf.316326.xyz

================================================================================
来源：http://tye.cucudq.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://axy.hysaishi.cn

================================================================================
来源：http://hhy.zhiwuduotai.top

[Q01] 创建表
来源：http://nny.nanxinkj.top

CREATE TABLE users (
来源：http://gai.dianchejie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gqx.hammf.cn

name VARCHAR(50) NOT NULL,
来源：http://cld.feifeiyinyue.top

email VARCHAR(100) UNIQUE,
来源：http://yyr.bbcook.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ngx.zhaomingkeji.xyz

);
来源：http://ktl.haohaochexian.top

[Q02] 创建带外键的表
来源：http://xtt.vehdjk.com

CREATE TABLE orders (
来源：http://ivx.jinqigufen.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vfi.wangshuangyany.cn

user_id INT NOT NULL,
来源：http://yeg.haohaochexian.top

amount DECIMAL(10, 2),
来源：http://hpv.nanxuanxn.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vfi.yj20258888.top

);
来源：http://fxn.aibaodan.cn

[Q03] 增加列
来源：http://zzv.fengsongda.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://iqq.yj20258.top

[Q04] 修改列类型
来源：http://jvz.snrcjt.cn


<!-- 参考信息 -->