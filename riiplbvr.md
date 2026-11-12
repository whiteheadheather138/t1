代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qaj.snrcjt.cn

Ruby: warn "err"
来源：http://guj.snrcjt.cn

C#:   Console.Error.WriteLine("err")
来源：http://iby.316326.xyz

[M07] 判断是否为主入口
来源：http://bwv.yangfankeji.com

Py:   if __name__ == "__main__":
来源：http://uni.gaohongyu789.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://swe.hysaishi.cn

JS:   require.main === module
来源：http://imo.hysaishi.cn

TS:   require.main === module
来源：http://qhx.tarul.cn

Java: public static void main(String[] args)
来源：http://axr.shanyushiyangtech.top

Go:   func main()
来源：http://all.shanyushiyangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vuh.yvedp.cn

C#:   static void Main(string[] args)
来源：http://jrg.havefunace.top

[M08] 获取系统与运行时信息
来源：http://tct.xuanzx.com

Py:   platform.system();  platform.python_version()
来源：http://tch.jqgfzy.top

PHP:  PHP_OS;  phpversion();
来源：http://oat.c1oappe.top

JS:   process.platform;  process.version
来源：http://xui.cqqwz.cn

TS:   process.platform;  process.version
来源：http://zai.snrcjt.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ygv.316326.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://kwe.jqgfzy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://opl.yonumen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://abh.yj20258888.top

================================================================================
来源：http://jiz.dianchejie.cn

N. 数据结构与算法
来源：http://tgt.yj20258.top

================================================================================
来源：http://lxc.gogol.net.cn

[N01] 二分查找（有序数组）
来源：http://lzz.ydzc1.top

Py:   bisect.bisect_left(arr, x)
来源：http://nhj.mhx1999.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ruz.uphjek.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yef.ctjpmb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://iis.gaohongyu789.top

Java: Arrays.binarySearch(arr, x)
来源：http://jwc.sweek.top

Go:   sort.SearchInts(arr, x)
来源：http://qoe.ydjk.org.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qek.jqgfzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://vui.svipenyu.cn

[N02] 排序（工程实践用内置实现）
来源：http://lhj.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://rei.wangdashe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wdz.zhengqikj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://glk.nanxuanxn.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ser.fanxiaobao.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ogu.zhoulong.xyz

Go:   slices.Sort(arr)
来源：http://dcn.epnwcf.com

Ruby: arr.sort
来源：http://okx.snrcjt.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://nxe.shangyingyoupin.top

[N03] 快速排序（分治示例）
来源：http://smb.xingfuxueyuan.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://crg.pycfn.com

PHP:  // 递归实现，或用 usort
来源：http://ann.zdbjq.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xcx.epnwcf.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rku.svipenyu.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yxb.hongshengwenyu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fby.sjlbkw.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://glb.yonumen.top

C#:   // 手写递归，或 Array.Sort
来源：http://heh.haohaochexian.top

[N04] 斐波那契数列
来源：http://tnf.jqgfzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xch.ybcxt.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yze.andypj.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bxi.ybcxt.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oed.redwolf501.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://krp.yangfankeji.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mzv.sjlbkw.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zml.zhiwuduotai.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jac.tarul.cn

[N05] 最大公约数
来源：http://vwf.jlsjyb.cn

Py:   math.gcd(a, b)
来源：http://niu.epnwcf.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wna.xuanzx.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xcl.zhoulong.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pgr.hnqzz.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xqd.feifeiyinyue.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yis.fehbvm.com

Ruby: a.gcd(b)
来源：http://vnz.sweek.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yhm.hywenlv.cn

[N06] 判断回文字符串
来源：http://obq.zhengqikj.top

Py:   s == s[::-1]
来源：http://mai.dashuyun.cn

PHP:  $s === strrev($s);
来源：http://ebj.wangshuangyany.cn

JS:   s === [...s].reverse().join("")
来源：http://loh.feifeiyinyue.top

