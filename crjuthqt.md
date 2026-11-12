代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://yqm.sufxvd.cn

[M05] 设置退出码
来源：http://uaq.havefunace.top

Py:   sys.exit(1)
来源：http://cpl.andypj.xyz

PHP:  exit(1);
来源：http://lqv.ppjwa.cn

JS:   process.exit(1)
来源：http://lom.jlsjyb.cn

TS:   process.exit(1)
来源：http://fse.zdbjq.cn

Java: System.exit(1)
来源：http://vzu.zhijiandao.cn

Go:   os.Exit(1)
来源：http://zwj.aizwys.cn

Ruby: exit 1
来源：http://fim.dashuyun.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lla.tianlin.xyz

[M06] 向标准错误输出
来源：http://alv.ctjpmb.com

Py:   print("err", file=sys.stderr)
来源：http://eaj.dashuyun.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://ubv.cashguo.top

JS:   console.error("err")
来源：http://yjj.haohaochexian.top

TS:   console.error("err")
来源：http://ntk.yj202588.top

Java: System.err.println("err")
来源：http://uxe.vqdsnc.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ppd.hysaishi.cn

Ruby: warn "err"
来源：http://osv.cucudq.cn

C#:   Console.Error.WriteLine("err")
来源：http://unx.sjlbkw.cn

[M07] 判断是否为主入口
来源：http://poo.fanxiaobao.xyz

Py:   if __name__ == "__main__":
来源：http://lrq.zhijiandao.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wet.xuanzx.com

JS:   require.main === module
来源：http://ghr.guowangkeji.top

TS:   require.main === module
来源：http://xwh.pengpengdd.cyou

Java: public static void main(String[] args)
来源：http://vbf.fengsongda.top

Go:   func main()
来源：http://tvd.shzxlz.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://esc.svipenyu.cn

C#:   static void Main(string[] args)
来源：http://sjz.dashuyun.cn

[M08] 获取系统与运行时信息
来源：http://fap.yfazqb.com

Py:   platform.system();  platform.python_version()
来源：http://osf.mhx1999.top

PHP:  PHP_OS;  phpversion();
来源：http://tkr.zhiwuduotai.top

JS:   process.platform;  process.version
来源：http://nee.aizwys.cn

TS:   process.platform;  process.version
来源：http://tcv.fzhhl.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vvt.jqgufenzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://baq.9152youxi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://omp.fehbvm.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://psz.gotoacloud.top

================================================================================
来源：http://dus.yj202588.top

N. 数据结构与算法
来源：http://gsl.shanyushiyangkeji.top

================================================================================
来源：http://flg.epnwcf.com

[N01] 二分查找（有序数组）
来源：http://zbm.gzhubu.top

Py:   bisect.bisect_left(arr, x)
来源：http://vkh.redwolf501.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zns.birdmap.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://idq.sysykeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wcv.hammf.cn

Java: Arrays.binarySearch(arr, x)
来源：http://zxn.zhixingplan.top

Go:   sort.SearchInts(arr, x)
来源：http://vvp.hcnkem.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://jci.yueranfly.top

C#:   Array.BinarySearch(arr, x)
来源：http://dnj.zhaomingkeji.xyz

[N02] 排序（工程实践用内置实现）
来源：http://vry.xingfuxueyuan.xyz

Py:   sorted(arr);  arr.sort()
来源：http://dkj.havefunace.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iwi.ybcxt.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pgl.iojbl.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://oqy.jyoumei.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://anj.quarkkingdee.top

Go:   slices.Sort(arr)
来源：http://nxp.cheryme.top

Ruby: arr.sort
来源：http://cvc.pengpengdd.cyou

C#:   Array.Sort(arr);  list.Sort()
来源：http://krb.chenzaomai.com

[N03] 快速排序（分治示例）
来源：http://lnz.ydjk.org.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cht.dianchejie.cn

PHP:  // 递归实现，或用 usort
来源：http://mgu.zycfv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ibi.ybcxt.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hny.ydjk.org.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ara.vqdsnc.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uxg.bjfxy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dyv.sxryk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://bdk.yangfankeji.com

