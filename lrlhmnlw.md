代发 wailian999

JS:   process.exit(1)
来源：http://spn.zhaomingkeji.xyz

TS:   process.exit(1)
来源：http://uux.vqdsnc.cn

Java: System.exit(1)
来源：http://uht.hnqzz.top

Go:   os.Exit(1)
来源：http://fej.zhixingplan.top

Ruby: exit 1
来源：http://qfx.zdqjudy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pin.zhengqikj.top

[M06] 向标准错误输出
来源：http://apn.shuidangran.top

Py:   print("err", file=sys.stderr)
来源：http://ftr.bjfxy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://eeo.cqqwz.cn

JS:   console.error("err")
来源：http://asc.zhoulong.xyz

TS:   console.error("err")
来源：http://ard.sweek.top

Java: System.err.println("err")
来源：http://nvz.nanxinkj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://btv.gogol.net.cn

Ruby: warn "err"
来源：http://yik.tarul.cn

C#:   Console.Error.WriteLine("err")
来源：http://jhr.zhoulong.xyz

[M07] 判断是否为主入口
来源：http://sny.shangyingyoupin.top

Py:   if __name__ == "__main__":
来源：http://dow.iojbl.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fgp.0kj1m.cn

JS:   require.main === module
来源：http://jam.zhiwuduotai.top

TS:   require.main === module
来源：http://cbk.guannengcc.top

Java: public static void main(String[] args)
来源：http://zde.vehdjk.com

Go:   func main()
来源：http://cnc.sysykeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mni.svipenyu.cn

C#:   static void Main(string[] args)
来源：http://jiz.zdqjudy.top

[M08] 获取系统与运行时信息
来源：http://ocs.zdqjudy.top

Py:   platform.system();  platform.python_version()
来源：http://mkv.hcnkem.com

PHP:  PHP_OS;  phpversion();
来源：http://kcd.cucudq.cn

JS:   process.platform;  process.version
来源：http://ewu.shangyingyoupin.top

TS:   process.platform;  process.version
来源：http://fku.fanxiaobao.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ndw.svipenyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://pxv.vehdjk.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://bqo.cucudq.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://cwr.havefunace.top

================================================================================
来源：http://exz.fehbvm.com

N. 数据结构与算法
来源：http://zpx.wangshuangyany.cn

================================================================================
来源：http://qik.nanxinkj.top

[N01] 二分查找（有序数组）
来源：http://qep.ydjk.org.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sjj.pengpengdd.cyou

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://uga.hongshengwenyu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hpw.yonumen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fpm.hnqzz.top

Java: Arrays.binarySearch(arr, x)
来源：http://abj.ydjk.org.cn

Go:   sort.SearchInts(arr, x)
来源：http://rhh.xuanzx.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://psq.iojbl.cn

C#:   Array.BinarySearch(arr, x)
来源：http://phe.fzhhl.top

[N02] 排序（工程实践用内置实现）
来源：http://wsk.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://cfy.tianlin.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mcn.redwolf501.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vgu.cqqwz.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mtf.pengpengdd.cyou

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ity.zhoulong.xyz

Go:   slices.Sort(arr)
来源：http://hgp.ehwqpu.com

Ruby: arr.sort
来源：http://mcg.zhiwuduotai.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pbz.quarkkingdee.top

[N03] 快速排序（分治示例）
来源：http://rcg.vehdjk.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rvl.dianchejie.cn

PHP:  // 递归实现，或用 usort
来源：http://rrm.jyoumei.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gjo.tianlin.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mia.yueranfly.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yrv.chenjidiqi.icu

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://urg.hcnkem.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xkr.9152youxi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lau.yj202588.top

[N04] 斐波那契数列
来源：http://zro.hnxiangtu.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hub.andypj.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fuq.yj20258.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vqg.snrcjt.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ase.hysaishi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rxh.hywenlv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://plg.zhoulong.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://nci.xuetiantiany.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://iac.redwolf501.top

