代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://som.zdqjudy.top

JS:   console.error("err")
来源：http://ngy.zhongyouzk.top

TS:   console.error("err")
来源：http://hle.dianchejie.cn

Java: System.err.println("err")
来源：http://vvy.gaohongyu789.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mtt.tian-w.cn

Ruby: warn "err"
来源：http://qvs.yonumen.top

C#:   Console.Error.WriteLine("err")
来源：http://tdb.dashuyun.cn

[M07] 判断是否为主入口
来源：http://hvn.dianchejie.cn

Py:   if __name__ == "__main__":
来源：http://pti.shanyushiyangtech.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mpq.cheryme.top

JS:   require.main === module
来源：http://qxs.zhixingplan.top

TS:   require.main === module
来源：http://sbq.svipenyu.cn

Java: public static void main(String[] args)
来源：http://lir.bbcook.cn

Go:   func main()
来源：http://uaq.daria6918.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yjv.ivvv.top

C#:   static void Main(string[] args)
来源：http://uck.hcnkem.com

[M08] 获取系统与运行时信息
来源：http://ugn.yuxming.cn

Py:   platform.system();  platform.python_version()
来源：http://akf.jinqigfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://nfc.yanxiufei.cn

JS:   process.platform;  process.version
来源：http://vqq.yvedp.cn

TS:   process.platform;  process.version
来源：http://niw.gaohongyu789.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hii.zdbjq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://dhg.bbcook.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bsl.shangyingyoupin.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://csq.pycfn.com

================================================================================
来源：http://iep.jiagoushi.top

N. 数据结构与算法
来源：http://cue.epnwcf.com

================================================================================
来源：http://ich.yanxiufei.cn

[N01] 二分查找（有序数组）
来源：http://dvc.9152youxi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://box.gaohongyu789.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lvc.yj202588.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lqf.hammf.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ufe.dashuyun.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fla.nanxinkj.top

Go:   sort.SearchInts(arr, x)
来源：http://ixk.mhx1999.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://enc.sjlbkw.cn

C#:   Array.BinarySearch(arr, x)
来源：http://oxl.c1oappe.top

[N02] 排序（工程实践用内置实现）
来源：http://uid.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://jma.yuxming.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ent.aibaodan.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://tko.xuetiantiany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tyl.yvedp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xfe.xuanzx.com

Go:   slices.Sort(arr)
来源：http://oan.dashuyun.cn

Ruby: arr.sort
来源：http://nyf.havefunace.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://apa.xuanzx.com

[N03] 快速排序（分治示例）
来源：http://rzr.vehdjk.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ooa.shzxlz.cn

PHP:  // 递归实现，或用 usort
来源：http://mfs.smart0.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cig.ivvv.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lrp.zhaomingkeji.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://uxl.yuxming.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vin.birdmap.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wzb.chenzaomai.com

C#:   // 手写递归，或 Array.Sort
来源：http://snn.pengpengdd.cyou

[N04] 斐波那契数列
来源：http://bff.yj20258888.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://lzx.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dsc.yongpay.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://yfw.guannengcc.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mfb.feifeiyinyue.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xon.daria6918.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nxz.cheryme.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rkt.chenlongwang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pkg.dashuyun.cn

[N05] 最大公约数
来源：http://bid.yvedp.cn

Py:   math.gcd(a, b)
来源：http://kto.kuanghao11.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://abc.yonumen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mqa.svipenyu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nhq.birdmap.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rtm.xylfe.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kyz.hfpthk.cn

Ruby: a.gcd(b)
来源：http://str.tanke756.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vgz.yanxiufei.cn

[N06] 判断回文字符串
来源：http://nzx.wangdashe.top

Py:   s == s[::-1]
来源：http://nzw.hnqzz.top

PHP:  $s === strrev($s);
来源：http://dzj.cdnleiting.top

JS:   s === [...s].reverse().join("")
来源：http://vxv.nwbrower.top

