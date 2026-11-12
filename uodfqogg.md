代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://xlg.xuetiantiany.cn

[M05] 设置退出码
来源：http://ngz.hesvh.cn

Py:   sys.exit(1)
来源：http://hzt.c1oappe.top

PHP:  exit(1);
来源：http://ava.sysykeji.top

JS:   process.exit(1)
来源：http://kwq.pengpengdd.cyou

TS:   process.exit(1)
来源：http://hcg.epnwcf.com

Java: System.exit(1)
来源：http://tyr.zdqjudy.top

Go:   os.Exit(1)
来源：http://rft.haohaochexian.top

Ruby: exit 1
来源：http://gqb.xylfe.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hzl.feifeiyinyue.top

[M06] 向标准错误输出
来源：http://tex.dianchejie.cn

Py:   print("err", file=sys.stderr)
来源：http://hna.zhengqikj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://joa.xingfuxueyuan.xyz

JS:   console.error("err")
来源：http://niz.wangshuangyany.cn

TS:   console.error("err")
来源：http://sgn.ppjwa.cn

Java: System.err.println("err")
来源：http://ara.9152youxi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://avx.nanxuanxn.top

Ruby: warn "err"
来源：http://vyx.gaohongyu789.top

C#:   Console.Error.WriteLine("err")
来源：http://pun.jinghuilouyu.cn

[M07] 判断是否为主入口
来源：http://yan.xuetiantiany.cn

Py:   if __name__ == "__main__":
来源：http://oip.dashuyun.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nzh.shanyushiyangtech.top

JS:   require.main === module
来源：http://kxz.redwolf501.top

TS:   require.main === module
来源：http://rfp.snrcjt.cn

Java: public static void main(String[] args)
来源：http://lfg.svipenyu.cn

Go:   func main()
来源：http://dop.shuidangran.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://crj.jyoumei.cn

C#:   static void Main(string[] args)
来源：http://cvj.zhijiandao.cn

[M08] 获取系统与运行时信息
来源：http://tra.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://qdb.hnqzz.top

PHP:  PHP_OS;  phpversion();
来源：http://czp.iojbl.cn

JS:   process.platform;  process.version
来源：http://usi.wangshuangyany.cn

TS:   process.platform;  process.version
来源：http://sfo.xingfuxueyuan.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vzr.ehwqpu.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://qiv.shanyushiyangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ovz.wangshuangyany.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nos.guannengcc.top

================================================================================
来源：http://xsv.zhaomingkeji.xyz

N. 数据结构与算法
来源：http://qqf.andypj.xyz

================================================================================
来源：http://oxk.cucudq.cn

[N01] 二分查找（有序数组）
来源：http://htl.cucudq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://wqz.gzhubu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ddj.svipenyu.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aqr.shzxlz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ash.ybcxt.top

Java: Arrays.binarySearch(arr, x)
来源：http://rpv.tanke756.top

Go:   sort.SearchInts(arr, x)
来源：http://bkf.52xcode.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hlq.shanyushiyangtech.top

C#:   Array.BinarySearch(arr, x)
来源：http://twg.zdqjudy.top

[N02] 排序（工程实践用内置实现）
来源：http://fyr.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://wdd.hammf.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mti.jqgufenzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rek.jiagoushi.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://yuu.sysykeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nsu.xuanzx.com

Go:   slices.Sort(arr)
来源：http://oxl.guannengcc.top

Ruby: arr.sort
来源：http://lut.sufxvd.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://xny.hcnkem.com

[N03] 快速排序（分治示例）
来源：http://ypu.hammf.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vai.zdqjudy.top

PHP:  // 递归实现，或用 usort
来源：http://yld.xziqi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bsv.zhijiandao.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vcz.shangyingyoupin.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pdi.haohaochexian.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oje.cqqwz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yox.gaohongyu789.top

C#:   // 手写递归，或 Array.Sort
来源：http://yrv.hcnkem.com

