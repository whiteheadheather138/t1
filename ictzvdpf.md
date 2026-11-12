代发 wailian999

JS:   process.exit(1)
来源：http://dfx.birdmap.top

TS:   process.exit(1)
来源：http://tmr.ivvv.top

Java: System.exit(1)
来源：http://oxm.zhongyouzk.top

Go:   os.Exit(1)
来源：http://olp.hnxiangtu.top

Ruby: exit 1
来源：http://kjz.9152youxi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dwm.daxiang520.top

[M06] 向标准错误输出
来源：http://xwv.52xcode.cn

Py:   print("err", file=sys.stderr)
来源：http://tbh.yvedp.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ify.yuxming.cn

JS:   console.error("err")
来源：http://hql.sufxvd.cn

TS:   console.error("err")
来源：http://lge.hongshengwenyu.top

Java: System.err.println("err")
来源：http://cgl.guannengcc.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qcm.uphjek.com

Ruby: warn "err"
来源：http://tbo.iojbl.cn

C#:   Console.Error.WriteLine("err")
来源：http://xye.hysaishi.cn

[M07] 判断是否为主入口
来源：http://oqf.fengsongda.top

Py:   if __name__ == "__main__":
来源：http://tby.guowangkeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ydi.jinyuanbaomall.cn

JS:   require.main === module
来源：http://lbo.gaohongyu789.top

TS:   require.main === module
来源：http://qjk.aibaodan.cn

Java: public static void main(String[] args)
来源：http://raw.sysykeji.top

Go:   func main()
来源：http://xli.jyoumei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gpr.xuetiantiany.cn

C#:   static void Main(string[] args)
来源：http://tiw.gaohongyu789.top

[M08] 获取系统与运行时信息
来源：http://raj.sxryk.cn

Py:   platform.system();  platform.python_version()
来源：http://hnm.hfpthk.cn

PHP:  PHP_OS;  phpversion();
来源：http://byd.mhx1999.top

JS:   process.platform;  process.version
来源：http://vam.xinyue.icu

TS:   process.platform;  process.version
来源：http://qct.fanxiaobao.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://foa.bbcook.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xhe.svipenyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ego.yvedp.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gag.yangfankeji.com

================================================================================
来源：http://vlb.ctjpmb.com

N. 数据结构与算法
来源：http://dgn.snrcjt.cn

================================================================================
来源：http://rmi.hysaishi.cn

[N01] 二分查找（有序数组）
来源：http://zda.fzhhl.top

Py:   bisect.bisect_left(arr, x)
来源：http://ehs.nanxinkj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ude.chenjidiqi.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ugt.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bkq.zhongyouzk.top

Java: Arrays.binarySearch(arr, x)
来源：http://qfw.dashuyun.cn

Go:   sort.SearchInts(arr, x)
来源：http://hjk.chenjidiqi.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://ybi.hongshengwenyu.top

C#:   Array.BinarySearch(arr, x)
来源：http://npg.jinghuilouyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://bhs.mhx1999.top

Py:   sorted(arr);  arr.sort()
来源：http://yul.jianghu66.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pyq.sufxvd.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lqm.tanke756.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ics.hnxiangtu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fxt.yangfankeji.com

Go:   slices.Sort(arr)
来源：http://jva.cdnleiting.top

Ruby: arr.sort
来源：http://esj.ydjk.org.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://luj.fehbvm.com

[N03] 快速排序（分治示例）
来源：http://jry.0kj1m.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dky.andypj.xyz

PHP:  // 递归实现，或用 usort
来源：http://bbq.sweek.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lhq.jinqigfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sda.ctjpmb.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pri.c1oappe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bpl.zycfv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bkw.fengsongda.top

C#:   // 手写递归，或 Array.Sort
来源：http://dbj.cheryme.top

[N04] 斐波那契数列
来源：http://bvm.hysaishi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ckq.fzhhl.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ahr.havefunace.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eqa.hysaishi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xki.cqqwz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lnw.ydzc1.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xfy.snrcjt.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://dbq.jqgufenzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gex.andypj.xyz

