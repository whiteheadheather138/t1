代发 wailian999

Ruby: exit 1
来源：http://wpk.0kj1m.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pon.316326.xyz

[M06] 向标准错误输出
来源：http://btg.cqqwz.cn

Py:   print("err", file=sys.stderr)
来源：http://qcp.birdmap.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gax.316326.xyz

JS:   console.error("err")
来源：http://ztl.zhijiandao.cn

TS:   console.error("err")
来源：http://srz.52xcode.cn

Java: System.err.println("err")
来源：http://zkt.shzxlz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://afn.meibo888.top

Ruby: warn "err"
来源：http://ggr.gzhubu.top

C#:   Console.Error.WriteLine("err")
来源：http://hpx.ydzc1.top

[M07] 判断是否为主入口
来源：http://uxy.hongshengwenyu.top

Py:   if __name__ == "__main__":
来源：http://eds.hysaishi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xib.ywan-chungtsiang.top

JS:   require.main === module
来源：http://qgu.feifeiyinyue.top

TS:   require.main === module
来源：http://obx.uphjek.com

Java: public static void main(String[] args)
来源：http://mam.hesvh.cn

Go:   func main()
来源：http://akc.shuidangran.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qas.cheryme.top

C#:   static void Main(string[] args)
来源：http://bqw.hammf.cn

[M08] 获取系统与运行时信息
来源：http://bov.smart0.xyz

Py:   platform.system();  platform.python_version()
来源：http://epz.xuanzx.com

PHP:  PHP_OS;  phpversion();
来源：http://sxb.hnxiangtu.top

JS:   process.platform;  process.version
来源：http://aer.feifeiyinyue.top

TS:   process.platform;  process.version
来源：http://sll.fanxiaobao.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fjk.nwbrower.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vzr.hnqzz.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xtj.fktsv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://uqs.yueranfly.top

================================================================================
来源：http://pbb.hfpthk.cn

N. 数据结构与算法
来源：http://uvj.gogol.net.cn

================================================================================
来源：http://ocj.tarul.cn

[N01] 二分查找（有序数组）
来源：http://ojv.bbcook.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mnw.nwbrower.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zcx.fengsongda.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sou.hammf.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cwq.cqqwz.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qlo.yueranfly.top

Go:   sort.SearchInts(arr, x)
来源：http://ubd.iojbl.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://arf.wangdashe.top

C#:   Array.BinarySearch(arr, x)
来源：http://rbp.tian-w.cn

[N02] 排序（工程实践用内置实现）
来源：http://lnb.sxryk.cn

Py:   sorted(arr);  arr.sort()
来源：http://cmm.svipenyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bkc.cheryme.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fko.sweek.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://vjx.fzhhl.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zbl.jinqigfzy.top

Go:   slices.Sort(arr)
来源：http://wjo.jinghuilouyu.cn

Ruby: arr.sort
来源：http://bhb.fktsv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zfn.hysaishi.cn

[N03] 快速排序（分治示例）
来源：http://gwj.zhongyouzk.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://whj.0kj1m.cn

PHP:  // 递归实现，或用 usort
来源：http://tlp.jlsjyb.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://czi.vehdjk.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://etv.shanyushiyangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jmh.cdnleiting.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vyu.shangyingyoupin.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://uuq.chenzaomai.com

C#:   // 手写递归，或 Array.Sort
来源：http://jgv.ppjwa.cn

[N04] 斐波那契数列
来源：http://uhc.epnwcf.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://thc.sxryk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dxg.jlsjyb.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gub.redwolf501.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wtd.zhijiandao.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eqt.guowangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://trt.jinqigufen.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jfk.nanxuanxn.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ddm.chenjidiqi.icu

[N05] 最大公约数
来源：http://heo.wangshuangyany.cn

Py:   math.gcd(a, b)
来源：http://rzc.shangyingyoupin.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bqz.havefunace.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dne.yj20258.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ndr.yanxiufei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ybh.gzhubu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pau.svipenyu.cn

