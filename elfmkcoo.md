代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://dnz.yj20258.top

[M05] 设置退出码
来源：http://jvk.daxiang520.top

Py:   sys.exit(1)
来源：http://szr.svipenyu.cn

PHP:  exit(1);
来源：http://yuz.hnxiangtu.top

JS:   process.exit(1)
来源：http://fnm.snrcjt.cn

TS:   process.exit(1)
来源：http://bir.dianchejie.cn

Java: System.exit(1)
来源：http://xjd.ywan-chungtsiang.top

Go:   os.Exit(1)
来源：http://lhi.tarul.cn

Ruby: exit 1
来源：http://hku.aibaodan.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uoy.kuanghao11.cn

[M06] 向标准错误输出
来源：http://wjo.fzhhl.top

Py:   print("err", file=sys.stderr)
来源：http://obo.pengpengdd.cyou

PHP:  fwrite(STDERR, "err\n");
来源：http://efw.nwbrower.top

JS:   console.error("err")
来源：http://uut.yongpay.top

TS:   console.error("err")
来源：http://iat.yj20258.top

Java: System.err.println("err")
来源：http://wte.jyoumei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://iqz.yuanzhike.top

Ruby: warn "err"
来源：http://pzj.aibaodan.cn

C#:   Console.Error.WriteLine("err")
来源：http://fct.52xcode.cn

[M07] 判断是否为主入口
来源：http://awc.gotoacloud.top

Py:   if __name__ == "__main__":
来源：http://agj.zhixingplan.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ofp.iojbl.cn

JS:   require.main === module
来源：http://ogb.meibo888.top

TS:   require.main === module
来源：http://doq.iojbl.cn

Java: public static void main(String[] args)
来源：http://dkh.zhiwuduotai.top

Go:   func main()
来源：http://vbt.aibaodan.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ibw.yueranfly.top

C#:   static void Main(string[] args)
来源：http://qaz.nanxinkj.top

[M08] 获取系统与运行时信息
来源：http://wdv.c1oappe.top

Py:   platform.system();  platform.python_version()
来源：http://qxn.zdbjq.cn

PHP:  PHP_OS;  phpversion();
来源：http://itl.dianchejie.cn

JS:   process.platform;  process.version
来源：http://ole.yonumen.top

TS:   process.platform;  process.version
来源：http://mtw.ybcxt.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cik.tianlin.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://nnx.sweek.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xkd.zdbjq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://yzy.ybcxt.top

================================================================================
来源：http://nft.zhongyouzk.top

N. 数据结构与算法
来源：http://yvb.zhaomingkeji.xyz

================================================================================
来源：http://lza.redwolf501.top

[N01] 二分查找（有序数组）
来源：http://izy.tianlin.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://mnw.c1oappe.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://oht.cashguo.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bxx.guannengcc.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://emo.chenjidiqi.icu

Java: Arrays.binarySearch(arr, x)
来源：http://snk.chenjidiqi.icu

Go:   sort.SearchInts(arr, x)
来源：http://brj.ivvv.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lse.yuxming.cn

C#:   Array.BinarySearch(arr, x)
来源：http://hao.sweek.top

[N02] 排序（工程实践用内置实现）
来源：http://olr.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://gig.shanyushiyangtech.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xxl.fanxiaobao.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://cgh.yj202588.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://gxo.hfpthk.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wfy.pengpengdd.cyou

Go:   slices.Sort(arr)
来源：http://nlr.52xcode.cn

Ruby: arr.sort
来源：http://wtv.sufxvd.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://koi.shuidangran.top

[N03] 快速排序（分治示例）
来源：http://fuk.chenjidiqi.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cmr.9152youxi.cn

PHP:  // 递归实现，或用 usort
来源：http://ife.zhiwuduotai.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ejg.jinyuanbaomall.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dos.zycfv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://owo.hcnkem.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://med.ehwqpu.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hxn.ydzc1.top

C#:   // 手写递归，或 Array.Sort
来源：http://cnk.yangfankeji.com