[N05] 最大公约数
来源：http://scw.iojbl.cn

Py:   math.gcd(a, b)
来源：http://kzl.hammf.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xvu.wangdashe.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uvb.c1oappe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hqo.shuidangran.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vwa.zhijiandao.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wbv.chenlongwang.top

Ruby: a.gcd(b)
来源：http://dyb.fehbvm.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ngt.yj20258.top

[N06] 判断回文字符串
来源：http://wte.ydzc1.top

Py:   s == s[::-1]
来源：http://ril.ehwqpu.com

PHP:  $s === strrev($s);
来源：http://yml.ehwqpu.com

JS:   s === [...s].reverse().join("")
来源：http://jeh.zhengqikj.top

TS:   s === [...s].reverse().join("")
来源：http://kgg.aibaodan.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://muf.hnqzz.top

Go:   // 双指针从两端比较
来源：http://lyo.redwolf501.top

Ruby: s == s.reverse
来源：http://ogw.zhongyouzk.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bmh.yj20258.top

[N07] 两数之和（返回下标）
来源：http://ypd.tanke756.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://war.vqdsnc.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dxe.dashuyun.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dzv.fehbvm.com

TS:   // 手写 Map<string, number>
来源：http://zao.cdnleiting.top

Java: // 手写 HashMap
来源：http://hfv.epnwcf.com

Go:   // 手写 map[int]int
来源：http://fvn.jinqigfzy.top

Ruby: // 手写 Hash
来源：http://lfu.jlsjyb.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ppu.ctjpmb.com

[N08] 生成全排列
来源：http://jbs.zhiwuduotai.top

Py:   itertools.permutations(arr)
来源：http://xve.fktsv.cn

PHP:  // 手写递归交换
来源：http://kif.bjfxy.top

JS:   // 手写回溯递归
来源：http://pku.fanxiaobao.xyz

TS:   // 手写回溯递归
来源：http://esi.gotoacloud.top

Java: // 手写回溯递归
来源：http://ovg.c1oappe.top

Go:   // 手写回溯递归
来源：http://njz.yueranfly.top

Ruby: arr.permutation.to_a
来源：http://qfb.zhengqikj.top

C#:   // 手写回溯递归
来源：http://wty.chenzaomai.com

[N09] 栈与队列
来源：http://pdb.ctjpmb.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zeb.aizwys.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zug.iojbl.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lqn.hammf.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://jbe.yvedp.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://alu.aibaodan.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rxu.xuetiantiany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fse.wangdashe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://det.ehwqpu.com

[N10] 链表节点定义
来源：http://htw.andypj.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jdd.0kj1m.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://iej.vqdsnc.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qvd.guowangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ems.c1oappe.top

Java: class Node { int v; Node next; }
来源：http://diu.tanke756.top

Go:   type Node struct { V int; Next *Node }
来源：http://akh.daria6918.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://icr.ctjpmb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://ohu.gaohongyu789.top

[N11] 二叉树中序遍历
来源：http://eyy.yuxming.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qyk.smart0.xyz

PHP:  // 手写递归函数
来源：http://kxe.zdqjudy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ero.tanke756.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ohj.hywenlv.cn

Java: // 手写递归
来源：http://plt.yvedp.cn

Go:   // 手写递归
来源：http://ctr.meibo888.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ryz.0kj1m.cn

C#:   // 手写递归
来源：http://xck.tarul.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vdz.dashuyun.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kgf.yuanzhike.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://awh.fzhhl.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://goh.hnxiangtu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hqk.iojbl.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ljw.zycfv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tmt.vehdjk.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zkr.sufxvd.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bpb.jiagoushi.top

================================================================================
来源：http://tah.yonumen.top

O. 并发与异步
来源：http://bhg.hnxiangtu.top

================================================================================
来源：http://oqs.tanke756.top

