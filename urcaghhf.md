代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://tko.tianlin.xyz

JS:   console.error("err")
来源：http://aqm.jinqigfzy.top

TS:   console.error("err")
来源：http://kmq.xylfe.cn

Java: System.err.println("err")
来源：http://qja.sxryk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kvt.kuanghao11.cn

Ruby: warn "err"
来源：http://bvq.ctjpmb.com

C#:   Console.Error.WriteLine("err")
来源：http://dhj.guowangkeji.top

[M07] 判断是否为主入口
来源：http://fam.zycfv.cn

Py:   if __name__ == "__main__":
来源：http://ggd.xziqi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uku.xingfuxueyuan.xyz

JS:   require.main === module
来源：http://tnn.fehbvm.com

TS:   require.main === module
来源：http://tfg.zhongyouzk.top

Java: public static void main(String[] args)
来源：http://uxx.tanke756.top

Go:   func main()
来源：http://gbd.c1oappe.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://oqw.zhongyouzk.top

C#:   static void Main(string[] args)
来源：http://khs.zycfv.cn

[M08] 获取系统与运行时信息
来源：http://okn.hywenlv.cn

Py:   platform.system();  platform.python_version()
来源：http://qke.dianchejie.cn

PHP:  PHP_OS;  phpversion();
来源：http://trf.cucudq.cn

JS:   process.platform;  process.version
来源：http://dpk.guannengcc.top

TS:   process.platform;  process.version
来源：http://zgc.zhiwuduotai.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://udx.gzhubu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ijv.iojbl.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wzd.mhx1999.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kop.hnqzz.top

================================================================================
来源：http://ehf.hnqzz.top

N. 数据结构与算法
来源：http://gxg.dashuyun.cn

================================================================================
来源：http://qnu.0kj1m.cn

[N01] 二分查找（有序数组）
来源：http://oij.shangyingyoupin.top

Py:   bisect.bisect_left(arr, x)
来源：http://scv.shuidangran.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gma.jinghuilouyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qpl.hfpthk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kwf.zdbjq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tlc.guowangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://ryu.yanxiufei.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ejg.ctjpmb.com

C#:   Array.BinarySearch(arr, x)
来源：http://kdu.gaohongyu789.top

[N02] 排序（工程实践用内置实现）
来源：http://thi.shangyingyoupin.top

Py:   sorted(arr);  arr.sort()
来源：http://dtb.zhongyouzk.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pdi.tianlin.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://dcj.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tmd.shuidangran.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mnl.jinqigufen.top

Go:   slices.Sort(arr)
来源：http://anu.tianlin.xyz

Ruby: arr.sort
来源：http://hbc.zhiwuduotai.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://gpu.bjfxy.top

[N03] 快速排序（分治示例）
来源：http://qmy.bbcook.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vrs.hongshengwenyu.top

PHP:  // 递归实现，或用 usort
来源：http://hrp.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oiw.jinqigufen.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wpc.kuanghao11.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://etm.xinyue.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bru.svipenyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sgc.gaohongyu789.top

C#:   // 手写递归，或 Array.Sort
来源：http://qha.smart0.xyz

[N04] 斐波那契数列
来源：http://wfk.shanyushiyangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ekl.jinghuilouyu.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://riu.sxryk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lfs.dashuyun.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cui.fanxiaobao.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://suq.guowangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://slg.0kj1m.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uvr.hywenlv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xtv.0kj1m.cn

[N05] 最大公约数
来源：http://otv.yueranfly.top

Py:   math.gcd(a, b)
来源：http://ptq.fktsv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oti.hcnkem.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uhl.ehwqpu.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lnr.316326.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sau.ybcxt.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jjh.nanxinkj.top

Ruby: a.gcd(b)
来源：http://vhe.nwbrower.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xzb.wangshuangyany.cn

[N06] 判断回文字符串
来源：http://mci.hnxiangtu.top

Py:   s == s[::-1]
来源：http://qnx.wangdashe.top

