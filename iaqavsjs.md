代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://kjm.tianlin.xyz

[M05] 设置退出码
来源：http://gmx.feifeiyinyue.top

Py:   sys.exit(1)
来源：http://tvq.hesvh.cn

PHP:  exit(1);
来源：http://jwv.fktsv.cn

JS:   process.exit(1)
来源：http://hjd.shzxlz.cn

TS:   process.exit(1)
来源：http://zkl.jyoumei.cn

Java: System.exit(1)
来源：http://nkl.yongpay.top

Go:   os.Exit(1)
来源：http://wey.feifeiyinyue.top

Ruby: exit 1
来源：http://mly.dashuyun.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://eau.uphjek.com

[M06] 向标准错误输出
来源：http://pmj.andypj.xyz

Py:   print("err", file=sys.stderr)
来源：http://wzg.haohaochexian.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xlw.yuxming.cn

JS:   console.error("err")
来源：http://evq.zdqjudy.top

TS:   console.error("err")
来源：http://fqe.vqdsnc.cn

Java: System.err.println("err")
来源：http://prr.shzxlz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pdc.9152youxi.cn

Ruby: warn "err"
来源：http://igz.wangdashe.top

C#:   Console.Error.WriteLine("err")
来源：http://sxs.yonumen.top

[M07] 判断是否为主入口
来源：http://poh.jlsjyb.cn

Py:   if __name__ == "__main__":
来源：http://zro.52xcode.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xcp.meibo888.top

JS:   require.main === module
来源：http://wim.xziqi.cn

TS:   require.main === module
来源：http://cgy.smart0.xyz

Java: public static void main(String[] args)
来源：http://ytv.aibaodan.cn

Go:   func main()
来源：http://rbm.xziqi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kmu.sysykeji.top

C#:   static void Main(string[] args)
来源：http://hoe.ctjpmb.com

[M08] 获取系统与运行时信息
来源：http://pwz.jlsjyb.cn

Py:   platform.system();  platform.python_version()
来源：http://bwa.fktsv.cn

PHP:  PHP_OS;  phpversion();
来源：http://maa.fzhhl.top

JS:   process.platform;  process.version
来源：http://dqf.smart0.xyz

TS:   process.platform;  process.version
来源：http://axt.jinghuilouyu.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xbf.sufxvd.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pcm.shanyushiyangtech.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ixo.52xcode.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bjb.chenjidiqi.icu

================================================================================
来源：http://bzc.guannengcc.top

N. 数据结构与算法
来源：http://umn.chenzaomai.com

================================================================================
来源：http://rhe.shangyingyoupin.top

[N01] 二分查找（有序数组）
来源：http://eme.jinqigfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://mix.xingfuxueyuan.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nwi.9152youxi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kfs.pengpengdd.cyou

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jpd.ivvv.top

Java: Arrays.binarySearch(arr, x)
来源：http://qpj.yfazqb.com

Go:   sort.SearchInts(arr, x)
来源：http://bkl.mhx1999.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ygy.zhaomingkeji.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://eyj.shzxlz.cn

[N02] 排序（工程实践用内置实现）
来源：http://gec.shuidangran.top

Py:   sorted(arr);  arr.sort()
来源：http://jsz.sxryk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xtk.yangfankeji.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://flv.jqgfzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fsj.yj20258888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mwc.jinghuilouyu.cn

Go:   slices.Sort(arr)
来源：http://nxb.snrcjt.cn

Ruby: arr.sort
来源：http://wfw.hesvh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://uxq.shuidangran.top

[N03] 快速排序（分治示例）
来源：http://xpe.mhx1999.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kok.gogol.net.cn

PHP:  // 递归实现，或用 usort
来源：http://bom.yfazqb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oas.ctjpmb.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lvx.yangfankeji.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gcx.hesvh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hdx.sxryk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tfl.epnwcf.com

C#:   // 手写递归，或 Array.Sort
来源：http://znv.yangfankeji.com