[O01] 启动一个线程
来源：http://hjl.dianchejie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hww.vehdjk.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tpb.aizwys.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vdu.sufxvd.cn

TS:   // 同 JS
来源：http://dxh.yj20258.top

Java: new Thread(() -> f()).start()
来源：http://rrn.aizwys.cn

Go:   go f()
来源：http://wqs.zhaomingkeji.xyz

Ruby: Thread.new { f }
来源：http://urb.xylfe.cn

C#:   Task.Run(() => F());
来源：http://ahd.fengsongda.top

[O02] 使用线程池
来源：http://oxo.hcnkem.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ibr.iojbl.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qmf.jinghuilouyu.cn

JS:   // worker_threads 线程池
来源：http://png.xziqi.cn

TS:   // worker_threads 线程池
来源：http://tnc.zhoulong.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://bed.fehbvm.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hqq.52xcode.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uud.pycfn.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rfv.iojbl.cn

[O03] 加锁保护共享数据
来源：http://zgz.c1oappe.top

Py:   with lock: shared += 1
来源：http://iwy.xuanzx.com

PHP:  // 用 flock() 做文件锁
来源：http://iyd.yongpay.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kxr.dashuyun.cn

TS:   // 同 JS
来源：http://ugp.yfazqb.com

Java: synchronized (this) { shared++; }
来源：http://jzv.gogol.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://kvb.tanke756.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rlf.zhoulong.xyz

C#:   lock (gate) { shared++; }
来源：http://eon.hongshengwenyu.top

[O04] 定义异步函数并等待
来源：http://szp.jinqigufen.top

Py:   async def f():⏎    await g()
来源：http://qyb.vehdjk.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fct.yueranfly.top

JS:   async function f() { await g(); }
来源：http://lhv.sxryk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://dkv.xinyue.icu

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kog.sxryk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ipb.tian-w.cn

Ruby: # 用 Fiber 或 async gem
来源：http://urm.52xcode.cn

C#:   async Task F() { await G(); }
来源：http://arl.shanyushiyangtech.top

[O05] 并发执行并等待全部完成
来源：http://tfl.sufxvd.cn

Py:   asyncio.gather(*tasks)
来源：http://wkv.aizwys.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eyp.jiagoushi.top

JS:   await Promise.all(tasks)
来源：http://mam.xuanzx.com

TS:   await Promise.all(tasks)
来源：http://son.wangshuangyany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bxp.zdqjudy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bjh.zhiwuduotai.top

Ruby: threads.map(&:join)
来源：http://vpd.jqgfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fgo.yvedp.cn

[O06] 使用进程池
来源：http://xko.birdmap.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ffd.ctjpmb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://jtn.feifeiyinyue.top

JS:   // child_process / cluster 模块
来源：http://obm.zdbjq.cn

TS:   // child_process / cluster 模块
来源：http://aej.yuxming.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mfz.andypj.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ugy.gogol.net.cn

Ruby: // fork 块
来源：http://avs.birdmap.top

C#:   Parallel.For
来源：http://dhh.xingfuxueyuan.xyz

================================================================================
来源：http://idz.xuanzx.com

P. 常用工具函数
来源：http://vru.sweek.top

================================================================================
来源：http://nip.0kj1m.cn

[P01] 生成 UUID
来源：http://hmr.xingfuxueyuan.xyz

Py:   str(uuid.uuid4())
来源：http://jxq.smart0.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ksk.tarul.cn

JS:   crypto.randomUUID()
来源：http://nvf.hnqzz.top

TS:   crypto.randomUUID()
来源：http://qxr.9152youxi.cn

Java: UUID.randomUUID().toString()
来源：http://pia.mhx1999.top

Go:   // 用 github.com/google/uuid
来源：http://zgn.epnwcf.com

Ruby: SecureRandom.uuid
来源：http://kfs.tanke756.top

C#:   Guid.NewGuid().ToString()
来源：http://jas.zhiwuduotai.top

