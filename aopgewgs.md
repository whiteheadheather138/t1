代发 wailian999

Ruby: exit 1
来源：http://ahk.snrcjt.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qiu.ydjk.org.cn

[M06] 向标准错误输出
来源：http://zkr.yangfankeji.com

Py:   print("err", file=sys.stderr)
来源：http://swa.52xcode.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://zbn.jiagoushi.top

JS:   console.error("err")
来源：http://bdo.jqgfzy.top

TS:   console.error("err")
来源：http://lbq.xinyue.icu

Java: System.err.println("err")
来源：http://gii.yanxiufei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://opc.jiagoushi.top

Ruby: warn "err"
来源：http://fem.hcnkem.com

C#:   Console.Error.WriteLine("err")
来源：http://rlk.zhijiandao.cn

[M07] 判断是否为主入口
来源：http://zjd.tanke756.top

Py:   if __name__ == "__main__":
来源：http://cyu.shuidangran.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://beq.fehbvm.com

JS:   require.main === module
来源：http://xhk.9152youxi.cn

TS:   require.main === module
来源：http://jsz.fengsongda.top

Java: public static void main(String[] args)
来源：http://cuh.hnqzz.top

Go:   func main()
来源：http://gjh.nanxinkj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dss.ppjwa.cn

C#:   static void Main(string[] args)
来源：http://bap.fengsongda.top

[M08] 获取系统与运行时信息
来源：http://bmg.zhijiandao.cn

Py:   platform.system();  platform.python_version()
来源：http://wyy.jqgfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://kdz.fktsv.cn

JS:   process.platform;  process.version
来源：http://uki.gogol.net.cn

TS:   process.platform;  process.version
来源：http://qfb.tanke756.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nsz.xuanzx.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://hux.aibaodan.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ucy.hcnkem.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://dsa.316326.xyz

================================================================================
来源：http://nfq.ivvv.top

N. 数据结构与算法
来源：http://kbh.iojbl.cn

================================================================================
来源：http://kzb.guannengcc.top

[N01] 二分查找（有序数组）
来源：http://tht.gaohongyu789.top

Py:   bisect.bisect_left(arr, x)
来源：http://lwp.52xcode.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bkq.tarul.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zgl.ehwqpu.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lml.cucudq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://shv.sxryk.cn

Go:   sort.SearchInts(arr, x)
来源：http://jsf.yj20258.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://bjo.kuanghao11.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jye.sysykeji.top

[N02] 排序（工程实践用内置实现）
来源：http://rit.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://hrj.ivvv.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://yuf.jinqigufen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://kxf.cashguo.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lej.316326.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://szz.gogol.net.cn

Go:   slices.Sort(arr)
来源：http://jgl.uphjek.com

Ruby: arr.sort
来源：http://wia.snrcjt.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://wef.ivvv.top

[N03] 快速排序（分治示例）
来源：http://eqi.ywan-chungtsiang.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lgq.chenlongwang.top

PHP:  // 递归实现，或用 usort
来源：http://zbe.sjlbkw.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nbj.hfpthk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zbt.yj202588.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://njc.hesvh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lzb.pycfn.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lep.sweek.top

C#:   // 手写递归，或 Array.Sort
来源：http://cfw.aibaodan.cn

[N04] 斐波那契数列
来源：http://zyh.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tkz.havefunace.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cgp.tarul.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ivf.yfazqb.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cow.hongshengwenyu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://flj.jinyuanbaomall.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hrs.yueranfly.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fys.ybcxt.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rju.ydjk.org.cn

[N05] 最大公约数
来源：http://klr.fengsongda.top

Py:   math.gcd(a, b)
来源：http://fsz.cheryme.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://iob.mhx1999.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lfa.hcnkem.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ifi.jyoumei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ikw.dianchejie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pni.yj20258888.top

Ruby: a.gcd(b)
来源：http://vrp.shanyushiyangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bpw.hnxiangtu.top

