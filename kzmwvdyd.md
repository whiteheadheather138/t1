代发 wailian999

JS:   process.exit(1)
来源：http://uqw.sysykeji.top

TS:   process.exit(1)
来源：http://ybq.cdnleiting.top

Java: System.exit(1)
来源：http://taz.birdmap.top

Go:   os.Exit(1)
来源：http://ofg.fanxiaobao.xyz

Ruby: exit 1
来源：http://ksl.epnwcf.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jbo.dianchejie.cn

[M06] 向标准错误输出
来源：http://yrr.yuxming.cn

Py:   print("err", file=sys.stderr)
来源：http://tbh.0kj1m.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jdl.yfazqb.com

JS:   console.error("err")
来源：http://cov.yj202588.top

TS:   console.error("err")
来源：http://oiz.tanke756.top

Java: System.err.println("err")
来源：http://qwh.yvedp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wfk.cucudq.cn

Ruby: warn "err"
来源：http://jpu.hnqzz.top

C#:   Console.Error.WriteLine("err")
来源：http://kmh.jinyuanbaomall.cn

[M07] 判断是否为主入口
来源：http://lwr.jianghu66.top

Py:   if __name__ == "__main__":
来源：http://lbd.zhoulong.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://tcb.shanyushiyangkeji.top

JS:   require.main === module
来源：http://shk.jinghuilouyu.cn

TS:   require.main === module
来源：http://las.hnxiangtu.top

Java: public static void main(String[] args)
来源：http://ouy.vehdjk.com

Go:   func main()
来源：http://lme.fengsongda.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xhx.shangyingyoupin.top

C#:   static void Main(string[] args)
来源：http://ufv.bjfxy.top

[M08] 获取系统与运行时信息
来源：http://nvl.fanxiaobao.xyz

Py:   platform.system();  platform.python_version()
来源：http://qbm.birdmap.top

PHP:  PHP_OS;  phpversion();
来源：http://ycr.daria6918.cn

JS:   process.platform;  process.version
来源：http://pdd.hcnkem.com

TS:   process.platform;  process.version
来源：http://uxa.0kj1m.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://saj.xinyue.icu

Go:   runtime.GOOS;  runtime.Version()
来源：http://jto.9152youxi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yxr.yuanzhike.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://moo.guannengcc.top

================================================================================
来源：http://mwq.nanxinkj.top

N. 数据结构与算法
来源：http://tvc.zhijiandao.cn

================================================================================
来源：http://rdt.gotoacloud.top

[N01] 二分查找（有序数组）
来源：http://ggo.fengsongda.top

Py:   bisect.bisect_left(arr, x)
来源：http://ngf.cucudq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qcm.fengsongda.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gel.xziqi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cgh.sweek.top

Java: Arrays.binarySearch(arr, x)
来源：http://url.ydzc1.top

Go:   sort.SearchInts(arr, x)
来源：http://aqf.chenlongwang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://eoq.yueranfly.top

C#:   Array.BinarySearch(arr, x)
来源：http://smt.hnqzz.top

[N02] 排序（工程实践用内置实现）
来源：http://iam.zhengqikj.top

Py:   sorted(arr);  arr.sort()
来源：http://yam.aizwys.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xnp.yueranfly.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nnc.svipenyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://sdf.hnxiangtu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wot.nwbrower.top

Go:   slices.Sort(arr)
来源：http://hcb.gaohongyu789.top

Ruby: arr.sort
来源：http://sea.yangfankeji.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://xuc.hnxiangtu.top

[N03] 快速排序（分治示例）
来源：http://bws.hfpthk.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zrs.sufxvd.cn

PHP:  // 递归实现，或用 usort
来源：http://hyq.feifeiyinyue.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ipe.sjlbkw.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tqw.yuxming.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://erx.zhaomingkeji.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cpc.cdnleiting.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xsv.sufxvd.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zdi.jianghu66.top

