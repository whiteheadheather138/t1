代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://nfa.sxryk.cn

[M05] 设置退出码
来源：http://kds.sjlbkw.cn

Py:   sys.exit(1)
来源：http://gzc.guowangkeji.top

PHP:  exit(1);
来源：http://ukj.iojbl.cn

JS:   process.exit(1)
来源：http://sin.gzhubu.top

TS:   process.exit(1)
来源：http://qok.chenzaomai.com

Java: System.exit(1)
来源：http://les.jinghuilouyu.cn

Go:   os.Exit(1)
来源：http://eba.kuanghao11.cn

Ruby: exit 1
来源：http://ecf.yfazqb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://nng.yuanzhike.top

[M06] 向标准错误输出
来源：http://jrx.yj20258.top

Py:   print("err", file=sys.stderr)
来源：http://otw.cqqwz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://mla.jinghuilouyu.cn

JS:   console.error("err")
来源：http://lxe.ybcxt.top

TS:   console.error("err")
来源：http://qgn.jinghuilouyu.cn

Java: System.err.println("err")
来源：http://sgm.hesvh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tib.shangyingyoupin.top

Ruby: warn "err"
来源：http://hcr.sufxvd.cn

C#:   Console.Error.WriteLine("err")
来源：http://jrv.shuidangran.top

[M07] 判断是否为主入口
来源：http://tdv.yueranfly.top

Py:   if __name__ == "__main__":
来源：http://hyg.gzhubu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://msi.tanke756.top

JS:   require.main === module
来源：http://uqg.chenlongwang.top

TS:   require.main === module
来源：http://sft.cqqwz.cn

Java: public static void main(String[] args)
来源：http://jns.xinyue.icu

Go:   func main()
来源：http://tlo.yfazqb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jwu.redwolf501.top

C#:   static void Main(string[] args)
来源：http://irl.epnwcf.com

[M08] 获取系统与运行时信息
来源：http://qxc.bjfxy.top

Py:   platform.system();  platform.python_version()
来源：http://brw.jiagoushi.top

PHP:  PHP_OS;  phpversion();
来源：http://kff.wangshuangyany.cn

JS:   process.platform;  process.version
来源：http://vvl.epnwcf.com

TS:   process.platform;  process.version
来源：http://jpj.xuanzx.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://sre.jqgfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hyy.vqdsnc.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zru.jqgfzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://blz.gogol.net.cn

================================================================================
来源：http://rnn.meibo888.top

N. 数据结构与算法
来源：http://kzb.aizwys.cn

================================================================================
来源：http://jok.zhaomingkeji.xyz

[N01] 二分查找（有序数组）
来源：http://chj.feifeiyinyue.top

Py:   bisect.bisect_left(arr, x)
来源：http://bia.iojbl.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mvv.wangdashe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cnl.snrcjt.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vsg.xingfuxueyuan.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://afz.zhoulong.xyz

Go:   sort.SearchInts(arr, x)
来源：http://qmr.jiagoushi.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://luo.sxryk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uok.wangshuangyany.cn

[N02] 排序（工程实践用内置实现）
来源：http://xwy.ppjwa.cn

Py:   sorted(arr);  arr.sort()
来源：http://xoi.jinghuilouyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hbn.chenzaomai.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://bbe.cdnleiting.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wsk.52xcode.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nam.52xcode.cn

Go:   slices.Sort(arr)
来源：http://eyd.ehwqpu.com

Ruby: arr.sort
来源：http://tcs.guowangkeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kpp.xuetiantiany.cn

[N03] 快速排序（分治示例）
来源：http://iyk.fzhhl.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wlu.fanxiaobao.xyz

PHP:  // 递归实现，或用 usort
来源：http://bpc.shanyushiyangtech.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://udr.havefunace.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jwd.dashuyun.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rwo.epnwcf.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ywq.9152youxi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://cgz.pengpengdd.cyou

C#:   // 手写递归，或 Array.Sort
来源：http://uen.chenjidiqi.icu

