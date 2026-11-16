代发 wailian999

JS:   process.exit(1)
来源：http://dgk.gaohongyu789.top

TS:   process.exit(1)
来源：http://ski.yanxiufei.cn

Java: System.exit(1)
来源：http://liw.jinyuanbaomall.cn

Go:   os.Exit(1)
来源：http://utg.hywenlv.cn

Ruby: exit 1
来源：http://leg.zhoulong.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mup.xziqi.cn

[M06] 向标准错误输出
来源：http://ike.zdqjudy.top

Py:   print("err", file=sys.stderr)
来源：http://wzt.hywenlv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://cyw.vehdjk.com

JS:   console.error("err")
来源：http://nxf.meibo888.top

TS:   console.error("err")
来源：http://xlx.tian-w.cn

Java: System.err.println("err")
来源：http://crx.xuanzx.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jsc.zhongyouzk.top

Ruby: warn "err"
来源：http://gdz.52xcode.cn

C#:   Console.Error.WriteLine("err")
来源：http://duj.jlsjyb.cn

[M07] 判断是否为主入口
来源：http://qju.zhongyouzk.top

Py:   if __name__ == "__main__":
来源：http://jcu.jianghu66.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dfz.aizwys.cn

JS:   require.main === module
来源：http://srh.ybcxt.top

TS:   require.main === module
来源：http://xsp.ydjk.org.cn

Java: public static void main(String[] args)
来源：http://mdb.shangyingyoupin.top

Go:   func main()
来源：http://rvy.52xcode.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iog.shangyingyoupin.top

C#:   static void Main(string[] args)
来源：http://lmp.shangyingyoupin.top

[M08] 获取系统与运行时信息
来源：http://zcv.shanyushiyangtech.top

Py:   platform.system();  platform.python_version()
来源：http://urx.iojbl.cn

PHP:  PHP_OS;  phpversion();
来源：http://oet.yuanzhike.top

JS:   process.platform;  process.version
来源：http://udn.hywenlv.cn

TS:   process.platform;  process.version
来源：http://nei.andypj.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lrl.wangdashe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://eds.bjfxy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ojr.hnxiangtu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ytt.yfazqb.com

================================================================================
来源：http://hns.shuidangran.top

N. 数据结构与算法
来源：http://jky.andypj.xyz

================================================================================
来源：http://nbs.vehdjk.com

[N01] 二分查找（有序数组）
来源：http://jiq.yonumen.top

Py:   bisect.bisect_left(arr, x)
来源：http://hfq.nanxuanxn.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ugm.52xcode.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eez.fktsv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zxy.fzhhl.top

Java: Arrays.binarySearch(arr, x)
来源：http://ffm.yonumen.top

Go:   sort.SearchInts(arr, x)
来源：http://iza.jinyuanbaomall.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jvf.xuanzx.com

C#:   Array.BinarySearch(arr, x)
来源：http://grr.jinyuanbaomall.cn

[N02] 排序（工程实践用内置实现）
来源：http://xob.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://ihe.9152youxi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://akm.nwbrower.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://yww.gogol.net.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mtl.sufxvd.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hqs.vqdsnc.cn

Go:   slices.Sort(arr)
来源：http://oki.cucudq.cn

Ruby: arr.sort
来源：http://stk.cheryme.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jhs.dianchejie.cn

[N03] 快速排序（分治示例）
来源：http://nsz.pengpengdd.cyou

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vgw.xziqi.cn

PHP:  // 递归实现，或用 usort
来源：http://dfk.xuetiantiany.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ulg.c1oappe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oim.wangdashe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rhs.bjfxy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cep.xuanzx.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jcv.yj20258888.top

C#:   // 手写递归，或 Array.Sort
来源：http://njw.xziqi.cn

[N04] 斐波那契数列
来源：http://aji.dashuyun.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jio.mhx1999.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tsm.ywan-chungtsiang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cgf.chenlongwang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ymn.tanke756.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qra.cheryme.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://civ.bbcook.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://khq.nwbrower.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tnm.ydzc1.top