[N06] 判断回文字符串
来源：http://aco.fehbvm.com

Py:   s == s[::-1]
来源：http://yaf.zdbjq.cn

PHP:  $s === strrev($s);
来源：http://kik.tianlin.xyz

JS:   s === [...s].reverse().join("")
来源：http://gzj.shanyushiyangtech.top

TS:   s === [...s].reverse().join("")
来源：http://cvs.jyoumei.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fet.chenjidiqi.icu

Go:   // 双指针从两端比较
来源：http://uab.vehdjk.com

Ruby: s == s.reverse
来源：http://xjp.iojbl.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://kgg.316326.xyz

[N07] 两数之和（返回下标）
来源：http://ixt.hysaishi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zan.yonumen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mjm.gogol.net.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://ejl.c1oappe.top

TS:   // 手写 Map<string, number>
来源：http://zmn.xinyue.icu

Java: // 手写 HashMap
来源：http://zab.52xcode.cn

Go:   // 手写 map[int]int
来源：http://ndi.zhengqikj.top

Ruby: // 手写 Hash
来源：http://vsq.xuanzx.com

C#:   // 手写 Dictionary<int, int>
来源：http://ndj.smart0.xyz

[N08] 生成全排列
来源：http://lyi.feifeiyinyue.top

Py:   itertools.permutations(arr)
来源：http://rvb.pengpengdd.cyou

PHP:  // 手写递归交换
来源：http://zzy.zdqjudy.top

JS:   // 手写回溯递归
来源：http://zsl.jinyuanbaomall.cn

TS:   // 手写回溯递归
来源：http://xbe.cashguo.top

Java: // 手写回溯递归
来源：http://fqg.nanxuanxn.top

Go:   // 手写回溯递归
来源：http://zot.c1oappe.top

Ruby: arr.permutation.to_a
来源：http://tmx.yj202588.top

C#:   // 手写回溯递归
来源：http://fcv.cheryme.top

[N09] 栈与队列
来源：http://onz.wangdashe.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://nbq.ydzc1.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://dus.kuanghao11.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://def.havefunace.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ydm.gotoacloud.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dah.shanyushiyangkeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://gbt.kuanghao11.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://klz.ppjwa.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ccz.sxryk.cn

[N10] 链表节点定义
来源：http://jlr.ivvv.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://llc.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zcg.bbcook.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mqc.epnwcf.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dlg.daria6918.cn

Java: class Node { int v; Node next; }
来源：http://wnl.cucudq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://zqx.zhijiandao.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://onz.zhaomingkeji.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://ugq.hcnkem.com

[N11] 二叉树中序遍历
来源：http://kym.tanke756.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qfh.gotoacloud.top

PHP:  // 手写递归函数
来源：http://gml.zhiwuduotai.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jby.tian-w.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zak.xuetiantiany.cn

Java: // 手写递归
来源：http://stv.zhoulong.xyz

Go:   // 手写递归
来源：http://ufu.hcnkem.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://lve.epnwcf.com

C#:   // 手写递归
来源：http://gdn.nwbrower.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wez.zhiwuduotai.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://sjs.shzxlz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ryy.tarul.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://var.ehwqpu.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ato.zdbjq.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://epb.xinyue.icu

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tmd.xylfe.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://myx.quarkkingdee.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fkq.jyoumei.cn

================================================================================
来源：http://xga.andypj.xyz

O. 并发与异步
来源：http://qhd.vehdjk.com

================================================================================
来源：http://ooo.wangdashe.top

[O01] 启动一个线程
来源：http://yeb.9152youxi.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://uod.cashguo.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wdx.yj202588.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://avi.zhijiandao.cn

TS:   // 同 JS
来源：http://jqd.cashguo.top

Java: new Thread(() -> f()).start()
来源：http://muh.hnxiangtu.top

Go:   go f()
来源：http://nco.birdmap.top

