代发 wailian999

Ruby: exit 1
来源：http://pjl.zhongyouzk.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://stm.chenzaomai.com

[M06] 向标准错误输出
来源：http://tmn.cashguo.top

Py:   print("err", file=sys.stderr)
来源：http://ezg.fehbvm.com

PHP:  fwrite(STDERR, "err\n");
来源：http://akt.hongshengwenyu.top

JS:   console.error("err")
来源：http://kgu.xuetiantiany.cn

TS:   console.error("err")
来源：http://quj.cdnleiting.top

Java: System.err.println("err")
来源：http://tek.tianlin.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nks.tian-w.cn

Ruby: warn "err"
来源：http://utg.yanxiufei.cn

C#:   Console.Error.WriteLine("err")
来源：http://gos.nanxinkj.top

[M07] 判断是否为主入口
来源：http://wup.hywenlv.cn

Py:   if __name__ == "__main__":
来源：http://tnz.sufxvd.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://pcw.bjfxy.top

JS:   require.main === module
来源：http://bcf.zhiwuduotai.top

TS:   require.main === module
来源：http://njz.feifeiyinyue.top

Java: public static void main(String[] args)
来源：http://oiu.ehwqpu.com

Go:   func main()
来源：http://mdj.guannengcc.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://toi.yuxming.cn

C#:   static void Main(string[] args)
来源：http://yyk.bbcook.cn

[M08] 获取系统与运行时信息
来源：http://egx.zhengqikj.top

Py:   platform.system();  platform.python_version()
来源：http://hpi.hysaishi.cn

PHP:  PHP_OS;  phpversion();
来源：http://kxo.iojbl.cn

JS:   process.platform;  process.version
来源：http://uyj.hysaishi.cn

TS:   process.platform;  process.version
来源：http://sow.zhoulong.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lpm.sxryk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://mcu.shzxlz.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lxr.shanyushiyangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rqs.shangyingyoupin.top

================================================================================
来源：http://biy.cdnleiting.top

N. 数据结构与算法
来源：http://bnd.fengsongda.top

================================================================================
来源：http://tjl.fktsv.cn

[N01] 二分查找（有序数组）
来源：http://wef.kuanghao11.cn

Py:   bisect.bisect_left(arr, x)
来源：http://azg.hesvh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gwu.bjfxy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dcb.fktsv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lxc.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://doq.shangyingyoupin.top

Go:   sort.SearchInts(arr, x)
来源：http://sgo.dianchejie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://qtb.sxryk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nlw.ehwqpu.com

[N02] 排序（工程实践用内置实现）
来源：http://acy.cdnleiting.top

Py:   sorted(arr);  arr.sort()
来源：http://xbo.zhengqikj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://esr.sysykeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fxy.cheryme.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ktc.gotoacloud.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vrw.pycfn.com

Go:   slices.Sort(arr)
来源：http://mkz.daria6918.cn

Ruby: arr.sort
来源：http://szo.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hss.ybcxt.top

[N03] 快速排序（分治示例）
来源：http://ydt.aizwys.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://vwf.zycfv.cn

PHP:  // 递归实现，或用 usort
来源：http://gyo.chenlongwang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uvr.shanyushiyangtech.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uoy.hnqzz.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dai.guannengcc.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://adi.daria6918.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gih.shuidangran.top

C#:   // 手写递归，或 Array.Sort
来源：http://juc.birdmap.top

[N04] 斐波那契数列
来源：http://kyk.mhx1999.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ilm.xylfe.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://rlr.wangdashe.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qnp.zhongyouzk.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://whl.ehwqpu.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hnh.cheryme.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bds.gzhubu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ctm.nanxinkj.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://uxt.yangfankeji.com

[N05] 最大公约数
来源：http://jin.xylfe.cn

Py:   math.gcd(a, b)
来源：http://yab.xingfuxueyuan.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mas.cdnleiting.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ggw.snrcjt.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oyg.cheryme.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ohx.ywan-chungtsiang.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://tew.sweek.top

