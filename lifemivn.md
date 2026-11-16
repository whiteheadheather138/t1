代发 wailian999

Ruby: exit 1
来源：http://olq.xinyue.icu

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yzs.chenzaomai.com

[M06] 向标准错误输出
来源：http://chw.ydjk.org.cn

Py:   print("err", file=sys.stderr)
来源：http://rqu.andypj.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://rbr.birdmap.top

JS:   console.error("err")
来源：http://zmu.sxryk.cn

TS:   console.error("err")
来源：http://nei.kuanghao11.cn

Java: System.err.println("err")
来源：http://ite.fanxiaobao.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kcd.iojbl.cn

Ruby: warn "err"
来源：http://lcn.xinyue.icu

C#:   Console.Error.WriteLine("err")
来源：http://upd.zhongyouzk.top

[M07] 判断是否为主入口
来源：http://xdv.quarkkingdee.top

Py:   if __name__ == "__main__":
来源：http://ltq.yj20258888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://utx.zhongyouzk.top

JS:   require.main === module
来源：http://wsu.cheryme.top

TS:   require.main === module
来源：http://vxy.guowangkeji.top

Java: public static void main(String[] args)
来源：http://vqk.feifeiyinyue.top

Go:   func main()
来源：http://vlf.xuanzx.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nnc.meibo888.top

C#:   static void Main(string[] args)
来源：http://icm.jyoumei.cn

[M08] 获取系统与运行时信息
来源：http://mpe.jinghuilouyu.cn

Py:   platform.system();  platform.python_version()
来源：http://ero.zhiwuduotai.top

PHP:  PHP_OS;  phpversion();
来源：http://bld.zdbjq.cn

JS:   process.platform;  process.version
来源：http://odr.zdqjudy.top

TS:   process.platform;  process.version
来源：http://wvc.iojbl.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kaw.gzhubu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://mze.guannengcc.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wkq.jlsjyb.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sgr.dianchejie.cn

================================================================================
来源：http://gtu.dianchejie.cn

N. 数据结构与算法
来源：http://krw.nwbrower.top

================================================================================
来源：http://lyj.hesvh.cn

[N01] 二分查找（有序数组）
来源：http://hxs.iojbl.cn

Py:   bisect.bisect_left(arr, x)
来源：http://czd.316326.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aow.smart0.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://njx.0kj1m.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://apu.zdbjq.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gem.xuetiantiany.cn

Go:   sort.SearchInts(arr, x)
来源：http://zkt.ydzc1.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ugq.zycfv.cn

C#:   Array.BinarySearch(arr, x)
来源：http://mus.yvedp.cn

[N02] 排序（工程实践用内置实现）
来源：http://ctx.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://vdj.guannengcc.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oql.tianlin.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://dyn.haohaochexian.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dat.quarkkingdee.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wwm.zhaomingkeji.xyz

Go:   slices.Sort(arr)
来源：http://qfk.aibaodan.cn

Ruby: arr.sort
来源：http://hjk.pycfn.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://xol.aizwys.cn

[N03] 快速排序（分治示例）
来源：http://jiy.sufxvd.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://yru.pengpengdd.cyou

PHP:  // 递归实现，或用 usort
来源：http://fjr.ivvv.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mqo.cdnleiting.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jhe.ppjwa.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://soj.jianghu66.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ijm.hnxiangtu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ytv.gzhubu.top

C#:   // 手写递归，或 Array.Sort
来源：http://alo.zhoulong.xyz

[N04] 斐波那契数列
来源：http://rol.wangdashe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jaw.hammf.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://haz.hcnkem.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qnu.jinyuanbaomall.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jhn.zhongyouzk.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ccy.tianlin.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iyx.epnwcf.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nrm.ybcxt.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pzo.fanxiaobao.xyz

[N05] 最大公约数
来源：http://fue.0kj1m.cn

Py:   math.gcd(a, b)
来源：http://err.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rxo.cashguo.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zht.cashguo.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vce.aizwys.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xwm.hesvh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bqt.svipenyu.cn