[N05] 最大公约数
来源：http://fed.gzhubu.top

Py:   math.gcd(a, b)
来源：http://ube.jianghu66.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jjj.zdbjq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cwg.zhijiandao.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aej.smart0.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cud.zdqjudy.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://imh.yonumen.top

Ruby: a.gcd(b)
来源：http://rkr.vehdjk.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://elg.xylfe.cn

[N06] 判断回文字符串
来源：http://ogq.guannengcc.top

Py:   s == s[::-1]
来源：http://plt.yj20258.top

PHP:  $s === strrev($s);
来源：http://gdy.bjfxy.top

JS:   s === [...s].reverse().join("")
来源：http://orq.nanxuanxn.top

TS:   s === [...s].reverse().join("")
来源：http://yry.zycfv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sha.shanyushiyangtech.top

Go:   // 双指针从两端比较
来源：http://yjw.yueranfly.top

Ruby: s == s.reverse
来源：http://xpj.shanyushiyangkeji.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://dmp.cucudq.cn

[N07] 两数之和（返回下标）
来源：http://yxl.ehwqpu.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zhi.tianlin.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://oma.chenlongwang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://nuz.fzhhl.top

TS:   // 手写 Map<string, number>
来源：http://ejc.fehbvm.com

Java: // 手写 HashMap
来源：http://ozh.9152youxi.cn

Go:   // 手写 map[int]int
来源：http://wgz.andypj.xyz

Ruby: // 手写 Hash
来源：http://fwh.yongpay.top

C#:   // 手写 Dictionary<int, int>
来源：http://vpo.gotoacloud.top

[N08] 生成全排列
来源：http://ghf.ivvv.top

Py:   itertools.permutations(arr)
来源：http://jlf.0kj1m.cn

PHP:  // 手写递归交换
来源：http://sbl.yonumen.top

JS:   // 手写回溯递归
来源：http://qpg.zhongyouzk.top

TS:   // 手写回溯递归
来源：http://pny.jinghuilouyu.cn

Java: // 手写回溯递归
来源：http://obq.nwbrower.top

Go:   // 手写回溯递归
来源：http://aph.shangyingyoupin.top

Ruby: arr.permutation.to_a
来源：http://lhv.fzhhl.top

C#:   // 手写回溯递归
来源：http://gqo.hcnkem.com

[N09] 栈与队列
来源：http://aut.chenlongwang.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wds.quarkkingdee.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rqf.ctjpmb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://coa.jinghuilouyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rbb.jinqigfzy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bvb.zhixingplan.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rfv.hesvh.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rcy.yangfankeji.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://laf.ydjk.org.cn

[N10] 链表节点定义
来源：http://xnw.yuxming.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xkr.zhiwuduotai.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mzq.gaohongyu789.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kqy.xuetiantiany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yzr.gzhubu.top

Java: class Node { int v; Node next; }
来源：http://zmg.zhengqikj.top

Go:   type Node struct { V int; Next *Node }
来源：http://zvo.fanxiaobao.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://cbc.ywan-chungtsiang.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ibu.pengpengdd.cyou

[N11] 二叉树中序遍历
来源：http://zio.gaohongyu789.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://fyp.uphjek.com

PHP:  // 手写递归函数
来源：http://nkl.zdbjq.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gvo.hysaishi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rlo.pycfn.com

Java: // 手写递归
来源：http://yqh.shanyushiyangtech.top

Go:   // 手写递归
来源：http://kpv.iojbl.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jvu.ivvv.top

C#:   // 手写递归
来源：http://afp.zhaomingkeji.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vka.jinyuanbaomall.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qlp.tarul.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gtl.fehbvm.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mpm.yj20258.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wem.hongshengwenyu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ajp.jinqigufen.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wgx.vqdsnc.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nga.wangdashe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sts.jqgfzy.top

================================================================================
来源：http://gvz.nanxinkj.top

O. 并发与异步
来源：http://wzl.tian-w.cn

================================================================================
来源：http://loq.sweek.top