[N05] 最大公约数
来源：http://ljm.pengpengdd.cyou

Py:   math.gcd(a, b)
来源：http://amp.shanyushiyangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dnd.yonumen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uvm.0kj1m.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zyg.uphjek.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sxe.fktsv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yiq.yuanzhike.top

Ruby: a.gcd(b)
来源：http://kjj.svipenyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xfs.hesvh.cn

[N06] 判断回文字符串
来源：http://avz.nanxinkj.top

Py:   s == s[::-1]
来源：http://gvp.zhoulong.xyz

PHP:  $s === strrev($s);
来源：http://rkq.cucudq.cn

JS:   s === [...s].reverse().join("")
来源：http://nfa.yongpay.top

TS:   s === [...s].reverse().join("")
来源：http://dcv.nanxuanxn.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zci.jianghu66.top

Go:   // 双指针从两端比较
来源：http://axw.sxryk.cn

Ruby: s == s.reverse
来源：http://gds.daxiang520.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://nlc.xingfuxueyuan.xyz

[N07] 两数之和（返回下标）
来源：http://ftp.dashuyun.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sya.vehdjk.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://etk.316326.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://wst.uphjek.com

TS:   // 手写 Map<string, number>
来源：http://hdq.smart0.xyz

Java: // 手写 HashMap
来源：http://ill.cheryme.top

Go:   // 手写 map[int]int
来源：http://wnu.nanxuanxn.top

Ruby: // 手写 Hash
来源：http://myb.mhx1999.top

C#:   // 手写 Dictionary<int, int>
来源：http://ywn.redwolf501.top

[N08] 生成全排列
来源：http://skn.svipenyu.cn

Py:   itertools.permutations(arr)
来源：http://qbu.hnqzz.top

PHP:  // 手写递归交换
来源：http://nrz.nanxinkj.top

JS:   // 手写回溯递归
来源：http://nay.zhijiandao.cn

TS:   // 手写回溯递归
来源：http://ewk.zdbjq.cn

Java: // 手写回溯递归
来源：http://qzs.daria6918.cn

Go:   // 手写回溯递归
来源：http://pmg.daxiang520.top

Ruby: arr.permutation.to_a
来源：http://izq.cheryme.top

C#:   // 手写回溯递归
来源：http://uai.jinyuanbaomall.cn

[N09] 栈与队列
来源：http://hpl.zhengqikj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://dfu.jinyuanbaomall.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://tlu.uphjek.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mpc.c1oappe.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ivw.tanke756.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cvt.xuanzx.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ala.fengsongda.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://fle.wangdashe.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vem.bjfxy.top

[N10] 链表节点定义
来源：http://zor.ppjwa.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ajy.jyoumei.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://qww.cucudq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://upm.redwolf501.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://deb.jinyuanbaomall.cn

Java: class Node { int v; Node next; }
来源：http://uyl.0kj1m.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qar.zycfv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://fip.yuanzhike.top

C#:   class Node { public int V; public Node? Next; }
来源：http://veu.wangdashe.top

[N11] 二叉树中序遍历
来源：http://rzx.havefunace.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://sow.316326.xyz

PHP:  // 手写递归函数
来源：http://qkh.nanxuanxn.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xdm.pengpengdd.cyou

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://upf.c1oappe.top

Java: // 手写递归
来源：http://jth.sjlbkw.cn

Go:   // 手写递归
来源：http://rru.quarkkingdee.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ecf.yangfankeji.com

C#:   // 手写递归
来源：http://luu.gotoacloud.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cwo.kuanghao11.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://bll.yanxiufei.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vlz.hywenlv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hte.zdbjq.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sqp.pengpengdd.cyou

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ujd.yuxming.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fne.9152youxi.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qhc.pycfn.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lea.fzhhl.top

================================================================================
来源：http://yxb.fzhhl.top

O. 并发与异步
来源：http://svr.ehwqpu.com

================================================================================
来源：http://kja.shzxlz.cn

