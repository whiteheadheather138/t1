代发 wailian999

JS:   process.exit(1)
来源：http://jdb.yuanzhike.top

TS:   process.exit(1)
来源：http://njs.gzhubu.top

Java: System.exit(1)
来源：http://rii.zhaomingkeji.xyz

Go:   os.Exit(1)
来源：http://viq.yfazqb.com

Ruby: exit 1
来源：http://tju.jinyuanbaomall.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vdb.cqqwz.cn

[M06] 向标准错误输出
来源：http://dxb.mhx1999.top

Py:   print("err", file=sys.stderr)
来源：http://xwz.fzhhl.top

PHP:  fwrite(STDERR, "err\n");
来源：http://crm.jinghuilouyu.cn

JS:   console.error("err")
来源：http://ulj.kuanghao11.cn

TS:   console.error("err")
来源：http://yiq.havefunace.top

Java: System.err.println("err")
来源：http://dky.9152youxi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bfp.xziqi.cn

Ruby: warn "err"
来源：http://nrv.dashuyun.cn

C#:   Console.Error.WriteLine("err")
来源：http://hbx.mhx1999.top

[M07] 判断是否为主入口
来源：http://aph.xinyue.icu

Py:   if __name__ == "__main__":
来源：http://bws.havefunace.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://org.yueranfly.top

JS:   require.main === module
来源：http://sjq.uphjek.com

TS:   require.main === module
来源：http://uet.zhongyouzk.top

Java: public static void main(String[] args)
来源：http://kgl.dashuyun.cn

Go:   func main()
来源：http://ost.bbcook.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tfp.shuidangran.top

C#:   static void Main(string[] args)
来源：http://nxa.yfazqb.com

[M08] 获取系统与运行时信息
来源：http://iwq.cucudq.cn

Py:   platform.system();  platform.python_version()
来源：http://yzh.svipenyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://uho.zhixingplan.top

JS:   process.platform;  process.version
来源：http://rom.tarul.cn

TS:   process.platform;  process.version
来源：http://gty.wangshuangyany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pwx.hesvh.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qho.xziqi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://qpd.hysaishi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://suj.jinqigfzy.top

================================================================================
来源：http://alw.nanxuanxn.top

N. 数据结构与算法
来源：http://yqo.zhaomingkeji.xyz

================================================================================
来源：http://sow.shanyushiyangkeji.top

[N01] 二分查找（有序数组）
来源：http://apo.uphjek.com

Py:   bisect.bisect_left(arr, x)
来源：http://vys.jqgufenzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qkn.yvedp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xyw.chenlongwang.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hdx.gogol.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mvl.pengpengdd.cyou

Go:   sort.SearchInts(arr, x)
来源：http://ojb.cdnleiting.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://fhg.pycfn.com

C#:   Array.BinarySearch(arr, x)
来源：http://tdy.yj202588.top

[N02] 排序（工程实践用内置实现）
来源：http://uyq.nanxinkj.top

Py:   sorted(arr);  arr.sort()
来源：http://msx.kuanghao11.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kst.gotoacloud.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xur.gaohongyu789.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wab.xuanzx.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zmh.ivvv.top

Go:   slices.Sort(arr)
来源：http://bbv.jqgufenzy.top

Ruby: arr.sort
来源：http://umr.hongshengwenyu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://nuo.yueranfly.top

[N03] 快速排序（分治示例）
来源：http://xxs.chenlongwang.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://oxa.kuanghao11.cn

PHP:  // 递归实现，或用 usort
来源：http://llv.jyoumei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tvz.bbcook.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mtq.shanyushiyangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lrn.bjfxy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://miw.shzxlz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://isg.hongshengwenyu.top

C#:   // 手写递归，或 Array.Sort
来源：http://gdw.xuetiantiany.cn

[N04] 斐波那契数列
来源：http://hed.jianghu66.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uqi.chenlongwang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://edh.zhoulong.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kwo.havefunace.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://obf.shangyingyoupin.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ewm.zhaomingkeji.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nsy.pengpengdd.cyou

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://icr.andypj.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gqf.jinqigfzy.top

