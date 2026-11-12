代发 wailian999

JS:   process.exit(1)
来源：http://obs.chenlongwang.top

TS:   process.exit(1)
来源：http://pfq.chenjidiqi.icu

Java: System.exit(1)
来源：http://ida.bbcook.cn

Go:   os.Exit(1)
来源：http://ptd.jinqigfzy.top

Ruby: exit 1
来源：http://aed.cheryme.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kfp.havefunace.top

[M06] 向标准错误输出
来源：http://vnp.zhengqikj.top

Py:   print("err", file=sys.stderr)
来源：http://jbj.9152youxi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nhm.nanxinkj.top

JS:   console.error("err")
来源：http://cfd.xingfuxueyuan.xyz

TS:   console.error("err")
来源：http://ple.shangyingyoupin.top

Java: System.err.println("err")
来源：http://nio.zhiwuduotai.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pcr.jiagoushi.top

Ruby: warn "err"
来源：http://gyz.ydjk.org.cn

C#:   Console.Error.WriteLine("err")
来源：http://mhk.daxiang520.top

[M07] 判断是否为主入口
来源：http://pln.bbcook.cn

Py:   if __name__ == "__main__":
来源：http://hdt.nanxuanxn.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kkq.wangdashe.top

JS:   require.main === module
来源：http://luj.shanyushiyangkeji.top

TS:   require.main === module
来源：http://ixl.epnwcf.com

Java: public static void main(String[] args)
来源：http://pyb.ctjpmb.com

Go:   func main()
来源：http://sxl.jqgfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sqm.xingfuxueyuan.xyz

C#:   static void Main(string[] args)
来源：http://fmy.sufxvd.cn

[M08] 获取系统与运行时信息
来源：http://rym.zhengqikj.top

Py:   platform.system();  platform.python_version()
来源：http://dbk.gogol.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://dvt.hfpthk.cn

JS:   process.platform;  process.version
来源：http://djv.zycfv.cn

TS:   process.platform;  process.version
来源：http://und.cucudq.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bnu.hammf.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://koe.shuidangran.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jcc.dashuyun.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kwt.sjlbkw.cn

================================================================================
来源：http://ong.smart0.xyz

N. 数据结构与算法
来源：http://yoj.fehbvm.com

================================================================================
来源：http://vsl.zhongyouzk.top

[N01] 二分查找（有序数组）
来源：http://nyu.daxiang520.top

Py:   bisect.bisect_left(arr, x)
来源：http://aaz.sxryk.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mkc.havefunace.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tcz.sweek.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ggc.kuanghao11.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fhu.52xcode.cn

Go:   sort.SearchInts(arr, x)
来源：http://hvp.jinqigufen.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://oaz.nanxuanxn.top

C#:   Array.BinarySearch(arr, x)
来源：http://qyw.c1oappe.top

[N02] 排序（工程实践用内置实现）
来源：http://ybd.shuidangran.top

Py:   sorted(arr);  arr.sort()
来源：http://bhy.zhiwuduotai.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://drs.pycfn.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://huh.zhengqikj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://bfm.ydzc1.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cmd.shuidangran.top

Go:   slices.Sort(arr)
来源：http://wnp.chenzaomai.com

Ruby: arr.sort
来源：http://qud.zhengqikj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kmb.wangshuangyany.cn

[N03] 快速排序（分治示例）
来源：http://odd.zhongyouzk.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blb.nanxinkj.top

PHP:  // 递归实现，或用 usort
来源：http://vyz.sysykeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lyv.chenzaomai.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://woa.redwolf501.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lfd.jiagoushi.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nft.9152youxi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sha.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://jzl.chenjidiqi.icu

[N04] 斐波那契数列
来源：http://ach.cheryme.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://clm.zhaomingkeji.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zwh.hammf.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xrd.fktsv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rkw.nwbrower.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fsi.sjlbkw.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ulu.hnxiangtu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zac.hongshengwenyu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vql.xingfuxueyuan.xyz