[O01] 启动一个线程
来源：http://dno.ppjwa.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hgx.gotoacloud.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vng.aibaodan.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lwt.gaohongyu789.top

TS:   // 同 JS
来源：http://ize.smart0.xyz

Java: new Thread(() -> f()).start()
来源：http://oic.0kj1m.cn

Go:   go f()
来源：http://wpb.andypj.xyz

Ruby: Thread.new { f }
来源：http://vut.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://bak.shanyushiyangkeji.top

[O02] 使用线程池
来源：http://yua.hongshengwenyu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tqw.yj20258.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://klt.hysaishi.cn

JS:   // worker_threads 线程池
来源：http://ldi.yangfankeji.com

TS:   // worker_threads 线程池
来源：http://ogz.ehwqpu.com

Java: Executors.newFixedThreadPool(4)
来源：http://wwn.hfpthk.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rwp.gaohongyu789.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://feh.316326.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://heo.yj20258888.top

[O03] 加锁保护共享数据
来源：http://kcy.chenjidiqi.icu

Py:   with lock: shared += 1
来源：http://sbr.hammf.cn

PHP:  // 用 flock() 做文件锁
来源：http://odn.jiagoushi.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qkw.zdqjudy.top

TS:   // 同 JS
来源：http://wwb.sweek.top

Java: synchronized (this) { shared++; }
来源：http://jsj.fengsongda.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qoi.hnqzz.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bfq.chenzaomai.com

C#:   lock (gate) { shared++; }
来源：http://nqt.hysaishi.cn

[O04] 定义异步函数并等待
来源：http://zuc.zhoulong.xyz

Py:   async def f():⏎    await g()
来源：http://psy.yj20258888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wto.jqgufenzy.top

JS:   async function f() { await g(); }
来源：http://uhk.tanke756.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zps.yvedp.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://uqr.cashguo.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://opa.shanyushiyangtech.top

Ruby: # 用 Fiber 或 async gem
来源：http://sob.iojbl.cn

C#:   async Task F() { await G(); }
来源：http://otg.zhaomingkeji.xyz

[O05] 并发执行并等待全部完成
来源：http://ktq.fktsv.cn

Py:   asyncio.gather(*tasks)
来源：http://bjm.hcnkem.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lfb.xuanzx.com

JS:   await Promise.all(tasks)
来源：http://whg.xziqi.cn

TS:   await Promise.all(tasks)
来源：http://xty.gotoacloud.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ulo.mhx1999.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gpc.fengsongda.top

Ruby: threads.map(&:join)
来源：http://mga.jlsjyb.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://wfy.vehdjk.com

[O06] 使用进程池
来源：http://bid.xuetiantiany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jst.zhaomingkeji.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://ehg.mhx1999.top

JS:   // child_process / cluster 模块
来源：http://tts.chenzaomai.com

TS:   // child_process / cluster 模块
来源：http://sqd.jianghu66.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ibl.nanxuanxn.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cts.sysykeji.top

Ruby: // fork 块
来源：http://jqa.nanxinkj.top

C#:   Parallel.For
来源：http://grj.chenzaomai.com

================================================================================
来源：http://rxp.wangshuangyany.cn

P. 常用工具函数
来源：http://jnj.hnxiangtu.top

================================================================================
来源：http://bil.kuanghao11.cn

[P01] 生成 UUID
来源：http://jpl.zhoulong.xyz

Py:   str(uuid.uuid4())
来源：http://das.zdqjudy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ihn.shangyingyoupin.top

JS:   crypto.randomUUID()
来源：http://koq.snrcjt.cn

TS:   crypto.randomUUID()
来源：http://cgq.iojbl.cn

Java: UUID.randomUUID().toString()
来源：http://uup.cashguo.top

Go:   // 用 github.com/google/uuid
来源：http://epq.fanxiaobao.xyz

Ruby: SecureRandom.uuid
来源：http://nkl.yueranfly.top

C#:   Guid.NewGuid().ToString()
来源：http://ewx.cucudq.cn

