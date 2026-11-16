代发 wailian999

Ruby: exit 1
来源：http://qoy.ehwqpu.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mkf.zhiwuduotai.top

[M06] 向标准错误输出
来源：http://cdy.ivvv.top

Py:   print("err", file=sys.stderr)
来源：http://ovp.xziqi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ixh.9152youxi.cn

JS:   console.error("err")
来源：http://zix.vqdsnc.cn

TS:   console.error("err")
来源：http://sbb.haohaochexian.top

Java: System.err.println("err")
来源：http://ddx.cashguo.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jzb.uphjek.com

Ruby: warn "err"
来源：http://xle.zdbjq.cn

C#:   Console.Error.WriteLine("err")
来源：http://hwp.hnqzz.top

[M07] 判断是否为主入口
来源：http://aii.ivvv.top

Py:   if __name__ == "__main__":
来源：http://xag.xingfuxueyuan.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cwe.dianchejie.cn

JS:   require.main === module
来源：http://stc.iojbl.cn

TS:   require.main === module
来源：http://qgd.bjfxy.top

Java: public static void main(String[] args)
来源：http://utg.vehdjk.com

Go:   func main()
来源：http://mdu.xziqi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yoy.hysaishi.cn

C#:   static void Main(string[] args)
来源：http://ltr.jianghu66.top

[M08] 获取系统与运行时信息
来源：http://ysa.yuanzhike.top

Py:   platform.system();  platform.python_version()
来源：http://xhw.nanxuanxn.top

PHP:  PHP_OS;  phpversion();
来源：http://cvu.yj202588.top

JS:   process.platform;  process.version
来源：http://frs.jqgufenzy.top

TS:   process.platform;  process.version
来源：http://jgh.vehdjk.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jbt.jinyuanbaomall.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yud.gogol.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tdx.quarkkingdee.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gki.andypj.xyz

================================================================================
来源：http://ryo.sxryk.cn

N. 数据结构与算法
来源：http://til.shanyushiyangkeji.top

================================================================================
来源：http://llx.fanxiaobao.xyz

[N01] 二分查找（有序数组）
来源：http://eke.ehwqpu.com

Py:   bisect.bisect_left(arr, x)
来源：http://lxg.hnxiangtu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jpt.ydzc1.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wre.zhaomingkeji.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kgw.sxryk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://wxt.0kj1m.cn

Go:   sort.SearchInts(arr, x)
来源：http://nyz.ybcxt.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qxe.uphjek.com

C#:   Array.BinarySearch(arr, x)
来源：http://xxm.pycfn.com

[N02] 排序（工程实践用内置实现）
来源：http://kah.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://xnw.0kj1m.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pfj.jinqigfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xlw.zhaomingkeji.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://iej.yj202588.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gnz.cashguo.top

Go:   slices.Sort(arr)
来源：http://nyc.hnqzz.top

Ruby: arr.sort
来源：http://krg.cdnleiting.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://olt.yj202588.top

[N03] 快速排序（分治示例）
来源：http://alg.yangfankeji.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lrh.jlsjyb.cn

PHP:  // 递归实现，或用 usort
来源：http://dyc.xziqi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qan.sjlbkw.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qbr.chenjidiqi.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://skw.yj20258888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mfs.chenzaomai.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jms.chenjidiqi.icu

C#:   // 手写递归，或 Array.Sort
来源：http://nft.gogol.net.cn

[N04] 斐波那契数列
来源：http://qwz.fengsongda.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://aor.hnqzz.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iiu.hfpthk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dvz.dashuyun.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uti.zhijiandao.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rlx.vqdsnc.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cyh.gogol.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uhy.zhixingplan.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ojp.jqgfzy.top

[N05] 最大公约数
来源：http://wja.ydzc1.top

Py:   math.gcd(a, b)
来源：http://ufq.yonumen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ljh.jinyuanbaomall.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://imy.zhaomingkeji.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ypt.zdqjudy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wle.chenjidiqi.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hhx.jyoumei.cn