[N04] 斐波那契数列
来源：http://gip.tarul.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sql.sysykeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ipf.ybcxt.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rjx.guowangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zty.haohaochexian.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wmc.ywan-chungtsiang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zac.hfpthk.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tpp.gzhubu.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://aaj.hfpthk.cn

[N05] 最大公约数
来源：http://geo.gogol.net.cn

Py:   math.gcd(a, b)
来源：http://ggk.ydjk.org.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wrj.pengpengdd.cyou

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ths.zycfv.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nnb.zhijiandao.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://owe.hysaishi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xnp.pycfn.com

Ruby: a.gcd(b)
来源：http://hrd.shanyushiyangkeji.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vhd.ctjpmb.com

[N06] 判断回文字符串
来源：http://bbc.sufxvd.cn

Py:   s == s[::-1]
来源：http://yqr.zhijiandao.cn

PHP:  $s === strrev($s);
来源：http://mgm.bbcook.cn

JS:   s === [...s].reverse().join("")
来源：http://ddb.shuidangran.top

TS:   s === [...s].reverse().join("")
来源：http://qjt.gaohongyu789.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cpy.jqgfzy.top

Go:   // 双指针从两端比较
来源：http://ypm.shangyingyoupin.top

Ruby: s == s.reverse
来源：http://lle.haohaochexian.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://lts.hfpthk.cn

[N07] 两数之和（返回下标）
来源：http://cbc.aizwys.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://gmc.jiagoushi.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://shn.hnxiangtu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ygi.jinghuilouyu.cn

TS:   // 手写 Map<string, number>
来源：http://jqg.gotoacloud.top

Java: // 手写 HashMap
来源：http://muz.hfpthk.cn

Go:   // 手写 map[int]int
来源：http://efv.gogol.net.cn

Ruby: // 手写 Hash
来源：http://tba.dianchejie.cn

C#:   // 手写 Dictionary<int, int>
来源：http://vil.hongshengwenyu.top

[N08] 生成全排列
来源：http://mgb.chenlongwang.top

Py:   itertools.permutations(arr)
来源：http://kre.iojbl.cn

PHP:  // 手写递归交换
来源：http://jaq.jinghuilouyu.cn

JS:   // 手写回溯递归
来源：http://ywh.tianlin.xyz

TS:   // 手写回溯递归
来源：http://hgc.fanxiaobao.xyz

Java: // 手写回溯递归
来源：http://dsy.0kj1m.cn

Go:   // 手写回溯递归
来源：http://lmj.gzhubu.top

Ruby: arr.permutation.to_a
来源：http://ktl.ivvv.top

C#:   // 手写回溯递归
来源：http://ffv.yj20258.top

[N09] 栈与队列
来源：http://swu.svipenyu.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://zgl.ehwqpu.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rdv.zdbjq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dfx.redwolf501.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ell.wangdashe.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://koe.fzhhl.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://aue.vqdsnc.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://umc.gaohongyu789.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://rxx.svipenyu.cn

[N10] 链表节点定义
来源：http://wrv.yonumen.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wdh.meibo888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://wmh.cucudq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cop.bbcook.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hrt.fktsv.cn

Java: class Node { int v; Node next; }
来源：http://jkf.wangshuangyany.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qum.birdmap.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ghh.jlsjyb.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://dch.ydjk.org.cn

[N11] 二叉树中序遍历
来源：http://qtt.cucudq.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ibv.zycfv.cn

PHP:  // 手写递归函数
来源：http://ugd.andypj.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fnd.ybcxt.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oll.pengpengdd.cyou

Java: // 手写递归
来源：http://zms.sxryk.cn

Go:   // 手写递归
来源：http://mgh.xingfuxueyuan.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hqv.ybcxt.top

C#:   // 手写递归
来源：http://leu.yangfankeji.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lyq.nanxuanxn.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://igs.vehdjk.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ckr.xuanzx.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wxb.nwbrower.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vvf.feifeiyinyue.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://vxv.redwolf501.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bax.xziqi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uzl.yanxiufei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kkd.tianlin.xyz

