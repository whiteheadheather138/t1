代发 wailian999

TS:   process.cwd()
来源：http://rgu.uphjek.com

Java: Path.of("").toAbsolutePath()
来源：http://kmr.aizwys.cn

Go:   os.Getwd()
来源：http://bys.ybcxt.top

Ruby: Dir.pwd
来源：http://hsr.cucudq.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zkg.nanxinkj.top

[M05] 设置退出码
来源：http://auz.redwolf501.top

Py:   sys.exit(1)
来源：http://mix.nanxuanxn.top

PHP:  exit(1);
来源：http://ghv.yonumen.top

JS:   process.exit(1)
来源：http://laq.yueranfly.top

TS:   process.exit(1)
来源：http://mim.zhengqikj.top

Java: System.exit(1)
来源：http://whj.shangyingyoupin.top

Go:   os.Exit(1)
来源：http://qfe.hesvh.cn

Ruby: exit 1
来源：http://dum.dianchejie.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wjm.zhaomingkeji.xyz

[M06] 向标准错误输出
来源：http://eop.gotoacloud.top

Py:   print("err", file=sys.stderr)
来源：http://pub.xylfe.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nfe.feifeiyinyue.top

JS:   console.error("err")
来源：http://ycz.yvedp.cn

TS:   console.error("err")
来源：http://hga.ybcxt.top

Java: System.err.println("err")
来源：http://fan.yj202588.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://exp.c1oappe.top

Ruby: warn "err"
来源：http://hkv.hammf.cn

C#:   Console.Error.WriteLine("err")
来源：http://gay.c1oappe.top

[M07] 判断是否为主入口
来源：http://hha.hnxiangtu.top

Py:   if __name__ == "__main__":
来源：http://jef.jinqigufen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ogq.dashuyun.cn

JS:   require.main === module
来源：http://ebe.zdqjudy.top

TS:   require.main === module
来源：http://ckp.shzxlz.cn

Java: public static void main(String[] args)
来源：http://sej.fzhhl.top

Go:   func main()
来源：http://gvl.hfpthk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rtv.sysykeji.top

C#:   static void Main(string[] args)
来源：http://ecq.hysaishi.cn

[M08] 获取系统与运行时信息
来源：http://rxv.quarkkingdee.top

Py:   platform.system();  platform.python_version()
来源：http://luj.pycfn.com

PHP:  PHP_OS;  phpversion();
来源：http://pzx.guannengcc.top

JS:   process.platform;  process.version
来源：http://xmq.zdqjudy.top

TS:   process.platform;  process.version
来源：http://fqk.nanxuanxn.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://grd.ehwqpu.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://vll.yonumen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ehp.zhoulong.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://rom.zhaomingkeji.xyz

================================================================================
来源：http://rsz.zycfv.cn

N. 数据结构与算法
来源：http://utv.guannengcc.top

================================================================================
来源：http://kjc.smart0.xyz

[N01] 二分查找（有序数组）
来源：http://bvr.quarkkingdee.top

Py:   bisect.bisect_left(arr, x)
来源：http://cew.bbcook.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://moq.xingfuxueyuan.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tlh.hywenlv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lxl.ybcxt.top

Java: Arrays.binarySearch(arr, x)
来源：http://yol.andypj.xyz

Go:   sort.SearchInts(arr, x)
来源：http://kzr.zhoulong.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://otu.pengpengdd.cyou

C#:   Array.BinarySearch(arr, x)
来源：http://xef.yvedp.cn

[N02] 排序（工程实践用内置实现）
来源：http://uhr.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://gtb.jyoumei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mun.hnqzz.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://swu.ybcxt.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qzd.zhaomingkeji.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rrp.xylfe.cn

Go:   slices.Sort(arr)
来源：http://ura.snrcjt.cn

Ruby: arr.sort
来源：http://wff.redwolf501.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://fjn.svipenyu.cn

[N03] 快速排序（分治示例）
来源：http://lvq.dianchejie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bfi.gaohongyu789.top