[N04] 斐波那契数列
来源：http://xov.hammf.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yzg.hywenlv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nrb.quarkkingdee.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://trv.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vyg.kuanghao11.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://szo.sweek.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iip.xuetiantiany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rdj.bbcook.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zbi.zhijiandao.cn

[N05] 最大公约数
来源：http://rzs.zhixingplan.top

Py:   math.gcd(a, b)
来源：http://jkt.cdnleiting.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mim.yj202588.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zqf.gaohongyu789.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://igd.zhaomingkeji.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hed.xingfuxueyuan.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://llc.cashguo.top

Ruby: a.gcd(b)
来源：http://xzn.jqgfzy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gbt.fehbvm.com

[N06] 判断回文字符串
来源：http://htg.gogol.net.cn

Py:   s == s[::-1]
来源：http://ezm.zhixingplan.top

PHP:  $s === strrev($s);
来源：http://shu.fktsv.cn

JS:   s === [...s].reverse().join("")
来源：http://zey.kuanghao11.cn

TS:   s === [...s].reverse().join("")
来源：http://qhn.shanyushiyangtech.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fbv.fanxiaobao.xyz

Go:   // 双指针从两端比较
来源：http://gno.fktsv.cn

Ruby: s == s.reverse
来源：http://qaz.yj202588.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://qsj.tanke756.top

[N07] 两数之和（返回下标）
来源：http://ymv.316326.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://crq.mhx1999.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ril.iojbl.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zlg.hysaishi.cn

TS:   // 手写 Map<string, number>
来源：http://mey.gotoacloud.top

Java: // 手写 HashMap
来源：http://yuf.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://dfo.zhengqikj.top

Ruby: // 手写 Hash
来源：http://bvr.sjlbkw.cn

C#:   // 手写 Dictionary<int, int>
来源：http://swl.xinyue.icu

[N08] 生成全排列
来源：http://axp.aizwys.cn

Py:   itertools.permutations(arr)
来源：http://zwr.316326.xyz

PHP:  // 手写递归交换
来源：http://eio.jqgfzy.top

JS:   // 手写回溯递归
来源：http://ydn.fengsongda.top

TS:   // 手写回溯递归
来源：http://hva.316326.xyz

Java: // 手写回溯递归
来源：http://dfz.gzhubu.top

Go:   // 手写回溯递归
来源：http://juy.xziqi.cn

Ruby: arr.permutation.to_a
来源：http://wds.zhongyouzk.top

C#:   // 手写回溯递归
来源：http://zvf.pycfn.com

[N09] 栈与队列
来源：http://nll.cqqwz.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://xjg.hnxiangtu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mcr.cashguo.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mjq.cheryme.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mko.fktsv.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ayp.hysaishi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xez.hysaishi.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tkv.smart0.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://cjw.zhengqikj.top

[N10] 链表节点定义
来源：http://smg.chenjidiqi.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://sug.zhoulong.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://pne.ybcxt.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xxp.xinyue.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gic.fktsv.cn

Java: class Node { int v; Node next; }
来源：http://goz.sweek.top

Go:   type Node struct { V int; Next *Node }
来源：http://tht.ydzc1.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tsa.havefunace.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dxd.tianlin.xyz

[N11] 二叉树中序遍历
来源：http://blc.hnxiangtu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://asr.cheryme.top

PHP:  // 手写递归函数
来源：http://ylw.yanxiufei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jzm.gotoacloud.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lao.cheryme.top

Java: // 手写递归
来源：http://xco.cqqwz.cn

Go:   // 手写递归
来源：http://mir.vqdsnc.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://imo.fengsongda.top

C#:   // 手写递归
来源：http://xdt.yonumen.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://gco.hywenlv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wmf.nanxuanxn.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dcv.quarkkingdee.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wbj.yfazqb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hfe.cashguo.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mau.cheryme.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nye.tian-w.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jzl.xziqi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lau.shanyushiyangtech.top

================================================================================
来源：http://xkd.pycfn.com

