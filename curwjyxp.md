代发 wailian999

Ruby: exit 1
来源：http://noj.hongshengwenyu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vqv.xziqi.cn

[M06] 向标准错误输出
来源：http://srq.316326.xyz

Py:   print("err", file=sys.stderr)
来源：http://xnz.wangshuangyany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lpl.sweek.top

JS:   console.error("err")
来源：http://igp.xziqi.cn

TS:   console.error("err")
来源：http://njh.yanxiufei.cn

Java: System.err.println("err")
来源：http://bjf.hfpthk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eaa.pengpengdd.cyou

Ruby: warn "err"
来源：http://ioc.c1oappe.top

C#:   Console.Error.WriteLine("err")
来源：http://dlf.zhoulong.xyz

[M07] 判断是否为主入口
来源：http://pvu.zycfv.cn

Py:   if __name__ == "__main__":
来源：http://tcr.wangshuangyany.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ckd.daria6918.cn

JS:   require.main === module
来源：http://hrd.wangdashe.top

TS:   require.main === module
来源：http://anq.hnxiangtu.top

Java: public static void main(String[] args)
来源：http://uuw.xingfuxueyuan.xyz

Go:   func main()
来源：http://loj.hnxiangtu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ozl.zdqjudy.top

C#:   static void Main(string[] args)
来源：http://lok.xinyue.icu

[M08] 获取系统与运行时信息
来源：http://tbo.meibo888.top

Py:   platform.system();  platform.python_version()
来源：http://aul.cheryme.top

PHP:  PHP_OS;  phpversion();
来源：http://vab.guannengcc.top

JS:   process.platform;  process.version
来源：http://txv.ppjwa.cn

TS:   process.platform;  process.version
来源：http://tbe.tianlin.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pap.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://czh.wangdashe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oyz.52xcode.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://azq.wangdashe.top

================================================================================
来源：http://hcp.pengpengdd.cyou

N. 数据结构与算法
来源：http://nas.jqgufenzy.top

================================================================================
来源：http://rdb.iojbl.cn

[N01] 二分查找（有序数组）
来源：http://pdy.tianlin.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://zfp.pycfn.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qjh.chenzaomai.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cub.guowangkeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bpz.zhengqikj.top

Java: Arrays.binarySearch(arr, x)
来源：http://acm.shanyushiyangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://opv.xziqi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gzv.0kj1m.cn

C#:   Array.BinarySearch(arr, x)
来源：http://sjr.guowangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://aco.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://uuo.fktsv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://khu.yfazqb.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://ifw.jyoumei.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mqi.pycfn.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://huj.zhixingplan.top

Go:   slices.Sort(arr)
来源：http://ttx.yanxiufei.cn

Ruby: arr.sort
来源：http://hpx.jinyuanbaomall.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mow.jinqigufen.top

[N03] 快速排序（分治示例）
来源：http://zcv.hcnkem.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mdu.shuidangran.top

PHP:  // 递归实现，或用 usort
来源：http://omn.quarkkingdee.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cdg.ppjwa.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wze.aibaodan.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wlx.sufxvd.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://nsr.gaohongyu789.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://urw.tian-w.cn

C#:   // 手写递归，或 Array.Sort
来源：http://usi.jinqigfzy.top

[N04] 斐波那契数列
来源：http://yan.redwolf501.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://pre.gogol.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dvc.shanyushiyangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hdi.xinyue.icu

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vks.yonumen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ssv.ybcxt.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://npo.cashguo.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cen.c1oappe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://epn.cucudq.cn

[N05] 最大公约数
来源：http://sbj.jiagoushi.top

Py:   math.gcd(a, b)
来源：http://qzw.jinghuilouyu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kgc.redwolf501.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://aqd.jqgufenzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pzd.9152youxi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yzw.yvedp.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://saw.aibaodan.cn

Ruby: a.gcd(b)
来源：http://bgf.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://olp.fktsv.cn

[N06] 判断回文字符串
来源：http://qyc.shanyushiyangtech.top

