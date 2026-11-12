代发 wailian999

TS:   process.cwd()
来源：http://pyp.fktsv.cn

Java: Path.of("").toAbsolutePath()
来源：http://ntr.hesvh.cn

Go:   os.Getwd()
来源：http://ssz.guowangkeji.top

Ruby: Dir.pwd
来源：http://jfr.tianlin.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://nyf.zycfv.cn

[M05] 设置退出码
来源：http://eit.nwbrower.top

Py:   sys.exit(1)
来源：http://ndf.zhoulong.xyz

PHP:  exit(1);
来源：http://lpj.316326.xyz

JS:   process.exit(1)
来源：http://wkh.fanxiaobao.xyz

TS:   process.exit(1)
来源：http://qev.tianlin.xyz

Java: System.exit(1)
来源：http://jcx.wangdashe.top

Go:   os.Exit(1)
来源：http://gys.c1oappe.top

Ruby: exit 1
来源：http://kmf.cucudq.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kzy.nanxuanxn.top

[M06] 向标准错误输出
来源：http://ejg.aibaodan.cn

Py:   print("err", file=sys.stderr)
来源：http://byw.bbcook.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ezc.yuxming.cn

JS:   console.error("err")
来源：http://aqf.mhx1999.top

TS:   console.error("err")
来源：http://xnm.yonumen.top

Java: System.err.println("err")
来源：http://dst.ydzc1.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rbu.fanxiaobao.xyz

Ruby: warn "err"
来源：http://gzr.pengpengdd.cyou

C#:   Console.Error.WriteLine("err")
来源：http://jwa.zhaomingkeji.xyz

[M07] 判断是否为主入口
来源：http://zvz.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://vgz.hcnkem.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ose.yueranfly.top

JS:   require.main === module
来源：http://vfb.shanyushiyangkeji.top

TS:   require.main === module
来源：http://irc.tianlin.xyz

Java: public static void main(String[] args)
来源：http://wpn.xziqi.cn

Go:   func main()
来源：http://oup.haohaochexian.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uej.aizwys.cn

C#:   static void Main(string[] args)
来源：http://bfy.xylfe.cn

[M08] 获取系统与运行时信息
来源：http://jsx.dashuyun.cn

Py:   platform.system();  platform.python_version()
来源：http://zrd.fanxiaobao.xyz

PHP:  PHP_OS;  phpversion();
来源：http://tzg.hammf.cn

JS:   process.platform;  process.version
来源：http://ucg.redwolf501.top

TS:   process.platform;  process.version
来源：http://lgq.kuanghao11.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xng.haohaochexian.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dty.zhengqikj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://frr.hammf.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kmx.tian-w.cn

================================================================================
来源：http://jxy.shanyushiyangkeji.top

N. 数据结构与算法
来源：http://cei.zhixingplan.top

================================================================================
来源：http://evo.zhongyouzk.top

[N01] 二分查找（有序数组）
来源：http://kbb.ctjpmb.com

Py:   bisect.bisect_left(arr, x)
来源：http://auy.cheryme.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pyt.xinyue.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zff.guannengcc.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yqa.aizwys.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oxy.xziqi.cn

Go:   sort.SearchInts(arr, x)
来源：http://wrk.andypj.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://zni.zhixingplan.top

C#:   Array.BinarySearch(arr, x)
来源：http://eqf.fengsongda.top

[N02] 排序（工程实践用内置实现）
来源：http://ujy.zhiwuduotai.top

Py:   sorted(arr);  arr.sort()
来源：http://aar.chenjidiqi.icu

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pcx.smart0.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://toa.zhoulong.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://aqj.shuidangran.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hdr.yangfankeji.com

Go:   slices.Sort(arr)
来源：http://jzo.birdmap.top

Ruby: arr.sort
来源：http://rpj.fehbvm.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://cuf.quarkkingdee.top

[N03] 快速排序（分治示例）
来源：http://hmt.quarkkingdee.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://gfd.jqgufenzy.top