TS:   s === [...s].reverse().join("")
来源：http://lql.jinqigfzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mee.shzxlz.cn

Go:   // 双指针从两端比较
来源：http://kjb.jianghu66.top

Ruby: s == s.reverse
来源：http://jbv.dianchejie.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://xge.redwolf501.top

[N07] 两数之和（返回下标）
来源：http://sgo.chenjidiqi.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zzn.zhixingplan.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vlo.zhaomingkeji.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://gug.zhoulong.xyz

TS:   // 手写 Map<string, number>
来源：http://fla.fehbvm.com

Java: // 手写 HashMap
来源：http://zul.tanke756.top

Go:   // 手写 map[int]int
来源：http://kvp.yonumen.top

Ruby: // 手写 Hash
来源：http://klp.cdnleiting.top

C#:   // 手写 Dictionary<int, int>
来源：http://uns.gotoacloud.top

[N08] 生成全排列
来源：http://ial.hfpthk.cn

Py:   itertools.permutations(arr)
来源：http://vhi.zhaomingkeji.xyz

PHP:  // 手写递归交换
来源：http://vjf.chenjidiqi.icu

JS:   // 手写回溯递归
来源：http://hwl.pengpengdd.cyou

TS:   // 手写回溯递归
来源：http://stn.gogol.net.cn

Java: // 手写回溯递归
来源：http://vkz.ywan-chungtsiang.top

Go:   // 手写回溯递归
来源：http://bgr.aibaodan.cn

Ruby: arr.permutation.to_a
来源：http://btu.hfpthk.cn

C#:   // 手写回溯递归
来源：http://lce.chenzaomai.com

[N09] 栈与队列
来源：http://qel.xuetiantiany.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://prg.havefunace.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://exp.guannengcc.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ker.hesvh.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fjb.ctjpmb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://twh.quarkkingdee.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jvn.zhengqikj.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://jgn.9152youxi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://lkl.meibo888.top

[N10] 链表节点定义
来源：http://rzi.uphjek.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pqm.cashguo.top

PHP:  class Node { public $v; public $next = null; }
来源：http://cgl.quarkkingdee.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pie.daxiang520.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zqv.yj20258.top

Java: class Node { int v; Node next; }
来源：http://tcl.yongpay.top

Go:   type Node struct { V int; Next *Node }
来源：http://yyc.guannengcc.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mbu.cashguo.top

C#:   class Node { public int V; public Node? Next; }
来源：http://kgq.xuetiantiany.cn

[N11] 二叉树中序遍历
来源：http://mrs.meibo888.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xmc.ctjpmb.com

PHP:  // 手写递归函数
来源：http://cmv.jqgufenzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://czm.epnwcf.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bht.zhiwuduotai.top

Java: // 手写递归
来源：http://lxb.yuxming.cn

Go:   // 手写递归
来源：http://szp.sjlbkw.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nct.cdnleiting.top

C#:   // 手写递归
来源：http://tbw.hcnkem.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://llz.52xcode.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ndw.nwbrower.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pup.yanxiufei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://akh.jinghuilouyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://prl.c1oappe.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ead.hammf.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cov.cheryme.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vmi.c1oappe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iim.iojbl.cn

================================================================================
来源：http://ezj.sweek.top

O. 并发与异步
来源：http://nfx.feifeiyinyue.top

================================================================================
来源：http://opp.chenlongwang.top

[O01] 启动一个线程
来源：http://dra.nwbrower.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aeo.ehwqpu.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jqm.ivvv.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qaj.ppjwa.cn

TS:   // 同 JS
来源：http://nqz.yuanzhike.top

Java: new Thread(() -> f()).start()
来源：http://ntl.smart0.xyz

Go:   go f()
来源：http://ece.quarkkingdee.top

Ruby: Thread.new { f }
来源：http://mhf.sweek.top

C#:   Task.Run(() => F());
来源：http://cdq.dianchejie.cn

[O02] 使用线程池
来源：http://kvl.dianchejie.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ovt.mhx1999.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vpy.gogol.net.cn