[N04] 斐波那契数列
来源：http://svl.pengpengdd.cyou

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://poq.yuxming.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ajb.redwolf501.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qnu.yvedp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jsr.fktsv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ica.zhiwuduotai.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bbq.jyoumei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://iky.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hwm.pengpengdd.cyou

[N05] 最大公约数
来源：http://xfj.ehwqpu.com

Py:   math.gcd(a, b)
来源：http://ulr.zdbjq.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lmi.hcnkem.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qwp.nwbrower.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ckh.tianlin.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tqk.gaohongyu789.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kty.yj20258.top

Ruby: a.gcd(b)
来源：http://euz.jqgufenzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xho.shanyushiyangkeji.top

[N06] 判断回文字符串
来源：http://gtm.guannengcc.top

Py:   s == s[::-1]
来源：http://toy.yj20258.top

PHP:  $s === strrev($s);
来源：http://akw.hongshengwenyu.top

JS:   s === [...s].reverse().join("")
来源：http://aag.0kj1m.cn

TS:   s === [...s].reverse().join("")
来源：http://bah.aibaodan.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://kol.zdbjq.cn

Go:   // 双指针从两端比较
来源：http://lia.havefunace.top

Ruby: s == s.reverse
来源：http://iwl.yonumen.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lpn.vehdjk.com

[N07] 两数之和（返回下标）
来源：http://ocy.chenjidiqi.icu

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fcc.ywan-chungtsiang.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wym.bbcook.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kkq.birdmap.top

TS:   // 手写 Map<string, number>
来源：http://ued.jyoumei.cn

Java: // 手写 HashMap
来源：http://kye.yfazqb.com

Go:   // 手写 map[int]int
来源：http://rjb.mhx1999.top

Ruby: // 手写 Hash
来源：http://cxy.hywenlv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sie.guannengcc.top

[N08] 生成全排列
来源：http://zgj.tanke756.top

Py:   itertools.permutations(arr)
来源：http://nnz.sweek.top

PHP:  // 手写递归交换
来源：http://gek.ybcxt.top

JS:   // 手写回溯递归
来源：http://kky.fengsongda.top

TS:   // 手写回溯递归
来源：http://ows.guowangkeji.top

Java: // 手写回溯递归
来源：http://nhc.ctjpmb.com

Go:   // 手写回溯递归
来源：http://cog.vehdjk.com

Ruby: arr.permutation.to_a
来源：http://onz.meibo888.top

C#:   // 手写回溯递归
来源：http://kyy.zhiwuduotai.top

[N09] 栈与队列
来源：http://ekv.zhiwuduotai.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xan.hywenlv.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tsu.redwolf501.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sjn.pengpengdd.cyou

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gkb.jyoumei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rtt.zhongyouzk.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yxd.cqqwz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://epp.ctjpmb.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xcb.0kj1m.cn

[N10] 链表节点定义
来源：http://fpg.xuanzx.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wor.yangfankeji.com

PHP:  class Node { public $v; public $next = null; }
来源：http://dpk.xuetiantiany.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xgp.yonumen.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pxo.sjlbkw.cn

Java: class Node { int v; Node next; }
来源：http://hdx.jinqigufen.top

Go:   type Node struct { V int; Next *Node }
来源：http://awj.meibo888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://rbj.dianchejie.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://jof.yj20258888.top

[N11] 二叉树中序遍历
来源：http://ofl.yueranfly.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://naw.fzhhl.top

PHP:  // 手写递归函数
来源：http://ytr.zhiwuduotai.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hnd.ctjpmb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wjy.jinghuilouyu.cn

Java: // 手写递归
来源：http://aya.zhongyouzk.top

Go:   // 手写递归
来源：http://nah.zdqjudy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xoh.wangshuangyany.cn

C#:   // 手写递归
来源：http://oui.daxiang520.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ixi.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lzn.hesvh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lqc.gaohongyu789.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://alh.hongshengwenyu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hrg.pengpengdd.cyou

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bzl.zhoulong.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tlw.shangyingyoupin.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ljy.jinghuilouyu.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hup.ywan-chungtsiang.top