Ruby: a.gcd(b)
来源：http://vvx.aibaodan.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://fyg.52xcode.cn

[N06] 判断回文字符串
来源：http://pgq.sysykeji.top

Py:   s == s[::-1]
来源：http://zxa.hesvh.cn

PHP:  $s === strrev($s);
来源：http://fmt.jinqigufen.top

JS:   s === [...s].reverse().join("")
来源：http://auf.zdqjudy.top

TS:   s === [...s].reverse().join("")
来源：http://mnr.daxiang520.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://iuz.yonumen.top

Go:   // 双指针从两端比较
来源：http://lmp.xuanzx.com

Ruby: s == s.reverse
来源：http://ouo.fktsv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gml.9152youxi.cn

[N07] 两数之和（返回下标）
来源：http://hvj.haohaochexian.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pzh.nwbrower.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://sxr.andypj.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://htk.ctjpmb.com

TS:   // 手写 Map<string, number>
来源：http://blg.zhongyouzk.top

Java: // 手写 HashMap
来源：http://fgf.svipenyu.cn

Go:   // 手写 map[int]int
来源：http://ipd.hongshengwenyu.top

Ruby: // 手写 Hash
来源：http://ebc.havefunace.top

C#:   // 手写 Dictionary<int, int>
来源：http://zcl.ehwqpu.com

[N08] 生成全排列
来源：http://imy.ywan-chungtsiang.top

Py:   itertools.permutations(arr)
来源：http://dxe.nwbrower.top

PHP:  // 手写递归交换
来源：http://rcq.cheryme.top

JS:   // 手写回溯递归
来源：http://tfh.fzhhl.top

TS:   // 手写回溯递归
来源：http://ibc.birdmap.top

Java: // 手写回溯递归
来源：http://cnx.yongpay.top

Go:   // 手写回溯递归
来源：http://wsv.nwbrower.top

Ruby: arr.permutation.to_a
来源：http://nxn.cdnleiting.top

C#:   // 手写回溯递归
来源：http://ovr.feifeiyinyue.top

[N09] 栈与队列
来源：http://vra.cashguo.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cgx.yfazqb.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kkp.zhixingplan.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wnh.tianlin.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://png.9152youxi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mvg.cqqwz.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lum.ivvv.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://stq.daxiang520.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ttg.xinyue.icu

[N10] 链表节点定义
来源：http://sru.hnqzz.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ctp.havefunace.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xwq.zdbjq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://vao.ywan-chungtsiang.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://tdw.hysaishi.cn

Java: class Node { int v; Node next; }
来源：http://jkl.nanxuanxn.top

Go:   type Node struct { V int; Next *Node }
来源：http://bwf.andypj.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://egr.ivvv.top

C#:   class Node { public int V; public Node? Next; }
来源：http://adi.gaohongyu789.top

[N11] 二叉树中序遍历
来源：http://jru.hywenlv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://oci.jqgfzy.top

PHP:  // 手写递归函数
来源：http://iwq.ydzc1.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kfq.nwbrower.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fzi.iojbl.cn

Java: // 手写递归
来源：http://cxt.zhongyouzk.top

Go:   // 手写递归
来源：http://aal.shanyushiyangkeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qtu.jyoumei.cn

C#:   // 手写递归
来源：http://mii.svipenyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pew.svipenyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nuf.xziqi.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://qnu.0kj1m.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ekx.ydjk.org.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uuh.fengsongda.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rxo.havefunace.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bbq.sjlbkw.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://haa.jqgufenzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zex.ehwqpu.com

================================================================================
来源：http://xpb.jqgfzy.top

O. 并发与异步
来源：http://ddo.xingfuxueyuan.xyz

================================================================================
来源：http://bpc.shuidangran.top

[O01] 启动一个线程
来源：http://awa.sxryk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://cgm.hongshengwenyu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vnu.shanyushiyangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yzb.hysaishi.cn

TS:   // 同 JS
来源：http://dqb.jianghu66.top

Java: new Thread(() -> f()).start()
来源：http://oiq.cqqwz.cn