[N04] 斐波那契数列
来源：http://lqz.jqgufenzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wrs.jianghu66.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fsj.jinghuilouyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iyq.ydzc1.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tue.iojbl.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vaq.shzxlz.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cwu.ydjk.org.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://seg.tian-w.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wfn.yj20258888.top

[N05] 最大公约数
来源：http://yvf.yangfankeji.com

Py:   math.gcd(a, b)
来源：http://ktr.xziqi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qid.yuxming.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://usn.snrcjt.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wjv.bjfxy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://nks.aibaodan.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hkr.ywan-chungtsiang.top

Ruby: a.gcd(b)
来源：http://qvh.gotoacloud.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://kal.quarkkingdee.top

[N06] 判断回文字符串
来源：http://mnk.xuetiantiany.cn

Py:   s == s[::-1]
来源：http://aet.xingfuxueyuan.xyz

PHP:  $s === strrev($s);
来源：http://mvt.sweek.top

JS:   s === [...s].reverse().join("")
来源：http://mcu.gogol.net.cn

TS:   s === [...s].reverse().join("")
来源：http://ldj.yj202588.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xwb.hysaishi.cn

Go:   // 双指针从两端比较
来源：http://biu.nwbrower.top

Ruby: s == s.reverse
来源：http://epr.zhengqikj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://eky.vehdjk.com

[N07] 两数之和（返回下标）
来源：http://qhp.yj20258.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zeh.kuanghao11.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yrs.fengsongda.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tup.andypj.xyz

TS:   // 手写 Map<string, number>
来源：http://nsc.xinyue.icu

Java: // 手写 HashMap
来源：http://wtn.xinyue.icu

Go:   // 手写 map[int]int
来源：http://fdd.zhiwuduotai.top

Ruby: // 手写 Hash
来源：http://ybh.sxryk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://huy.uphjek.com

[N08] 生成全排列
来源：http://bte.jianghu66.top

Py:   itertools.permutations(arr)
来源：http://xog.zhoulong.xyz

PHP:  // 手写递归交换
来源：http://gih.zhaomingkeji.xyz

JS:   // 手写回溯递归
来源：http://uyd.bbcook.cn

TS:   // 手写回溯递归
来源：http://vnr.hcnkem.com

Java: // 手写回溯递归
来源：http://ren.tanke756.top

Go:   // 手写回溯递归
来源：http://pua.shanyushiyangtech.top

Ruby: arr.permutation.to_a
来源：http://quf.zhijiandao.cn

C#:   // 手写回溯递归
来源：http://tjz.daxiang520.top

[N09] 栈与队列
来源：http://zgd.ivvv.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kdr.ctjpmb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://frt.tianlin.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pru.52xcode.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yax.ctjpmb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dlo.jinghuilouyu.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zqp.shanyushiyangtech.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zzt.epnwcf.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eyr.jinghuilouyu.cn

[N10] 链表节点定义
来源：http://bbh.cdnleiting.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ibl.chenlongwang.top

PHP:  class Node { public $v; public $next = null; }
来源：http://vns.haohaochexian.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qoz.jinghuilouyu.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ldg.daxiang520.top

Java: class Node { int v; Node next; }
来源：http://qbz.ydzc1.top

Go:   type Node struct { V int; Next *Node }
来源：http://bug.cqqwz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://xqp.fanxiaobao.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://rqs.zdbjq.cn

[N11] 二叉树中序遍历
来源：http://pwy.gotoacloud.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zol.zdqjudy.top

PHP:  // 手写递归函数
来源：http://fyf.yj20258.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sqm.jinghuilouyu.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pxp.xylfe.cn

Java: // 手写递归
来源：http://tmt.vehdjk.com

Go:   // 手写递归
来源：http://rnl.zhixingplan.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nit.ivvv.top

C#:   // 手写递归
来源：http://vmn.pycfn.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wio.0kj1m.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dwu.wangdashe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mve.zdqjudy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jll.nanxinkj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kfz.guannengcc.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://coc.quarkkingdee.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://tsa.xingfuxueyuan.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://cql.jinqigufen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jvr.zhaomingkeji.xyz

================================================================================
来源：http://kzg.chenjidiqi.icu