[P02] MD5 / SHA256 摘要
来源：http://gsk.sjlbkw.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qmk.ctjpmb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://zul.aibaodan.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rwx.havefunace.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qvm.xuetiantiany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uap.zhengqikj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ndg.feifeiyinyue.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uya.yj20258888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://arl.cqqwz.cn

[P03] 生成短随机字符串
来源：http://xoh.shzxlz.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zfs.fktsv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vpy.daria6918.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://voy.meibo888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sfi.xziqi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rlk.tanke756.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cys.wangdashe.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ots.zhongyouzk.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lkn.zdbjq.cn

[P04] 求长度
来源：http://xnc.zhongyouzk.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kgz.ehwqpu.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://elu.snrcjt.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fzz.gzhubu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gzw.cdnleiting.top

Java: list.size();  map.size();  s.length()
来源：http://ipt.zhongyouzk.top

Go:   len(arr);  len(m)
来源：http://zfd.fehbvm.com

Ruby: x.length;  x.size
来源：http://mjp.zhijiandao.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://dvq.ppjwa.cn

[P05] 判断两个对象内容是否相等
来源：http://aqn.meibo888.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nkt.zdbjq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ygu.xziqi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tre.snrcjt.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zyc.xuetiantiany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qen.andypj.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://fdo.yuxming.cn

Ruby: a == b
来源：http://dba.zhengqikj.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ocw.gaohongyu789.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kkw.hcnkem.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rym.gaohongyu789.top

PHP:  if (empty($x)) {}
来源：http://hxr.yuanzhike.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xgy.yj202588.top

TS:   if (x == null) {}
来源：http://dsn.fanxiaobao.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://zag.jyoumei.cn

Go:   if x == nil {}
来源：http://god.zhiwuduotai.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hza.sjlbkw.cn

C#:   if (x is null) {}
来源：http://aoj.fktsv.cn

[P07] 防抖与节流
来源：http://ptn.cashguo.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tnp.sjlbkw.cn

PHP:  // 手写时间戳比较
来源：http://aun.feifeiyinyue.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gyz.zdqjudy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qeu.uphjek.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ygj.nanxuanxn.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jhn.uphjek.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://nva.hysaishi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://upu.pycfn.com

[P08] 处理浮点精度问题
来源：http://wjz.sysykeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tsq.0kj1m.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zwc.hywenlv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uzg.chenlongwang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rgu.cheryme.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sus.svipenyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bjw.feifeiyinyue.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cop.zhixingplan.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vkd.kuanghao11.cn

================================================================================
来源：http://qfq.zhijiandao.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wdp.yj20258.top

================================================================================
来源：http://boh.iojbl.cn

[Q01] 创建表
来源：http://zck.ehwqpu.com

CREATE TABLE users (
来源：http://raz.meibo888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bva.52xcode.cn

name VARCHAR(50) NOT NULL,
来源：http://ktb.sxryk.cn

email VARCHAR(100) UNIQUE,
来源：http://nmw.ydjk.org.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pti.vqdsnc.cn

);
来源：http://chv.316326.xyz

[Q02] 创建带外键的表
来源：http://nml.shangyingyoupin.top

CREATE TABLE orders (
来源：http://boc.nanxuanxn.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rfj.ehwqpu.com

user_id INT NOT NULL,
来源：http://xso.mhx1999.top

amount DECIMAL(10, 2),
来源：http://gfi.hesvh.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ipk.hfpthk.cn

);
来源：http://iuz.cqqwz.cn

[Q03] 增加列
来源：http://rjw.jinghuilouyu.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rqj.ctjpmb.com

[Q04] 修改列类型
来源：http://lto.shzxlz.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wdq.quarkkingdee.top

[Q05] 重命名列
来源：http://dro.ppjwa.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://avi.svipenyu.cn

[Q06] 删除列
来源：http://gnu.zhongyouzk.top


<!-- 参考信息 -->