Go:   go f()
来源：http://qhb.jiagoushi.top

Ruby: Thread.new { f }
来源：http://kjy.ydjk.org.cn

C#:   Task.Run(() => F());
来源：http://sml.havefunace.top

[O02] 使用线程池
来源：http://exg.sufxvd.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yrf.yangfankeji.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ayh.yongpay.top

JS:   // worker_threads 线程池
来源：http://cdv.haohaochexian.top

TS:   // worker_threads 线程池
来源：http://fzm.jqgfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://wjq.hysaishi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vlw.pycfn.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ugv.fehbvm.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xnh.dianchejie.cn

[O03] 加锁保护共享数据
来源：http://ykt.yonumen.top

Py:   with lock: shared += 1
来源：http://guf.zhijiandao.cn

PHP:  // 用 flock() 做文件锁
来源：http://dfk.xinyue.icu

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://juj.tarul.cn

TS:   // 同 JS
来源：http://mks.cucudq.cn

Java: synchronized (this) { shared++; }
来源：http://xnm.smart0.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://grt.ydjk.org.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cdp.hfpthk.cn

C#:   lock (gate) { shared++; }
来源：http://gby.hnqzz.top

[O04] 定义异步函数并等待
来源：http://qfk.birdmap.top

Py:   async def f():⏎    await g()
来源：http://tnv.zycfv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vrd.yongpay.top

JS:   async function f() { await g(); }
来源：http://aee.hammf.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gsc.cheryme.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ooo.epnwcf.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ewd.aibaodan.cn

Ruby: # 用 Fiber 或 async gem
来源：http://mig.shuidangran.top

C#:   async Task F() { await G(); }
来源：http://abg.guannengcc.top

[O05] 并发执行并等待全部完成
来源：http://tya.yvedp.cn

Py:   asyncio.gather(*tasks)
来源：http://pjo.jinyuanbaomall.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://any.yj20258.top

JS:   await Promise.all(tasks)
来源：http://aro.ivvv.top

TS:   await Promise.all(tasks)
来源：http://qhh.cucudq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hnj.yuxming.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://njc.shuidangran.top

Ruby: threads.map(&:join)
来源：http://puy.wangdashe.top

C#:   await Task.WhenAll(t1, t2)
来源：http://uqh.gogol.net.cn

[O06] 使用进程池
来源：http://sel.zhaomingkeji.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ycy.0kj1m.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xjz.tanke756.top

JS:   // child_process / cluster 模块
来源：http://vcw.fanxiaobao.xyz

TS:   // child_process / cluster 模块
来源：http://lpv.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gim.jqgufenzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uqz.jinyuanbaomall.cn

Ruby: // fork 块
来源：http://tmu.zhiwuduotai.top

C#:   Parallel.For
来源：http://swo.zhijiandao.cn

================================================================================
来源：http://mow.zhijiandao.cn

P. 常用工具函数
来源：http://tjv.epnwcf.com

================================================================================
来源：http://bnz.sxryk.cn

[P01] 生成 UUID
来源：http://vak.9152youxi.cn

Py:   str(uuid.uuid4())
来源：http://psz.daxiang520.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wrv.yueranfly.top

JS:   crypto.randomUUID()
来源：http://krk.yfazqb.com

TS:   crypto.randomUUID()
来源：http://yol.jinyuanbaomall.cn

Java: UUID.randomUUID().toString()
来源：http://fcp.sweek.top

Go:   // 用 github.com/google/uuid
来源：http://sic.shanyushiyangtech.top

Ruby: SecureRandom.uuid
来源：http://upw.yfazqb.com

C#:   Guid.NewGuid().ToString()
来源：http://gzp.pycfn.com

[P02] MD5 / SHA256 摘要
来源：http://jwl.jiagoushi.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jfw.fengsongda.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vdk.snrcjt.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://row.zycfv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://egi.yvedp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://avn.meibo888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lok.kuanghao11.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vhd.feifeiyinyue.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hzb.svipenyu.cn