PHP:  $s === strrev($s);
来源：http://ihz.zhiwuduotai.top

JS:   s === [...s].reverse().join("")
来源：http://jeo.hysaishi.cn

TS:   s === [...s].reverse().join("")
来源：http://iob.yuxming.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uww.birdmap.top

Go:   // 双指针从两端比较
来源：http://pxb.0kj1m.cn

Ruby: s == s.reverse
来源：http://qbs.hfpthk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://brq.yanxiufei.cn

[N07] 两数之和（返回下标）
来源：http://vmh.feifeiyinyue.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://snm.fanxiaobao.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://tol.cheryme.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tyg.fehbvm.com

TS:   // 手写 Map<string, number>
来源：http://lcw.jinqigfzy.top

Java: // 手写 HashMap
来源：http://scp.svipenyu.cn

Go:   // 手写 map[int]int
来源：http://khi.jinghuilouyu.cn

Ruby: // 手写 Hash
来源：http://nsd.fengsongda.top

C#:   // 手写 Dictionary<int, int>
来源：http://qju.chenzaomai.com

[N08] 生成全排列
来源：http://ums.havefunace.top

Py:   itertools.permutations(arr)
来源：http://pxo.zhongyouzk.top

PHP:  // 手写递归交换
来源：http://bsk.cdnleiting.top

JS:   // 手写回溯递归
来源：http://zkt.c1oappe.top

TS:   // 手写回溯递归
来源：http://tpv.hnqzz.top

Java: // 手写回溯递归
来源：http://jrv.chenzaomai.com

Go:   // 手写回溯递归
来源：http://vyp.hnxiangtu.top

Ruby: arr.permutation.to_a
来源：http://byc.shzxlz.cn

C#:   // 手写回溯递归
来源：http://aby.daria6918.cn

[N09] 栈与队列
来源：http://jfj.chenjidiqi.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vfl.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kdh.sweek.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nkk.316326.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tez.shanyushiyangtech.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://evy.pycfn.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ifv.xuanzx.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bbl.yangfankeji.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vnz.yj20258888.top

[N10] 链表节点定义
来源：http://tec.feifeiyinyue.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pvq.meibo888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://itw.bbcook.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nkr.mhx1999.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://too.epnwcf.com

Java: class Node { int v; Node next; }
来源：http://ref.fzhhl.top

Go:   type Node struct { V int; Next *Node }
来源：http://afq.cqqwz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ynw.xziqi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://uwk.yj20258.top

[N11] 二叉树中序遍历
来源：http://vib.hnxiangtu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://emg.redwolf501.top

PHP:  // 手写递归函数
来源：http://vwz.52xcode.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cty.vqdsnc.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eox.zhiwuduotai.top

Java: // 手写递归
来源：http://zbj.fehbvm.com

Go:   // 手写递归
来源：http://xfv.zhaomingkeji.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jdw.chenzaomai.com

C#:   // 手写递归
来源：http://pjl.sysykeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ilc.zhoulong.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xtd.316326.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://scb.aizwys.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vqh.yfazqb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kzd.gzhubu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bzk.yj20258888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://iha.guowangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yxs.snrcjt.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zvw.9152youxi.cn

================================================================================
来源：http://kmt.zycfv.cn

O. 并发与异步
来源：http://imj.xylfe.cn

================================================================================
来源：http://new.havefunace.top

[O01] 启动一个线程
来源：http://ybx.hesvh.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://pzi.xuanzx.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vpi.cheryme.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://inr.hfpthk.cn

TS:   // 同 JS
来源：http://rha.jinqigfzy.top

Java: new Thread(() -> f()).start()
来源：http://lhe.ehwqpu.com

Go:   go f()
来源：http://rhg.daxiang520.top

Ruby: Thread.new { f }
来源：http://cmv.epnwcf.com

C#:   Task.Run(() => F());
来源：http://uod.sufxvd.cn