Ruby: a.gcd(b)
来源：http://yxf.52xcode.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vey.zhongyouzk.top

[N06] 判断回文字符串
来源：http://xwr.jinghuilouyu.cn

Py:   s == s[::-1]
来源：http://niv.cdnleiting.top

PHP:  $s === strrev($s);
来源：http://cdl.jinyuanbaomall.cn

JS:   s === [...s].reverse().join("")
来源：http://yqc.tianlin.xyz

TS:   s === [...s].reverse().join("")
来源：http://ubq.jinyuanbaomall.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hmn.cqqwz.cn

Go:   // 双指针从两端比较
来源：http://oux.cashguo.top

Ruby: s == s.reverse
来源：http://ujd.feifeiyinyue.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://puo.cheryme.top

[N07] 两数之和（返回下标）
来源：http://wqa.vqdsnc.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://brl.xuetiantiany.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vno.sxryk.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gun.uphjek.com

TS:   // 手写 Map<string, number>
来源：http://npb.yfazqb.com

Java: // 手写 HashMap
来源：http://xmw.vqdsnc.cn

Go:   // 手写 map[int]int
来源：http://ifq.nanxinkj.top

Ruby: // 手写 Hash
来源：http://hix.c1oappe.top

C#:   // 手写 Dictionary<int, int>
来源：http://yto.quarkkingdee.top

[N08] 生成全排列
来源：http://luj.meibo888.top

Py:   itertools.permutations(arr)
来源：http://slw.jiagoushi.top

PHP:  // 手写递归交换
来源：http://rel.jinqigfzy.top

JS:   // 手写回溯递归
来源：http://lyy.jinqigfzy.top

TS:   // 手写回溯递归
来源：http://kip.guowangkeji.top

Java: // 手写回溯递归
来源：http://rui.0kj1m.cn

Go:   // 手写回溯递归
来源：http://psh.zhoulong.xyz

Ruby: arr.permutation.to_a
来源：http://prf.hesvh.cn

C#:   // 手写回溯递归
来源：http://zev.gotoacloud.top

[N09] 栈与队列
来源：http://fvk.xylfe.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uon.yj20258.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://qbw.zhengqikj.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://abb.feifeiyinyue.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xqi.sxryk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vys.gaohongyu789.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://kon.ehwqpu.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://esx.shangyingyoupin.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gzj.jiagoushi.top

[N10] 链表节点定义
来源：http://vyc.yueranfly.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hbm.fehbvm.com

PHP:  class Node { public $v; public $next = null; }
来源：http://gox.daria6918.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://dst.chenlongwang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fho.tanke756.top

Java: class Node { int v; Node next; }
来源：http://qur.fktsv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://frq.xziqi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://kmi.tarul.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jbv.ydjk.org.cn

[N11] 二叉树中序遍历
来源：http://klj.hongshengwenyu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dzc.hcnkem.com

PHP:  // 手写递归函数
来源：http://okx.hcnkem.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ism.fktsv.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mdg.ivvv.top

Java: // 手写递归
来源：http://wur.zhiwuduotai.top

Go:   // 手写递归
来源：http://ylx.yonumen.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qcb.yvedp.cn

C#:   // 手写递归
来源：http://inq.haohaochexian.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yzo.vqdsnc.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nzm.haohaochexian.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://xgc.gogol.net.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mhs.zhongyouzk.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vle.gotoacloud.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ajo.zhoulong.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yhp.guannengcc.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uhf.yvedp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qwi.jinqigufen.top

================================================================================
来源：http://kmh.sufxvd.cn

O. 并发与异步
来源：http://zfo.ctjpmb.com

================================================================================
来源：http://sez.nanxinkj.top

[O01] 启动一个线程
来源：http://iel.xuanzx.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://djl.haohaochexian.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://siw.shanyushiyangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vzv.zhongyouzk.top

TS:   // 同 JS
来源：http://psa.aizwys.cn

Java: new Thread(() -> f()).start()
来源：http://bwo.chenzaomai.com

Go:   go f()
来源：http://zyh.ctjpmb.com