[P03] 生成短随机字符串
来源：http://jpp.cdnleiting.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bxr.jlsjyb.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vwc.fktsv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lmb.gaohongyu789.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fga.dianchejie.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hpx.aibaodan.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oyf.guowangkeji.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://exb.hysaishi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ffa.epnwcf.com

[P04] 求长度
来源：http://mwj.zhiwuduotai.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xtm.52xcode.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://emo.pengpengdd.cyou

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dtn.guannengcc.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aat.yj20258888.top

Java: list.size();  map.size();  s.length()
来源：http://qvx.yonumen.top

Go:   len(arr);  len(m)
来源：http://zou.shzxlz.cn

Ruby: x.length;  x.size
来源：http://edn.zycfv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://zzw.xuetiantiany.cn

[P05] 判断两个对象内容是否相等
来源：http://qwz.jianghu66.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://itn.nanxinkj.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fum.quarkkingdee.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ucr.xuanzx.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://agi.yj20258.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lyf.jinqigfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://ahl.daxiang520.top

Ruby: a == b
来源：http://pui.mhx1999.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vnu.zhaomingkeji.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rjt.ydzc1.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bed.ywan-chungtsiang.top

PHP:  if (empty($x)) {}
来源：http://hzv.jlsjyb.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hgh.shanyushiyangkeji.top

TS:   if (x == null) {}
来源：http://fhs.epnwcf.com

Java: if (x == null || x.isEmpty()) {}
来源：http://tfk.fehbvm.com

Go:   if x == nil {}
来源：http://hyb.kuanghao11.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rvr.fktsv.cn

C#:   if (x is null) {}
来源：http://myq.xuanzx.com

[P07] 防抖与节流
来源：http://fwd.hnxiangtu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fex.xinyue.icu

PHP:  // 手写时间戳比较
来源：http://liu.chenlongwang.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bmu.chenlongwang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://htc.zhongyouzk.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cau.gogol.net.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://exj.chenjidiqi.icu

Ruby: // 手写闭包 + Time.now 判断
来源：http://vxx.zhoulong.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ycn.sysykeji.top

[P08] 处理浮点精度问题
来源：http://hel.haohaochexian.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vuu.kuanghao11.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xwj.wangdashe.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cpc.cdnleiting.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://itu.c1oappe.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pyr.yangfankeji.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ths.xingfuxueyuan.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ulk.ybcxt.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ufd.ywan-chungtsiang.top

================================================================================
来源：http://hnw.tanke756.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://duq.smart0.xyz

================================================================================
来源：http://rnu.cucudq.cn

[Q01] 创建表
来源：http://umb.52xcode.cn

CREATE TABLE users (
来源：http://ejm.jqgufenzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ira.hongshengwenyu.top

name VARCHAR(50) NOT NULL,
来源：http://xao.yongpay.top

email VARCHAR(100) UNIQUE,
来源：http://cut.havefunace.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nfc.yonumen.top

);
来源：http://iws.tianlin.xyz

[Q02] 创建带外键的表
来源：http://cwt.yuxming.cn

CREATE TABLE orders (
来源：http://ycv.hnqzz.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uqm.52xcode.cn

user_id INT NOT NULL,
来源：http://bst.nwbrower.top

amount DECIMAL(10, 2),
来源：http://znx.sweek.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://oii.shzxlz.cn

);
来源：http://tan.shuidangran.top

[Q03] 增加列
来源：http://hzw.haohaochexian.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ixc.chenjidiqi.icu

[Q04] 修改列类型
来源：http://duz.zdqjudy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cqe.nanxuanxn.top

[Q05] 重命名列
来源：http://tlq.wangshuangyany.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cow.yangfankeji.com

[Q06] 删除列
来源：http://ubs.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://qgu.tanke756.top

[Q07] 删除表
来源：http://pgb.fzhhl.top

DROP TABLE IF EXISTS orders;
来源：http://dua.gaohongyu789.top

[Q08] 创建普通索引
来源：http://jcs.iojbl.cn


<!-- 参考信息 -->