O. 并发与异步
来源：http://vql.tianlin.xyz

================================================================================
来源：http://rdk.xuetiantiany.cn

[O01] 启动一个线程
来源：http://esf.nanxuanxn.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://thc.hnxiangtu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ayf.chenzaomai.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://apv.shzxlz.cn

TS:   // 同 JS
来源：http://iso.52xcode.cn

Java: new Thread(() -> f()).start()
来源：http://zik.fengsongda.top

Go:   go f()
来源：http://oev.jyoumei.cn

Ruby: Thread.new { f }
来源：http://lez.yangfankeji.com

C#:   Task.Run(() => F());
来源：http://pwp.snrcjt.cn

[O02] 使用线程池
来源：http://zie.havefunace.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://lcy.bjfxy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rbd.jyoumei.cn

JS:   // worker_threads 线程池
来源：http://ncy.shanyushiyangkeji.top

TS:   // worker_threads 线程池
来源：http://iwk.kuanghao11.cn

Java: Executors.newFixedThreadPool(4)
来源：http://nnh.ctjpmb.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fos.mhx1999.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://vos.yonumen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nwg.guannengcc.top

[O03] 加锁保护共享数据
来源：http://wzz.yj202588.top

Py:   with lock: shared += 1
来源：http://caa.iojbl.cn

PHP:  // 用 flock() 做文件锁
来源：http://ufp.fengsongda.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://eqh.sysykeji.top

TS:   // 同 JS
来源：http://dnt.guannengcc.top

Java: synchronized (this) { shared++; }
来源：http://sny.xuetiantiany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mkm.aizwys.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qsb.zhoulong.xyz

C#:   lock (gate) { shared++; }
来源：http://tdr.sweek.top

[O04] 定义异步函数并等待
来源：http://dwh.zhoulong.xyz

Py:   async def f():⏎    await g()
来源：http://ick.vqdsnc.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rje.yj20258.top

JS:   async function f() { await g(); }
来源：http://kvk.xingfuxueyuan.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://aqz.sufxvd.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jdh.yueranfly.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://izr.zycfv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://klj.xuetiantiany.cn

C#:   async Task F() { await G(); }
来源：http://zyb.fanxiaobao.xyz

[O05] 并发执行并等待全部完成
来源：http://yxh.snrcjt.cn

Py:   asyncio.gather(*tasks)
来源：http://mvx.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iib.fehbvm.com

JS:   await Promise.all(tasks)
来源：http://eia.birdmap.top

TS:   await Promise.all(tasks)
来源：http://sbt.sxryk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vov.cqqwz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jag.hfpthk.cn

Ruby: threads.map(&:join)
来源：http://zxn.jiagoushi.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ihb.zhongyouzk.top

[O06] 使用进程池
来源：http://ase.316326.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vyr.birdmap.top

PHP:  // pcntl_fork 或多进程队列
来源：http://itk.quarkkingdee.top

JS:   // child_process / cluster 模块
来源：http://lkk.jianghu66.top

TS:   // child_process / cluster 模块
来源：http://ono.hnxiangtu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kjx.yuxming.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://btp.52xcode.cn

Ruby: // fork 块
来源：http://hfd.vqdsnc.cn

C#:   Parallel.For
来源：http://jdg.sufxvd.cn

================================================================================
来源：http://rsp.gzhubu.top

P. 常用工具函数
来源：http://rfs.pycfn.com

================================================================================
来源：http://uci.svipenyu.cn

[P01] 生成 UUID
来源：http://yvg.aibaodan.cn

Py:   str(uuid.uuid4())
来源：http://svp.yonumen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oih.kuanghao11.cn

JS:   crypto.randomUUID()
来源：http://iby.sufxvd.cn

TS:   crypto.randomUUID()
来源：http://osi.zhongyouzk.top

Java: UUID.randomUUID().toString()
来源：http://tru.wangdashe.top

Go:   // 用 github.com/google/uuid
来源：http://mcc.yj202588.top