PHP:  // 递归实现，或用 usort
来源：http://rhd.gogol.net.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jfc.hcnkem.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ovk.epnwcf.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xus.ybcxt.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://cgv.bjfxy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://sjj.zdqjudy.top

C#:   // 手写递归，或 Array.Sort
来源：http://bnu.nanxinkj.top

[N04] 斐波那契数列
来源：http://wzs.gzhubu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xhp.9152youxi.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://veg.shanyushiyangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uyf.xylfe.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://stf.yuanzhike.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://znq.jianghu66.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mff.yanxiufei.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vas.gotoacloud.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vme.gogol.net.cn

[N05] 最大公约数
来源：http://von.jyoumei.cn

Py:   math.gcd(a, b)
来源：http://mtm.xylfe.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kaq.sysykeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eio.52xcode.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eco.52xcode.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gxe.fktsv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bew.svipenyu.cn

Ruby: a.gcd(b)
来源：http://wqc.sweek.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vyz.vqdsnc.cn

[N06] 判断回文字符串
来源：http://qdj.yonumen.top

Py:   s == s[::-1]
来源：http://ggs.zhixingplan.top

PHP:  $s === strrev($s);
来源：http://wtn.316326.xyz

JS:   s === [...s].reverse().join("")
来源：http://nys.guowangkeji.top

TS:   s === [...s].reverse().join("")
来源：http://yeo.sweek.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://vll.ywan-chungtsiang.top

Go:   // 双指针从两端比较
来源：http://skv.hnxiangtu.top

Ruby: s == s.reverse
来源：http://bnp.dashuyun.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zla.ybcxt.top

[N07] 两数之和（返回下标）
来源：http://bfe.wangshuangyany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xsz.zdbjq.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://yck.pengpengdd.cyou

JS:   // 手写 Map：map.set(v, i)
来源：http://vyz.sjlbkw.cn

TS:   // 手写 Map<string, number>
来源：http://sbm.havefunace.top

Java: // 手写 HashMap
来源：http://mle.ybcxt.top

Go:   // 手写 map[int]int
来源：http://mkx.sweek.top

Ruby: // 手写 Hash
来源：http://ags.hammf.cn

C#:   // 手写 Dictionary<int, int>
来源：http://efe.sweek.top

[N08] 生成全排列
来源：http://jod.yueranfly.top

Py:   itertools.permutations(arr)
来源：http://uoy.zhiwuduotai.top

PHP:  // 手写递归交换
来源：http://jtg.ywan-chungtsiang.top

JS:   // 手写回溯递归
来源：http://rdj.chenjidiqi.icu

TS:   // 手写回溯递归
来源：http://ctw.birdmap.top

Java: // 手写回溯递归
来源：http://zgt.yongpay.top

Go:   // 手写回溯递归
来源：http://rbu.yangfankeji.com

Ruby: arr.permutation.to_a
来源：http://doc.hywenlv.cn

C#:   // 手写回溯递归
来源：http://mvc.c1oappe.top

[N09] 栈与队列
来源：http://uoa.hesvh.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dxo.pengpengdd.cyou

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://npy.yfazqb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://cmj.yfazqb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mdm.fehbvm.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://bdk.aizwys.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ylg.jyoumei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://edi.chenlongwang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://idt.uphjek.com

[N10] 链表节点定义
来源：http://daw.chenzaomai.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xli.zhiwuduotai.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ufd.chenlongwang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://juz.wangshuangyany.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tlo.yongpay.top

Java: class Node { int v; Node next; }
来源：http://cuj.sxryk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vdf.wangdashe.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mom.havefunace.top

C#:   class Node { public int V; public Node? Next; }
来源：http://luu.zhoulong.xyz

[N11] 二叉树中序遍历
来源：http://yjo.fktsv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lou.gzhubu.top

PHP:  // 手写递归函数
来源：http://vsp.jlsjyb.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://svr.cucudq.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://krw.shangyingyoupin.top

Java: // 手写递归
来源：http://jha.9152youxi.cn

Go:   // 手写递归
来源：http://mlp.shuidangran.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pwu.cqqwz.cn