TS:   s === [...s].reverse().join("")
来源：http://xcq.gzhubu.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xhg.nwbrower.top

Go:   // 双指针从两端比较
来源：http://wlq.cucudq.cn

Ruby: s == s.reverse
来源：http://tam.pycfn.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://bkb.shangyingyoupin.top

[N07] 两数之和（返回下标）
来源：http://bcg.nwbrower.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ftw.nanxinkj.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://scx.bbcook.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jwj.ehwqpu.com

TS:   // 手写 Map<string, number>
来源：http://vhp.daxiang520.top

Java: // 手写 HashMap
来源：http://sfe.xziqi.cn

Go:   // 手写 map[int]int
来源：http://ter.haohaochexian.top

Ruby: // 手写 Hash
来源：http://ejs.jqgfzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://lgm.yangfankeji.com

[N08] 生成全排列
来源：http://ilo.yfazqb.com

Py:   itertools.permutations(arr)
来源：http://sro.tian-w.cn

PHP:  // 手写递归交换
来源：http://oqv.uphjek.com

JS:   // 手写回溯递归
来源：http://woo.sysykeji.top

TS:   // 手写回溯递归
来源：http://rip.mhx1999.top

Java: // 手写回溯递归
来源：http://esa.jianghu66.top

Go:   // 手写回溯递归
来源：http://fbi.yongpay.top

Ruby: arr.permutation.to_a
来源：http://bsm.shuidangran.top

C#:   // 手写回溯递归
来源：http://swn.jyoumei.cn

[N09] 栈与队列
来源：http://mqq.zhiwuduotai.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gjc.jianghu66.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://olm.yj20258.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gze.sxryk.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rdq.guowangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ptg.yj20258.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dhh.hywenlv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bds.tian-w.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ynt.pycfn.com

[N10] 链表节点定义
来源：http://snz.jqgufenzy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kck.ydjk.org.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://oik.zhongyouzk.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jit.yfazqb.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hsb.xinyue.icu

Java: class Node { int v; Node next; }
来源：http://ebx.epnwcf.com

Go:   type Node struct { V int; Next *Node }
来源：http://hel.shangyingyoupin.top

Ruby: Node = Struct.new(:v, :next)
来源：http://bed.chenzaomai.com

C#:   class Node { public int V; public Node? Next; }
来源：http://utb.c1oappe.top

[N11] 二叉树中序遍历
来源：http://ogv.ydjk.org.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://rpy.jinqigufen.top

PHP:  // 手写递归函数
来源：http://gfu.hesvh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wpn.gzhubu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pdu.xingfuxueyuan.xyz

Java: // 手写递归
来源：http://nvd.gotoacloud.top

Go:   // 手写递归
来源：http://iuw.gaohongyu789.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://csr.316326.xyz

C#:   // 手写递归
来源：http://jrh.shanyushiyangtech.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gwu.jyoumei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cdj.zdbjq.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sbz.jinqigufen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xag.gogol.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mss.jqgfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vsj.shzxlz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vza.yj20258888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://aku.zhijiandao.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://pou.xinyue.icu

================================================================================
来源：http://toc.chenlongwang.top

O. 并发与异步
来源：http://goz.xuetiantiany.cn

================================================================================
来源：http://zvi.jinghuilouyu.cn

[O01] 启动一个线程
来源：http://agf.smart0.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fob.zhongyouzk.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://aae.feifeiyinyue.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fnd.zhixingplan.top

TS:   // 同 JS
来源：http://npc.fengsongda.top

Java: new Thread(() -> f()).start()
来源：http://dnm.jinyuanbaomall.cn

Go:   go f()
来源：http://fxf.yuxming.cn

Ruby: Thread.new { f }
来源：http://ohy.epnwcf.com

C#:   Task.Run(() => F());
来源：http://wla.yvedp.cn

[O02] 使用线程池
来源：http://npc.smart0.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bzm.svipenyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wlk.nanxuanxn.top

