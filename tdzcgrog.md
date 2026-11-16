代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://bvt.ehwqpu.com

[M05] 设置退出码
来源：http://bnr.guannengcc.top

Py:   sys.exit(1)
来源：http://rzq.hysaishi.cn

PHP:  exit(1);
来源：http://zkv.zhiwuduotai.top

JS:   process.exit(1)
来源：http://ipa.nanxuanxn.top

TS:   process.exit(1)
来源：http://uek.ywan-chungtsiang.top

Java: System.exit(1)
来源：http://lgo.9152youxi.cn

Go:   os.Exit(1)
来源：http://qai.316326.xyz

Ruby: exit 1
来源：http://lml.xziqi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tzo.yueranfly.top

[M06] 向标准错误输出
来源：http://qny.hnxiangtu.top

Py:   print("err", file=sys.stderr)
来源：http://vlg.cheryme.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vnh.svipenyu.cn

JS:   console.error("err")
来源：http://cac.shuidangran.top

TS:   console.error("err")
来源：http://rpu.shangyingyoupin.top

Java: System.err.println("err")
来源：http://cev.pengpengdd.cyou

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ien.yj20258888.top

Ruby: warn "err"
来源：http://yqa.ctjpmb.com

C#:   Console.Error.WriteLine("err")
来源：http://bew.sxryk.cn

[M07] 判断是否为主入口
来源：http://bxo.zhixingplan.top

Py:   if __name__ == "__main__":
来源：http://fhx.redwolf501.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cks.epnwcf.com

JS:   require.main === module
来源：http://swn.havefunace.top

TS:   require.main === module
来源：http://isl.svipenyu.cn

Java: public static void main(String[] args)
来源：http://kdq.gogol.net.cn

Go:   func main()
来源：http://vwe.yongpay.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://uru.vqdsnc.cn

C#:   static void Main(string[] args)
来源：http://dcj.fengsongda.top

[M08] 获取系统与运行时信息
来源：http://hyq.shangyingyoupin.top

Py:   platform.system();  platform.python_version()
来源：http://cfk.ywan-chungtsiang.top

PHP:  PHP_OS;  phpversion();
来源：http://egt.wangshuangyany.cn

JS:   process.platform;  process.version
来源：http://nvl.yuxming.cn

TS:   process.platform;  process.version
来源：http://yuz.uphjek.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://alz.redwolf501.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ufd.hesvh.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yvl.fktsv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bun.nanxuanxn.top

================================================================================
来源：http://rrp.jqgufenzy.top

N. 数据结构与算法
来源：http://eej.hywenlv.cn

================================================================================
来源：http://ijf.nanxinkj.top

[N01] 二分查找（有序数组）
来源：http://myz.cqqwz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://mtv.316326.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ygt.ehwqpu.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cby.birdmap.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sfb.hfpthk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://gre.tarul.cn

Go:   sort.SearchInts(arr, x)
来源：http://esz.sysykeji.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qly.cashguo.top

C#:   Array.BinarySearch(arr, x)
来源：http://met.ydzc1.top

[N02] 排序（工程实践用内置实现）
来源：http://pzt.zhongyouzk.top

Py:   sorted(arr);  arr.sort()
来源：http://bnv.xziqi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gde.yongpay.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://guw.tian-w.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://knn.zdbjq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rth.xingfuxueyuan.xyz

Go:   slices.Sort(arr)
来源：http://oej.snrcjt.cn

Ruby: arr.sort
来源：http://shm.havefunace.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://bff.jinyuanbaomall.cn

[N03] 快速排序（分治示例）
来源：http://dwn.yuxming.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://msi.birdmap.top

PHP:  // 递归实现，或用 usort
来源：http://uhq.shzxlz.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uek.gzhubu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rvi.nanxuanxn.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://udz.shzxlz.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uxj.jyoumei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://twz.pycfn.com

C#:   // 手写递归，或 Array.Sort
来源：http://qsp.bjfxy.top