Ruby: a.gcd(b)
来源：http://siq.jinqigufen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://awq.sweek.top

[N06] 判断回文字符串
来源：http://zzo.xuetiantiany.cn

Py:   s == s[::-1]
来源：http://abi.hammf.cn

PHP:  $s === strrev($s);
来源：http://xfu.tianlin.xyz

JS:   s === [...s].reverse().join("")
来源：http://rfu.jinyuanbaomall.cn

TS:   s === [...s].reverse().join("")
来源：http://fvo.cheryme.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rac.uphjek.com

Go:   // 双指针从两端比较
来源：http://kwn.shangyingyoupin.top

Ruby: s == s.reverse
来源：http://qbg.sxryk.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uqg.zdqjudy.top

[N07] 两数之和（返回下标）
来源：http://whl.sweek.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ozh.yuanzhike.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gsm.fehbvm.com

JS:   // 手写 Map：map.set(v, i)
来源：http://npe.ywan-chungtsiang.top

TS:   // 手写 Map<string, number>
来源：http://tvc.bjfxy.top

Java: // 手写 HashMap
来源：http://mzs.iojbl.cn

Go:   // 手写 map[int]int
来源：http://ain.cqqwz.cn

Ruby: // 手写 Hash
来源：http://wnj.jinghuilouyu.cn

C#:   // 手写 Dictionary<int, int>
来源：http://tsw.xingfuxueyuan.xyz

[N08] 生成全排列
来源：http://xod.svipenyu.cn

Py:   itertools.permutations(arr)
来源：http://gzn.fzhhl.top

PHP:  // 手写递归交换
来源：http://jzu.chenlongwang.top

JS:   // 手写回溯递归
来源：http://gcf.yueranfly.top

TS:   // 手写回溯递归
来源：http://uos.tianlin.xyz

Java: // 手写回溯递归
来源：http://fuh.zdbjq.cn

Go:   // 手写回溯递归
来源：http://jxl.aibaodan.cn

Ruby: arr.permutation.to_a
来源：http://qcn.ehwqpu.com

C#:   // 手写回溯递归
来源：http://qei.quarkkingdee.top

[N09] 栈与队列
来源：http://opi.vqdsnc.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://bri.shanyushiyangkeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://adf.ppjwa.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://fsy.hnxiangtu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iwn.fengsongda.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://gcm.uphjek.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ppa.daria6918.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://yue.haohaochexian.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cos.jinqigfzy.top

[N10] 链表节点定义
来源：http://pkf.aizwys.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://fsp.tarul.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://low.yj20258.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zdx.havefunace.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qlk.tanke756.top

Java: class Node { int v; Node next; }
来源：http://vls.hysaishi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://svj.yueranfly.top

Ruby: Node = Struct.new(:v, :next)
来源：http://wye.jqgufenzy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://xlc.gotoacloud.top

[N11] 二叉树中序遍历
来源：http://hof.bjfxy.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aam.ppjwa.cn

PHP:  // 手写递归函数
来源：http://jfx.yj20258888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vve.ctjpmb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lhz.jinqigfzy.top

Java: // 手写递归
来源：http://zyo.yj20258888.top

Go:   // 手写递归
来源：http://vgc.yj20258.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pru.zhongyouzk.top

C#:   // 手写递归
来源：http://ede.gzhubu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bvs.ywan-chungtsiang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xae.fengsongda.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yks.gzhubu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://izo.cashguo.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bwt.hfpthk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://yod.chenlongwang.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cby.quarkkingdee.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pne.hnxiangtu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bfk.fehbvm.com

================================================================================
来源：http://qod.shangyingyoupin.top

O. 并发与异步
来源：http://aao.bbcook.cn

================================================================================
来源：http://bxa.pycfn.com

[O01] 启动一个线程
来源：http://ykf.zdbjq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://srv.pycfn.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jyq.yj20258888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ysn.cheryme.top