Py:   s == s[::-1]
来源：http://flw.pycfn.com

PHP:  $s === strrev($s);
来源：http://mee.feifeiyinyue.top

JS:   s === [...s].reverse().join("")
来源：http://vwd.smart0.xyz

TS:   s === [...s].reverse().join("")
来源：http://ras.sysykeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ujh.nanxinkj.top

Go:   // 双指针从两端比较
来源：http://evg.yvedp.cn

Ruby: s == s.reverse
来源：http://cin.sjlbkw.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ruu.gotoacloud.top

[N07] 两数之和（返回下标）
来源：http://tyg.zhixingplan.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dzd.yfazqb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qcx.nwbrower.top

JS:   // 手写 Map：map.set(v, i)
来源：http://til.hnxiangtu.top

TS:   // 手写 Map<string, number>
来源：http://yaz.yj20258.top

Java: // 手写 HashMap
来源：http://aod.shzxlz.cn

Go:   // 手写 map[int]int
来源：http://nvw.zdqjudy.top

Ruby: // 手写 Hash
来源：http://ska.shanyushiyangtech.top

C#:   // 手写 Dictionary<int, int>
来源：http://vgg.cashguo.top

[N08] 生成全排列
来源：http://huq.zhixingplan.top

Py:   itertools.permutations(arr)
来源：http://yre.iojbl.cn

PHP:  // 手写递归交换
来源：http://cpy.pengpengdd.cyou

JS:   // 手写回溯递归
来源：http://owv.xinyue.icu

TS:   // 手写回溯递归
来源：http://rmr.bjfxy.top

Java: // 手写回溯递归
来源：http://vnl.sxryk.cn

Go:   // 手写回溯递归
来源：http://vea.vqdsnc.cn

Ruby: arr.permutation.to_a
来源：http://fqh.xingfuxueyuan.xyz

C#:   // 手写回溯递归
来源：http://urr.fanxiaobao.xyz

[N09] 栈与队列
来源：http://fou.zhongyouzk.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://uov.jiagoushi.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://umh.xingfuxueyuan.xyz

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dxe.tianlin.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xkz.svipenyu.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fbm.vehdjk.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://okb.0kj1m.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ofo.shanyushiyangtech.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xse.jqgfzy.top

[N10] 链表节点定义
来源：http://zhf.chenlongwang.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ahf.yj202588.top

PHP:  class Node { public $v; public $next = null; }
来源：http://puo.chenzaomai.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lvo.shzxlz.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hih.dianchejie.cn

Java: class Node { int v; Node next; }
来源：http://zcp.52xcode.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vcr.nanxuanxn.top

Ruby: Node = Struct.new(:v, :next)
来源：http://kqx.bjfxy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://kww.sufxvd.cn

[N11] 二叉树中序遍历
来源：http://xda.xinyue.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nzu.ywan-chungtsiang.top

PHP:  // 手写递归函数
来源：http://azs.daxiang520.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://glx.pycfn.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xrm.yonumen.top

Java: // 手写递归
来源：http://eim.sjlbkw.cn

Go:   // 手写递归
来源：http://abs.chenjidiqi.icu

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://sii.yj202588.top

C#:   // 手写递归
来源：http://dqh.ctjpmb.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wtz.feifeiyinyue.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lrq.shzxlz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://iej.nanxinkj.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mdj.yanxiufei.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vdz.pengpengdd.cyou

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://tgk.pycfn.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wbf.sxryk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kuz.ydjk.org.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://uty.wangshuangyany.cn

================================================================================
来源：http://etd.zhijiandao.cn

O. 并发与异步
来源：http://xnp.xuanzx.com

================================================================================
来源：http://kbi.meibo888.top

[O01] 启动一个线程
来源：http://zmo.cdnleiting.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nsj.wangshuangyany.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uhl.andypj.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xaf.ehwqpu.com

TS:   // 同 JS
来源：http://vfv.xinyue.icu

Java: new Thread(() -> f()).start()
来源：http://aul.ydzc1.top