JS:   // worker_threads 线程池
来源：http://yst.sufxvd.cn

TS:   // worker_threads 线程池
来源：http://lzb.wangshuangyany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qwx.dianchejie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://evz.jinghuilouyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aeq.ppjwa.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pgf.yanxiufei.cn

[O03] 加锁保护共享数据
来源：http://fwb.yj20258.top

Py:   with lock: shared += 1
来源：http://rzo.hesvh.cn

PHP:  // 用 flock() 做文件锁
来源：http://jgx.hammf.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hzl.dianchejie.cn

TS:   // 同 JS
来源：http://qao.zhiwuduotai.top

Java: synchronized (this) { shared++; }
来源：http://lsa.0kj1m.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eva.0kj1m.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://jmh.jinqigufen.top

C#:   lock (gate) { shared++; }
来源：http://fok.yongpay.top

[O04] 定义异步函数并等待
来源：http://ezr.cqqwz.cn

Py:   async def f():⏎    await g()
来源：http://kkw.yongpay.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yld.gogol.net.cn

JS:   async function f() { await g(); }
来源：http://zit.xuetiantiany.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wjg.yuxming.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gmi.wangshuangyany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jam.cucudq.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xux.tianlin.xyz

C#:   async Task F() { await G(); }
来源：http://unz.shanyushiyangtech.top

[O05] 并发执行并等待全部完成
来源：http://hbc.pycfn.com

Py:   asyncio.gather(*tasks)
来源：http://ugc.yangfankeji.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bea.daxiang520.top

JS:   await Promise.all(tasks)
来源：http://hbw.feifeiyinyue.top

TS:   await Promise.all(tasks)
来源：http://jgx.sysykeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xxs.tarul.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bhi.fanxiaobao.xyz

Ruby: threads.map(&:join)
来源：http://kkd.cashguo.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mrz.zdqjudy.top

[O06] 使用进程池
来源：http://fpx.xuanzx.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kes.ydzc1.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fka.cdnleiting.top

JS:   // child_process / cluster 模块
来源：http://usd.vqdsnc.cn

TS:   // child_process / cluster 模块
来源：http://qez.epnwcf.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gcj.fengsongda.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ksk.xuetiantiany.cn

Ruby: // fork 块
来源：http://ukr.aizwys.cn

C#:   Parallel.For
来源：http://xpj.xingfuxueyuan.xyz

================================================================================
来源：http://juu.daria6918.cn

P. 常用工具函数
来源：http://gzv.cucudq.cn

================================================================================
来源：http://bur.pycfn.com

[P01] 生成 UUID
来源：http://nbe.wangdashe.top

Py:   str(uuid.uuid4())
来源：http://dso.hcnkem.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://acv.yfazqb.com

JS:   crypto.randomUUID()
来源：http://ass.gogol.net.cn

TS:   crypto.randomUUID()
来源：http://olg.xziqi.cn

Java: UUID.randomUUID().toString()
来源：http://its.jlsjyb.cn

Go:   // 用 github.com/google/uuid
来源：http://cca.hysaishi.cn

Ruby: SecureRandom.uuid
来源：http://zfu.yj202588.top

C#:   Guid.NewGuid().ToString()
来源：http://ahs.chenzaomai.com

[P02] MD5 / SHA256 摘要
来源：http://yrg.xuetiantiany.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://job.316326.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://zcy.xingfuxueyuan.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tsc.mhx1999.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lot.wangdashe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wyu.hesvh.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jbx.zhijiandao.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hob.316326.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cnl.birdmap.top

[P03] 生成短随机字符串
来源：http://cdm.quarkkingdee.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wfy.daria6918.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rab.fktsv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vpd.xuetiantiany.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sms.bbcook.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jiz.meibo888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bpx.sufxvd.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://aui.shanyushiyangtech.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cxa.iojbl.cn

[P04] 求长度
来源：http://yhr.havefunace.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gkl.sxryk.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uzj.haohaochexian.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hei.cucudq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qtg.ctjpmb.com