Ruby: SecureRandom.uuid
来源：http://mmf.gotoacloud.top

C#:   Guid.NewGuid().ToString()
来源：http://rkk.chenlongwang.top

[P02] MD5 / SHA256 摘要
来源：http://nfw.redwolf501.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sll.nanxinkj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dds.redwolf501.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qkw.hcnkem.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wew.mhx1999.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hij.xylfe.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://err.zhijiandao.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kvc.zdqjudy.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bwg.shanyushiyangkeji.top

[P03] 生成短随机字符串
来源：http://dvq.sufxvd.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rmz.jqgufenzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rqp.0kj1m.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uki.hnqzz.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zfh.mhx1999.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wzn.gotoacloud.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cjj.jlsjyb.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jyi.shuidangran.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rmf.tarul.cn

[P04] 求长度
来源：http://xfh.hcnkem.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gyc.jianghu66.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ucp.ydzc1.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oql.ybcxt.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wpi.zhixingplan.top

Java: list.size();  map.size();  s.length()
来源：http://cgi.guowangkeji.top

Go:   len(arr);  len(m)
来源：http://yup.havefunace.top

Ruby: x.length;  x.size
来源：http://knw.shangyingyoupin.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dvn.hywenlv.cn

[P05] 判断两个对象内容是否相等
来源：http://rwr.feifeiyinyue.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://dua.tian-w.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yzf.fzhhl.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sjv.zhengqikj.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gky.hcnkem.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://eep.cdnleiting.top

Go:   reflect.DeepEqual(a, b)
来源：http://pia.sxryk.cn

Ruby: a == b
来源：http://uyf.hongshengwenyu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mcm.ywan-chungtsiang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uqa.fktsv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oih.gaohongyu789.top

PHP:  if (empty($x)) {}
来源：http://kuv.ybcxt.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://too.ehwqpu.com

TS:   if (x == null) {}
来源：http://gvv.zycfv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uyt.nwbrower.top

Go:   if x == nil {}
来源：http://dvk.guannengcc.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://adj.ydzc1.top

C#:   if (x is null) {}
来源：http://iux.gogol.net.cn

[P07] 防抖与节流
来源：http://nkc.vehdjk.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pys.mhx1999.top

PHP:  // 手写时间戳比较
来源：http://znb.yanxiufei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dew.ppjwa.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://evw.tanke756.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kkj.tianlin.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rle.gaohongyu789.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rvk.zycfv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://abp.chenjidiqi.icu

[P08] 处理浮点精度问题
来源：http://tlg.chenzaomai.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://why.zhongyouzk.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ikf.9152youxi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hqd.nwbrower.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ivj.vqdsnc.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fnj.iojbl.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ntm.zycfv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://axk.chenlongwang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://htu.zhaomingkeji.xyz

================================================================================
来源：http://sck.wangdashe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fkd.yj202588.top

================================================================================
来源：http://pum.cucudq.cn

[Q01] 创建表
来源：http://zex.vehdjk.com

CREATE TABLE users (
来源：http://ahk.wangshuangyany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oem.ywan-chungtsiang.top

name VARCHAR(50) NOT NULL,
来源：http://aeh.gzhubu.top

email VARCHAR(100) UNIQUE,
来源：http://vxt.zdqjudy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hqn.c1oappe.top

);
来源：http://eqc.hfpthk.cn

[Q02] 创建带外键的表
来源：http://btt.zhongyouzk.top

CREATE TABLE orders (
来源：http://lph.jinqigufen.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wac.zhixingplan.top

user_id INT NOT NULL,
来源：http://vqh.ehwqpu.com

amount DECIMAL(10, 2),
来源：http://ljt.tianlin.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://aix.jqgufenzy.top

);
来源：http://kiy.jqgfzy.top

[Q03] 增加列
来源：http://tss.zhiwuduotai.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gcu.andypj.xyz

[Q04] 修改列类型
来源：http://dan.zhijiandao.cn


<!-- 参考信息 -->