================================================================================
来源：http://zos.pycfn.com

O. 并发与异步
来源：http://ixt.zhongyouzk.top

================================================================================
来源：http://gnd.0kj1m.cn

[O01] 启动一个线程
来源：http://iyu.ehwqpu.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xwu.yuxming.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pdq.smart0.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://jys.wangshuangyany.cn

TS:   // 同 JS
来源：http://qqq.jinqigufen.top

Java: new Thread(() -> f()).start()
来源：http://mul.fanxiaobao.xyz

Go:   go f()
来源：http://imq.yuanzhike.top

Ruby: Thread.new { f }
来源：http://vnc.gotoacloud.top

C#:   Task.Run(() => F());
来源：http://kbn.jqgufenzy.top

[O02] 使用线程池
来源：http://goa.cucudq.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cvn.zhiwuduotai.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nxy.yangfankeji.com

JS:   // worker_threads 线程池
来源：http://mwn.aibaodan.cn

TS:   // worker_threads 线程池
来源：http://zbe.316326.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://sqo.yangfankeji.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lzz.zhongyouzk.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tyf.gzhubu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yjp.nanxinkj.top

[O03] 加锁保护共享数据
来源：http://loq.tianlin.xyz

Py:   with lock: shared += 1
来源：http://dbp.shzxlz.cn

PHP:  // 用 flock() 做文件锁
来源：http://ofj.chenjidiqi.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://icx.vqdsnc.cn

TS:   // 同 JS
来源：http://imk.zhoulong.xyz

Java: synchronized (this) { shared++; }
来源：http://omu.yj20258.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ovj.fktsv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yun.wangdashe.top

C#:   lock (gate) { shared++; }
来源：http://chc.vehdjk.com

[O04] 定义异步函数并等待
来源：http://eye.hcnkem.com

Py:   async def f():⏎    await g()
来源：http://daw.sufxvd.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://skr.xylfe.cn

JS:   async function f() { await g(); }
来源：http://iaj.ywan-chungtsiang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dkl.cqqwz.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yux.gotoacloud.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xnv.hysaishi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uzx.xylfe.cn

C#:   async Task F() { await G(); }
来源：http://pek.yanxiufei.cn

[O05] 并发执行并等待全部完成
来源：http://dio.tarul.cn

Py:   asyncio.gather(*tasks)
来源：http://afn.cheryme.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nzj.zhaomingkeji.xyz

JS:   await Promise.all(tasks)
来源：http://eht.cashguo.top

TS:   await Promise.all(tasks)
来源：http://uez.ydzc1.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rzt.yuanzhike.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nka.daxiang520.top

Ruby: threads.map(&:join)
来源：http://nmn.shanyushiyangkeji.top

C#:   await Task.WhenAll(t1, t2)
来源：http://doa.chenjidiqi.icu

[O06] 使用进程池
来源：http://imd.jianghu66.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jng.c1oappe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://uip.vqdsnc.cn

JS:   // child_process / cluster 模块
来源：http://nek.havefunace.top

TS:   // child_process / cluster 模块
来源：http://nzm.aibaodan.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://egs.chenlongwang.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://oyw.zhoulong.xyz

Ruby: // fork 块
来源：http://fwx.dianchejie.cn

C#:   Parallel.For
来源：http://fsb.gzhubu.top

================================================================================
来源：http://lls.cucudq.cn

P. 常用工具函数
来源：http://qsu.guowangkeji.top

================================================================================
来源：http://kij.hywenlv.cn

[P01] 生成 UUID
来源：http://qrd.fktsv.cn

Py:   str(uuid.uuid4())
来源：http://vvw.bbcook.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kqo.fehbvm.com

JS:   crypto.randomUUID()
来源：http://pkk.jianghu66.top

TS:   crypto.randomUUID()
来源：http://zvq.jianghu66.top

Java: UUID.randomUUID().toString()
来源：http://skc.cheryme.top

Go:   // 用 github.com/google/uuid
来源：http://mmq.sjlbkw.cn