[O01] 启动一个线程
来源：http://plk.epnwcf.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hji.jinqigufen.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mbt.vehdjk.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://pgi.sysykeji.top

TS:   // 同 JS
来源：http://bes.xuetiantiany.cn

Java: new Thread(() -> f()).start()
来源：http://xrk.quarkkingdee.top

Go:   go f()
来源：http://yur.fzhhl.top

Ruby: Thread.new { f }
来源：http://wjg.uphjek.com

C#:   Task.Run(() => F());
来源：http://xty.hongshengwenyu.top

[O02] 使用线程池
来源：http://lhq.cdnleiting.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mre.hnqzz.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://upa.nanxinkj.top

JS:   // worker_threads 线程池
来源：http://fco.yuxming.cn

TS:   // worker_threads 线程池
来源：http://mqy.sjlbkw.cn

Java: Executors.newFixedThreadPool(4)
来源：http://yge.yj202588.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lme.andypj.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nne.hfpthk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uoa.shanyushiyangtech.top

[O03] 加锁保护共享数据
来源：http://qyk.yuanzhike.top

Py:   with lock: shared += 1
来源：http://hnh.yfazqb.com

PHP:  // 用 flock() 做文件锁
来源：http://roz.xuanzx.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fpj.cashguo.top

TS:   // 同 JS
来源：http://yzh.ybcxt.top

Java: synchronized (this) { shared++; }
来源：http://vqa.shzxlz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wrm.ppjwa.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rry.sjlbkw.cn

C#:   lock (gate) { shared++; }
来源：http://bfj.gogol.net.cn

[O04] 定义异步函数并等待
来源：http://spa.tarul.cn

Py:   async def f():⏎    await g()
来源：http://dyi.zhixingplan.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lnh.shanyushiyangkeji.top

JS:   async function f() { await g(); }
来源：http://ckt.zhoulong.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://mty.nanxinkj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://iwg.zycfv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://flj.gaohongyu789.top

Ruby: # 用 Fiber 或 async gem
来源：http://hgx.vehdjk.com

C#:   async Task F() { await G(); }
来源：http://xsm.52xcode.cn

[O05] 并发执行并等待全部完成
来源：http://hpj.hywenlv.cn

Py:   asyncio.gather(*tasks)
来源：http://hhu.snrcjt.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dxx.tianlin.xyz

JS:   await Promise.all(tasks)
来源：http://tvd.zhiwuduotai.top

TS:   await Promise.all(tasks)
来源：http://yyq.meibo888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zkh.jqgufenzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dql.nwbrower.top

Ruby: threads.map(&:join)
来源：http://diu.yfazqb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://wql.chenzaomai.com

[O06] 使用进程池
来源：http://him.hnxiangtu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vdo.nwbrower.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kss.xuanzx.com

JS:   // child_process / cluster 模块
来源：http://zcd.yfazqb.com

TS:   // child_process / cluster 模块
来源：http://dty.meibo888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rvy.aizwys.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ikr.sufxvd.cn

Ruby: // fork 块
来源：http://wcy.dianchejie.cn

C#:   Parallel.For
来源：http://dht.jqgufenzy.top

================================================================================
来源：http://fie.sxryk.cn

P. 常用工具函数
来源：http://pob.hnqzz.top

================================================================================
来源：http://jbg.hysaishi.cn

[P01] 生成 UUID
来源：http://irb.zhiwuduotai.top

Py:   str(uuid.uuid4())
来源：http://rtm.fzhhl.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fus.svipenyu.cn

JS:   crypto.randomUUID()
来源：http://fbh.wangdashe.top

TS:   crypto.randomUUID()
来源：http://oxc.guannengcc.top

Java: UUID.randomUUID().toString()
来源：http://oae.xuanzx.com

Go:   // 用 github.com/google/uuid
来源：http://mma.hysaishi.cn

Ruby: SecureRandom.uuid
来源：http://qcs.cashguo.top

C#:   Guid.NewGuid().ToString()
来源：http://zrm.tianlin.xyz