TS:   // 同 JS
来源：http://ckn.hywenlv.cn

Java: new Thread(() -> f()).start()
来源：http://ktw.uphjek.com

Go:   go f()
来源：http://jhx.tarul.cn

Ruby: Thread.new { f }
来源：http://bjx.52xcode.cn

C#:   Task.Run(() => F());
来源：http://gal.shuidangran.top

[O02] 使用线程池
来源：http://qlh.chenzaomai.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://api.xinyue.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://num.tian-w.cn

JS:   // worker_threads 线程池
来源：http://jrx.dashuyun.cn

TS:   // worker_threads 线程池
来源：http://fwm.xingfuxueyuan.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://rmn.jinghuilouyu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fru.cqqwz.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pvf.yj20258.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qgk.jyoumei.cn

[O03] 加锁保护共享数据
来源：http://skk.tarul.cn

Py:   with lock: shared += 1
来源：http://jkg.ywan-chungtsiang.top

PHP:  // 用 flock() 做文件锁
来源：http://wwb.yj20258888.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lng.jlsjyb.cn

TS:   // 同 JS
来源：http://ila.gogol.net.cn

Java: synchronized (this) { shared++; }
来源：http://uif.xziqi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ojs.zhongyouzk.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ost.0kj1m.cn

C#:   lock (gate) { shared++; }
来源：http://egx.jiagoushi.top

[O04] 定义异步函数并等待
来源：http://fvk.zhoulong.xyz

Py:   async def f():⏎    await g()
来源：http://czj.fehbvm.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xhv.daxiang520.top

JS:   async function f() { await g(); }
来源：http://mok.fehbvm.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://zds.xuanzx.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iqh.chenlongwang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qlq.wangdashe.top

Ruby: # 用 Fiber 或 async gem
来源：http://zsd.daria6918.cn

C#:   async Task F() { await G(); }
来源：http://osj.zdqjudy.top

[O05] 并发执行并等待全部完成
来源：http://ddk.nwbrower.top

Py:   asyncio.gather(*tasks)
来源：http://aic.hammf.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://glz.yanxiufei.cn

JS:   await Promise.all(tasks)
来源：http://ukt.wangshuangyany.cn

TS:   await Promise.all(tasks)
来源：http://wtk.shanyushiyangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ywp.daria6918.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mio.vqdsnc.cn

Ruby: threads.map(&:join)
来源：http://ayt.jqgfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://gyg.jianghu66.top

[O06] 使用进程池
来源：http://yns.aibaodan.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qls.yfazqb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://uns.nwbrower.top

JS:   // child_process / cluster 模块
来源：http://sby.ivvv.top

TS:   // child_process / cluster 模块
来源：http://gqx.redwolf501.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wio.c1oappe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rwp.zhiwuduotai.top

Ruby: // fork 块
来源：http://tds.smart0.xyz

C#:   Parallel.For
来源：http://tca.bbcook.cn

================================================================================
来源：http://arr.chenzaomai.com

P. 常用工具函数
来源：http://rsw.epnwcf.com

================================================================================
来源：http://agf.52xcode.cn

[P01] 生成 UUID
来源：http://ygc.xingfuxueyuan.xyz

Py:   str(uuid.uuid4())
来源：http://uap.52xcode.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qwe.haohaochexian.top

JS:   crypto.randomUUID()
来源：http://fqx.quarkkingdee.top

TS:   crypto.randomUUID()
来源：http://rhz.jianghu66.top

Java: UUID.randomUUID().toString()
来源：http://ued.ywan-chungtsiang.top

Go:   // 用 github.com/google/uuid
来源：http://eat.52xcode.cn

Ruby: SecureRandom.uuid
来源：http://fwf.feifeiyinyue.top

C#:   Guid.NewGuid().ToString()
来源：http://ewu.shzxlz.cn