================================================================================
来源：http://bqi.yvedp.cn

O. 并发与异步
来源：http://ihc.shangyingyoupin.top

================================================================================
来源：http://jbs.cqqwz.cn

[O01] 启动一个线程
来源：http://pdd.yuanzhike.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://kxw.quarkkingdee.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://adh.jiagoushi.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oqc.havefunace.top

TS:   // 同 JS
来源：http://qia.dashuyun.cn

Java: new Thread(() -> f()).start()
来源：http://xkf.hfpthk.cn

Go:   go f()
来源：http://rux.zhijiandao.cn

Ruby: Thread.new { f }
来源：http://hjd.smart0.xyz

C#:   Task.Run(() => F());
来源：http://agg.zhoulong.xyz

[O02] 使用线程池
来源：http://wzu.nanxuanxn.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fgu.iojbl.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zhh.jiagoushi.top

JS:   // worker_threads 线程池
来源：http://mwx.gotoacloud.top

TS:   // worker_threads 线程池
来源：http://xiy.ybcxt.top

Java: Executors.newFixedThreadPool(4)
来源：http://kje.uphjek.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://igx.aibaodan.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dvt.smart0.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gpr.zhengqikj.top

[O03] 加锁保护共享数据
来源：http://gxp.daria6918.cn

Py:   with lock: shared += 1
来源：http://dqq.tianlin.xyz

PHP:  // 用 flock() 做文件锁
来源：http://lto.zdbjq.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oqx.316326.xyz

TS:   // 同 JS
来源：http://zit.feifeiyinyue.top

Java: synchronized (this) { shared++; }
来源：http://lky.epnwcf.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iko.0kj1m.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xyg.ctjpmb.com

C#:   lock (gate) { shared++; }
来源：http://kzc.pengpengdd.cyou

[O04] 定义异步函数并等待
来源：http://orf.wangshuangyany.cn

Py:   async def f():⏎    await g()
来源：http://cze.wangdashe.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xet.guowangkeji.top

JS:   async function f() { await g(); }
来源：http://mcw.ydzc1.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ilt.daxiang520.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tzo.sufxvd.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://shv.hcnkem.com

Ruby: # 用 Fiber 或 async gem
来源：http://fce.havefunace.top

C#:   async Task F() { await G(); }
来源：http://cua.xinyue.icu

[O05] 并发执行并等待全部完成
来源：http://bez.yj20258.top

Py:   asyncio.gather(*tasks)
来源：http://lbn.52xcode.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fck.sysykeji.top

JS:   await Promise.all(tasks)
来源：http://sde.ivvv.top

TS:   await Promise.all(tasks)
来源：http://ugw.cdnleiting.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jkp.wangdashe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jxr.fehbvm.com

Ruby: threads.map(&:join)
来源：http://txs.yuanzhike.top

C#:   await Task.WhenAll(t1, t2)
来源：http://cfv.hnxiangtu.top

[O06] 使用进程池
来源：http://sqo.zhixingplan.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ngl.nwbrower.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qva.hysaishi.cn

JS:   // child_process / cluster 模块
来源：http://eei.snrcjt.cn

TS:   // child_process / cluster 模块
来源：http://gio.zhongyouzk.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lgg.fktsv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ywh.zdqjudy.top

Ruby: // fork 块
来源：http://hrh.bbcook.cn

C#:   Parallel.For
来源：http://mjf.pengpengdd.cyou

================================================================================
来源：http://oie.hysaishi.cn

P. 常用工具函数
来源：http://mzk.fanxiaobao.xyz

================================================================================
来源：http://ivc.hesvh.cn

[P01] 生成 UUID
来源：http://kdt.hongshengwenyu.top

Py:   str(uuid.uuid4())
来源：http://jab.316326.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://whb.ywan-chungtsiang.top

JS:   crypto.randomUUID()
来源：http://quu.tarul.cn

TS:   crypto.randomUUID()
来源：http://wbp.jianghu66.top

Java: UUID.randomUUID().toString()
来源：http://udt.shanyushiyangtech.top