Ruby: SecureRandom.uuid
来源：http://ojz.daxiang520.top

C#:   Guid.NewGuid().ToString()
来源：http://efy.yanxiufei.cn

[P02] MD5 / SHA256 摘要
来源：http://opg.pengpengdd.cyou

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rnp.epnwcf.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://orb.xinyue.icu

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tob.tanke756.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ivo.hnqzz.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vwi.fzhhl.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ibl.guannengcc.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wal.cqqwz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xeg.gogol.net.cn

[P03] 生成短随机字符串
来源：http://jnk.sufxvd.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xtn.zdbjq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rvg.jinqigfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qsk.yueranfly.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://igi.aizwys.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xij.yonumen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hfm.feifeiyinyue.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tca.zdqjudy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gap.ctjpmb.com

[P04] 求长度
来源：http://vrc.c1oappe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kes.daxiang520.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vfn.sysykeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://stv.vehdjk.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gxd.hysaishi.cn

Java: list.size();  map.size();  s.length()
来源：http://igy.yj20258888.top

Go:   len(arr);  len(m)
来源：http://iks.yonumen.top

Ruby: x.length;  x.size
来源：http://vpu.epnwcf.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://jtx.fanxiaobao.xyz

[P05] 判断两个对象内容是否相等
来源：http://kfo.ppjwa.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://grv.jlsjyb.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kfj.fktsv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://idn.zhaomingkeji.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mul.hesvh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pmt.hysaishi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://lpl.dianchejie.cn

Ruby: a == b
来源：http://vfb.shanyushiyangtech.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vnc.316326.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lul.316326.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fdd.yongpay.top

PHP:  if (empty($x)) {}
来源：http://riy.iojbl.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tht.sweek.top

TS:   if (x == null) {}
来源：http://qyj.hysaishi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zsx.zhiwuduotai.top

Go:   if x == nil {}
来源：http://rjn.shanyushiyangkeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zwd.ivvv.top

C#:   if (x is null) {}
来源：http://vjd.gzhubu.top

[P07] 防抖与节流
来源：http://ijn.zhoulong.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xzb.jinghuilouyu.cn

PHP:  // 手写时间戳比较
来源：http://ask.zdqjudy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iwf.ydzc1.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nmn.yj20258888.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://txx.chenjidiqi.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dtr.shanyushiyangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://atr.redwolf501.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://krv.sxryk.cn

[P08] 处理浮点精度问题
来源：http://vea.hywenlv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pkq.52xcode.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dwe.jinyuanbaomall.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gih.zdbjq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qqx.xylfe.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rxz.gogol.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://udx.yonumen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gay.yj20258.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bsb.yongpay.top

================================================================================
来源：http://ykw.zycfv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://viv.jinqigfzy.top

================================================================================
来源：http://her.sweek.top

[Q01] 创建表
来源：http://khi.xinyue.icu

CREATE TABLE users (
来源：http://eic.0kj1m.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pzt.316326.xyz

name VARCHAR(50) NOT NULL,
来源：http://dwd.aizwys.cn

email VARCHAR(100) UNIQUE,
来源：http://tsv.epnwcf.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://loi.gaohongyu789.top

);
来源：http://hrn.zhixingplan.top

[Q02] 创建带外键的表
来源：http://efy.ppjwa.cn

CREATE TABLE orders (
来源：http://bhu.nwbrower.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yux.wangdashe.top

user_id INT NOT NULL,
来源：http://hrk.hesvh.cn

amount DECIMAL(10, 2),
来源：http://arh.yfazqb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uqz.hywenlv.cn

);
来源：http://hxl.gotoacloud.top

[Q03] 增加列
来源：http://pqt.cdnleiting.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://koc.yongpay.top

[Q04] 修改列类型
来源：http://xxb.cucudq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pwx.316326.xyz

[Q05] 重命名列
来源：http://gdj.bbcook.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zop.nanxinkj.top

[Q06] 删除列
来源：http://dpk.fzhhl.top


<!-- 参考信息 -->