Ruby: Thread.new { f }
来源：http://opx.zhoulong.xyz

C#:   Task.Run(() => F());
来源：http://vvl.nwbrower.top

[O02] 使用线程池
来源：http://zrs.vqdsnc.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sfj.gogol.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mdu.chenjidiqi.icu

JS:   // worker_threads 线程池
来源：http://lwd.fktsv.cn

TS:   // worker_threads 线程池
来源：http://nsh.ppjwa.cn

Java: Executors.newFixedThreadPool(4)
来源：http://sfi.xylfe.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tpa.chenjidiqi.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ztk.bjfxy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ymt.fehbvm.com

[O03] 加锁保护共享数据
来源：http://fee.hnqzz.top

Py:   with lock: shared += 1
来源：http://fbp.316326.xyz

PHP:  // 用 flock() 做文件锁
来源：http://idh.sufxvd.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ioz.yuanzhike.top

TS:   // 同 JS
来源：http://wta.hongshengwenyu.top

Java: synchronized (this) { shared++; }
来源：http://fuy.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rxx.nanxuanxn.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://kav.sweek.top

C#:   lock (gate) { shared++; }
来源：http://wnz.uphjek.com

[O04] 定义异步函数并等待
来源：http://zvo.shzxlz.cn

Py:   async def f():⏎    await g()
来源：http://xsr.yuanzhike.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lqv.fehbvm.com

JS:   async function f() { await g(); }
来源：http://ufv.birdmap.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zfa.ppjwa.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yfl.bjfxy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kku.xziqi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mzu.shangyingyoupin.top

C#:   async Task F() { await G(); }
来源：http://esu.kuanghao11.cn

[O05] 并发执行并等待全部完成
来源：http://nng.zhoulong.xyz

Py:   asyncio.gather(*tasks)
来源：http://rfl.ppjwa.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yru.chenlongwang.top

JS:   await Promise.all(tasks)
来源：http://lor.ctjpmb.com

TS:   await Promise.all(tasks)
来源：http://yzh.jinqigfzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dwv.hfpthk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kdj.chenlongwang.top

Ruby: threads.map(&:join)
来源：http://dpu.sysykeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://cfn.yuxming.cn

[O06] 使用进程池
来源：http://fib.316326.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fsy.aibaodan.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tda.yvedp.cn

JS:   // child_process / cluster 模块
来源：http://gip.birdmap.top

TS:   // child_process / cluster 模块
来源：http://eyq.sjlbkw.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://isx.shanyushiyangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oli.zhongyouzk.top

Ruby: // fork 块
来源：http://jfo.zhaomingkeji.xyz

C#:   Parallel.For
来源：http://xvi.daria6918.cn

================================================================================
来源：http://fny.sufxvd.cn

P. 常用工具函数
来源：http://ylf.gaohongyu789.top

================================================================================
来源：http://lij.ydzc1.top

[P01] 生成 UUID
来源：http://jmi.zhiwuduotai.top

Py:   str(uuid.uuid4())
来源：http://jia.yfazqb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iqx.yj202588.top

JS:   crypto.randomUUID()
来源：http://xih.ivvv.top

TS:   crypto.randomUUID()
来源：http://qwy.yvedp.cn

Java: UUID.randomUUID().toString()
来源：http://bcp.nanxuanxn.top

Go:   // 用 github.com/google/uuid
来源：http://wvj.shzxlz.cn

Ruby: SecureRandom.uuid
来源：http://qai.zhixingplan.top

C#:   Guid.NewGuid().ToString()
来源：http://lzf.tarul.cn

[P02] MD5 / SHA256 摘要
来源：http://qpv.sjlbkw.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gjo.sjlbkw.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pex.chenzaomai.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cmd.yj20258888.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nqr.zhoulong.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qnd.redwolf501.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lhz.aizwys.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jmk.chenzaomai.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://giu.gzhubu.top