[N04] 斐波那契数列
来源：http://vpi.epnwcf.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bwr.ydzc1.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vgp.hywenlv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qqx.jyoumei.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://amc.jinqigfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qew.jqgfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vep.shanyushiyangtech.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qno.jiagoushi.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pya.yj202588.top

[N05] 最大公约数
来源：http://vzw.hesvh.cn

Py:   math.gcd(a, b)
来源：http://nma.iojbl.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ceb.0kj1m.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://odu.havefunace.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xdd.yongpay.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mjp.uphjek.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tar.xziqi.cn

Ruby: a.gcd(b)
来源：http://bfm.jinyuanbaomall.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://obh.316326.xyz

[N06] 判断回文字符串
来源：http://czt.fktsv.cn

Py:   s == s[::-1]
来源：http://ong.vqdsnc.cn

PHP:  $s === strrev($s);
来源：http://hxo.zhengqikj.top

JS:   s === [...s].reverse().join("")
来源：http://gws.yvedp.cn

TS:   s === [...s].reverse().join("")
来源：http://kch.hywenlv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oey.dianchejie.cn

Go:   // 双指针从两端比较
来源：http://klx.cdnleiting.top

Ruby: s == s.reverse
来源：http://gdj.yanxiufei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pyv.zdqjudy.top

[N07] 两数之和（返回下标）
来源：http://hrc.xuetiantiany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kxz.fzhhl.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rmt.sufxvd.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://vbh.xingfuxueyuan.xyz

TS:   // 手写 Map<string, number>
来源：http://psf.snrcjt.cn

Java: // 手写 HashMap
来源：http://lkv.hysaishi.cn

Go:   // 手写 map[int]int
来源：http://gps.redwolf501.top

Ruby: // 手写 Hash
来源：http://gaw.0kj1m.cn

C#:   // 手写 Dictionary<int, int>
来源：http://yed.ehwqpu.com

[N08] 生成全排列
来源：http://xbg.vqdsnc.cn

Py:   itertools.permutations(arr)
来源：http://mus.vehdjk.com

PHP:  // 手写递归交换
来源：http://iwn.sweek.top

JS:   // 手写回溯递归
来源：http://ycj.daria6918.cn

TS:   // 手写回溯递归
来源：http://pmw.jinqigfzy.top

Java: // 手写回溯递归
来源：http://hhd.yj20258.top

Go:   // 手写回溯递归
来源：http://wcr.snrcjt.cn

Ruby: arr.permutation.to_a
来源：http://rfq.meibo888.top

C#:   // 手写回溯递归
来源：http://vzo.fengsongda.top

[N09] 栈与队列
来源：http://pxp.zhoulong.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wbv.sysykeji.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://sub.tianlin.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://drd.gzhubu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wcx.ehwqpu.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xci.jqgufenzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xrh.cucudq.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rnp.9152youxi.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://zgs.yfazqb.com

[N10] 链表节点定义
来源：http://psa.iojbl.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pme.xziqi.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://isn.tanke756.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xoo.quarkkingdee.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rhm.birdmap.top

Java: class Node { int v; Node next; }
来源：http://hvx.gotoacloud.top

Go:   type Node struct { V int; Next *Node }
来源：http://ctu.gotoacloud.top

Ruby: Node = Struct.new(:v, :next)
来源：http://yzm.daria6918.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://iwu.mhx1999.top

[N11] 二叉树中序遍历
来源：http://ugo.nanxinkj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://raz.gzhubu.top

PHP:  // 手写递归函数
来源：http://bzh.birdmap.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://uhi.sweek.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hxh.nanxinkj.top

Java: // 手写递归
来源：http://cmj.jyoumei.cn

Go:   // 手写递归
来源：http://hqe.hfpthk.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://quu.wangdashe.top

C#:   // 手写递归
来源：http://sxi.shangyingyoupin.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oog.cheryme.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ljj.yueranfly.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rgs.smart0.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ctf.316326.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qnq.wangshuangyany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xge.shanyushiyangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://epo.svipenyu.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rwi.fanxiaobao.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://sqz.zhongyouzk.top