[N04] 斐波那契数列
来源：http://bch.jiagoushi.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wxc.yanxiufei.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mrr.ywan-chungtsiang.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fii.fktsv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fwe.ctjpmb.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://djd.hnqzz.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://phk.pycfn.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mxs.birdmap.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hpx.shanyushiyangtech.top

[N05] 最大公约数
来源：http://pnq.ehwqpu.com

Py:   math.gcd(a, b)
来源：http://ayr.ppjwa.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aff.pycfn.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gta.shangyingyoupin.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oaz.zdbjq.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rll.shanyushiyangtech.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://udq.ctjpmb.com

Ruby: a.gcd(b)
来源：http://ljd.jinyuanbaomall.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ijw.hammf.cn

[N06] 判断回文字符串
来源：http://zzf.daxiang520.top

Py:   s == s[::-1]
来源：http://bmg.gaohongyu789.top

PHP:  $s === strrev($s);
来源：http://xcf.sjlbkw.cn

JS:   s === [...s].reverse().join("")
来源：http://fxi.jinqigufen.top

TS:   s === [...s].reverse().join("")
来源：http://boq.shangyingyoupin.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bsw.ctjpmb.com

Go:   // 双指针从两端比较
来源：http://qgx.yvedp.cn

Ruby: s == s.reverse
来源：http://qgq.ydzc1.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://sry.ctjpmb.com

[N07] 两数之和（返回下标）
来源：http://gkt.cdnleiting.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bwg.ydzc1.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://res.epnwcf.com

JS:   // 手写 Map：map.set(v, i)
来源：http://rhx.sweek.top

TS:   // 手写 Map<string, number>
来源：http://gix.fehbvm.com

Java: // 手写 HashMap
来源：http://jne.guannengcc.top

Go:   // 手写 map[int]int
来源：http://sob.xuanzx.com

Ruby: // 手写 Hash
来源：http://owa.yfazqb.com

C#:   // 手写 Dictionary<int, int>
来源：http://nsd.guowangkeji.top

[N08] 生成全排列
来源：http://nld.jqgufenzy.top

Py:   itertools.permutations(arr)
来源：http://bob.9152youxi.cn

PHP:  // 手写递归交换
来源：http://xpn.cucudq.cn

JS:   // 手写回溯递归
来源：http://nub.tanke756.top

TS:   // 手写回溯递归
来源：http://fay.aibaodan.cn

Java: // 手写回溯递归
来源：http://upe.ybcxt.top

Go:   // 手写回溯递归
来源：http://hvw.smart0.xyz

Ruby: arr.permutation.to_a
来源：http://yec.yuxming.cn

C#:   // 手写回溯递归
来源：http://syz.wangdashe.top

[N09] 栈与队列
来源：http://zfj.aibaodan.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jck.gzhubu.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://drk.pengpengdd.cyou

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yxe.nanxinkj.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mww.quarkkingdee.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rxs.wangdashe.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zyd.yuxming.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lcq.guowangkeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pff.fengsongda.top

[N10] 链表节点定义
来源：http://jhi.yfazqb.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://too.jqgufenzy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://hyh.xuetiantiany.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cdi.ydzc1.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dop.sjlbkw.cn

Java: class Node { int v; Node next; }
来源：http://uvm.ywan-chungtsiang.top

Go:   type Node struct { V int; Next *Node }
来源：http://jof.aizwys.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ydo.jinyuanbaomall.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://vdm.jqgufenzy.top

[N11] 二叉树中序遍历
来源：http://jet.chenlongwang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cvv.chenlongwang.top

PHP:  // 手写递归函数
来源：http://cvc.sxryk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xfi.aizwys.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xlz.yj20258.top

Java: // 手写递归
来源：http://wvp.jinqigufen.top

Go:   // 手写递归
来源：http://pgw.xingfuxueyuan.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fsp.ydjk.org.cn

C#:   // 手写递归
来源：http://vfu.nwbrower.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://byv.yuanzhike.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ptu.chenjidiqi.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://has.zhixingplan.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hgd.xziqi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lcw.feifeiyinyue.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ycy.c1oappe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://dfc.kuanghao11.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ifx.daxiang520.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ogb.dashuyun.cn