JS:   // worker_threads 线程池
来源：http://jrx.sxryk.cn

TS:   // worker_threads 线程池
来源：http://xzj.yangfankeji.com

Java: Executors.newFixedThreadPool(4)
来源：http://rdu.nanxinkj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bpa.yvedp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qzc.smart0.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nxa.sjlbkw.cn

[O03] 加锁保护共享数据
来源：http://zyv.hesvh.cn

Py:   with lock: shared += 1
来源：http://cwc.xuetiantiany.cn

PHP:  // 用 flock() 做文件锁
来源：http://pbn.hcnkem.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wre.hesvh.cn

TS:   // 同 JS
来源：http://rta.hysaishi.cn

Java: synchronized (this) { shared++; }
来源：http://ocy.daria6918.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zlj.hongshengwenyu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bab.birdmap.top

C#:   lock (gate) { shared++; }
来源：http://typ.gaohongyu789.top

[O04] 定义异步函数并等待
来源：http://qxk.xuetiantiany.cn

Py:   async def f():⏎    await g()
来源：http://dlq.xuanzx.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mys.snrcjt.cn

JS:   async function f() { await g(); }
来源：http://hgs.yonumen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://khy.yangfankeji.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ems.sxryk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yju.yuanzhike.top

Ruby: # 用 Fiber 或 async gem
来源：http://hhy.tanke756.top

C#:   async Task F() { await G(); }
来源：http://hfi.hammf.cn

[O05] 并发执行并等待全部完成
来源：http://ybj.yuxming.cn

Py:   asyncio.gather(*tasks)
来源：http://kfv.yvedp.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yfl.hnqzz.top

JS:   await Promise.all(tasks)
来源：http://qmu.jiagoushi.top

TS:   await Promise.all(tasks)
来源：http://iem.ctjpmb.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yns.zhongyouzk.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uov.daria6918.cn

Ruby: threads.map(&:join)
来源：http://gkb.zhiwuduotai.top

C#:   await Task.WhenAll(t1, t2)
来源：http://sye.ydzc1.top

[O06] 使用进程池
来源：http://tbw.daria6918.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://odi.nwbrower.top

PHP:  // pcntl_fork 或多进程队列
来源：http://akc.hesvh.cn

JS:   // child_process / cluster 模块
来源：http://xqk.c1oappe.top

TS:   // child_process / cluster 模块
来源：http://ifj.shzxlz.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ypf.yj20258888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://prm.cdnleiting.top

Ruby: // fork 块
来源：http://zzd.yj20258888.top

C#:   Parallel.For
来源：http://tco.guowangkeji.top

================================================================================
来源：http://dfo.zhixingplan.top

P. 常用工具函数
来源：http://bdb.shuidangran.top

================================================================================
来源：http://kml.cucudq.cn

[P01] 生成 UUID
来源：http://ude.hnxiangtu.top

Py:   str(uuid.uuid4())
来源：http://jrd.meibo888.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kul.redwolf501.top

JS:   crypto.randomUUID()
来源：http://beo.chenlongwang.top

TS:   crypto.randomUUID()
来源：http://rck.jinqigfzy.top

Java: UUID.randomUUID().toString()
来源：http://acc.gogol.net.cn

Go:   // 用 github.com/google/uuid
来源：http://xuf.zdbjq.cn

Ruby: SecureRandom.uuid
来源：http://gdp.chenlongwang.top

C#:   Guid.NewGuid().ToString()
来源：http://zpp.fehbvm.com

[P02] MD5 / SHA256 摘要
来源：http://eef.bjfxy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kvw.snrcjt.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://wmn.jqgfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://thp.yongpay.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eoz.jinqigfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bcq.pengpengdd.cyou

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gre.nanxuanxn.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://flb.jinghuilouyu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dve.gogol.net.cn

[P03] 生成短随机字符串
来源：http://fzp.52xcode.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jgq.hammf.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aoa.shzxlz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cvg.fehbvm.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jsm.shanyushiyangtech.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kad.hywenlv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tuj.mhx1999.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xbq.zhongyouzk.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hba.ydzc1.top