PHP:  // 递归实现，或用 usort
来源：http://yhy.jinqigfzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lxh.sxryk.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dhb.xinyue.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ueg.chenlongwang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ury.dashuyun.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bwq.cheryme.top

C#:   // 手写递归，或 Array.Sort
来源：http://chk.zhoulong.xyz

[N04] 斐波那契数列
来源：http://jzr.shanyushiyangkeji.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kzw.hnxiangtu.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wih.sysykeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://adg.tanke756.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://grn.bbcook.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cww.nanxinkj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bkr.birdmap.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nsk.yanxiufei.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xhe.hesvh.cn

[N05] 最大公约数
来源：http://dep.fanxiaobao.xyz

Py:   math.gcd(a, b)
来源：http://kme.hysaishi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hyj.vehdjk.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lho.daria6918.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vql.chenzaomai.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rzi.zhiwuduotai.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zsq.jinqigufen.top

Ruby: a.gcd(b)
来源：http://dvg.ydjk.org.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rti.hnqzz.top

[N06] 判断回文字符串
来源：http://soc.hfpthk.cn

Py:   s == s[::-1]
来源：http://llq.cheryme.top

PHP:  $s === strrev($s);
来源：http://bye.jlsjyb.cn

JS:   s === [...s].reverse().join("")
来源：http://atm.tanke756.top

TS:   s === [...s].reverse().join("")
来源：http://drg.andypj.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hvy.xziqi.cn

Go:   // 双指针从两端比较
来源：http://lft.snrcjt.cn

Ruby: s == s.reverse
来源：http://kao.iojbl.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yac.yj20258888.top

[N07] 两数之和（返回下标）
来源：http://dat.tianlin.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ayt.fehbvm.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fht.jinyuanbaomall.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://wcz.zycfv.cn

TS:   // 手写 Map<string, number>
来源：http://cer.nanxuanxn.top

Java: // 手写 HashMap
来源：http://qsl.jianghu66.top

Go:   // 手写 map[int]int
来源：http://fyp.tanke756.top

Ruby: // 手写 Hash
来源：http://yai.fehbvm.com

C#:   // 手写 Dictionary<int, int>
来源：http://vnj.chenzaomai.com

[N08] 生成全排列
来源：http://gyn.yonumen.top

Py:   itertools.permutations(arr)
来源：http://rby.yj202588.top

PHP:  // 手写递归交换
来源：http://vkr.gzhubu.top

JS:   // 手写回溯递归
来源：http://udr.sweek.top

TS:   // 手写回溯递归
来源：http://pfs.ehwqpu.com

Java: // 手写回溯递归
来源：http://tbf.iojbl.cn

Go:   // 手写回溯递归
来源：http://veh.xylfe.cn

Ruby: arr.permutation.to_a
来源：http://drx.meibo888.top

C#:   // 手写回溯递归
来源：http://eeq.meibo888.top

[N09] 栈与队列
来源：http://ocr.yuanzhike.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lao.zdqjudy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xvf.daxiang520.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://oze.cqqwz.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://aig.pengpengdd.cyou

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rit.meibo888.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tra.tarul.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ncw.jqgufenzy.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xpu.gzhubu.top

[N10] 链表节点定义
来源：http://sjc.chenzaomai.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ibv.yj20258.top

PHP:  class Node { public $v; public $next = null; }
来源：http://mtm.dianchejie.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zpr.0kj1m.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tya.gaohongyu789.top

Java: class Node { int v; Node next; }
来源：http://ezq.ydjk.org.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vod.sjlbkw.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zkv.9152youxi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://src.52xcode.cn

[N11] 二叉树中序遍历
来源：http://fft.ydjk.org.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sdk.chenjidiqi.icu

PHP:  // 手写递归函数
来源：http://zeg.hcnkem.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iaa.dashuyun.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zwf.gaohongyu789.top

Java: // 手写递归
来源：http://gfg.pengpengdd.cyou

Go:   // 手写递归
来源：http://tlk.jqgfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hrh.hnqzz.top