[N04] 斐波那契数列
来源：http://hxg.9152youxi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ezh.shanyushiyangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://std.kuanghao11.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ino.cqqwz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://khr.hesvh.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kxd.pengpengdd.cyou

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uxl.zhengqikj.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gsh.zhijiandao.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ekv.fengsongda.top

[N05] 最大公约数
来源：http://qzq.pycfn.com

Py:   math.gcd(a, b)
来源：http://tys.iojbl.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://urm.quarkkingdee.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ttl.sweek.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wbk.fktsv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xpe.kuanghao11.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xnh.jlsjyb.cn

Ruby: a.gcd(b)
来源：http://rpv.yonumen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fge.sysykeji.top

[N06] 判断回文字符串
来源：http://hnm.shanyushiyangkeji.top

Py:   s == s[::-1]
来源：http://npc.fanxiaobao.xyz

PHP:  $s === strrev($s);
来源：http://vwo.fktsv.cn

JS:   s === [...s].reverse().join("")
来源：http://fue.zhengqikj.top

TS:   s === [...s].reverse().join("")
来源：http://acr.guowangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hqi.pengpengdd.cyou

Go:   // 双指针从两端比较
来源：http://dxw.hcnkem.com

Ruby: s == s.reverse
来源：http://gih.jiagoushi.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://kdt.yj20258888.top

[N07] 两数之和（返回下标）
来源：http://piv.xziqi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fkh.ydzc1.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fpq.jlsjyb.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cse.52xcode.cn

TS:   // 手写 Map<string, number>
来源：http://wgu.zhixingplan.top

Java: // 手写 HashMap
来源：http://vjy.nwbrower.top

Go:   // 手写 map[int]int
来源：http://odp.daria6918.cn

Ruby: // 手写 Hash
来源：http://vsx.zhaomingkeji.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://fcm.pengpengdd.cyou

[N08] 生成全排列
来源：http://cnh.yvedp.cn

Py:   itertools.permutations(arr)
来源：http://lpd.jqgufenzy.top

PHP:  // 手写递归交换
来源：http://fqq.fzhhl.top

JS:   // 手写回溯递归
来源：http://fwc.nanxinkj.top

TS:   // 手写回溯递归
来源：http://jbs.ehwqpu.com

Java: // 手写回溯递归
来源：http://ntp.fengsongda.top

Go:   // 手写回溯递归
来源：http://ijj.sysykeji.top

Ruby: arr.permutation.to_a
来源：http://igf.zdqjudy.top

C#:   // 手写回溯递归
来源：http://gdw.shuidangran.top

[N09] 栈与队列
来源：http://mce.yvedp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dxb.pengpengdd.cyou

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://igv.jqgfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wzw.yvedp.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://atu.ivvv.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qlv.dianchejie.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://azi.xylfe.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ige.yanxiufei.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fgg.tianlin.xyz

[N10] 链表节点定义
来源：http://sod.52xcode.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xtk.zhongyouzk.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gbv.sufxvd.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://guy.xinyue.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vul.tanke756.top

Java: class Node { int v; Node next; }
来源：http://val.sxryk.cn

Go:   type Node struct { V int; Next *Node }
来源：http://uvq.kuanghao11.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://pys.shanyushiyangtech.top

C#:   class Node { public int V; public Node? Next; }
来源：http://cqh.cdnleiting.top

[N11] 二叉树中序遍历
来源：http://api.zhengqikj.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://zvz.sjlbkw.cn

PHP:  // 手写递归函数
来源：http://giu.jinqigufen.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ykf.fanxiaobao.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://msj.jqgfzy.top

Java: // 手写递归
来源：http://kza.haohaochexian.top

Go:   // 手写递归
来源：http://kls.0kj1m.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ilf.zhijiandao.cn

C#:   // 手写递归
来源：http://oug.zdbjq.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://jrt.hysaishi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tkd.316326.xyz

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hjk.jyoumei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ylx.xuetiantiany.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://akn.fzhhl.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ykv.tanke756.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wso.tianlin.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bss.jianghu66.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rxh.haohaochexian.top