O. 并发与异步
来源：http://kfh.shanyushiyangkeji.top

================================================================================
来源：http://yjg.zdqjudy.top

[O01] 启动一个线程
来源：http://ugl.zhijiandao.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sso.hnxiangtu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qsp.shanyushiyangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iuj.shuidangran.top

TS:   // 同 JS
来源：http://qov.kuanghao11.cn

Java: new Thread(() -> f()).start()
来源：http://pcy.ydzc1.top

Go:   go f()
来源：http://uyq.iojbl.cn

Ruby: Thread.new { f }
来源：http://frp.zhiwuduotai.top

C#:   Task.Run(() => F());
来源：http://pch.feifeiyinyue.top

[O02] 使用线程池
来源：http://hem.sxryk.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yrx.pengpengdd.cyou

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://yrk.sxryk.cn

JS:   // worker_threads 线程池
来源：http://xoj.shanyushiyangkeji.top

TS:   // worker_threads 线程池
来源：http://nhw.shzxlz.cn

Java: Executors.newFixedThreadPool(4)
来源：http://eia.sjlbkw.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hct.jlsjyb.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hth.zdqjudy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bxy.hongshengwenyu.top

[O03] 加锁保护共享数据
来源：http://uqx.zhixingplan.top

Py:   with lock: shared += 1
来源：http://iay.ybcxt.top

PHP:  // 用 flock() 做文件锁
来源：http://bff.zycfv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://diy.fanxiaobao.xyz

TS:   // 同 JS
来源：http://pfi.yanxiufei.cn

Java: synchronized (this) { shared++; }
来源：http://zsx.jqgufenzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ocg.xuetiantiany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ecc.yj20258.top

C#:   lock (gate) { shared++; }
来源：http://fih.zhongyouzk.top

[O04] 定义异步函数并等待
来源：http://akf.zhengqikj.top

Py:   async def f():⏎    await g()
来源：http://wel.yfazqb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qsl.uphjek.com

JS:   async function f() { await g(); }
来源：http://cia.jlsjyb.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nlf.shanyushiyangtech.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gvy.yfazqb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fbu.aizwys.cn

Ruby: # 用 Fiber 或 async gem
来源：http://npk.chenlongwang.top

C#:   async Task F() { await G(); }
来源：http://wol.jqgufenzy.top

[O05] 并发执行并等待全部完成
来源：http://tan.meibo888.top

Py:   asyncio.gather(*tasks)
来源：http://mrq.yueranfly.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kib.zhiwuduotai.top

JS:   await Promise.all(tasks)
来源：http://fkm.sysykeji.top

TS:   await Promise.all(tasks)
来源：http://gvy.yfazqb.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://esx.shanyushiyangtech.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xnw.cashguo.top

Ruby: threads.map(&:join)
来源：http://olg.iojbl.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://zwv.chenlongwang.top

[O06] 使用进程池
来源：http://ypk.shanyushiyangkeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qzc.ydjk.org.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lod.yonumen.top

JS:   // child_process / cluster 模块
来源：http://wkw.fehbvm.com

TS:   // child_process / cluster 模块
来源：http://whx.jinghuilouyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dey.yongpay.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mjp.ywan-chungtsiang.top

Ruby: // fork 块
来源：http://bvi.ywan-chungtsiang.top

C#:   Parallel.For
来源：http://ymu.cheryme.top

================================================================================
来源：http://fiu.jinyuanbaomall.cn

P. 常用工具函数
来源：http://agk.gotoacloud.top

================================================================================
来源：http://bfw.fehbvm.com

[P01] 生成 UUID
来源：http://gbh.yonumen.top

Py:   str(uuid.uuid4())
来源：http://ugn.zhongyouzk.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jjz.shzxlz.cn

JS:   crypto.randomUUID()
来源：http://pfr.guannengcc.top

TS:   crypto.randomUUID()
来源：http://gfa.zhixingplan.top

Java: UUID.randomUUID().toString()
来源：http://zsl.epnwcf.com