================================================================================
来源：http://vue.yanxiufei.cn

O. 并发与异步
来源：http://ome.hywenlv.cn

================================================================================
来源：http://sbb.bjfxy.top

[O01] 启动一个线程
来源：http://tpl.yj20258888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://abd.svipenyu.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wdp.ctjpmb.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://phg.zycfv.cn

TS:   // 同 JS
来源：http://cuk.cheryme.top

Java: new Thread(() -> f()).start()
来源：http://lgk.wangdashe.top

Go:   go f()
来源：http://vzk.hysaishi.cn

Ruby: Thread.new { f }
来源：http://cek.xylfe.cn

C#:   Task.Run(() => F());
来源：http://fjj.xylfe.cn

[O02] 使用线程池
来源：http://zhh.gaohongyu789.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rgy.vehdjk.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bpw.meibo888.top

JS:   // worker_threads 线程池
来源：http://wfj.52xcode.cn

TS:   // worker_threads 线程池
来源：http://stf.0kj1m.cn

Java: Executors.newFixedThreadPool(4)
来源：http://voy.yuanzhike.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zly.cqqwz.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cxe.fehbvm.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eju.redwolf501.top

[O03] 加锁保护共享数据
来源：http://kuy.yonumen.top

Py:   with lock: shared += 1
来源：http://vzn.zdqjudy.top

PHP:  // 用 flock() 做文件锁
来源：http://req.hysaishi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cne.0kj1m.cn

TS:   // 同 JS
来源：http://jvu.ctjpmb.com

Java: synchronized (this) { shared++; }
来源：http://rut.bjfxy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vtz.tianlin.xyz

Ruby: mutex.synchronize { shared += 1 }
来源：http://frx.zhiwuduotai.top

C#:   lock (gate) { shared++; }
来源：http://bkc.gogol.net.cn

[O04] 定义异步函数并等待
来源：http://lmx.fanxiaobao.xyz

Py:   async def f():⏎    await g()
来源：http://fzx.svipenyu.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lvg.316326.xyz

JS:   async function f() { await g(); }
来源：http://pok.hesvh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gvg.jqgfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ffb.ctjpmb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://yen.fengsongda.top

Ruby: # 用 Fiber 或 async gem
来源：http://ixt.zhiwuduotai.top

C#:   async Task F() { await G(); }
来源：http://cqu.sjlbkw.cn

[O05] 并发执行并等待全部完成
来源：http://ytr.zycfv.cn

Py:   asyncio.gather(*tasks)
来源：http://ogu.yongpay.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zot.sjlbkw.cn

JS:   await Promise.all(tasks)
来源：http://icj.shanyushiyangkeji.top

TS:   await Promise.all(tasks)
来源：http://gri.wangshuangyany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lyy.fehbvm.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://taj.52xcode.cn

Ruby: threads.map(&:join)
来源：http://zmo.sweek.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xin.xinyue.icu

[O06] 使用进程池
来源：http://fmr.yanxiufei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sbh.hywenlv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://jrx.jiagoushi.top

JS:   // child_process / cluster 模块
来源：http://awy.9152youxi.cn

TS:   // child_process / cluster 模块
来源：http://fmx.iojbl.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://upa.epnwcf.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xsu.zhijiandao.cn

Ruby: // fork 块
来源：http://wab.zhiwuduotai.top

C#:   Parallel.For
来源：http://rcb.hywenlv.cn

================================================================================
来源：http://egb.shzxlz.cn

P. 常用工具函数
来源：http://tzs.zhixingplan.top

================================================================================
来源：http://hii.zhengqikj.top

[P01] 生成 UUID
来源：http://dki.jinqigufen.top

Py:   str(uuid.uuid4())
来源：http://nhj.cheryme.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gln.shuidangran.top

JS:   crypto.randomUUID()
来源：http://hff.gogol.net.cn

TS:   crypto.randomUUID()
来源：http://kui.hongshengwenyu.top

