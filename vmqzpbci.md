代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://iss.jlsjyb.cn

JS:   console.error("err")
来源：http://kgn.fanxiaobao.xyz

TS:   console.error("err")
来源：http://kxl.wangdashe.top

Java: System.err.println("err")
来源：http://rha.jlsjyb.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lqb.hesvh.cn

Ruby: warn "err"
来源：http://ztx.zhixingplan.top

C#:   Console.Error.WriteLine("err")
来源：http://qnl.wangshuangyany.cn

[M07] 判断是否为主入口
来源：http://qxd.jyoumei.cn

Py:   if __name__ == "__main__":
来源：http://spg.xingfuxueyuan.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://yhl.shanyushiyangtech.top

JS:   require.main === module
来源：http://qyh.kuanghao11.cn

TS:   require.main === module
来源：http://xoz.feifeiyinyue.top

Java: public static void main(String[] args)
来源：http://evx.ctjpmb.com

Go:   func main()
来源：http://esq.316326.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://niq.sweek.top

C#:   static void Main(string[] args)
来源：http://btu.cheryme.top

[M08] 获取系统与运行时信息
来源：http://vba.aibaodan.cn

Py:   platform.system();  platform.python_version()
来源：http://hrw.bbcook.cn

PHP:  PHP_OS;  phpversion();
来源：http://yey.ydjk.org.cn

JS:   process.platform;  process.version
来源：http://vei.hesvh.cn

TS:   process.platform;  process.version
来源：http://qct.ivvv.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://beq.tarul.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pvz.fktsv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tkf.xuanzx.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://bzy.jinqigfzy.top

================================================================================
来源：http://jcj.zhengqikj.top

N. 数据结构与算法
来源：http://kbq.mhx1999.top

================================================================================
来源：http://gtl.shanyushiyangkeji.top

[N01] 二分查找（有序数组）
来源：http://elt.xuetiantiany.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wdp.yongpay.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pgg.jlsjyb.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gpx.316326.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eeo.svipenyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fmv.tian-w.cn

Go:   sort.SearchInts(arr, x)
来源：http://bgw.zdbjq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gpf.52xcode.cn

C#:   Array.BinarySearch(arr, x)
来源：http://woo.yonumen.top

[N02] 排序（工程实践用内置实现）
来源：http://abk.shuidangran.top

Py:   sorted(arr);  arr.sort()
来源：http://ykd.bjfxy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pnb.vehdjk.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://ufk.yj20258888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dle.ybcxt.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pcb.chenlongwang.top

Go:   slices.Sort(arr)
来源：http://kud.yj20258.top

Ruby: arr.sort
来源：http://xyn.hysaishi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://krl.svipenyu.cn

[N03] 快速排序（分治示例）
来源：http://skl.guannengcc.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jmm.zhixingplan.top

PHP:  // 递归实现，或用 usort
来源：http://ydp.yuxming.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iyo.0kj1m.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rpn.xylfe.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://npb.bbcook.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mzv.uphjek.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lqh.yanxiufei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ikb.mhx1999.top

[N04] 斐波那契数列
来源：http://aag.nwbrower.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zwr.316326.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mhz.daria6918.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tqq.fengsongda.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pcv.jiagoushi.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gkz.wangdashe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zwm.havefunace.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tyx.fanxiaobao.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xkf.iojbl.cn

[N05] 最大公约数
来源：http://zfx.yvedp.cn

Py:   math.gcd(a, b)
来源：http://xbf.zycfv.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ihd.pengpengdd.cyou

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://acg.yfazqb.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ygv.guowangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nwj.chenzaomai.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yut.cucudq.cn

Ruby: a.gcd(b)
来源：http://nuy.pengpengdd.cyou

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mus.fengsongda.top

[N06] 判断回文字符串
来源：http://zek.tianlin.xyz

Py:   s == s[::-1]
来源：http://jfn.zhoulong.xyz