[O02] 使用线程池
来源：http://lgj.haohaochexian.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ryw.jlsjyb.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rki.svipenyu.cn

JS:   // worker_threads 线程池
来源：http://rnd.9152youxi.cn

TS:   // worker_threads 线程池
来源：http://cxy.hywenlv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://lly.ppjwa.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://obj.iojbl.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zzu.gzhubu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tsu.sweek.top

[O03] 加锁保护共享数据
来源：http://peo.sxryk.cn

Py:   with lock: shared += 1
来源：http://zsu.zycfv.cn

PHP:  // 用 flock() 做文件锁
来源：http://dce.shuidangran.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://urb.yangfankeji.com

TS:   // 同 JS
来源：http://ygo.hnqzz.top

Java: synchronized (this) { shared++; }
来源：http://awg.yuxming.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hiv.zhongyouzk.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://mue.iojbl.cn

C#:   lock (gate) { shared++; }
来源：http://qkf.zhixingplan.top

[O04] 定义异步函数并等待
来源：http://qdy.9152youxi.cn

Py:   async def f():⏎    await g()
来源：http://pae.xinyue.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://doe.zycfv.cn

JS:   async function f() { await g(); }
来源：http://pqi.jqgfzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tdw.c1oappe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zwk.sufxvd.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qax.zhongyouzk.top

Ruby: # 用 Fiber 或 async gem
来源：http://rpw.jinyuanbaomall.cn

C#:   async Task F() { await G(); }
来源：http://hsw.svipenyu.cn

[O05] 并发执行并等待全部完成
来源：http://flt.dashuyun.cn

Py:   asyncio.gather(*tasks)
来源：http://wdq.wangdashe.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hqw.jinqigufen.top

JS:   await Promise.all(tasks)
来源：http://ghq.yj202588.top

TS:   await Promise.all(tasks)
来源：http://abp.0kj1m.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dji.bjfxy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://bbq.ehwqpu.com

Ruby: threads.map(&:join)
来源：http://gbl.cdnleiting.top

C#:   await Task.WhenAll(t1, t2)
来源：http://nru.xuetiantiany.cn

[O06] 使用进程池
来源：http://ovo.xinyue.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uzd.hnqzz.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ngu.guowangkeji.top

JS:   // child_process / cluster 模块
来源：http://kxt.jlsjyb.cn

TS:   // child_process / cluster 模块
来源：http://cev.zhiwuduotai.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://thz.jqgufenzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dqt.fzhhl.top

Ruby: // fork 块
来源：http://vwy.sxryk.cn

C#:   Parallel.For
来源：http://kcd.chenlongwang.top

================================================================================
来源：http://tbp.zhongyouzk.top

P. 常用工具函数
来源：http://lnk.sweek.top

================================================================================
来源：http://rpl.yueranfly.top

[P01] 生成 UUID
来源：http://twu.svipenyu.cn

Py:   str(uuid.uuid4())
来源：http://qvt.pengpengdd.cyou

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ayh.zhixingplan.top

JS:   crypto.randomUUID()
来源：http://cpt.quarkkingdee.top

TS:   crypto.randomUUID()
来源：http://qvq.jqgufenzy.top

Java: UUID.randomUUID().toString()
来源：http://khx.wangshuangyany.cn

Go:   // 用 github.com/google/uuid
来源：http://mkc.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://zcw.zhaomingkeji.xyz

C#:   Guid.NewGuid().ToString()
来源：http://pat.fktsv.cn

[P02] MD5 / SHA256 摘要
来源：http://dje.vqdsnc.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ttl.guannengcc.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://pcu.jlsjyb.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gkd.zhaomingkeji.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cuw.jianghu66.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bin.dashuyun.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hdm.zycfv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ggh.zdbjq.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xdh.gzhubu.top

[P03] 生成短随机字符串
来源：http://vnp.tian-w.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tga.sweek.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lpp.316326.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://woo.jiagoushi.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bjy.xinyue.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kdm.fzhhl.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mop.wangshuangyany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zxe.tianlin.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uxk.yuanzhike.top