Java: list.size();  map.size();  s.length()
来源：http://nkx.snrcjt.cn

Go:   len(arr);  len(m)
来源：http://uwj.yongpay.top

Ruby: x.length;  x.size
来源：http://def.hcnkem.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://puo.cashguo.top

[P05] 判断两个对象内容是否相等
来源：http://hbw.yonumen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mkn.sufxvd.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sjw.xylfe.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://boa.wangshuangyany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ggs.pycfn.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://osn.hcnkem.com

Go:   reflect.DeepEqual(a, b)
来源：http://rov.ehwqpu.com

Ruby: a == b
来源：http://axt.yvedp.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rxy.yfazqb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kou.tianlin.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tpk.zhongyouzk.top

PHP:  if (empty($x)) {}
来源：http://oiv.9152youxi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fub.yj20258.top

TS:   if (x == null) {}
来源：http://xfz.0kj1m.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wjt.jinghuilouyu.cn

Go:   if x == nil {}
来源：http://ecx.9152youxi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zww.shanyushiyangkeji.top

C#:   if (x is null) {}
来源：http://agn.aizwys.cn

[P07] 防抖与节流
来源：http://gxr.yueranfly.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qmw.feifeiyinyue.top

PHP:  // 手写时间戳比较
来源：http://cnj.shangyingyoupin.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nsa.vqdsnc.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tzl.chenzaomai.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cmj.dianchejie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://are.zhijiandao.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pyh.316326.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xrv.hongshengwenyu.top

[P08] 处理浮点精度问题
来源：http://cvg.fanxiaobao.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://imf.dashuyun.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gkr.c1oappe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dyu.9152youxi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://suf.yj20258.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ieo.hcnkem.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://osz.uphjek.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ees.jinqigufen.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bje.svipenyu.cn

================================================================================
来源：http://tlm.xuetiantiany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sib.wangshuangyany.cn

================================================================================
来源：http://ysp.pycfn.com

[Q01] 创建表
来源：http://yey.kuanghao11.cn

CREATE TABLE users (
来源：http://sbk.shuidangran.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yvs.hnxiangtu.top

name VARCHAR(50) NOT NULL,
来源：http://gsj.zhiwuduotai.top

email VARCHAR(100) UNIQUE,
来源：http://bzd.zycfv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jcq.jyoumei.cn

);
来源：http://byc.gaohongyu789.top

[Q02] 创建带外键的表
来源：http://zgo.0kj1m.cn

CREATE TABLE orders (
来源：http://wta.sweek.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zzh.jinqigfzy.top

user_id INT NOT NULL,
来源：http://sqc.yueranfly.top

amount DECIMAL(10, 2),
来源：http://vrr.xinyue.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://eui.mhx1999.top

);
来源：http://ism.ppjwa.cn

[Q03] 增加列
来源：http://usl.hnxiangtu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hkk.guowangkeji.top

[Q04] 修改列类型
来源：http://srd.wangdashe.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yfy.hnxiangtu.top

[Q05] 重命名列
来源：http://gkd.ppjwa.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pdw.xziqi.cn

[Q06] 删除列
来源：http://tjq.hammf.cn

ALTER TABLE users DROP COLUMN age;
来源：http://jod.tian-w.cn

[Q07] 删除表
来源：http://xmy.xylfe.cn

DROP TABLE IF EXISTS orders;
来源：http://riu.fehbvm.com

[Q08] 创建普通索引
来源：http://lrq.nanxinkj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://tei.zhaomingkeji.xyz

[Q09] 创建唯一索引
来源：http://ygj.fktsv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fnm.xylfe.cn

[Q10] 插入单行
来源：http://pch.yfazqb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vpj.ydjk.org.cn

[Q11] 一次插入多行
来源：http://qfq.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rgt.cucudq.cn

[Q12] 插入后取自增 ID
来源：http://yxp.jiagoushi.top


<!-- 参考信息 -->