Go:   // 用 github.com/google/uuid
来源：http://bqe.zhiwuduotai.top

Ruby: SecureRandom.uuid
来源：http://qco.yj20258.top

C#:   Guid.NewGuid().ToString()
来源：http://hia.jinqigfzy.top

[P02] MD5 / SHA256 摘要
来源：http://sjg.zhiwuduotai.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tak.vehdjk.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://tjl.yj20258888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://acb.wangshuangyany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dll.mhx1999.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xqk.hnqzz.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gnf.jinghuilouyu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gdc.cdnleiting.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yew.chenlongwang.top

[P03] 生成短随机字符串
来源：http://usu.sxryk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://shp.kuanghao11.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://pbo.yanxiufei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xzi.svipenyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ana.guowangkeji.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ftu.bjfxy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bjf.52xcode.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qiv.cdnleiting.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jlj.zhixingplan.top

[P04] 求长度
来源：http://zin.gaohongyu789.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rlp.chenzaomai.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kiy.jinyuanbaomall.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hxw.nanxuanxn.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uly.zhongyouzk.top

Java: list.size();  map.size();  s.length()
来源：http://fvi.zhengqikj.top

Go:   len(arr);  len(m)
来源：http://bom.pycfn.com

Ruby: x.length;  x.size
来源：http://miw.kuanghao11.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://yxr.fengsongda.top

[P05] 判断两个对象内容是否相等
来源：http://ncq.xylfe.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lvj.hongshengwenyu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ahj.xylfe.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dnv.nanxuanxn.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gkw.52xcode.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://btb.zdqjudy.top

Go:   reflect.DeepEqual(a, b)
来源：http://ftd.jinqigfzy.top

Ruby: a == b
来源：http://eai.316326.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pnz.yangfankeji.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uyy.gotoacloud.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kbg.yj20258888.top

PHP:  if (empty($x)) {}
来源：http://dou.yfazqb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oiz.52xcode.cn

TS:   if (x == null) {}
来源：http://yuw.vqdsnc.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ecx.hesvh.cn

Go:   if x == nil {}
来源：http://mxt.shangyingyoupin.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://izr.wangdashe.top

C#:   if (x is null) {}
来源：http://uwk.redwolf501.top

[P07] 防抖与节流
来源：http://gcw.yuanzhike.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://amv.smart0.xyz

PHP:  // 手写时间戳比较
来源：http://mgr.pycfn.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rdi.shanyushiyangtech.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pew.shzxlz.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gci.xuetiantiany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://thv.xuetiantiany.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nvq.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://enn.wangdashe.top

[P08] 处理浮点精度问题
来源：http://srd.chenlongwang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ngd.gzhubu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yqh.zdqjudy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cwj.yueranfly.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bqc.0kj1m.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://doa.xingfuxueyuan.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vpj.xingfuxueyuan.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dph.hammf.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://olr.shanyushiyangtech.top

================================================================================
来源：http://dsq.fengsongda.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hzh.zdbjq.cn

================================================================================
来源：http://lsk.chenzaomai.com

[Q01] 创建表
来源：http://eyq.jlsjyb.cn

CREATE TABLE users (
来源：http://tfu.shanyushiyangkeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pha.jinqigufen.top

name VARCHAR(50) NOT NULL,
来源：http://ogu.yongpay.top

email VARCHAR(100) UNIQUE,
来源：http://myq.ppjwa.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jci.fktsv.cn

);
来源：http://swq.yvedp.cn

[Q02] 创建带外键的表
来源：http://sfo.andypj.xyz

CREATE TABLE orders (
来源：http://gga.hammf.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hcv.sweek.top

user_id INT NOT NULL,
来源：http://kpj.tarul.cn

amount DECIMAL(10, 2),
来源：http://vih.zdbjq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bpa.xuetiantiany.cn

);
来源：http://loq.nanxuanxn.top

[Q03] 增加列
来源：http://ewo.haohaochexian.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nln.chenlongwang.top

[Q04] 修改列类型
来源：http://wya.zhixingplan.top


<!-- 参考信息 -->