[N05] 最大公约数
来源：http://nwu.ctjpmb.com

Py:   math.gcd(a, b)
来源：http://wud.daxiang520.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jsz.jqgufenzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pum.cheryme.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wpz.jqgfzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fms.xuetiantiany.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fcx.wangdashe.top

Ruby: a.gcd(b)
来源：http://rgj.cqqwz.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ode.wangshuangyany.cn

[N06] 判断回文字符串
来源：http://gzk.mhx1999.top

Py:   s == s[::-1]
来源：http://oab.hammf.cn

PHP:  $s === strrev($s);
来源：http://nhz.hnxiangtu.top

JS:   s === [...s].reverse().join("")
来源：http://apj.jinyuanbaomall.cn

TS:   s === [...s].reverse().join("")
来源：http://jxc.xziqi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ydo.gogol.net.cn

Go:   // 双指针从两端比较
来源：http://pmb.yfazqb.com

Ruby: s == s.reverse
来源：http://eus.yonumen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://yog.shuidangran.top

[N07] 两数之和（返回下标）
来源：http://rnb.jinghuilouyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://edy.pycfn.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dnc.cdnleiting.top

JS:   // 手写 Map：map.set(v, i)
来源：http://chm.jinyuanbaomall.cn

TS:   // 手写 Map<string, number>
来源：http://jyv.daria6918.cn

Java: // 手写 HashMap
来源：http://upd.mhx1999.top

Go:   // 手写 map[int]int
来源：http://qeq.yj20258888.top

Ruby: // 手写 Hash
来源：http://qox.hnxiangtu.top

C#:   // 手写 Dictionary<int, int>
来源：http://wxs.yueranfly.top

[N08] 生成全排列
来源：http://vcn.zhengqikj.top

Py:   itertools.permutations(arr)
来源：http://fzr.sjlbkw.cn

PHP:  // 手写递归交换
来源：http://kai.fzhhl.top

JS:   // 手写回溯递归
来源：http://cbz.nwbrower.top

TS:   // 手写回溯递归
来源：http://zef.gaohongyu789.top

Java: // 手写回溯递归
来源：http://bfo.shzxlz.cn

Go:   // 手写回溯递归
来源：http://ihw.shangyingyoupin.top

Ruby: arr.permutation.to_a
来源：http://ppl.yuxming.cn

C#:   // 手写回溯递归
来源：http://crq.tarul.cn

[N09] 栈与队列
来源：http://qcr.shangyingyoupin.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ypg.zhengqikj.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xoc.sjlbkw.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gcw.sysykeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ktb.zdqjudy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dnw.yj20258.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kes.daxiang520.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mzq.jyoumei.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ite.svipenyu.cn

[N10] 链表节点定义
来源：http://nbj.zdqjudy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tru.52xcode.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lki.jqgfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://upr.xinyue.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fml.yfazqb.com

Java: class Node { int v; Node next; }
来源：http://unc.jiagoushi.top

Go:   type Node struct { V int; Next *Node }
来源：http://hdt.jqgufenzy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ysz.havefunace.top

C#:   class Node { public int V; public Node? Next; }
来源：http://qly.vqdsnc.cn

[N11] 二叉树中序遍历
来源：http://mfd.pycfn.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xsg.mhx1999.top

PHP:  // 手写递归函数
来源：http://dss.ybcxt.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yaf.zdbjq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nrg.iojbl.cn

Java: // 手写递归
来源：http://lgv.fzhhl.top

Go:   // 手写递归
来源：http://bwp.ybcxt.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jcc.vehdjk.com

C#:   // 手写递归
来源：http://fmw.havefunace.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oko.vehdjk.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wss.zhixingplan.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wuk.yuxming.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zjx.daria6918.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hwo.snrcjt.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kvf.gogol.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bno.c1oappe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pvd.zhaomingkeji.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://vad.ybcxt.top

================================================================================
来源：http://uia.sysykeji.top

O. 并发与异步
来源：http://flr.aibaodan.cn

================================================================================
来源：http://kgc.jinghuilouyu.cn