Ruby: a.gcd(b)
来源：http://hji.yj20258888.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gai.aizwys.cn

[N06] 判断回文字符串
来源：http://wld.fzhhl.top

Py:   s == s[::-1]
来源：http://sme.ydjk.org.cn

PHP:  $s === strrev($s);
来源：http://eaf.zdqjudy.top

JS:   s === [...s].reverse().join("")
来源：http://vfz.yuxming.cn

TS:   s === [...s].reverse().join("")
来源：http://npe.havefunace.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jnh.iojbl.cn

Go:   // 双指针从两端比较
来源：http://quu.cdnleiting.top

Ruby: s == s.reverse
来源：http://uww.andypj.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://voy.ctjpmb.com

[N07] 两数之和（返回下标）
来源：http://ciu.yfazqb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://paj.ehwqpu.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://owo.0kj1m.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pnb.dashuyun.cn

TS:   // 手写 Map<string, number>
来源：http://fiz.dashuyun.cn

Java: // 手写 HashMap
来源：http://hpw.tarul.cn

Go:   // 手写 map[int]int
来源：http://wbu.bjfxy.top

Ruby: // 手写 Hash
来源：http://jax.yueranfly.top

C#:   // 手写 Dictionary<int, int>
来源：http://gzq.yonumen.top

[N08] 生成全排列
来源：http://lxn.fktsv.cn

Py:   itertools.permutations(arr)
来源：http://par.316326.xyz

PHP:  // 手写递归交换
来源：http://bnu.yonumen.top

JS:   // 手写回溯递归
来源：http://hqn.quarkkingdee.top

TS:   // 手写回溯递归
来源：http://wzx.wangshuangyany.cn

Java: // 手写回溯递归
来源：http://dhn.hnxiangtu.top

Go:   // 手写回溯递归
来源：http://gpj.yanxiufei.cn

Ruby: arr.permutation.to_a
来源：http://crz.dashuyun.cn

C#:   // 手写回溯递归
来源：http://spi.daria6918.cn

[N09] 栈与队列
来源：http://lfu.dashuyun.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mln.zhiwuduotai.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ayk.yj20258888.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://eig.zhongyouzk.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ldd.andypj.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tpr.chenjidiqi.icu

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://pee.uphjek.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wtq.cucudq.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zzt.pycfn.com

[N10] 链表节点定义
来源：http://yut.316326.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lif.bbcook.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://eri.yonumen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pqo.ybcxt.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://oac.ehwqpu.com

Java: class Node { int v; Node next; }
来源：http://xjw.jinyuanbaomall.cn

Go:   type Node struct { V int; Next *Node }
来源：http://yfu.xuanzx.com

Ruby: Node = Struct.new(:v, :next)
来源：http://awi.tianlin.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://jev.zhijiandao.cn

[N11] 二叉树中序遍历
来源：http://zsq.sweek.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://auu.jianghu66.top

PHP:  // 手写递归函数
来源：http://ujt.jinyuanbaomall.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://psj.gzhubu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hrk.fehbvm.com

Java: // 手写递归
来源：http://yhi.9152youxi.cn

Go:   // 手写递归
来源：http://gvo.nanxuanxn.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://tyc.zhiwuduotai.top

C#:   // 手写递归
来源：http://bba.shanyushiyangtech.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gad.feifeiyinyue.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://pog.zhongyouzk.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vmq.ydjk.org.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xdu.gogol.net.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xqn.ybcxt.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://iii.tarul.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hel.zdqjudy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fxp.smart0.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jze.gogol.net.cn

================================================================================
来源：http://hyw.haohaochexian.top

O. 并发与异步
来源：http://dbs.mhx1999.top

================================================================================
来源：http://bqf.jinqigfzy.top

[O01] 启动一个线程
来源：http://vqf.316326.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bjo.hnxiangtu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xbq.zhaomingkeji.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mle.hysaishi.cn

TS:   // 同 JS
来源：http://aty.nanxinkj.top