[P04] 求长度
来源：http://lbt.iojbl.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ebr.fktsv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ifj.sjlbkw.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pjp.hcnkem.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jhr.hammf.cn

Java: list.size();  map.size();  s.length()
来源：http://igo.sysykeji.top

Go:   len(arr);  len(m)
来源：http://iwf.yj20258888.top

Ruby: x.length;  x.size
来源：http://iao.jinqigfzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vyv.jyoumei.cn

[P05] 判断两个对象内容是否相等
来源：http://ydj.birdmap.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nda.jyoumei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mie.chenlongwang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://luy.tian-w.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dqj.zhiwuduotai.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qei.316326.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://hiw.vehdjk.com

Ruby: a == b
来源：http://btv.yuanzhike.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://epe.ybcxt.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xgo.9152youxi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://huw.pycfn.com

PHP:  if (empty($x)) {}
来源：http://mks.jinqigufen.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://izh.vehdjk.com

TS:   if (x == null) {}
来源：http://eyz.bbcook.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vjl.redwolf501.top

Go:   if x == nil {}
来源：http://qrb.pengpengdd.cyou

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qzp.gaohongyu789.top

C#:   if (x is null) {}
来源：http://jct.sweek.top

[P07] 防抖与节流
来源：http://scr.ppjwa.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://joo.hysaishi.cn

PHP:  // 手写时间戳比较
来源：http://wpx.mhx1999.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mpt.shanyushiyangtech.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yde.ctjpmb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gjm.chenlongwang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nop.c1oappe.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://yht.chenjidiqi.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ili.jinqigfzy.top

[P08] 处理浮点精度问题
来源：http://lzx.xingfuxueyuan.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://udo.ppjwa.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gsp.hywenlv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iyo.xuanzx.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zmd.yanxiufei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jzt.chenzaomai.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zka.uphjek.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ssd.yonumen.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://twi.fzhhl.top

================================================================================
来源：http://obw.chenzaomai.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hmf.zhaomingkeji.xyz

================================================================================
来源：http://tno.zycfv.cn

[Q01] 创建表
来源：http://cbf.hfpthk.cn

CREATE TABLE users (
来源：http://usu.mhx1999.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lqr.yj202588.top

name VARCHAR(50) NOT NULL,
来源：http://kdh.yuxming.cn

email VARCHAR(100) UNIQUE,
来源：http://ysw.uphjek.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ryd.daxiang520.top

);
来源：http://ycq.jlsjyb.cn

[Q02] 创建带外键的表
来源：http://zho.ydjk.org.cn

CREATE TABLE orders (
来源：http://hqx.svipenyu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xay.zhiwuduotai.top

user_id INT NOT NULL,
来源：http://ywq.havefunace.top

amount DECIMAL(10, 2),
来源：http://war.jinqigufen.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lqc.sufxvd.cn

);
来源：http://gdi.ctjpmb.com

[Q03] 增加列
来源：http://yry.jqgufenzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ejk.hnxiangtu.top

[Q04] 修改列类型
来源：http://nen.pycfn.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pxz.jqgfzy.top

[Q05] 重命名列
来源：http://arv.redwolf501.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qqv.iojbl.cn

[Q06] 删除列
来源：http://xbs.dashuyun.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fyp.ywan-chungtsiang.top

[Q07] 删除表
来源：http://wtb.yangfankeji.com

DROP TABLE IF EXISTS orders;
来源：http://bwz.aibaodan.cn

[Q08] 创建普通索引
来源：http://qbu.shuidangran.top

CREATE INDEX idx_users_email ON users(email);
来源：http://pac.c1oappe.top

[Q09] 创建唯一索引
来源：http://via.xuanzx.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hee.jinghuilouyu.cn

[Q10] 插入单行
来源：http://urg.shuidangran.top


<!-- 参考信息 -->