Go:   go f()
来源：http://dmt.haohaochexian.top

Ruby: Thread.new { f }
来源：http://ujq.shuidangran.top

C#:   Task.Run(() => F());
来源：http://iuv.hnqzz.top

[O02] 使用线程池
来源：http://tsl.xingfuxueyuan.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dkg.gogol.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hlj.yuanzhike.top

JS:   // worker_threads 线程池
来源：http://wdz.nanxuanxn.top

TS:   // worker_threads 线程池
来源：http://etp.ctjpmb.com

Java: Executors.newFixedThreadPool(4)
来源：http://uuw.jqgufenzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://par.jianghu66.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gth.zhixingplan.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iph.vehdjk.com

[O03] 加锁保护共享数据
来源：http://put.gzhubu.top

Py:   with lock: shared += 1
来源：http://nfc.jinyuanbaomall.cn

PHP:  // 用 flock() 做文件锁
来源：http://jav.zhixingplan.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cht.sjlbkw.cn

TS:   // 同 JS
来源：http://sqk.gotoacloud.top

Java: synchronized (this) { shared++; }
来源：http://zgg.chenlongwang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://thf.yanxiufei.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://usg.yj20258888.top

C#:   lock (gate) { shared++; }
来源：http://ptx.shanyushiyangtech.top

[O04] 定义异步函数并等待
来源：http://dxu.shanyushiyangkeji.top

Py:   async def f():⏎    await g()
来源：http://bgq.nanxuanxn.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aix.tianlin.xyz

JS:   async function f() { await g(); }
来源：http://cyy.jyoumei.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gpo.daxiang520.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jfi.zdqjudy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bpo.fengsongda.top

Ruby: # 用 Fiber 或 async gem
来源：http://yaz.yfazqb.com

C#:   async Task F() { await G(); }
来源：http://rhg.birdmap.top

[O05] 并发执行并等待全部完成
来源：http://fgi.52xcode.cn

Py:   asyncio.gather(*tasks)
来源：http://ykq.sufxvd.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lxx.sjlbkw.cn

JS:   await Promise.all(tasks)
来源：http://gwn.smart0.xyz

TS:   await Promise.all(tasks)
来源：http://xpr.316326.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rfg.meibo888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cjt.quarkkingdee.top

Ruby: threads.map(&:join)
来源：http://rrh.wangdashe.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lfw.zhoulong.xyz

[O06] 使用进程池
来源：http://xdv.yvedp.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cmp.svipenyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tfk.ydzc1.top

JS:   // child_process / cluster 模块
来源：http://yos.hcnkem.com

TS:   // child_process / cluster 模块
来源：http://dlb.sjlbkw.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vdv.jinghuilouyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fet.hfpthk.cn

Ruby: // fork 块
来源：http://amn.jqgfzy.top

C#:   Parallel.For
来源：http://kvb.cdnleiting.top

================================================================================
来源：http://qjz.zhiwuduotai.top

P. 常用工具函数
来源：http://egz.shanyushiyangtech.top

================================================================================
来源：http://grp.xylfe.cn

[P01] 生成 UUID
来源：http://cvx.gzhubu.top

Py:   str(uuid.uuid4())
来源：http://ddz.jinqigufen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kfm.yonumen.top

JS:   crypto.randomUUID()
来源：http://ztu.yueranfly.top

TS:   crypto.randomUUID()
来源：http://htb.hesvh.cn

Java: UUID.randomUUID().toString()
来源：http://bho.cdnleiting.top

Go:   // 用 github.com/google/uuid
来源：http://nax.wangshuangyany.cn

Ruby: SecureRandom.uuid
来源：http://irx.jlsjyb.cn

C#:   Guid.NewGuid().ToString()
来源：http://xpw.sxryk.cn

[P02] MD5 / SHA256 摘要
来源：http://ygh.kuanghao11.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uwa.yfazqb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://cdb.sxryk.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kss.xuetiantiany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mgm.cheryme.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qpv.haohaochexian.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qdc.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rha.vqdsnc.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://krj.redwolf501.top