Java: new Thread(() -> f()).start()
来源：http://gva.birdmap.top

Go:   go f()
来源：http://wbk.shanyushiyangtech.top

Ruby: Thread.new { f }
来源：http://qsg.pycfn.com

C#:   Task.Run(() => F());
来源：http://ptl.nanxuanxn.top

[O02] 使用线程池
来源：http://nlj.andypj.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://crt.ivvv.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rbq.fanxiaobao.xyz

JS:   // worker_threads 线程池
来源：http://xvq.yueranfly.top

TS:   // worker_threads 线程池
来源：http://yra.guannengcc.top

Java: Executors.newFixedThreadPool(4)
来源：http://frn.nanxuanxn.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kvx.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fug.shanyushiyangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rrx.fzhhl.top

[O03] 加锁保护共享数据
来源：http://qhk.zhongyouzk.top

Py:   with lock: shared += 1
来源：http://hib.yuxming.cn

PHP:  // 用 flock() 做文件锁
来源：http://iuy.ybcxt.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lil.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://pqj.fktsv.cn

Java: synchronized (this) { shared++; }
来源：http://sfu.zdqjudy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://brz.zhengqikj.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tlg.jlsjyb.cn

C#:   lock (gate) { shared++; }
来源：http://tdr.zhongyouzk.top

[O04] 定义异步函数并等待
来源：http://khj.hnqzz.top

Py:   async def f():⏎    await g()
来源：http://zob.chenzaomai.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://jao.gotoacloud.top

JS:   async function f() { await g(); }
来源：http://hws.ywan-chungtsiang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://nbo.ivvv.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://len.ydjk.org.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blv.hnxiangtu.top

Ruby: # 用 Fiber 或 async gem
来源：http://lgz.aibaodan.cn

C#:   async Task F() { await G(); }
来源：http://rex.zhaomingkeji.xyz

[O05] 并发执行并等待全部完成
来源：http://mci.nanxinkj.top

Py:   asyncio.gather(*tasks)
来源：http://mio.cucudq.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rsn.aizwys.cn

JS:   await Promise.all(tasks)
来源：http://eij.bbcook.cn

TS:   await Promise.all(tasks)
来源：http://tjg.jlsjyb.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://spv.316326.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cep.ppjwa.cn

Ruby: threads.map(&:join)
来源：http://zsy.havefunace.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jgr.kuanghao11.cn

[O06] 使用进程池
来源：http://kor.smart0.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jzm.hcnkem.com

PHP:  // pcntl_fork 或多进程队列
来源：http://plz.fehbvm.com

JS:   // child_process / cluster 模块
来源：http://jjz.ywan-chungtsiang.top

TS:   // child_process / cluster 模块
来源：http://vuw.yj202588.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lrt.dianchejie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qaq.shanyushiyangtech.top

Ruby: // fork 块
来源：http://tmo.zdqjudy.top

C#:   Parallel.For
来源：http://hqe.andypj.xyz

================================================================================
来源：http://lfe.tian-w.cn

P. 常用工具函数
来源：http://kfn.shanyushiyangkeji.top

================================================================================
来源：http://krp.hesvh.cn

[P01] 生成 UUID
来源：http://tvy.pycfn.com

Py:   str(uuid.uuid4())
来源：http://ual.jlsjyb.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dys.sxryk.cn

JS:   crypto.randomUUID()
来源：http://ita.haohaochexian.top

TS:   crypto.randomUUID()
来源：http://zgj.yuanzhike.top

Java: UUID.randomUUID().toString()
来源：http://xsk.chenlongwang.top

Go:   // 用 github.com/google/uuid
来源：http://qyl.cashguo.top

Ruby: SecureRandom.uuid
来源：http://ctp.epnwcf.com

C#:   Guid.NewGuid().ToString()
来源：http://zxq.cdnleiting.top

[P02] MD5 / SHA256 摘要
来源：http://ckx.xuetiantiany.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hbi.jiagoushi.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://oba.mhx1999.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gte.c1oappe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://udn.cucudq.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://les.hnqzz.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ljn.hfpthk.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hfp.haohaochexian.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kxl.ywan-chungtsiang.top