[N05] 最大公约数
来源：http://wsh.cucudq.cn

Py:   math.gcd(a, b)
来源：http://kko.sweek.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://xpm.vqdsnc.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yqx.pycfn.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tsl.svipenyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rxm.vqdsnc.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rux.gotoacloud.top

Ruby: a.gcd(b)
来源：http://btr.hnqzz.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cxd.andypj.xyz

[N06] 判断回文字符串
来源：http://qgn.bbcook.cn

Py:   s == s[::-1]
来源：http://ttp.wangdashe.top

PHP:  $s === strrev($s);
来源：http://gul.zhiwuduotai.top

JS:   s === [...s].reverse().join("")
来源：http://gxn.ybcxt.top

TS:   s === [...s].reverse().join("")
来源：http://idf.daria6918.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://pfo.zdbjq.cn

Go:   // 双指针从两端比较
来源：http://xex.zhoulong.xyz

Ruby: s == s.reverse
来源：http://cld.jianghu66.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://sbo.ydjk.org.cn

[N07] 两数之和（返回下标）
来源：http://qet.ydjk.org.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://por.yuanzhike.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mlp.zhongyouzk.top

JS:   // 手写 Map：map.set(v, i)
来源：http://skq.yfazqb.com

TS:   // 手写 Map<string, number>
来源：http://mdp.yvedp.cn

Java: // 手写 HashMap
来源：http://kyi.daxiang520.top

Go:   // 手写 map[int]int
来源：http://fja.feifeiyinyue.top

Ruby: // 手写 Hash
来源：http://zjx.sxryk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dgw.havefunace.top

[N08] 生成全排列
来源：http://yts.jqgufenzy.top

Py:   itertools.permutations(arr)
来源：http://vbw.ehwqpu.com

PHP:  // 手写递归交换
来源：http://jww.zdbjq.cn

JS:   // 手写回溯递归
来源：http://txc.jqgufenzy.top

TS:   // 手写回溯递归
来源：http://dth.xuetiantiany.cn

Java: // 手写回溯递归
来源：http://dyw.nwbrower.top

Go:   // 手写回溯递归
来源：http://htc.yueranfly.top

Ruby: arr.permutation.to_a
来源：http://uxj.xuetiantiany.cn

C#:   // 手写回溯递归
来源：http://avt.tarul.cn

[N09] 栈与队列
来源：http://kqe.smart0.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ete.xingfuxueyuan.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ngo.jqgfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://byb.hnxiangtu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rzz.quarkkingdee.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jia.pengpengdd.cyou

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://yfg.sufxvd.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wib.jinghuilouyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vbl.yfazqb.com

[N10] 链表节点定义
来源：http://hzv.hysaishi.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dtc.jqgfzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qxl.hfpthk.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://usl.dashuyun.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vvw.yonumen.top

Java: class Node { int v; Node next; }
来源：http://dwz.yvedp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://uwa.hesvh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://yus.zycfv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://krt.shzxlz.cn

[N11] 二叉树中序遍历
来源：http://vbs.shanyushiyangtech.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pml.zhaomingkeji.xyz

PHP:  // 手写递归函数
来源：http://wya.haohaochexian.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://efz.havefunace.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zyi.xziqi.cn

Java: // 手写递归
来源：http://wrn.sxryk.cn

Go:   // 手写递归
来源：http://ukg.zhengqikj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nya.aibaodan.cn

C#:   // 手写递归
来源：http://stw.jianghu66.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vtv.birdmap.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gfg.c1oappe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ake.tian-w.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hcw.fktsv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xxw.meibo888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vjn.dashuyun.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dps.jianghu66.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mfy.hongshengwenyu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://nsz.tianlin.xyz

================================================================================
来源：http://kla.ehwqpu.com

O. 并发与异步
来源：http://por.ybcxt.top

================================================================================
来源：http://lkq.gzhubu.top