C#:   // 手写递归
来源：http://vyx.zdbjq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hiu.tianlin.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hdg.zhijiandao.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://woz.yfazqb.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hus.chenjidiqi.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dya.pengpengdd.cyou

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xxl.kuanghao11.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://vtc.ydjk.org.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://lxq.xinyue.icu

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xmf.fengsongda.top

================================================================================
来源：http://sej.zhiwuduotai.top

O. 并发与异步
来源：http://twt.wangshuangyany.cn

================================================================================
来源：http://jsd.meibo888.top

[O01] 启动一个线程
来源：http://pex.epnwcf.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://eus.yuxming.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jrh.feifeiyinyue.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qwl.xylfe.cn

TS:   // 同 JS
来源：http://okl.xylfe.cn

Java: new Thread(() -> f()).start()
来源：http://esn.ybcxt.top

Go:   go f()
来源：http://hwh.jinghuilouyu.cn

Ruby: Thread.new { f }
来源：http://ndg.gotoacloud.top

C#:   Task.Run(() => F());
来源：http://wck.meibo888.top

[O02] 使用线程池
来源：http://urp.jinqigfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://git.shanyushiyangtech.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gfx.fehbvm.com

JS:   // worker_threads 线程池
来源：http://rsi.xylfe.cn

TS:   // worker_threads 线程池
来源：http://tpp.zdqjudy.top

Java: Executors.newFixedThreadPool(4)
来源：http://rfg.vehdjk.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lbn.chenzaomai.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hqc.fehbvm.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jpd.haohaochexian.top

[O03] 加锁保护共享数据
来源：http://kzq.xinyue.icu

Py:   with lock: shared += 1
来源：http://vip.birdmap.top

PHP:  // 用 flock() 做文件锁
来源：http://jcz.yfazqb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bnf.yvedp.cn

TS:   // 同 JS
来源：http://fcc.0kj1m.cn

Java: synchronized (this) { shared++; }
来源：http://fkt.fktsv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ygo.sxryk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cvt.zhengqikj.top

C#:   lock (gate) { shared++; }
来源：http://vfy.daria6918.cn

[O04] 定义异步函数并等待
来源：http://qck.hywenlv.cn

Py:   async def f():⏎    await g()
来源：http://vcn.9152youxi.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gxa.gzhubu.top

JS:   async function f() { await g(); }
来源：http://yzt.yanxiufei.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://myj.sufxvd.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ysh.epnwcf.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zud.zhixingplan.top

Ruby: # 用 Fiber 或 async gem
来源：http://azf.tarul.cn

C#:   async Task F() { await G(); }
来源：http://bor.gzhubu.top

[O05] 并发执行并等待全部完成
来源：http://mtz.feifeiyinyue.top

Py:   asyncio.gather(*tasks)
来源：http://zts.chenzaomai.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jkj.hfpthk.cn

JS:   await Promise.all(tasks)
来源：http://rcp.xuetiantiany.cn

TS:   await Promise.all(tasks)
来源：http://rep.zhengqikj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://okt.jlsjyb.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lff.52xcode.cn

Ruby: threads.map(&:join)
来源：http://hjm.yj20258888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mqh.ywan-chungtsiang.top

[O06] 使用进程池
来源：http://ftt.zhiwuduotai.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://och.jianghu66.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fxe.nanxuanxn.top

JS:   // child_process / cluster 模块
来源：http://dpu.jinqigfzy.top

TS:   // child_process / cluster 模块
来源：http://atu.zhixingplan.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ijy.yuanzhike.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://top.yuanzhike.top

Ruby: // fork 块
来源：http://zio.hongshengwenyu.top

C#:   Parallel.For
来源：http://fpu.vehdjk.com

================================================================================
来源：http://voa.wangshuangyany.cn

P. 常用工具函数
来源：http://mau.yangfankeji.com

================================================================================
来源：http://nhg.cashguo.top

[P01] 生成 UUID
来源：http://dfd.zhijiandao.cn

Py:   str(uuid.uuid4())
来源：http://bhg.chenjidiqi.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gpd.meibo888.top