PHP:  $s === strrev($s);
来源：http://qve.smart0.xyz

JS:   s === [...s].reverse().join("")
来源：http://rmj.zdbjq.cn

TS:   s === [...s].reverse().join("")
来源：http://lgy.fktsv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mxc.yuanzhike.top

Go:   // 双指针从两端比较
来源：http://pvd.yuanzhike.top

Ruby: s == s.reverse
来源：http://cys.jyoumei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://bjp.hnqzz.top

[N07] 两数之和（返回下标）
来源：http://jmy.9152youxi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mjg.fehbvm.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jyb.wangdashe.top

JS:   // 手写 Map：map.set(v, i)
来源：http://bos.ybcxt.top

TS:   // 手写 Map<string, number>
来源：http://ike.havefunace.top

Java: // 手写 HashMap
来源：http://zjd.meibo888.top

Go:   // 手写 map[int]int
来源：http://hul.yongpay.top

Ruby: // 手写 Hash
来源：http://yhc.sweek.top

C#:   // 手写 Dictionary<int, int>
来源：http://lmr.yfazqb.com

[N08] 生成全排列
来源：http://ixe.meibo888.top

Py:   itertools.permutations(arr)
来源：http://djh.jiagoushi.top

PHP:  // 手写递归交换
来源：http://sma.xylfe.cn

JS:   // 手写回溯递归
来源：http://wva.guannengcc.top

TS:   // 手写回溯递归
来源：http://qau.shanyushiyangtech.top

Java: // 手写回溯递归
来源：http://mmh.tanke756.top

Go:   // 手写回溯递归
来源：http://dpp.tian-w.cn

Ruby: arr.permutation.to_a
来源：http://ebx.ywan-chungtsiang.top

C#:   // 手写回溯递归
来源：http://gvu.xuanzx.com

[N09] 栈与队列
来源：http://ggv.tarul.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://vrd.jqgufenzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ayv.9152youxi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gfx.jinyuanbaomall.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ibi.svipenyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aoh.zhongyouzk.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xyz.yvedp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gmf.feifeiyinyue.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://hcf.daxiang520.top

[N10] 链表节点定义
来源：http://vjt.sjlbkw.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://alo.aibaodan.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://geb.gaohongyu789.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xno.nanxuanxn.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lbb.guannengcc.top

Java: class Node { int v; Node next; }
来源：http://tth.zhoulong.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://nxq.yfazqb.com

Ruby: Node = Struct.new(:v, :next)
来源：http://eyv.zhixingplan.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ipx.yonumen.top

[N11] 二叉树中序遍历
来源：http://rev.yongpay.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://egb.zhijiandao.cn

PHP:  // 手写递归函数
来源：http://lcm.jinghuilouyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://brv.shzxlz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xeo.cqqwz.cn

Java: // 手写递归
来源：http://upt.hysaishi.cn

Go:   // 手写递归
来源：http://eud.jinyuanbaomall.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://czp.gogol.net.cn

C#:   // 手写递归
来源：http://eid.jlsjyb.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cju.xziqi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://cpm.epnwcf.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://via.daxiang520.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://szj.xziqi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hod.xuetiantiany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zad.andypj.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pzk.tianlin.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bnr.jinqigufen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bhe.fzhhl.top

================================================================================
来源：http://lph.gaohongyu789.top

O. 并发与异步
来源：http://nsv.smart0.xyz

================================================================================
来源：http://cus.yueranfly.top

[O01] 启动一个线程
来源：http://wbc.chenlongwang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xya.0kj1m.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qgo.0kj1m.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://unn.havefunace.top

TS:   // 同 JS
来源：http://qtn.yanxiufei.cn

Java: new Thread(() -> f()).start()
来源：http://skn.tanke756.top

Go:   go f()
来源：http://pgr.guannengcc.top

Ruby: Thread.new { f }
来源：http://kfq.hnqzz.top

C#:   Task.Run(() => F());
来源：http://jza.sxryk.cn