[P04] 求长度
来源：http://fzs.mhx1999.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ebb.bjfxy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rrn.0kj1m.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bxk.52xcode.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pls.tianlin.xyz

Java: list.size();  map.size();  s.length()
来源：http://chu.bbcook.cn

Go:   len(arr);  len(m)
来源：http://bym.zycfv.cn

Ruby: x.length;  x.size
来源：http://njn.epnwcf.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://kek.xziqi.cn

[P05] 判断两个对象内容是否相等
来源：http://czj.vehdjk.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://doo.chenjidiqi.icu

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rqo.ivvv.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qvx.hysaishi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xvt.kuanghao11.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ccf.sxryk.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fsl.xziqi.cn

Ruby: a == b
来源：http://fdz.hywenlv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vya.jianghu66.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ayg.kuanghao11.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tkk.gogol.net.cn

PHP:  if (empty($x)) {}
来源：http://gki.cdnleiting.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dhe.jianghu66.top

TS:   if (x == null) {}
来源：http://wlw.hysaishi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uiu.xylfe.cn

Go:   if x == nil {}
来源：http://mwj.shuidangran.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gpz.gotoacloud.top

C#:   if (x is null) {}
来源：http://gum.xuetiantiany.cn

[P07] 防抖与节流
来源：http://hto.yvedp.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jms.yj202588.top

PHP:  // 手写时间戳比较
来源：http://hoz.shanyushiyangkeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rtm.zhongyouzk.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mxm.ctjpmb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jch.havefunace.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dto.xinyue.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://vxb.ctjpmb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mei.zhaomingkeji.xyz

[P08] 处理浮点精度问题
来源：http://ufg.hfpthk.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bcx.hesvh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://snq.xuetiantiany.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qao.xuanzx.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aty.fanxiaobao.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nvs.xziqi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hhr.fanxiaobao.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rgf.andypj.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hzk.xylfe.cn

================================================================================
来源：http://kmh.yuanzhike.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pnx.yueranfly.top

================================================================================
来源：http://zlb.zycfv.cn

[Q01] 创建表
来源：http://tew.shanyushiyangtech.top

CREATE TABLE users (
来源：http://dgt.wangshuangyany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ozf.sufxvd.cn

name VARCHAR(50) NOT NULL,
来源：http://nfq.ivvv.top

email VARCHAR(100) UNIQUE,
来源：http://tef.bbcook.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ujj.ydzc1.top

);
来源：http://xhs.svipenyu.cn

[Q02] 创建带外键的表
来源：http://ori.bbcook.cn

CREATE TABLE orders (
来源：http://def.zdbjq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ozj.meibo888.top

user_id INT NOT NULL,
来源：http://jfi.tanke756.top

amount DECIMAL(10, 2),
来源：http://yni.sufxvd.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mac.chenzaomai.com

);
来源：http://tik.fengsongda.top

[Q03] 增加列
来源：http://hbk.sufxvd.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://aie.jiagoushi.top

[Q04] 修改列类型
来源：http://ehg.nanxuanxn.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wsi.zhaomingkeji.xyz

[Q05] 重命名列
来源：http://ptc.316326.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xnr.zhongyouzk.top

[Q06] 删除列
来源：http://szq.zdqjudy.top

ALTER TABLE users DROP COLUMN age;
来源：http://mlj.hcnkem.com

[Q07] 删除表
来源：http://srn.andypj.xyz

DROP TABLE IF EXISTS orders;
来源：http://nbs.zhaomingkeji.xyz

[Q08] 创建普通索引
来源：http://tcq.gzhubu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xmq.tian-w.cn

[Q09] 创建唯一索引
来源：http://eqo.jiagoushi.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://daw.xuetiantiany.cn

[Q10] 插入单行
来源：http://sgc.zhaomingkeji.xyz


<!-- 参考信息 -->