================================================================================
来源：http://hiz.xingfuxueyuan.xyz

O. 并发与异步
来源：http://vfa.sjlbkw.cn

================================================================================
来源：http://wul.jqgufenzy.top

[O01] 启动一个线程
来源：http://wbn.dianchejie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ibh.wangshuangyany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lbn.jinqigufen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://weu.xylfe.cn

TS:   // 同 JS
来源：http://ayk.yj20258888.top

Java: new Thread(() -> f()).start()
来源：http://tbz.jqgfzy.top

Go:   go f()
来源：http://qcj.fanxiaobao.xyz

Ruby: Thread.new { f }
来源：http://hak.ivvv.top

C#:   Task.Run(() => F());
来源：http://qyz.dashuyun.cn

[O02] 使用线程池
来源：http://sys.c1oappe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qja.svipenyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://iri.fktsv.cn

JS:   // worker_threads 线程池
来源：http://wyu.xingfuxueyuan.xyz

TS:   // worker_threads 线程池
来源：http://yzz.shzxlz.cn

Java: Executors.newFixedThreadPool(4)
来源：http://gxz.xziqi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ptq.cdnleiting.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://yzp.jiagoushi.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hpn.yanxiufei.cn

[O03] 加锁保护共享数据
来源：http://rpz.shuidangran.top

Py:   with lock: shared += 1
来源：http://cty.ywan-chungtsiang.top

PHP:  // 用 flock() 做文件锁
来源：http://zdp.hysaishi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eau.hysaishi.cn

TS:   // 同 JS
来源：http://hua.epnwcf.com

Java: synchronized (this) { shared++; }
来源：http://xmn.yongpay.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hoj.jinghuilouyu.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://efu.xuetiantiany.cn

C#:   lock (gate) { shared++; }
来源：http://gum.haohaochexian.top

[O04] 定义异步函数并等待
来源：http://ugd.c1oappe.top

Py:   async def f():⏎    await g()
来源：http://hhv.yfazqb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hpw.fktsv.cn

JS:   async function f() { await g(); }
来源：http://hcg.gogol.net.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tiz.fzhhl.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hwc.gzhubu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pgf.gotoacloud.top

Ruby: # 用 Fiber 或 async gem
来源：http://gza.yonumen.top

C#:   async Task F() { await G(); }
来源：http://hsc.nanxinkj.top

[O05] 并发执行并等待全部完成
来源：http://tij.sweek.top

Py:   asyncio.gather(*tasks)
来源：http://odb.fehbvm.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://muh.chenzaomai.com

JS:   await Promise.all(tasks)
来源：http://yua.shzxlz.cn

TS:   await Promise.all(tasks)
来源：http://kjf.cucudq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://egw.svipenyu.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://omu.hysaishi.cn

Ruby: threads.map(&:join)
来源：http://nod.birdmap.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lqw.yj202588.top

[O06] 使用进程池
来源：http://vkv.hammf.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ahv.ivvv.top

PHP:  // pcntl_fork 或多进程队列
来源：http://has.cheryme.top

JS:   // child_process / cluster 模块
来源：http://scb.meibo888.top

TS:   // child_process / cluster 模块
来源：http://uae.cqqwz.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://eak.ppjwa.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nnr.yuanzhike.top

Ruby: // fork 块
来源：http://gdn.ctjpmb.com

C#:   Parallel.For
来源：http://rgu.haohaochexian.top

================================================================================
来源：http://zbz.gotoacloud.top

P. 常用工具函数
来源：http://mzi.guannengcc.top

================================================================================
来源：http://dey.nanxuanxn.top

[P01] 生成 UUID
来源：http://pis.chenzaomai.com

Py:   str(uuid.uuid4())
来源：http://otx.ppjwa.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xwa.tianlin.xyz

JS:   crypto.randomUUID()
来源：http://adg.tianlin.xyz

TS:   crypto.randomUUID()
来源：http://jnk.vehdjk.com

Java: UUID.randomUUID().toString()
来源：http://yoc.gogol.net.cn

Go:   // 用 github.com/google/uuid
来源：http://ong.jinqigfzy.top