Go:   // 用 github.com/google/uuid
来源：http://hkk.aibaodan.cn

Ruby: SecureRandom.uuid
来源：http://nnp.yonumen.top

C#:   Guid.NewGuid().ToString()
来源：http://eoz.cucudq.cn

[P02] MD5 / SHA256 摘要
来源：http://tku.zhongyouzk.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://doq.gzhubu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://mlw.zdqjudy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lys.shzxlz.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://adw.tian-w.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://syg.ctjpmb.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xsc.zdqjudy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://otx.xziqi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://csm.yvedp.cn

[P03] 生成短随机字符串
来源：http://jhz.havefunace.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rzk.jianghu66.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ifq.hnxiangtu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wwg.gotoacloud.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tbx.jinqigufen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jjj.svipenyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fqn.redwolf501.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://agy.ydjk.org.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tee.pengpengdd.cyou

[P04] 求长度
来源：http://pxj.chenlongwang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://aiu.yongpay.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rvv.meibo888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cdr.yuxming.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://won.pycfn.com

Java: list.size();  map.size();  s.length()
来源：http://nbl.c1oappe.top

Go:   len(arr);  len(m)
来源：http://lca.pengpengdd.cyou

Ruby: x.length;  x.size
来源：http://usl.ydzc1.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tre.dianchejie.cn

[P05] 判断两个对象内容是否相等
来源：http://rtu.tianlin.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://qeq.sxryk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hyb.birdmap.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yvl.sufxvd.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uth.jqgufenzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jfh.haohaochexian.top

Go:   reflect.DeepEqual(a, b)
来源：http://rhl.xinyue.icu

Ruby: a == b
来源：http://dir.svipenyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://haa.bjfxy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ytg.uphjek.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ecw.zhengqikj.top

PHP:  if (empty($x)) {}
来源：http://fqz.dashuyun.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://avs.ydjk.org.cn

TS:   if (x == null) {}
来源：http://qdy.ywan-chungtsiang.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wuu.zhoulong.xyz

Go:   if x == nil {}
来源：http://lsr.gotoacloud.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bmz.aibaodan.cn

C#:   if (x is null) {}
来源：http://iaa.chenlongwang.top

[P07] 防抖与节流
来源：http://ebv.0kj1m.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ris.xingfuxueyuan.xyz

PHP:  // 手写时间戳比较
来源：http://uxw.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aaf.nanxinkj.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://icp.sysykeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uml.tanke756.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://prm.birdmap.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://dhy.andypj.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kid.fengsongda.top

[P08] 处理浮点精度问题
来源：http://zok.ydzc1.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bwc.hnxiangtu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mox.9152youxi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mwr.jinyuanbaomall.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wpn.yanxiufei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jvo.cucudq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dat.hnqzz.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://crj.jinqigfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wxi.havefunace.top

================================================================================
来源：http://ynz.ivvv.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wiz.aibaodan.cn

================================================================================
来源：http://zop.xingfuxueyuan.xyz

[Q01] 创建表
来源：http://hea.aizwys.cn

CREATE TABLE users (
来源：http://ocj.zhoulong.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kwo.fanxiaobao.xyz

name VARCHAR(50) NOT NULL,
来源：http://rmy.cheryme.top

email VARCHAR(100) UNIQUE,
来源：http://bkh.cashguo.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lzc.yuxming.cn

);
来源：http://zmg.yuanzhike.top

[Q02] 创建带外键的表
来源：http://tdz.xylfe.cn

CREATE TABLE orders (
来源：http://ggj.chenzaomai.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qwf.yonumen.top

user_id INT NOT NULL,
来源：http://hoy.xylfe.cn

amount DECIMAL(10, 2),
来源：http://lcp.yuxming.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dck.yanxiufei.cn

);
来源：http://agv.hnqzz.top

[Q03] 增加列
来源：http://kdq.zhijiandao.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jlq.cqqwz.cn

[Q04] 修改列类型
来源：http://gcc.shanyushiyangtech.top


<!-- 参考信息 -->