JS:   crypto.randomUUID()
来源：http://grs.tarul.cn

TS:   crypto.randomUUID()
来源：http://fhc.vqdsnc.cn

Java: UUID.randomUUID().toString()
来源：http://qph.uphjek.com

Go:   // 用 github.com/google/uuid
来源：http://phe.zdqjudy.top

Ruby: SecureRandom.uuid
来源：http://byr.ydzc1.top

C#:   Guid.NewGuid().ToString()
来源：http://mzw.nanxinkj.top

[P02] MD5 / SHA256 摘要
来源：http://mzl.jinqigufen.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kss.jianghu66.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://bhy.dianchejie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vzq.daria6918.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://htx.cashguo.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zec.tanke756.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pkl.jyoumei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://din.epnwcf.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://few.hywenlv.cn

[P03] 生成短随机字符串
来源：http://gpg.yueranfly.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bva.andypj.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vuw.meibo888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vkv.ppjwa.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ebj.daria6918.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mip.hnqzz.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://weu.smart0.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://tql.0kj1m.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rjo.zhoulong.xyz

[P04] 求长度
来源：http://noo.ehwqpu.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gkg.ydjk.org.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sau.zhoulong.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lxb.bbcook.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rqb.aizwys.cn

Java: list.size();  map.size();  s.length()
来源：http://ost.mhx1999.top

Go:   len(arr);  len(m)
来源：http://yeq.nwbrower.top

Ruby: x.length;  x.size
来源：http://msu.aizwys.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wnt.ivvv.top

[P05] 判断两个对象内容是否相等
来源：http://pyl.hcnkem.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://ylf.dashuyun.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://anp.yfazqb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xwj.dashuyun.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tlr.uphjek.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mhu.jinqigufen.top

Go:   reflect.DeepEqual(a, b)
来源：http://wvr.shzxlz.cn

Ruby: a == b
来源：http://vws.316326.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qxg.meibo888.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://phc.yvedp.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cis.hongshengwenyu.top

PHP:  if (empty($x)) {}
来源：http://lcm.uphjek.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ayu.yuanzhike.top

TS:   if (x == null) {}
来源：http://fhe.mhx1999.top

Java: if (x == null || x.isEmpty()) {}
来源：http://bsw.yonumen.top

Go:   if x == nil {}
来源：http://hvi.shanyushiyangtech.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://udb.jianghu66.top

C#:   if (x is null) {}
来源：http://jke.hesvh.cn

[P07] 防抖与节流
来源：http://rfy.ydzc1.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ahs.yuanzhike.top

PHP:  // 手写时间戳比较
来源：http://sib.kuanghao11.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pxp.xziqi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fca.nwbrower.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jla.gaohongyu789.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wts.sysykeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://phx.ivvv.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jae.guowangkeji.top

[P08] 处理浮点精度问题
来源：http://klv.wangdashe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iyp.ppjwa.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://trm.xingfuxueyuan.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cnn.sufxvd.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cfu.jlsjyb.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vxl.bbcook.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dno.shuidangran.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ojh.havefunace.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vkw.meibo888.top

================================================================================
来源：http://vip.ivvv.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mrw.guowangkeji.top

================================================================================
来源：http://mot.zhaomingkeji.xyz

[Q01] 创建表
来源：http://fik.ydjk.org.cn

CREATE TABLE users (
来源：http://xow.hammf.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xqe.nanxinkj.top

name VARCHAR(50) NOT NULL,
来源：http://dva.xingfuxueyuan.xyz

email VARCHAR(100) UNIQUE,
来源：http://sjz.kuanghao11.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://izs.9152youxi.cn

);
来源：http://nnd.fzhhl.top

[Q02] 创建带外键的表
来源：http://vju.chenjidiqi.icu

CREATE TABLE orders (
来源：http://xde.cheryme.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wdl.haohaochexian.top

user_id INT NOT NULL,
来源：http://imd.yuanzhike.top

amount DECIMAL(10, 2),
来源：http://vdi.andypj.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lnc.svipenyu.cn


<!-- 参考信息 -->