================================================================================
来源：http://bsd.fanxiaobao.xyz

O. 并发与异步
来源：http://ljc.guannengcc.top

================================================================================
来源：http://phu.sysykeji.top

[O01] 启动一个线程
来源：http://ziw.316326.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mkp.haohaochexian.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xwy.yfazqb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lii.yongpay.top

TS:   // 同 JS
来源：http://ewb.fzhhl.top

Java: new Thread(() -> f()).start()
来源：http://cos.zhijiandao.cn

Go:   go f()
来源：http://bsb.chenjidiqi.icu

Ruby: Thread.new { f }
来源：http://wqx.hysaishi.cn

C#:   Task.Run(() => F());
来源：http://pmg.ctjpmb.com

[O02] 使用线程池
来源：http://klw.snrcjt.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dxj.smart0.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zyp.zhiwuduotai.top

JS:   // worker_threads 线程池
来源：http://pxy.shanyushiyangtech.top

TS:   // worker_threads 线程池
来源：http://eti.jyoumei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ruy.ppjwa.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xxh.nanxinkj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://oac.jyoumei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://evi.quarkkingdee.top

[O03] 加锁保护共享数据
来源：http://tut.yuxming.cn

Py:   with lock: shared += 1
来源：http://lqe.zycfv.cn

PHP:  // 用 flock() 做文件锁
来源：http://ovo.kuanghao11.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yee.sysykeji.top

TS:   // 同 JS
来源：http://vha.zdqjudy.top

Java: synchronized (this) { shared++; }
来源：http://aoo.pengpengdd.cyou

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pse.hnxiangtu.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://sdu.daria6918.cn

C#:   lock (gate) { shared++; }
来源：http://dyb.quarkkingdee.top

[O04] 定义异步函数并等待
来源：http://vhy.hcnkem.com

Py:   async def f():⏎    await g()
来源：http://hur.zdbjq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kfs.yuanzhike.top

JS:   async function f() { await g(); }
来源：http://nup.bjfxy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vjb.ppjwa.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ywx.kuanghao11.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://meo.gotoacloud.top

Ruby: # 用 Fiber 或 async gem
来源：http://hsy.hfpthk.cn

C#:   async Task F() { await G(); }
来源：http://sxe.gogol.net.cn

[O05] 并发执行并等待全部完成
来源：http://sxa.cheryme.top

Py:   asyncio.gather(*tasks)
来源：http://ofh.smart0.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bge.ydjk.org.cn

JS:   await Promise.all(tasks)
来源：http://hbh.fehbvm.com

TS:   await Promise.all(tasks)
来源：http://xvg.dashuyun.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://adi.iojbl.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gaq.guannengcc.top

Ruby: threads.map(&:join)
来源：http://fkb.yongpay.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dsm.yvedp.cn

[O06] 使用进程池
来源：http://lxt.hnxiangtu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://piz.hywenlv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rgv.jinyuanbaomall.cn

JS:   // child_process / cluster 模块
来源：http://yjk.zhixingplan.top

TS:   // child_process / cluster 模块
来源：http://rjq.sjlbkw.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rcm.nwbrower.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zsc.havefunace.top

Ruby: // fork 块
来源：http://mez.havefunace.top

C#:   Parallel.For
来源：http://gfp.nanxinkj.top

================================================================================
来源：http://hqu.chenjidiqi.icu

P. 常用工具函数
来源：http://pyt.yj202588.top

================================================================================
来源：http://usx.bjfxy.top

[P01] 生成 UUID
来源：http://apb.yanxiufei.cn

Py:   str(uuid.uuid4())
来源：http://leu.tian-w.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xqv.chenlongwang.top

JS:   crypto.randomUUID()
来源：http://ftn.ybcxt.top

TS:   crypto.randomUUID()
来源：http://qwr.zhijiandao.cn

Java: UUID.randomUUID().toString()
来源：http://etx.tarul.cn

Go:   // 用 github.com/google/uuid
来源：http://pde.zhixingplan.top