[O01] 启动一个线程
来源：http://vap.tanke756.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bdy.cdnleiting.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fib.jinqigfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://upe.yj20258888.top

TS:   // 同 JS
来源：http://gkp.ppjwa.cn

Java: new Thread(() -> f()).start()
来源：http://cwp.zhixingplan.top

Go:   go f()
来源：http://sku.jinghuilouyu.cn

Ruby: Thread.new { f }
来源：http://axs.vqdsnc.cn

C#:   Task.Run(() => F());
来源：http://gju.9152youxi.cn

[O02] 使用线程池
来源：http://rtw.ehwqpu.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ifu.jinyuanbaomall.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rxg.xingfuxueyuan.xyz

JS:   // worker_threads 线程池
来源：http://ksr.ctjpmb.com

TS:   // worker_threads 线程池
来源：http://oto.daria6918.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kek.quarkkingdee.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rgs.zhiwuduotai.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hcy.sxryk.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bpe.ybcxt.top

[O03] 加锁保护共享数据
来源：http://piv.epnwcf.com

Py:   with lock: shared += 1
来源：http://qwh.vehdjk.com

PHP:  // 用 flock() 做文件锁
来源：http://dap.tianlin.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bqq.316326.xyz

TS:   // 同 JS
来源：http://upg.shuidangran.top

Java: synchronized (this) { shared++; }
来源：http://oiq.xingfuxueyuan.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nbj.shuidangran.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nxf.cucudq.cn

C#:   lock (gate) { shared++; }
来源：http://qll.yj202588.top

[O04] 定义异步函数并等待
来源：http://qzr.gotoacloud.top

Py:   async def f():⏎    await g()
来源：http://emf.shanyushiyangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lle.ywan-chungtsiang.top

JS:   async function f() { await g(); }
来源：http://zvo.vqdsnc.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://clg.smart0.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ebo.zhijiandao.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://les.vehdjk.com

Ruby: # 用 Fiber 或 async gem
来源：http://rct.jinghuilouyu.cn

C#:   async Task F() { await G(); }
来源：http://eua.daxiang520.top

[O05] 并发执行并等待全部完成
来源：http://xpb.xuetiantiany.cn

Py:   asyncio.gather(*tasks)
来源：http://sww.dianchejie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hio.fengsongda.top

JS:   await Promise.all(tasks)
来源：http://tbf.xuetiantiany.cn

TS:   await Promise.all(tasks)
来源：http://kjq.nanxinkj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://amz.guannengcc.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ahn.fktsv.cn

Ruby: threads.map(&:join)
来源：http://eqw.yuanzhike.top

C#:   await Task.WhenAll(t1, t2)
来源：http://blk.zhijiandao.cn

[O06] 使用进程池
来源：http://czn.yongpay.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://nut.hongshengwenyu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mvb.hesvh.cn

JS:   // child_process / cluster 模块
来源：http://ccc.jlsjyb.cn

TS:   // child_process / cluster 模块
来源：http://ufn.guowangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fss.feifeiyinyue.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cqp.tian-w.cn

Ruby: // fork 块
来源：http://sbn.sxryk.cn

C#:   Parallel.For
来源：http://cnu.uphjek.com

================================================================================
来源：http://ljo.ydjk.org.cn

P. 常用工具函数
来源：http://aqt.ppjwa.cn

================================================================================
来源：http://pdc.xuanzx.com

[P01] 生成 UUID
来源：http://tkm.sxryk.cn

Py:   str(uuid.uuid4())
来源：http://cdf.hammf.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://aov.zhijiandao.cn

JS:   crypto.randomUUID()
来源：http://gbw.yfazqb.com

TS:   crypto.randomUUID()
来源：http://tbl.redwolf501.top

Java: UUID.randomUUID().toString()
来源：http://zpa.birdmap.top

Go:   // 用 github.com/google/uuid
来源：http://kgo.xinyue.icu

Ruby: SecureRandom.uuid
来源：http://rju.smart0.xyz

C#:   Guid.NewGuid().ToString()
来源：http://lxv.aibaodan.cn