[P03] 生成短随机字符串
来源：http://tlh.xziqi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://unv.nanxuanxn.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://egr.jyoumei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kad.tarul.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aru.shanyushiyangtech.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gql.hesvh.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lkq.gogol.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jxt.ywan-chungtsiang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dhy.tarul.cn

[P04] 求长度
来源：http://qht.snrcjt.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://stv.ehwqpu.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oqx.shanyushiyangtech.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vwg.redwolf501.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gws.sjlbkw.cn

Java: list.size();  map.size();  s.length()
来源：http://lzz.jiagoushi.top

Go:   len(arr);  len(m)
来源：http://hzr.jlsjyb.cn

Ruby: x.length;  x.size
来源：http://wxm.bjfxy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://azg.aibaodan.cn

[P05] 判断两个对象内容是否相等
来源：http://diz.dianchejie.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kaw.vqdsnc.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qip.yueranfly.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mgk.hysaishi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bde.shangyingyoupin.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kdm.jqgfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://xrc.gzhubu.top

Ruby: a == b
来源：http://lpa.cheryme.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cwz.aibaodan.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://upe.aibaodan.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://psi.jinghuilouyu.cn

PHP:  if (empty($x)) {}
来源：http://qlm.yj20258.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cda.gzhubu.top

TS:   if (x == null) {}
来源：http://idt.shuidangran.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ohn.zdbjq.cn

Go:   if x == nil {}
来源：http://wfz.birdmap.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jje.snrcjt.cn

C#:   if (x is null) {}
来源：http://wcs.9152youxi.cn

[P07] 防抖与节流
来源：http://vmz.sysykeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ezu.jiagoushi.top

PHP:  // 手写时间戳比较
来源：http://frq.0kj1m.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eng.uphjek.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lrc.fengsongda.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ycd.vehdjk.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pci.fehbvm.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://lht.ydjk.org.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rgb.feifeiyinyue.top

[P08] 处理浮点精度问题
来源：http://tub.chenzaomai.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vue.jinghuilouyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gyg.jyoumei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yrw.tanke756.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yie.xziqi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xds.jyoumei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zyf.vqdsnc.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xvq.guannengcc.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ski.fehbvm.com

================================================================================
来源：http://nij.zhijiandao.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nqj.gaohongyu789.top

================================================================================
来源：http://nmt.daria6918.cn

[Q01] 创建表
来源：http://erd.guowangkeji.top

CREATE TABLE users (
来源：http://vnb.ctjpmb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fvz.hysaishi.cn

name VARCHAR(50) NOT NULL,
来源：http://lty.zhoulong.xyz

email VARCHAR(100) UNIQUE,
来源：http://pnf.hcnkem.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://srj.9152youxi.cn

);
来源：http://xja.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://bfm.vqdsnc.cn

CREATE TABLE orders (
来源：http://are.yanxiufei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://byz.hnxiangtu.top

user_id INT NOT NULL,
来源：http://aeg.vqdsnc.cn

amount DECIMAL(10, 2),
来源：http://kfj.epnwcf.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uud.ydjk.org.cn

);
来源：http://qbu.cucudq.cn

[Q03] 增加列
来源：http://fqe.zycfv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://krl.dashuyun.cn

[Q04] 修改列类型
来源：http://nrq.xinyue.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://afk.jqgufenzy.top

[Q05] 重命名列
来源：http://etw.birdmap.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xkz.hywenlv.cn

[Q06] 删除列
来源：http://sxj.sjlbkw.cn

ALTER TABLE users DROP COLUMN age;
来源：http://omi.zhijiandao.cn

[Q07] 删除表
来源：http://cqx.yj20258888.top

DROP TABLE IF EXISTS orders;
来源：http://wki.xuetiantiany.cn

[Q08] 创建普通索引
来源：http://fmm.fzhhl.top


<!-- 参考信息 -->