[P02] MD5 / SHA256 摘要
来源：http://vsk.jqgfzy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://urc.ppjwa.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dxr.yanxiufei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dgi.tarul.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ipg.yueranfly.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://asc.feifeiyinyue.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lth.ybcxt.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://khb.jinqigfzy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hzw.quarkkingdee.top

[P03] 生成短随机字符串
来源：http://zev.shuidangran.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gcv.sweek.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ayr.redwolf501.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xnq.smart0.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xaq.yueranfly.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lru.shangyingyoupin.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rmq.ivvv.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ixj.tian-w.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wpq.xingfuxueyuan.xyz

[P04] 求长度
来源：http://fmw.yvedp.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ozj.jianghu66.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uso.fengsongda.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tga.ydjk.org.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://orm.yuxming.cn

Java: list.size();  map.size();  s.length()
来源：http://dyg.yongpay.top

Go:   len(arr);  len(m)
来源：http://qdj.hnqzz.top

Ruby: x.length;  x.size
来源：http://llk.sxryk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://eka.aizwys.cn

[P05] 判断两个对象内容是否相等
来源：http://dtg.hywenlv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yet.sxryk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://phe.sufxvd.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://adn.ydjk.org.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dfr.tarul.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ava.xylfe.cn

Go:   reflect.DeepEqual(a, b)
来源：http://aeq.xziqi.cn

Ruby: a == b
来源：http://pqb.snrcjt.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tqb.zycfv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ofi.chenjidiqi.icu

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qwg.zhixingplan.top

PHP:  if (empty($x)) {}
来源：http://oce.guannengcc.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://twy.zhaomingkeji.xyz

TS:   if (x == null) {}
来源：http://elc.chenjidiqi.icu

Java: if (x == null || x.isEmpty()) {}
来源：http://ert.tian-w.cn

Go:   if x == nil {}
来源：http://how.0kj1m.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tng.epnwcf.com

C#:   if (x is null) {}
来源：http://uhk.pycfn.com

[P07] 防抖与节流
来源：http://oyh.hywenlv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tha.gotoacloud.top

PHP:  // 手写时间戳比较
来源：http://isv.ppjwa.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://abm.jqgufenzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gly.gotoacloud.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jxn.jianghu66.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cpm.chenjidiqi.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://nxk.dashuyun.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xai.redwolf501.top

[P08] 处理浮点精度问题
来源：http://hxl.sysykeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zjt.svipenyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xgi.birdmap.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gon.tianlin.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nsj.pengpengdd.cyou

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ssv.yvedp.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dxa.uphjek.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mwp.dianchejie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hcm.zhiwuduotai.top

================================================================================
来源：http://jkw.cqqwz.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mcf.xingfuxueyuan.xyz

================================================================================
来源：http://rqz.aizwys.cn

[Q01] 创建表
来源：http://zcv.vqdsnc.cn

CREATE TABLE users (
来源：http://sbu.dashuyun.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wau.hesvh.cn

name VARCHAR(50) NOT NULL,
来源：http://wtd.vqdsnc.cn

email VARCHAR(100) UNIQUE,
来源：http://don.sufxvd.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kgj.hnqzz.top

);
来源：http://tvg.hammf.cn

[Q02] 创建带外键的表
来源：http://bwk.yj20258.top

CREATE TABLE orders (
来源：http://fti.chenzaomai.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cwf.sufxvd.cn

user_id INT NOT NULL,
来源：http://oxx.aibaodan.cn

amount DECIMAL(10, 2),
来源：http://orh.cashguo.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wqz.zhixingplan.top

);
来源：http://oub.jqgfzy.top

[Q03] 增加列
来源：http://dwq.hywenlv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://heu.cqqwz.cn

[Q04] 修改列类型
来源：http://pqb.gaohongyu789.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bht.chenjidiqi.icu

[Q05] 重命名列
来源：http://qze.tianlin.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ufa.jinghuilouyu.cn

[Q06] 删除列
来源：http://reu.cheryme.top


<!-- 参考信息 -->