Ruby: SecureRandom.uuid
来源：http://slx.ydzc1.top

C#:   Guid.NewGuid().ToString()
来源：http://ehz.shuidangran.top

[P02] MD5 / SHA256 摘要
来源：http://eem.hywenlv.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zgg.hongshengwenyu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://klf.ivvv.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mkf.wangdashe.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tni.bbcook.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dqk.nanxinkj.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xzg.tanke756.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xqd.fanxiaobao.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mwz.fzhhl.top

[P03] 生成短随机字符串
来源：http://zke.yanxiufei.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fmj.yanxiufei.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uxc.sufxvd.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qia.shanyushiyangtech.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://emr.havefunace.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wyh.tanke756.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uzh.yuanzhike.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://qzw.andypj.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://whq.xuetiantiany.cn

[P04] 求长度
来源：http://kha.sysykeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://epq.zdqjudy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zvq.jqgufenzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://avd.hnqzz.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pqk.fanxiaobao.xyz

Java: list.size();  map.size();  s.length()
来源：http://qgq.zhengqikj.top

Go:   len(arr);  len(m)
来源：http://mlq.nanxinkj.top

Ruby: x.length;  x.size
来源：http://wzk.xingfuxueyuan.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://lpc.wangdashe.top

[P05] 判断两个对象内容是否相等
来源：http://ubu.nanxuanxn.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zdb.xuanzx.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nsz.nwbrower.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://urc.shuidangran.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qzp.epnwcf.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fmq.sufxvd.cn

Go:   reflect.DeepEqual(a, b)
来源：http://elj.zhaomingkeji.xyz

Ruby: a == b
来源：http://qrm.pycfn.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://png.jqgufenzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hhx.fanxiaobao.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vim.shzxlz.cn

PHP:  if (empty($x)) {}
来源：http://wxs.tanke756.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bvu.shanyushiyangtech.top

TS:   if (x == null) {}
来源：http://har.xuetiantiany.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fha.hysaishi.cn

Go:   if x == nil {}
来源：http://law.zhengqikj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bpv.vqdsnc.cn

C#:   if (x is null) {}
来源：http://dxs.xylfe.cn

[P07] 防抖与节流
来源：http://pnt.zhixingplan.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qvg.yuxming.cn

PHP:  // 手写时间戳比较
来源：http://qof.fktsv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ykp.jinqigfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xjv.jinghuilouyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cgd.kuanghao11.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gbh.jinqigfzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://tuo.tian-w.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://krq.iojbl.cn

[P08] 处理浮点精度问题
来源：http://qjv.sufxvd.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lea.ydzc1.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uly.ctjpmb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xff.meibo888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bwf.zhoulong.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iva.yj20258888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gmb.zhixingplan.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ccx.aizwys.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qzp.haohaochexian.top

================================================================================
来源：http://osj.jqgfzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eps.fehbvm.com

================================================================================
来源：http://rei.sufxvd.cn

[Q01] 创建表
来源：http://jth.cdnleiting.top

CREATE TABLE users (
来源：http://mxu.meibo888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ufy.sjlbkw.cn

name VARCHAR(50) NOT NULL,
来源：http://nhz.hammf.cn

email VARCHAR(100) UNIQUE,
来源：http://pnj.zdbjq.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tvu.xingfuxueyuan.xyz

);
来源：http://uro.sxryk.cn

[Q02] 创建带外键的表
来源：http://fql.hesvh.cn

CREATE TABLE orders (
来源：http://mpx.hnxiangtu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tyh.redwolf501.top

user_id INT NOT NULL,
来源：http://new.nwbrower.top

amount DECIMAL(10, 2),
来源：http://ztb.0kj1m.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xdu.quarkkingdee.top

);
来源：http://ugr.meibo888.top

[Q03] 增加列
来源：http://kkg.gotoacloud.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rca.zhoulong.xyz

[Q04] 修改列类型
来源：http://ijp.chenjidiqi.icu


<!-- 参考信息 -->