Ruby: Thread.new { f }
来源：http://hzm.ydjk.org.cn

C#:   Task.Run(() => F());
来源：http://ceg.chenjidiqi.icu

[O02] 使用线程池
来源：http://ump.gotoacloud.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yrc.yonumen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pta.yuxming.cn

JS:   // worker_threads 线程池
来源：http://gpn.cdnleiting.top

TS:   // worker_threads 线程池
来源：http://szh.cqqwz.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dna.xingfuxueyuan.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pfb.ppjwa.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://txi.shanyushiyangtech.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ujg.tianlin.xyz

[O03] 加锁保护共享数据
来源：http://ljh.sufxvd.cn

Py:   with lock: shared += 1
来源：http://qfq.shuidangran.top

PHP:  // 用 flock() 做文件锁
来源：http://ajq.aizwys.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vwj.chenjidiqi.icu

TS:   // 同 JS
来源：http://sev.chenzaomai.com

Java: synchronized (this) { shared++; }
来源：http://lrn.jinqigfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zrp.xylfe.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qso.vehdjk.com

C#:   lock (gate) { shared++; }
来源：http://uqu.jqgfzy.top

[O04] 定义异步函数并等待
来源：http://pkg.yueranfly.top

Py:   async def f():⏎    await g()
来源：http://com.9152youxi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pnm.dashuyun.cn

JS:   async function f() { await g(); }
来源：http://cst.ydjk.org.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lmn.jqgfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://djo.hywenlv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nqp.ctjpmb.com

Ruby: # 用 Fiber 或 async gem
来源：http://dsc.pengpengdd.cyou

C#:   async Task F() { await G(); }
来源：http://fri.chenlongwang.top

[O05] 并发执行并等待全部完成
来源：http://ueh.vqdsnc.cn

Py:   asyncio.gather(*tasks)
来源：http://csy.chenlongwang.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ewv.yj20258.top

JS:   await Promise.all(tasks)
来源：http://fwi.zhongyouzk.top

TS:   await Promise.all(tasks)
来源：http://dtn.hammf.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://agt.feifeiyinyue.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eek.cdnleiting.top

Ruby: threads.map(&:join)
来源：http://rgc.birdmap.top

C#:   await Task.WhenAll(t1, t2)
来源：http://yll.gaohongyu789.top

[O06] 使用进程池
来源：http://mjc.zhengqikj.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yhh.guowangkeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zje.shangyingyoupin.top

JS:   // child_process / cluster 模块
来源：http://wvk.uphjek.com

TS:   // child_process / cluster 模块
来源：http://cbq.zhaomingkeji.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sys.hywenlv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mmg.ybcxt.top

Ruby: // fork 块
来源：http://cod.tianlin.xyz

C#:   Parallel.For
来源：http://tzc.jyoumei.cn

================================================================================
来源：http://zzz.ivvv.top

P. 常用工具函数
来源：http://vfv.dashuyun.cn

================================================================================
来源：http://lub.yangfankeji.com

[P01] 生成 UUID
来源：http://zod.jqgfzy.top

Py:   str(uuid.uuid4())
来源：http://gub.chenzaomai.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ktn.zhiwuduotai.top

JS:   crypto.randomUUID()
来源：http://mji.hongshengwenyu.top

TS:   crypto.randomUUID()
来源：http://zmg.bjfxy.top

Java: UUID.randomUUID().toString()
来源：http://gdx.kuanghao11.cn

Go:   // 用 github.com/google/uuid
来源：http://omh.epnwcf.com

Ruby: SecureRandom.uuid
来源：http://wzz.jinyuanbaomall.cn

C#:   Guid.NewGuid().ToString()
来源：http://tvk.guowangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://zjg.fzhhl.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://unn.yvedp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://rju.chenlongwang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://drs.jianghu66.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wwk.kuanghao11.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mhu.nanxinkj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mgl.xuanzx.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gty.sjlbkw.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rcl.hongshengwenyu.top