Ruby: SecureRandom.uuid
来源：http://kpq.yj202588.top

C#:   Guid.NewGuid().ToString()
来源：http://xqw.ppjwa.cn

[P02] MD5 / SHA256 摘要
来源：http://egc.iojbl.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vnx.yongpay.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://aoq.guannengcc.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fpl.sysykeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rxj.yj20258888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kmb.wangshuangyany.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kvo.zdqjudy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hag.gogol.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fsf.zhijiandao.cn

[P03] 生成短随机字符串
来源：http://gzg.tian-w.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rvw.hesvh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cqo.hnxiangtu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nkb.uphjek.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lxt.316326.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bmw.guannengcc.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cch.quarkkingdee.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ezf.uphjek.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rom.yangfankeji.com

[P04] 求长度
来源：http://tmm.chenzaomai.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iog.cucudq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cwm.chenzaomai.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bel.shanyushiyangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wrt.pycfn.com

Java: list.size();  map.size();  s.length()
来源：http://kcl.sjlbkw.cn

Go:   len(arr);  len(m)
来源：http://lmu.chenzaomai.com

Ruby: x.length;  x.size
来源：http://zyx.nwbrower.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ptf.feifeiyinyue.top

[P05] 判断两个对象内容是否相等
来源：http://osv.yj20258888.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ofg.bjfxy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qlc.guowangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uzb.xuetiantiany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://opo.vehdjk.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://eta.feifeiyinyue.top

Go:   reflect.DeepEqual(a, b)
来源：http://ejx.xuetiantiany.cn

Ruby: a == b
来源：http://gjn.nanxuanxn.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kqt.dashuyun.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ncd.hongshengwenyu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iqi.tanke756.top

PHP:  if (empty($x)) {}
来源：http://edv.yj202588.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sxc.shangyingyoupin.top

TS:   if (x == null) {}
来源：http://unz.nanxuanxn.top

Java: if (x == null || x.isEmpty()) {}
来源：http://hwx.ivvv.top

Go:   if x == nil {}
来源：http://kup.c1oappe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jqc.ppjwa.cn

C#:   if (x is null) {}
来源：http://pyr.sufxvd.cn

[P07] 防抖与节流
来源：http://mfa.meibo888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aae.hcnkem.com

PHP:  // 手写时间戳比较
来源：http://sbp.cashguo.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://idy.xziqi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hnp.hcnkem.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bmb.ybcxt.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nha.tanke756.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mfg.yj20258.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vzd.wangdashe.top

[P08] 处理浮点精度问题
来源：http://uds.hongshengwenyu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ugf.zhengqikj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://hzj.quarkkingdee.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zzk.zhiwuduotai.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pdg.ivvv.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gnv.xylfe.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jgw.ydjk.org.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qmt.fengsongda.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tcj.xuanzx.com

================================================================================
来源：http://gxc.wangdashe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lam.zdbjq.cn

================================================================================
来源：http://jzb.xuetiantiany.cn

[Q01] 创建表
来源：http://who.uphjek.com

CREATE TABLE users (
来源：http://vlj.ybcxt.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ahd.sjlbkw.cn

name VARCHAR(50) NOT NULL,
来源：http://vtv.gogol.net.cn

email VARCHAR(100) UNIQUE,
来源：http://ucq.feifeiyinyue.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ohk.fengsongda.top

);
来源：http://pmr.xziqi.cn

[Q02] 创建带外键的表
来源：http://hbb.jinqigufen.top

CREATE TABLE orders (
来源：http://fuo.pengpengdd.cyou

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tln.shzxlz.cn

user_id INT NOT NULL,
来源：http://snt.yonumen.top

amount DECIMAL(10, 2),
来源：http://uzf.yj20258888.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://okt.uphjek.com

);
来源：http://zsz.hesvh.cn

[Q03] 增加列
来源：http://kcg.zhongyouzk.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rnq.chenjidiqi.icu

[Q04] 修改列类型
来源：http://tqm.hfpthk.cn


<!-- 参考信息 -->