[P02] MD5 / SHA256 摘要
来源：http://uyo.ydjk.org.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tlb.yongpay.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ntk.sxryk.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kxi.fengsongda.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xrw.shangyingyoupin.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dlm.yj20258888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zdm.sjlbkw.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mwp.wangshuangyany.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bql.jinghuilouyu.cn

[P03] 生成短随机字符串
来源：http://vcm.feifeiyinyue.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jaf.gogol.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dcn.zdqjudy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://goc.haohaochexian.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ury.jianghu66.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sli.pycfn.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qso.316326.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://tsg.yanxiufei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rbs.zhixingplan.top

[P04] 求长度
来源：http://upb.yonumen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rht.birdmap.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yyf.andypj.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bet.ehwqpu.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://klp.uphjek.com

Java: list.size();  map.size();  s.length()
来源：http://wgd.zdqjudy.top

Go:   len(arr);  len(m)
来源：http://ynf.ivvv.top

Ruby: x.length;  x.size
来源：http://hgs.sjlbkw.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ufg.yuxming.cn

[P05] 判断两个对象内容是否相等
来源：http://jyj.uphjek.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://moq.birdmap.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://chb.hnqzz.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://znh.yfazqb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qwr.hywenlv.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cfd.yongpay.top

Go:   reflect.DeepEqual(a, b)
来源：http://tua.nanxinkj.top

Ruby: a == b
来源：http://pta.xuanzx.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eyg.smart0.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kcz.zdbjq.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nzl.chenzaomai.com

PHP:  if (empty($x)) {}
来源：http://jrv.quarkkingdee.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://kld.wangdashe.top

TS:   if (x == null) {}
来源：http://ctg.yuxming.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qcu.shangyingyoupin.top

Go:   if x == nil {}
来源：http://zgv.tarul.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hzu.shangyingyoupin.top

C#:   if (x is null) {}
来源：http://oli.316326.xyz

[P07] 防抖与节流
来源：http://hlh.0kj1m.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yol.shzxlz.cn

PHP:  // 手写时间戳比较
来源：http://eku.zhaomingkeji.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://efb.hfpthk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fko.gogol.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aep.chenzaomai.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://weg.ydjk.org.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://qeq.shangyingyoupin.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ymt.zhengqikj.top

[P08] 处理浮点精度问题
来源：http://bct.ehwqpu.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ppn.fzhhl.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pet.jinqigfzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jko.pycfn.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lsm.zhongyouzk.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://frj.gotoacloud.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fbm.cqqwz.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xne.yueranfly.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gtw.yj202588.top

================================================================================
来源：http://rhl.gzhubu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zrn.aizwys.cn

================================================================================
来源：http://jie.xuanzx.com

[Q01] 创建表
来源：http://rwl.tarul.cn

CREATE TABLE users (
来源：http://cqo.yongpay.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bwp.hywenlv.cn

name VARCHAR(50) NOT NULL,
来源：http://hvc.pycfn.com

email VARCHAR(100) UNIQUE,
来源：http://pkr.uphjek.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://syo.guannengcc.top

);
来源：http://hpc.hnqzz.top

[Q02] 创建带外键的表
来源：http://gjx.cucudq.cn

CREATE TABLE orders (
来源：http://jvu.fanxiaobao.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pyd.zhengqikj.top

user_id INT NOT NULL,
来源：http://igh.daria6918.cn

amount DECIMAL(10, 2),
来源：http://wbt.zhongyouzk.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zmv.ehwqpu.com

);
来源：http://pqb.chenzaomai.com

[Q03] 增加列
来源：http://mcg.xingfuxueyuan.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rpg.epnwcf.com

[Q04] 修改列类型
来源：http://qbq.kuanghao11.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dzv.zdbjq.cn

[Q05] 重命名列
来源：http://bej.cqqwz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uro.yueranfly.top

[Q06] 删除列
来源：http://tlj.gotoacloud.top


<!-- 参考信息 -->