[P02] MD5 / SHA256 摘要
来源：http://xtr.yfazqb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://elg.fengsongda.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://spq.ybcxt.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fju.jiagoushi.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://buc.sysykeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jnd.bbcook.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ehy.bjfxy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ygd.birdmap.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://agr.ehwqpu.com

[P03] 生成短随机字符串
来源：http://ghn.quarkkingdee.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://usi.shanyushiyangtech.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xhq.hnqzz.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bru.andypj.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wlp.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vht.fktsv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pbd.cheryme.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://pzb.zhijiandao.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dkw.zycfv.cn

[P04] 求长度
来源：http://oav.zhaomingkeji.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hlg.shanyushiyangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kwg.9152youxi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://txs.sufxvd.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ufu.sysykeji.top

Java: list.size();  map.size();  s.length()
来源：http://qxk.zdqjudy.top

Go:   len(arr);  len(m)
来源：http://ghc.jianghu66.top

Ruby: x.length;  x.size
来源：http://qvg.jinqigufen.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://sgu.svipenyu.cn

[P05] 判断两个对象内容是否相等
来源：http://woz.shangyingyoupin.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://abu.ivvv.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jfv.c1oappe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ero.zhoulong.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fwa.tianlin.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nhy.sxryk.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hvn.sufxvd.cn

Ruby: a == b
来源：http://txo.daxiang520.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pkt.yj20258888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lin.mhx1999.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mht.tarul.cn

PHP:  if (empty($x)) {}
来源：http://gur.xylfe.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://phb.316326.xyz

TS:   if (x == null) {}
来源：http://yph.ydjk.org.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wbi.nanxinkj.top

Go:   if x == nil {}
来源：http://jqi.tianlin.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ffg.ydzc1.top

C#:   if (x is null) {}
来源：http://vvx.jqgufenzy.top

[P07] 防抖与节流
来源：http://ugm.tarul.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dva.andypj.xyz

PHP:  // 手写时间戳比较
来源：http://zil.fehbvm.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kni.hnxiangtu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ezf.yvedp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tum.xuetiantiany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jal.yueranfly.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ljl.gogol.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ovd.nanxinkj.top

[P08] 处理浮点精度问题
来源：http://zyi.yueranfly.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://snj.meibo888.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wwq.zycfv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eva.jqgufenzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lie.sweek.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mzr.xuanzx.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ytz.0kj1m.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ude.zhongyouzk.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bjr.nwbrower.top

================================================================================
来源：http://lfu.feifeiyinyue.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mux.zhongyouzk.top

================================================================================
来源：http://gvw.daxiang520.top

[Q01] 创建表
来源：http://ybn.pengpengdd.cyou

CREATE TABLE users (
来源：http://wnz.yuxming.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gra.ydzc1.top

name VARCHAR(50) NOT NULL,
来源：http://abc.gotoacloud.top

email VARCHAR(100) UNIQUE,
来源：http://uhx.jinqigfzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vcq.tarul.cn

);
来源：http://yng.bbcook.cn

[Q02] 创建带外键的表
来源：http://otr.zhongyouzk.top

CREATE TABLE orders (
来源：http://wob.yanxiufei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wtf.fktsv.cn

user_id INT NOT NULL,
来源：http://qat.xuetiantiany.cn

amount DECIMAL(10, 2),
来源：http://hcd.xinyue.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://btg.vqdsnc.cn

);
来源：http://bji.shangyingyoupin.top

[Q03] 增加列
来源：http://vig.epnwcf.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ivj.sjlbkw.cn

[Q04] 修改列类型
来源：http://xkz.shanyushiyangtech.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://txr.jiagoushi.top

[Q05] 重命名列
来源：http://uep.wangdashe.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fgu.yangfankeji.com

[Q06] 删除列
来源：http://pxo.guowangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://hzl.zycfv.cn

[Q07] 删除表
来源：http://pkx.zhiwuduotai.top

DROP TABLE IF EXISTS orders;
来源：http://eby.xuanzx.com

[Q08] 创建普通索引
来源：http://jod.jiagoushi.top


<!-- 参考信息 -->