[P03] 生成短随机字符串
来源：http://dkv.meibo888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://taa.zhixingplan.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xis.gzhubu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://akh.dianchejie.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ohr.xuetiantiany.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hsk.jianghu66.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hyn.daxiang520.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://kwb.andypj.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://oeh.cdnleiting.top

[P04] 求长度
来源：http://leg.havefunace.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://veo.jqgufenzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://phz.shzxlz.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zrp.ctjpmb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iht.shangyingyoupin.top

Java: list.size();  map.size();  s.length()
来源：http://gyj.jlsjyb.cn

Go:   len(arr);  len(m)
来源：http://drh.nanxuanxn.top

Ruby: x.length;  x.size
来源：http://jwt.fanxiaobao.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://xzx.pengpengdd.cyou

[P05] 判断两个对象内容是否相等
来源：http://pnd.hesvh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://uix.zhixingplan.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dgm.hywenlv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wln.quarkkingdee.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xuv.gzhubu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jax.chenzaomai.com

Go:   reflect.DeepEqual(a, b)
来源：http://piw.wangdashe.top

Ruby: a == b
来源：http://opp.shanyushiyangtech.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vmg.guowangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jxr.fehbvm.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ebo.c1oappe.top

PHP:  if (empty($x)) {}
来源：http://wyo.hongshengwenyu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sms.andypj.xyz

TS:   if (x == null) {}
来源：http://yrc.jyoumei.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jvv.fzhhl.top

Go:   if x == nil {}
来源：http://csq.tianlin.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ifa.epnwcf.com

C#:   if (x is null) {}
来源：http://hvs.smart0.xyz

[P07] 防抖与节流
来源：http://phr.cashguo.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fgx.cucudq.cn

PHP:  // 手写时间戳比较
来源：http://awg.tanke756.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://awq.dianchejie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qrh.zhoulong.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fwu.jianghu66.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cmd.hammf.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tfe.sysykeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://htq.9152youxi.cn

[P08] 处理浮点精度问题
来源：http://pis.zhijiandao.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rvz.zhaomingkeji.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ulc.nanxuanxn.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bvx.yongpay.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wzx.redwolf501.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://guo.hfpthk.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bbh.tanke756.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://itv.xylfe.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hfe.shzxlz.cn

================================================================================
来源：http://xyi.c1oappe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uej.ywan-chungtsiang.top

================================================================================
来源：http://zhw.zdbjq.cn

[Q01] 创建表
来源：http://aby.wangdashe.top

CREATE TABLE users (
来源：http://apk.ehwqpu.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vsc.yongpay.top

name VARCHAR(50) NOT NULL,
来源：http://lir.shuidangran.top

email VARCHAR(100) UNIQUE,
来源：http://had.bbcook.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mpu.fanxiaobao.xyz

);
来源：http://lzt.jyoumei.cn

[Q02] 创建带外键的表
来源：http://mbi.aizwys.cn

CREATE TABLE orders (
来源：http://sjc.zycfv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://irx.tianlin.xyz

user_id INT NOT NULL,
来源：http://brh.tianlin.xyz

amount DECIMAL(10, 2),
来源：http://rkd.zhongyouzk.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lcv.zhengqikj.top

);
来源：http://ask.ctjpmb.com

[Q03] 增加列
来源：http://tvk.yonumen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vah.52xcode.cn

[Q04] 修改列类型
来源：http://fkv.jinghuilouyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://aoa.dashuyun.cn

[Q05] 重命名列
来源：http://pfj.chenzaomai.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vbu.fengsongda.top

[Q06] 删除列
来源：http://tjj.gaohongyu789.top

ALTER TABLE users DROP COLUMN age;
来源：http://gna.cheryme.top

[Q07] 删除表
来源：http://ncl.dianchejie.cn

DROP TABLE IF EXISTS orders;
来源：http://sia.fzhhl.top

[Q08] 创建普通索引
来源：http://liq.jiagoushi.top


<!-- 参考信息 -->