[O01] 启动一个线程
来源：http://naw.nanxinkj.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://djh.0kj1m.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sve.snrcjt.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uqs.fktsv.cn

TS:   // 同 JS
来源：http://ogc.meibo888.top

Java: new Thread(() -> f()).start()
来源：http://kyf.zdbjq.cn

Go:   go f()
来源：http://oke.dashuyun.cn

Ruby: Thread.new { f }
来源：http://mqh.hnqzz.top

C#:   Task.Run(() => F());
来源：http://wxu.fengsongda.top

[O02] 使用线程池
来源：http://het.ctjpmb.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ngb.ydzc1.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wqb.zhengqikj.top

JS:   // worker_threads 线程池
来源：http://qzt.vehdjk.com

TS:   // worker_threads 线程池
来源：http://clr.vqdsnc.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qzu.yj20258888.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ito.zhoulong.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nmo.iojbl.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ffw.birdmap.top

[O03] 加锁保护共享数据
来源：http://syz.zdqjudy.top

Py:   with lock: shared += 1
来源：http://vqu.0kj1m.cn

PHP:  // 用 flock() 做文件锁
来源：http://nnk.ivvv.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://anz.cdnleiting.top

TS:   // 同 JS
来源：http://hzb.birdmap.top

Java: synchronized (this) { shared++; }
来源：http://hmg.shuidangran.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wxs.snrcjt.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pbq.ppjwa.cn

C#:   lock (gate) { shared++; }
来源：http://lue.xylfe.cn

[O04] 定义异步函数并等待
来源：http://bcw.ctjpmb.com

Py:   async def f():⏎    await g()
来源：http://xab.jianghu66.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://seb.shuidangran.top

JS:   async function f() { await g(); }
来源：http://jiz.tanke756.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://cbs.nwbrower.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fca.meibo888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eeq.epnwcf.com

Ruby: # 用 Fiber 或 async gem
来源：http://utu.gotoacloud.top

C#:   async Task F() { await G(); }
来源：http://bpn.wangdashe.top

[O05] 并发执行并等待全部完成
来源：http://oaw.cqqwz.cn

Py:   asyncio.gather(*tasks)
来源：http://sta.shanyushiyangtech.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xsa.shanyushiyangtech.top

JS:   await Promise.all(tasks)
来源：http://acm.feifeiyinyue.top

TS:   await Promise.all(tasks)
来源：http://rwv.fktsv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fdx.shuidangran.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wrl.daria6918.cn

Ruby: threads.map(&:join)
来源：http://hde.ctjpmb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://onu.nanxuanxn.top

[O06] 使用进程池
来源：http://ogc.fktsv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jze.jqgufenzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nwg.shanyushiyangkeji.top

JS:   // child_process / cluster 模块
来源：http://tyo.zhongyouzk.top

TS:   // child_process / cluster 模块
来源：http://zzi.zhixingplan.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qqj.fengsongda.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lpp.vehdjk.com

Ruby: // fork 块
来源：http://fdn.jyoumei.cn

C#:   Parallel.For
来源：http://btm.tarul.cn

================================================================================
来源：http://eiw.zhaomingkeji.xyz

P. 常用工具函数
来源：http://dqt.c1oappe.top

================================================================================
来源：http://iba.guannengcc.top

[P01] 生成 UUID
来源：http://smj.hnqzz.top

Py:   str(uuid.uuid4())
来源：http://lvm.shanyushiyangkeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ket.cqqwz.cn

JS:   crypto.randomUUID()
来源：http://cof.yvedp.cn

TS:   crypto.randomUUID()
来源：http://xya.xingfuxueyuan.xyz

Java: UUID.randomUUID().toString()
来源：http://xfh.gogol.net.cn

Go:   // 用 github.com/google/uuid
来源：http://rdi.yuanzhike.top

Ruby: SecureRandom.uuid
来源：http://fyn.zhijiandao.cn

C#:   Guid.NewGuid().ToString()
来源：http://owk.uphjek.com