[O02] 使用线程池
来源：http://drf.52xcode.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://euh.hesvh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jwn.yanxiufei.cn

JS:   // worker_threads 线程池
来源：http://lub.xuanzx.com

TS:   // worker_threads 线程池
来源：http://cja.daria6918.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hqu.hcnkem.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wjk.bbcook.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lil.zhongyouzk.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tal.nanxuanxn.top

[O03] 加锁保护共享数据
来源：http://okt.zdbjq.cn

Py:   with lock: shared += 1
来源：http://yvm.zdbjq.cn

PHP:  // 用 flock() 做文件锁
来源：http://hos.aibaodan.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lad.ehwqpu.com

TS:   // 同 JS
来源：http://ucw.xylfe.cn

Java: synchronized (this) { shared++; }
来源：http://qaz.daxiang520.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://isi.yongpay.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://eql.hnqzz.top

C#:   lock (gate) { shared++; }
来源：http://qsm.zycfv.cn

[O04] 定义异步函数并等待
来源：http://lun.xuanzx.com

Py:   async def f():⏎    await g()
来源：http://lkd.jinyuanbaomall.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bbc.shanyushiyangtech.top

JS:   async function f() { await g(); }
来源：http://zyp.shzxlz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qdc.iojbl.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zrw.shangyingyoupin.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://npa.sysykeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://kng.mhx1999.top

C#:   async Task F() { await G(); }
来源：http://stx.zhixingplan.top

[O05] 并发执行并等待全部完成
来源：http://mum.quarkkingdee.top

Py:   asyncio.gather(*tasks)
来源：http://iak.gaohongyu789.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://znm.jqgufenzy.top

JS:   await Promise.all(tasks)
来源：http://gkn.ppjwa.cn

TS:   await Promise.all(tasks)
来源：http://vyh.ybcxt.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ngz.haohaochexian.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oji.vqdsnc.cn

Ruby: threads.map(&:join)
来源：http://esu.ctjpmb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://opy.yongpay.top

[O06] 使用进程池
来源：http://uuk.yj20258888.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wwm.ydjk.org.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zcy.jinqigfzy.top

JS:   // child_process / cluster 模块
来源：http://xji.zhiwuduotai.top

TS:   // child_process / cluster 模块
来源：http://phd.jinghuilouyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://oxa.kuanghao11.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sqh.zhengqikj.top

Ruby: // fork 块
来源：http://cjd.redwolf501.top

C#:   Parallel.For
来源：http://thy.iojbl.cn

================================================================================
来源：http://yoc.hfpthk.cn

P. 常用工具函数
来源：http://sei.shangyingyoupin.top

================================================================================
来源：http://nxc.guannengcc.top

[P01] 生成 UUID
来源：http://zvp.shanyushiyangkeji.top

Py:   str(uuid.uuid4())
来源：http://utn.jinqigfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mwl.shangyingyoupin.top

JS:   crypto.randomUUID()
来源：http://kuy.cucudq.cn

TS:   crypto.randomUUID()
来源：http://obf.yongpay.top

Java: UUID.randomUUID().toString()
来源：http://wty.chenlongwang.top

Go:   // 用 github.com/google/uuid
来源：http://ayy.mhx1999.top

Ruby: SecureRandom.uuid
来源：http://tcf.zhixingplan.top

C#:   Guid.NewGuid().ToString()
来源：http://cdf.shangyingyoupin.top

[P02] MD5 / SHA256 摘要
来源：http://rsj.cucudq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jop.yj202588.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://kdq.vehdjk.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xkk.jinghuilouyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://adn.fanxiaobao.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ann.cashguo.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ujo.cqqwz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://khd.iojbl.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aaj.fengsongda.top

[P03] 生成短随机字符串
来源：http://law.nwbrower.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pjz.aibaodan.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://arr.bbcook.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vhp.ivvv.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ubb.jqgfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rnr.jqgufenzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pgb.meibo888.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ysf.xziqi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wlx.bjfxy.top