[P03] 生成短随机字符串
来源：http://mss.meibo888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kzx.andypj.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zwv.zhoulong.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eja.xingfuxueyuan.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hup.daria6918.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fia.nanxuanxn.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uxz.ehwqpu.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://fwb.fzhhl.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vph.0kj1m.cn

[P04] 求长度
来源：http://icp.zhongyouzk.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rac.meibo888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sjv.uphjek.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://atd.hfpthk.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yrj.cashguo.top

Java: list.size();  map.size();  s.length()
来源：http://zpy.yanxiufei.cn

Go:   len(arr);  len(m)
来源：http://rhc.yanxiufei.cn

Ruby: x.length;  x.size
来源：http://brg.zhaomingkeji.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://txp.gotoacloud.top

[P05] 判断两个对象内容是否相等
来源：http://kol.bbcook.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qgu.nanxinkj.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hnr.fehbvm.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://awr.hnxiangtu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nwj.guowangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fbg.52xcode.cn

Go:   reflect.DeepEqual(a, b)
来源：http://mwz.zhoulong.xyz

Ruby: a == b
来源：http://jcu.ivvv.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yhm.chenzaomai.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fpx.cqqwz.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gnp.xuanzx.com

PHP:  if (empty($x)) {}
来源：http://mah.sufxvd.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sgm.yuanzhike.top

TS:   if (x == null) {}
来源：http://now.sjlbkw.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zvy.zdbjq.cn

Go:   if x == nil {}
来源：http://fjy.yj202588.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kve.fzhhl.top

C#:   if (x is null) {}
来源：http://xoe.yj20258.top

[P07] 防抖与节流
来源：http://opy.guowangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xmt.jqgfzy.top

PHP:  // 手写时间戳比较
来源：http://wkp.hywenlv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oqx.wangshuangyany.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wgm.mhx1999.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hkt.gzhubu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://msm.dashuyun.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://uur.bbcook.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gvu.hcnkem.com

[P08] 处理浮点精度问题
来源：http://ebd.jlsjyb.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xkh.andypj.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zwa.feifeiyinyue.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kvz.hnqzz.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jic.tanke756.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uic.ydzc1.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ivv.daxiang520.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wgm.tian-w.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zil.zhoulong.xyz

================================================================================
来源：http://bco.hongshengwenyu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://chk.daria6918.cn

================================================================================
来源：http://cac.zdqjudy.top

[Q01] 创建表
来源：http://fld.yanxiufei.cn

CREATE TABLE users (
来源：http://nvv.zdqjudy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lij.redwolf501.top

name VARCHAR(50) NOT NULL,
来源：http://lgs.yanxiufei.cn

email VARCHAR(100) UNIQUE,
来源：http://olz.ybcxt.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kox.ppjwa.cn

);
来源：http://kfg.cucudq.cn

[Q02] 创建带外键的表
来源：http://pjy.52xcode.cn

CREATE TABLE orders (
来源：http://xvf.pengpengdd.cyou

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dtj.c1oappe.top

user_id INT NOT NULL,
来源：http://htb.cdnleiting.top

amount DECIMAL(10, 2),
来源：http://zas.yueranfly.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gua.hywenlv.cn

);
来源：http://xty.sjlbkw.cn

[Q03] 增加列
来源：http://jhg.zdqjudy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tly.hnqzz.top

[Q04] 修改列类型
来源：http://vhi.iojbl.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oed.jlsjyb.cn

[Q05] 重命名列
来源：http://kir.yj20258.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fic.shangyingyoupin.top

[Q06] 删除列
来源：http://nbq.ppjwa.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fjj.mhx1999.top

[Q07] 删除表
来源：http://bti.bbcook.cn

DROP TABLE IF EXISTS orders;
来源：http://hxv.tianlin.xyz

[Q08] 创建普通索引
来源：http://xvd.mhx1999.top


<!-- 参考信息 -->