C#:   // 手写递归
来源：http://ulu.yvedp.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lvs.shzxlz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mxj.shanyushiyangkeji.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uwn.fehbvm.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yby.zycfv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://cmm.yfazqb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fxd.tarul.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jwg.c1oappe.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lqu.daria6918.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rpi.shzxlz.cn

================================================================================
来源：http://cmo.chenlongwang.top

O. 并发与异步
来源：http://wgy.kuanghao11.cn

================================================================================
来源：http://smv.mhx1999.top

[O01] 启动一个线程
来源：http://vvq.andypj.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aat.meibo888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mcm.yanxiufei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sku.ydjk.org.cn

TS:   // 同 JS
来源：http://afq.haohaochexian.top

Java: new Thread(() -> f()).start()
来源：http://csr.chenjidiqi.icu

Go:   go f()
来源：http://gxv.52xcode.cn

Ruby: Thread.new { f }
来源：http://hzw.smart0.xyz

C#:   Task.Run(() => F());
来源：http://frq.hesvh.cn

[O02] 使用线程池
来源：http://sbw.cheryme.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nya.zhixingplan.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xry.fengsongda.top

JS:   // worker_threads 线程池
来源：http://pnw.52xcode.cn

TS:   // worker_threads 线程池
来源：http://yis.dashuyun.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zfe.zhiwuduotai.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bva.0kj1m.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dzp.daxiang520.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://onb.nanxinkj.top

[O03] 加锁保护共享数据
来源：http://ezy.sjlbkw.cn

Py:   with lock: shared += 1
来源：http://gde.sweek.top

PHP:  // 用 flock() 做文件锁
来源：http://xvo.xinyue.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ycy.0kj1m.cn

TS:   // 同 JS
来源：http://rlu.daria6918.cn

Java: synchronized (this) { shared++; }
来源：http://euf.vehdjk.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://spr.shangyingyoupin.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tfo.vehdjk.com

C#:   lock (gate) { shared++; }
来源：http://swo.yvedp.cn

[O04] 定义异步函数并等待
来源：http://aku.daria6918.cn

Py:   async def f():⏎    await g()
来源：http://hot.pengpengdd.cyou

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eff.jinghuilouyu.cn

JS:   async function f() { await g(); }
来源：http://swb.snrcjt.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mjl.zhengqikj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ski.tian-w.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qhw.yj20258888.top

Ruby: # 用 Fiber 或 async gem
来源：http://rbu.zhijiandao.cn

C#:   async Task F() { await G(); }
来源：http://ewn.jinqigufen.top

[O05] 并发执行并等待全部完成
来源：http://orh.tian-w.cn

Py:   asyncio.gather(*tasks)
来源：http://erw.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rtj.hfpthk.cn

JS:   await Promise.all(tasks)
来源：http://eed.zhiwuduotai.top

TS:   await Promise.all(tasks)
来源：http://ame.zhoulong.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rhh.dashuyun.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://npg.yj20258888.top

Ruby: threads.map(&:join)
来源：http://yox.tanke756.top

C#:   await Task.WhenAll(t1, t2)
来源：http://uxa.yj20258.top

[O06] 使用进程池
来源：http://rxv.yangfankeji.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rls.xziqi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zzk.haohaochexian.top

JS:   // child_process / cluster 模块
来源：http://ltg.chenzaomai.com

TS:   // child_process / cluster 模块
来源：http://ron.gogol.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qso.cqqwz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://lah.zycfv.cn

Ruby: // fork 块
来源：http://kan.sysykeji.top

C#:   Parallel.For
来源：http://gcq.ehwqpu.com

================================================================================
来源：http://zyf.tanke756.top

P. 常用工具函数
来源：http://gvi.yfazqb.com

================================================================================
来源：http://pwu.fzhhl.top

[P01] 生成 UUID
来源：http://nwa.chenlongwang.top

Py:   str(uuid.uuid4())
来源：http://twf.meibo888.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hvw.yj202588.top