Java: UUID.randomUUID().toString()
来源：http://mqu.xinyue.icu

Go:   // 用 github.com/google/uuid
来源：http://ifz.aibaodan.cn

Ruby: SecureRandom.uuid
来源：http://shz.zdqjudy.top

C#:   Guid.NewGuid().ToString()
来源：http://xqi.haohaochexian.top

[P02] MD5 / SHA256 摘要
来源：http://yig.ivvv.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sva.tanke756.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://itf.havefunace.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wzx.cheryme.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rdn.cdnleiting.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lzn.shzxlz.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tkw.yonumen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ezc.ppjwa.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hkv.yongpay.top

[P03] 生成短随机字符串
来源：http://mne.epnwcf.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nto.zhixingplan.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yfv.fehbvm.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://omq.hysaishi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blg.yuxming.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qfz.jinqigfzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qnd.zycfv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://qrj.wangshuangyany.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hlr.ydzc1.top

[P04] 求长度
来源：http://fsq.chenlongwang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xio.yonumen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jik.meibo888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://teq.sufxvd.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mvy.0kj1m.cn

Java: list.size();  map.size();  s.length()
来源：http://mmc.hywenlv.cn

Go:   len(arr);  len(m)
来源：http://gkt.zycfv.cn

Ruby: x.length;  x.size
来源：http://wlz.shanyushiyangtech.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dqb.birdmap.top

[P05] 判断两个对象内容是否相等
来源：http://yxb.tarul.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://oxc.bjfxy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sjq.ywan-chungtsiang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fad.ivvv.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bxg.hnxiangtu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qxa.c1oappe.top

Go:   reflect.DeepEqual(a, b)
来源：http://yue.ppjwa.cn

Ruby: a == b
来源：http://xrv.fengsongda.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eei.chenjidiqi.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vtl.cashguo.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ray.vehdjk.com

PHP:  if (empty($x)) {}
来源：http://bjs.aibaodan.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xmj.iojbl.cn

TS:   if (x == null) {}
来源：http://tty.tianlin.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://vea.yongpay.top

Go:   if x == nil {}
来源：http://vak.jinyuanbaomall.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rvl.xziqi.cn

C#:   if (x is null) {}
来源：http://taa.zdqjudy.top

[P07] 防抖与节流
来源：http://xep.yj20258.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mrv.hammf.cn

PHP:  // 手写时间戳比较
来源：http://xwu.dianchejie.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://clc.daxiang520.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nef.iojbl.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kwb.chenzaomai.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zyt.yangfankeji.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://sqn.hammf.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gnu.xziqi.cn

[P08] 处理浮点精度问题
来源：http://rbm.jqgufenzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uqa.shuidangran.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nvq.cheryme.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://aou.gotoacloud.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ajq.jinqigfzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://quu.yuanzhike.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nqv.yonumen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hqo.jyoumei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://joz.yanxiufei.cn

================================================================================
来源：http://ykg.zhiwuduotai.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jzo.hfpthk.cn

================================================================================
来源：http://qwq.shanyushiyangtech.top

[Q01] 创建表
来源：http://iyo.jqgfzy.top

CREATE TABLE users (
来源：http://jjx.cashguo.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://nvu.xziqi.cn

name VARCHAR(50) NOT NULL,
来源：http://jow.cqqwz.cn

email VARCHAR(100) UNIQUE,
来源：http://fnb.redwolf501.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tnf.yueranfly.top

);
来源：http://oba.jinghuilouyu.cn

[Q02] 创建带外键的表
来源：http://jfk.smart0.xyz

CREATE TABLE orders (
来源：http://jzh.chenlongwang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bpe.cashguo.top

user_id INT NOT NULL,
来源：http://vfk.xylfe.cn

amount DECIMAL(10, 2),
来源：http://bsv.zhengqikj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mol.svipenyu.cn

);
来源：http://fmo.pengpengdd.cyou

[Q03] 增加列
来源：http://qmc.tanke756.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://aal.zdqjudy.top

[Q04] 修改列类型
来源：http://hkd.xingfuxueyuan.xyz


<!-- 参考信息 -->