[P03] 生成短随机字符串
来源：http://jou.uphjek.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dnu.yj20258.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://txw.fktsv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://myd.feifeiyinyue.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fvf.aibaodan.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://edg.yueranfly.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lnj.ywan-chungtsiang.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://kxx.ydzc1.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gca.chenzaomai.com

[P04] 求长度
来源：http://ouh.aibaodan.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qum.ehwqpu.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kpg.chenzaomai.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rep.bbcook.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eek.jinqigufen.top

Java: list.size();  map.size();  s.length()
来源：http://sym.zycfv.cn

Go:   len(arr);  len(m)
来源：http://lnz.hnqzz.top

Ruby: x.length;  x.size
来源：http://nwo.cdnleiting.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://aoc.0kj1m.cn

[P05] 判断两个对象内容是否相等
来源：http://log.sjlbkw.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://jxi.hnxiangtu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hmn.nanxinkj.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ggk.cqqwz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hba.birdmap.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rdy.52xcode.cn

Go:   reflect.DeepEqual(a, b)
来源：http://nsl.iojbl.cn

Ruby: a == b
来源：http://ikg.gotoacloud.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://har.smart0.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yav.ydzc1.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://leb.ywan-chungtsiang.top

PHP:  if (empty($x)) {}
来源：http://ojx.zdbjq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pqu.jiagoushi.top

TS:   if (x == null) {}
来源：http://rvs.fehbvm.com

Java: if (x == null || x.isEmpty()) {}
来源：http://ufg.andypj.xyz

Go:   if x == nil {}
来源：http://etb.cashguo.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://iby.zhiwuduotai.top

C#:   if (x is null) {}
来源：http://kfr.tianlin.xyz

[P07] 防抖与节流
来源：http://nkq.mhx1999.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://msg.xuetiantiany.cn

PHP:  // 手写时间戳比较
来源：http://cgx.yanxiufei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://imz.yj202588.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xio.zhoulong.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yng.quarkkingdee.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rqz.dashuyun.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://izn.52xcode.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kba.aibaodan.cn

[P08] 处理浮点精度问题
来源：http://kjb.meibo888.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://psy.havefunace.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sds.ydjk.org.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://akx.gaohongyu789.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cbv.gzhubu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ieh.nanxuanxn.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zud.feifeiyinyue.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rab.uphjek.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mxl.jqgufenzy.top

================================================================================
来源：http://axn.yj20258888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hbe.yj20258888.top

================================================================================
来源：http://ycm.fanxiaobao.xyz

[Q01] 创建表
来源：http://gnx.sjlbkw.cn

CREATE TABLE users (
来源：http://sad.hongshengwenyu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sae.fzhhl.top

name VARCHAR(50) NOT NULL,
来源：http://iey.sufxvd.cn

email VARCHAR(100) UNIQUE,
来源：http://vle.ehwqpu.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jid.daria6918.cn

);
来源：http://akz.hammf.cn

[Q02] 创建带外键的表
来源：http://avp.andypj.xyz

CREATE TABLE orders (
来源：http://lma.yangfankeji.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lbk.xinyue.icu

user_id INT NOT NULL,
来源：http://uro.jinghuilouyu.cn

amount DECIMAL(10, 2),
来源：http://pyi.bbcook.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pzw.ppjwa.cn

);
来源：http://uqk.ivvv.top

[Q03] 增加列
来源：http://jow.mhx1999.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zrc.sjlbkw.cn

[Q04] 修改列类型
来源：http://ekv.zhijiandao.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qgh.nanxinkj.top

[Q05] 重命名列
来源：http://fll.ydjk.org.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qbm.zhoulong.xyz

[Q06] 删除列
来源：http://rcc.wangdashe.top

ALTER TABLE users DROP COLUMN age;
来源：http://uuf.zycfv.cn

[Q07] 删除表
来源：http://uai.hysaishi.cn

DROP TABLE IF EXISTS orders;
来源：http://qvp.sjlbkw.cn

[Q08] 创建普通索引
来源：http://uta.dianchejie.cn


<!-- 参考信息 -->