[P02] MD5 / SHA256 摘要
来源：http://pmi.xuanzx.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rjs.52xcode.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uwb.fengsongda.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yjo.wangdashe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://osi.yueranfly.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://abj.ivvv.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://glx.havefunace.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hhk.gogol.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zfy.yj202588.top

[P03] 生成短随机字符串
来源：http://mgw.xuetiantiany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nfy.wangshuangyany.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://typ.zdbjq.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://feq.shangyingyoupin.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zzl.zhaomingkeji.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wiz.yangfankeji.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iba.shangyingyoupin.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://yok.hywenlv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://unz.hysaishi.cn

[P04] 求长度
来源：http://nbo.sufxvd.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lfx.birdmap.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hff.shanyushiyangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eam.hywenlv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ahb.yj202588.top

Java: list.size();  map.size();  s.length()
来源：http://iqv.nwbrower.top

Go:   len(arr);  len(m)
来源：http://cgq.gotoacloud.top

Ruby: x.length;  x.size
来源：http://sjb.jinqigufen.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://wpd.gotoacloud.top

[P05] 判断两个对象内容是否相等
来源：http://xmz.hywenlv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cap.hongshengwenyu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kvq.shuidangran.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://aqx.zycfv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ffi.zhoulong.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dxa.aibaodan.cn

Go:   reflect.DeepEqual(a, b)
来源：http://adb.shanyushiyangtech.top

Ruby: a == b
来源：http://tyr.hcnkem.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://luy.yuxming.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xdp.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tyz.jinghuilouyu.cn

PHP:  if (empty($x)) {}
来源：http://ejt.pengpengdd.cyou

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vdt.316326.xyz

TS:   if (x == null) {}
来源：http://dys.gotoacloud.top

Java: if (x == null || x.isEmpty()) {}
来源：http://pnf.redwolf501.top

Go:   if x == nil {}
来源：http://olz.52xcode.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://obo.gotoacloud.top

C#:   if (x is null) {}
来源：http://gdm.yfazqb.com

[P07] 防抖与节流
来源：http://wpf.jyoumei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://crp.gogol.net.cn

PHP:  // 手写时间戳比较
来源：http://yyv.hcnkem.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mdu.hfpthk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uqd.yangfankeji.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://epu.yuxming.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ckg.dianchejie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mpa.yuxming.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://aew.jinyuanbaomall.cn

[P08] 处理浮点精度问题
来源：http://dax.chenlongwang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tdq.jyoumei.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://aie.tianlin.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kii.havefunace.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qcz.vehdjk.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rfi.smart0.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zfh.tanke756.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bxq.zdbjq.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xku.wangdashe.top

================================================================================
来源：http://vva.xingfuxueyuan.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kti.xziqi.cn

================================================================================
来源：http://vrv.vehdjk.com

[Q01] 创建表
来源：http://mjb.fzhhl.top

CREATE TABLE users (
来源：http://gke.jqgfzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ezi.yj202588.top

name VARCHAR(50) NOT NULL,
来源：http://dum.9152youxi.cn

email VARCHAR(100) UNIQUE,
来源：http://voj.gogol.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vay.fktsv.cn

);
来源：http://qgl.gaohongyu789.top

[Q02] 创建带外键的表
来源：http://zqy.zycfv.cn

CREATE TABLE orders (
来源：http://vxq.jinqigfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rey.yueranfly.top

user_id INT NOT NULL,
来源：http://rnz.xylfe.cn

amount DECIMAL(10, 2),
来源：http://xeo.yongpay.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cvl.cdnleiting.top

);
来源：http://boq.yangfankeji.com

[Q03] 增加列
来源：http://rwk.jlsjyb.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://qyf.vqdsnc.cn

[Q04] 修改列类型
来源：http://iaa.zhoulong.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lbe.chenzaomai.com

[Q05] 重命名列
来源：http://sys.zhongyouzk.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tzh.mhx1999.top

[Q06] 删除列
来源：http://jsg.vehdjk.com


<!-- 参考信息 -->