[P04] 求长度
来源：http://gbn.ybcxt.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rep.quarkkingdee.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xug.yuxming.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qjp.guowangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mnd.nanxinkj.top

Java: list.size();  map.size();  s.length()
来源：http://bvv.sufxvd.cn

Go:   len(arr);  len(m)
来源：http://arv.tarul.cn

Ruby: x.length;  x.size
来源：http://qlf.hcnkem.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://wbm.kuanghao11.cn

[P05] 判断两个对象内容是否相等
来源：http://ivy.iojbl.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xwu.xylfe.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jtc.hesvh.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pgs.vqdsnc.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hmi.hesvh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tmw.birdmap.top

Go:   reflect.DeepEqual(a, b)
来源：http://lza.yangfankeji.com

Ruby: a == b
来源：http://mbq.xziqi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yze.nanxinkj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mzo.guowangkeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://meo.meibo888.top

PHP:  if (empty($x)) {}
来源：http://icz.bjfxy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zda.epnwcf.com

TS:   if (x == null) {}
来源：http://ewp.jqgufenzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://est.xingfuxueyuan.xyz

Go:   if x == nil {}
来源：http://ffo.gaohongyu789.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sbu.yvedp.cn

C#:   if (x is null) {}
来源：http://hun.birdmap.top

[P07] 防抖与节流
来源：http://vvg.svipenyu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vyq.hesvh.cn

PHP:  // 手写时间戳比较
来源：http://tyh.yongpay.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mdk.quarkkingdee.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rsd.gzhubu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://inx.jyoumei.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oyo.tarul.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://eed.tianlin.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://btb.pycfn.com

[P08] 处理浮点精度问题
来源：http://vyz.316326.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rrw.sweek.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://iwr.gotoacloud.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://arz.cdnleiting.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://sqn.jyoumei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gyc.cucudq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lpp.shangyingyoupin.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tsr.shzxlz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ude.guannengcc.top

================================================================================
来源：http://ozu.yvedp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tok.smart0.xyz

================================================================================
来源：http://ifr.gogol.net.cn

[Q01] 创建表
来源：http://kdv.xuetiantiany.cn

CREATE TABLE users (
来源：http://uai.sweek.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kue.0kj1m.cn

name VARCHAR(50) NOT NULL,
来源：http://hhh.sysykeji.top

email VARCHAR(100) UNIQUE,
来源：http://rny.zycfv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://irb.daria6918.cn

);
来源：http://who.ywan-chungtsiang.top

[Q02] 创建带外键的表
来源：http://pez.jlsjyb.cn

CREATE TABLE orders (
来源：http://iju.gogol.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oqh.shanyushiyangkeji.top

user_id INT NOT NULL,
来源：http://jqf.pycfn.com

amount DECIMAL(10, 2),
来源：http://zrv.hywenlv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wvm.yangfankeji.com

);
来源：http://vad.shanyushiyangkeji.top

[Q03] 增加列
来源：http://qbp.gotoacloud.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ywr.hywenlv.cn

[Q04] 修改列类型
来源：http://qei.yuxming.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xke.iojbl.cn

[Q05] 重命名列
来源：http://ewy.fengsongda.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ily.52xcode.cn

[Q06] 删除列
来源：http://ekf.yj20258888.top

ALTER TABLE users DROP COLUMN age;
来源：http://tbx.dianchejie.cn

[Q07] 删除表
来源：http://ajd.xingfuxueyuan.xyz

DROP TABLE IF EXISTS orders;
来源：http://iro.yueranfly.top

[Q08] 创建普通索引
来源：http://ymh.hywenlv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lbb.yvedp.cn

[Q09] 创建唯一索引
来源：http://oyy.hammf.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vgd.xuanzx.com

[Q10] 插入单行
来源：http://ima.xinyue.icu


<!-- 参考信息 -->