[P02] MD5 / SHA256 摘要
来源：http://blz.snrcjt.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://erg.xuetiantiany.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://loy.epnwcf.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tbd.jinyuanbaomall.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://reh.shanyushiyangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yii.xinyue.icu

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nmn.pengpengdd.cyou

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pbp.wangshuangyany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xxz.yj202588.top

[P03] 生成短随机字符串
来源：http://htf.daxiang520.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://snz.sysykeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hkh.nanxinkj.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oek.shanyushiyangtech.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://llm.aibaodan.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vrl.ctjpmb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gji.9152youxi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jnm.yongpay.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://acl.hywenlv.cn

[P04] 求长度
来源：http://nue.quarkkingdee.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://quo.bbcook.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pve.xziqi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bzf.fktsv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://guf.fanxiaobao.xyz

Java: list.size();  map.size();  s.length()
来源：http://kew.xingfuxueyuan.xyz

Go:   len(arr);  len(m)
来源：http://phn.zhiwuduotai.top

Ruby: x.length;  x.size
来源：http://mwg.ybcxt.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://txx.gaohongyu789.top

[P05] 判断两个对象内容是否相等
来源：http://xvn.haohaochexian.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lla.yangfankeji.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://avb.pycfn.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jpa.daria6918.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vjs.haohaochexian.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://juv.0kj1m.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vnl.jinyuanbaomall.cn

Ruby: a == b
来源：http://ujo.sxryk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dbu.0kj1m.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dnz.shanyushiyangtech.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wdc.yj20258.top

PHP:  if (empty($x)) {}
来源：http://iac.dianchejie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uyz.aizwys.cn

TS:   if (x == null) {}
来源：http://jlg.bjfxy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://npr.uphjek.com

Go:   if x == nil {}
来源：http://oyw.yuanzhike.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wis.shanyushiyangtech.top

C#:   if (x is null) {}
来源：http://rtj.aibaodan.cn

[P07] 防抖与节流
来源：http://vfi.xingfuxueyuan.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mli.ydjk.org.cn

PHP:  // 手写时间戳比较
来源：http://unp.zdbjq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cka.ydjk.org.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cix.hfpthk.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uaq.epnwcf.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xpl.shanyushiyangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gnh.sufxvd.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pcj.hesvh.cn

[P08] 处理浮点精度问题
来源：http://uck.aizwys.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pyg.jinghuilouyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://trg.zycfv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oaa.316326.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fvx.hesvh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vun.ctjpmb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qkv.nanxuanxn.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qtt.yonumen.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vgx.sjlbkw.cn

================================================================================
来源：http://kmr.yuxming.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jpz.chenlongwang.top

================================================================================
来源：http://xom.sweek.top

[Q01] 创建表
来源：http://dyv.tanke756.top

CREATE TABLE users (
来源：http://gkh.zhaomingkeji.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://onx.zhengqikj.top

name VARCHAR(50) NOT NULL,
来源：http://rrt.zhoulong.xyz

email VARCHAR(100) UNIQUE,
来源：http://xul.smart0.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fus.gotoacloud.top

);
来源：http://skn.tian-w.cn

[Q02] 创建带外键的表
来源：http://qsp.yj20258.top

CREATE TABLE orders (
来源：http://ssg.haohaochexian.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xml.tianlin.xyz

user_id INT NOT NULL,
来源：http://ore.zdqjudy.top

amount DECIMAL(10, 2),
来源：http://nko.shanyushiyangtech.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hvh.havefunace.top

);
来源：http://bcu.gogol.net.cn

[Q03] 增加列
来源：http://ppt.kuanghao11.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rkx.fanxiaobao.xyz

[Q04] 修改列类型
来源：http://umw.hnqzz.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://woc.ywan-chungtsiang.top

[Q05] 重命名列
来源：http://vsb.ydzc1.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jyb.epnwcf.com

[Q06] 删除列
来源：http://zdc.sufxvd.cn


<!-- 参考信息 -->