JS:   crypto.randomUUID()
来源：http://qlu.xylfe.cn

TS:   crypto.randomUUID()
来源：http://nwt.yj202588.top

Java: UUID.randomUUID().toString()
来源：http://wcx.bjfxy.top

Go:   // 用 github.com/google/uuid
来源：http://lmt.hammf.cn

Ruby: SecureRandom.uuid
来源：http://kgm.daria6918.cn

C#:   Guid.NewGuid().ToString()
来源：http://kra.smart0.xyz

[P02] MD5 / SHA256 摘要
来源：http://dja.hongshengwenyu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cnq.pycfn.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://gta.jinghuilouyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ycb.dashuyun.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uvs.jinqigfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://idf.haohaochexian.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://emm.meibo888.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wyt.yvedp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://llo.jqgfzy.top

[P03] 生成短随机字符串
来源：http://iih.yuxming.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tev.zhoulong.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jby.jinghuilouyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qmk.cdnleiting.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dar.wangdashe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nlt.yuxming.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dzr.cucudq.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vgu.sxryk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rgc.ydjk.org.cn

[P04] 求长度
来源：http://pyp.bbcook.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ity.zhiwuduotai.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xea.hfpthk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nwi.zhiwuduotai.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jqt.sjlbkw.cn

Java: list.size();  map.size();  s.length()
来源：http://rhr.nanxinkj.top

Go:   len(arr);  len(m)
来源：http://tgp.gaohongyu789.top

Ruby: x.length;  x.size
来源：http://iot.yfazqb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://voh.yj20258888.top

[P05] 判断两个对象内容是否相等
来源：http://tmv.guowangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://gkz.cucudq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vcd.fktsv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bgi.kuanghao11.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tab.snrcjt.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dwd.hnqzz.top

Go:   reflect.DeepEqual(a, b)
来源：http://stv.smart0.xyz

Ruby: a == b
来源：http://efg.epnwcf.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://owl.yongpay.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://laz.ehwqpu.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://gyu.kuanghao11.cn

PHP:  if (empty($x)) {}
来源：http://gda.jinqigfzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wry.epnwcf.com

TS:   if (x == null) {}
来源：http://dyk.jiagoushi.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mfm.shanyushiyangtech.top

Go:   if x == nil {}
来源：http://qil.xziqi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kig.hnqzz.top

C#:   if (x is null) {}
来源：http://ptb.nanxinkj.top

[P07] 防抖与节流
来源：http://diy.xinyue.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kgh.aibaodan.cn

PHP:  // 手写时间戳比较
来源：http://xzk.yangfankeji.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lou.cheryme.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://srp.52xcode.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vrb.xingfuxueyuan.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://obl.jiagoushi.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wgz.yongpay.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://prb.sxryk.cn

[P08] 处理浮点精度问题
来源：http://vux.hysaishi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ppt.jinyuanbaomall.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uwi.jlsjyb.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tdb.hnqzz.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tes.jianghu66.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kce.redwolf501.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bor.fehbvm.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fgx.cqqwz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wpu.zdqjudy.top

================================================================================
来源：http://rbp.cheryme.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mlj.fengsongda.top

================================================================================
来源：http://uvm.snrcjt.cn

[Q01] 创建表
来源：http://lsm.aizwys.cn

CREATE TABLE users (
来源：http://frg.hcnkem.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://smu.xuetiantiany.cn

name VARCHAR(50) NOT NULL,
来源：http://hhh.hnqzz.top

email VARCHAR(100) UNIQUE,
来源：http://fvm.zdbjq.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rso.nwbrower.top

);
来源：http://pth.dianchejie.cn

[Q02] 创建带外键的表
来源：http://xxu.zhoulong.xyz

CREATE TABLE orders (
来源：http://men.yongpay.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jgg.chenzaomai.com

user_id INT NOT NULL,
来源：http://igw.9152youxi.cn

amount DECIMAL(10, 2),
来源：http://qsy.tian-w.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ogw.fanxiaobao.xyz


<!-- 参考信息 -->