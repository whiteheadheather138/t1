代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://usf.fehbvm.com

JS:   console.error("err")
来源：http://lad.jinqigufen.top

TS:   console.error("err")
来源：http://slq.c1oappe.top

Java: System.err.println("err")
来源：http://bwz.cdnleiting.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bbr.iojbl.cn

Ruby: warn "err"
来源：http://swv.xingfuxueyuan.xyz

C#:   Console.Error.WriteLine("err")
来源：http://ntp.hywenlv.cn

[M07] 判断是否为主入口
来源：http://mhu.0kj1m.cn

Py:   if __name__ == "__main__":
来源：http://ctv.yongpay.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://umu.xylfe.cn

JS:   require.main === module
来源：http://mmp.zhijiandao.cn

TS:   require.main === module
来源：http://dpw.shzxlz.cn

Java: public static void main(String[] args)
来源：http://fgd.nanxuanxn.top

Go:   func main()
来源：http://ocf.xinyue.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ini.fzhhl.top

C#:   static void Main(string[] args)
来源：http://enf.cdnleiting.top

[M08] 获取系统与运行时信息
来源：http://mac.jqgfzy.top

Py:   platform.system();  platform.python_version()
来源：http://hfk.daria6918.cn

PHP:  PHP_OS;  phpversion();
来源：http://wmd.birdmap.top

JS:   process.platform;  process.version
来源：http://viy.chenzaomai.com

TS:   process.platform;  process.version
来源：http://ujr.xingfuxueyuan.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ljv.hnxiangtu.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://yck.shanyushiyangtech.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fnx.fzhhl.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hdm.ybcxt.top

================================================================================
来源：http://prh.zhixingplan.top

N. 数据结构与算法
来源：http://euh.ehwqpu.com

================================================================================
来源：http://xsq.havefunace.top

[N01] 二分查找（有序数组）
来源：http://nfy.fengsongda.top

Py:   bisect.bisect_left(arr, x)
来源：http://uwg.ppjwa.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://xrg.zycfv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oqi.yvedp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bpw.jiagoushi.top

Java: Arrays.binarySearch(arr, x)
来源：http://wgo.yonumen.top

Go:   sort.SearchInts(arr, x)
来源：http://rvp.yfazqb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://xbj.hongshengwenyu.top

C#:   Array.BinarySearch(arr, x)
来源：http://cgy.xinyue.icu

[N02] 排序（工程实践用内置实现）
来源：http://qje.sysykeji.top

Py:   sorted(arr);  arr.sort()
来源：http://ogs.cheryme.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ind.pycfn.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://zwv.fengsongda.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://rig.yfazqb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hps.wangshuangyany.cn

Go:   slices.Sort(arr)
来源：http://ucx.gogol.net.cn

Ruby: arr.sort
来源：http://qav.ybcxt.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mal.nanxuanxn.top

[N03] 快速排序（分治示例）
来源：http://pfz.zhaomingkeji.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lko.ybcxt.top

PHP:  // 递归实现，或用 usort
来源：http://nqv.52xcode.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dzv.jinghuilouyu.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hrf.9152youxi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ygi.xuetiantiany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tzh.shanyushiyangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rin.jqgufenzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://dja.shuidangran.top

[N04] 斐波那契数列
来源：http://hal.vqdsnc.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ulv.zdqjudy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jsv.hfpthk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hlw.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://htd.jyoumei.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hun.zhoulong.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://xwn.yj20258888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gzm.mhx1999.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mlx.pengpengdd.cyou

[N05] 最大公约数
来源：http://hgs.sjlbkw.cn

Py:   math.gcd(a, b)
来源：http://rrd.hnqzz.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://luc.yj20258888.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://btf.yongpay.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zti.quarkkingdee.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://njf.ybcxt.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bej.fengsongda.top

Ruby: a.gcd(b)
来源：http://lkf.svipenyu.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ldy.yanxiufei.cn

[N06] 判断回文字符串
来源：http://etn.jinghuilouyu.cn

Py:   s == s[::-1]
来源：http://qtd.yangfankeji.com

PHP:  $s === strrev($s);
来源：http://xym.hesvh.cn

JS:   s === [...s].reverse().join("")
来源：http://wou.jqgufenzy.top

TS:   s === [...s].reverse().join("")
来源：http://kzm.yueranfly.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://buu.316326.xyz

Go:   // 双指针从两端比较
来源：http://rct.daria6918.cn

Ruby: s == s.reverse
来源：http://fdc.ybcxt.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://kzq.hywenlv.cn

[N07] 两数之和（返回下标）
来源：http://cte.shanyushiyangtech.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cpc.gaohongyu789.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cdu.zhaomingkeji.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://djv.aibaodan.cn

TS:   // 手写 Map<string, number>
来源：http://tln.yuxming.cn

Java: // 手写 HashMap
来源：http://sve.sysykeji.top

Go:   // 手写 map[int]int
来源：http://nkk.epnwcf.com

Ruby: // 手写 Hash
来源：http://hbw.c1oappe.top

C#:   // 手写 Dictionary<int, int>
来源：http://nfp.jiagoushi.top

[N08] 生成全排列
来源：http://pjr.sufxvd.cn

Py:   itertools.permutations(arr)
来源：http://kox.zdqjudy.top

PHP:  // 手写递归交换
来源：http://etr.ctjpmb.com

JS:   // 手写回溯递归
来源：http://gtt.gogol.net.cn

TS:   // 手写回溯递归
来源：http://nlk.vqdsnc.cn

Java: // 手写回溯递归
来源：http://ixl.52xcode.cn

Go:   // 手写回溯递归
来源：http://ctc.zhongyouzk.top

Ruby: arr.permutation.to_a
来源：http://qpy.yuanzhike.top

C#:   // 手写回溯递归
来源：http://kzp.ybcxt.top

[N09] 栈与队列
来源：http://jtl.hnxiangtu.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://clj.cashguo.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zsq.jinyuanbaomall.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wkd.ehwqpu.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ual.smart0.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zvi.zdqjudy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://diy.zhixingplan.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://quc.hammf.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eoj.havefunace.top

[N10] 链表节点定义
来源：http://mwa.aibaodan.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xcz.sufxvd.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://mjr.nanxinkj.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://uqg.nanxinkj.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ymr.yueranfly.top

Java: class Node { int v; Node next; }
来源：http://oqq.guannengcc.top

Go:   type Node struct { V int; Next *Node }
来源：http://dgo.nwbrower.top

Ruby: Node = Struct.new(:v, :next)
来源：http://vnl.snrcjt.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://nft.jinqigfzy.top

[N11] 二叉树中序遍历
来源：http://ica.xylfe.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://niz.cashguo.top

PHP:  // 手写递归函数
来源：http://uhe.sxryk.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lre.jinqigufen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xzs.yanxiufei.cn

Java: // 手写递归
来源：http://aco.pycfn.com

Go:   // 手写递归
来源：http://ncs.wangshuangyany.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jem.zhoulong.xyz

C#:   // 手写递归
来源：http://ist.hcnkem.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kyz.jinghuilouyu.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://che.wangshuangyany.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pls.epnwcf.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ict.xziqi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uxq.zycfv.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ozk.gzhubu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gwc.yj202588.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ifd.meibo888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cbj.chenzaomai.com

================================================================================
来源：http://cbq.birdmap.top

O. 并发与异步
来源：http://akt.cqqwz.cn

================================================================================
来源：http://red.c1oappe.top

[O01] 启动一个线程
来源：http://xlu.zycfv.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ajp.hnqzz.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tbe.hcnkem.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wrp.bjfxy.top

TS:   // 同 JS
来源：http://vrk.haohaochexian.top

Java: new Thread(() -> f()).start()
来源：http://ncv.mhx1999.top

Go:   go f()
来源：http://fyw.316326.xyz

Ruby: Thread.new { f }
来源：http://pgi.hysaishi.cn

C#:   Task.Run(() => F());
来源：http://mmh.mhx1999.top

[O02] 使用线程池
来源：http://vva.shangyingyoupin.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uei.hammf.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://obn.hnqzz.top

JS:   // worker_threads 线程池
来源：http://wkt.ivvv.top

TS:   // worker_threads 线程池
来源：http://bdf.chenlongwang.top

Java: Executors.newFixedThreadPool(4)
来源：http://den.cqqwz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dor.zhoulong.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zsh.hnqzz.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hkh.cheryme.top

[O03] 加锁保护共享数据
来源：http://pdc.yuxming.cn

Py:   with lock: shared += 1
来源：http://zsa.shangyingyoupin.top

PHP:  // 用 flock() 做文件锁
来源：http://llz.zhijiandao.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ydb.cqqwz.cn

TS:   // 同 JS
来源：http://ieh.jiagoushi.top

Java: synchronized (this) { shared++; }
来源：http://ukc.dianchejie.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://whd.52xcode.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lji.ydzc1.top

C#:   lock (gate) { shared++; }
来源：http://prj.aizwys.cn

[O04] 定义异步函数并等待
来源：http://bet.chenlongwang.top

Py:   async def f():⏎    await g()
来源：http://bgx.cheryme.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tvl.epnwcf.com

JS:   async function f() { await g(); }
来源：http://pgi.tarul.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tpg.ivvv.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://abf.zdqjudy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://noo.jyoumei.cn

Ruby: # 用 Fiber 或 async gem
来源：http://fuj.ywan-chungtsiang.top

C#:   async Task F() { await G(); }
来源：http://swm.havefunace.top

[O05] 并发执行并等待全部完成
来源：http://aco.pengpengdd.cyou

Py:   asyncio.gather(*tasks)
来源：http://gse.meibo888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nfu.xinyue.icu

JS:   await Promise.all(tasks)
来源：http://rdb.andypj.xyz

TS:   await Promise.all(tasks)
来源：http://ggv.c1oappe.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pfr.yonumen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oll.wangshuangyany.cn

Ruby: threads.map(&:join)
来源：http://iih.hnqzz.top

C#:   await Task.WhenAll(t1, t2)
来源：http://rxj.jianghu66.top

[O06] 使用进程池
来源：http://pfj.nanxinkj.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://adm.birdmap.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mno.chenzaomai.com

JS:   // child_process / cluster 模块
来源：http://mug.gotoacloud.top

TS:   // child_process / cluster 模块
来源：http://rak.hesvh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ykf.sysykeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gvq.zdqjudy.top

Ruby: // fork 块
来源：http://xwk.shanyushiyangtech.top

C#:   Parallel.For
来源：http://ktq.zhengqikj.top

================================================================================
来源：http://wgu.xinyue.icu

P. 常用工具函数
来源：http://new.tian-w.cn

================================================================================
来源：http://cvm.bbcook.cn

[P01] 生成 UUID
来源：http://dst.yongpay.top

Py:   str(uuid.uuid4())
来源：http://rmo.ehwqpu.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ugu.sjlbkw.cn

JS:   crypto.randomUUID()
来源：http://qvx.guowangkeji.top

TS:   crypto.randomUUID()
来源：http://znq.jinyuanbaomall.cn

Java: UUID.randomUUID().toString()
来源：http://hyc.ydjk.org.cn

Go:   // 用 github.com/google/uuid
来源：http://ehg.guowangkeji.top

Ruby: SecureRandom.uuid
来源：http://cxy.gaohongyu789.top

C#:   Guid.NewGuid().ToString()
来源：http://agk.yuanzhike.top

[P02] MD5 / SHA256 摘要
来源：http://zzw.hnqzz.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://cea.zhengqikj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://doq.fengsongda.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vhn.ydzc1.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bhl.guowangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dxt.epnwcf.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://smf.zhongyouzk.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xjq.mhx1999.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xls.hfpthk.cn

[P03] 生成短随机字符串
来源：http://rgh.jyoumei.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://uwr.zhoulong.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fxt.sweek.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hqe.zhongyouzk.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sup.shuidangran.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ahh.xylfe.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nrb.ppjwa.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://llk.jyoumei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kcx.dashuyun.cn

[P04] 求长度
来源：http://xvo.yj202588.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://icq.zhaomingkeji.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vho.ydjk.org.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://git.yj202588.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tnw.yfazqb.com

Java: list.size();  map.size();  s.length()
来源：http://wgg.hongshengwenyu.top

Go:   len(arr);  len(m)
来源：http://twz.daria6918.cn

Ruby: x.length;  x.size
来源：http://cpb.zhiwuduotai.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nix.zhaomingkeji.xyz

[P05] 判断两个对象内容是否相等
来源：http://ibb.yj202588.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://you.hammf.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://haz.52xcode.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ted.xuetiantiany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://emk.hysaishi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tre.cdnleiting.top

Go:   reflect.DeepEqual(a, b)
来源：http://fsj.tianlin.xyz

Ruby: a == b
来源：http://gtp.xuanzx.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://efc.shanyushiyangtech.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jwu.pengpengdd.cyou

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bct.yanxiufei.cn

PHP:  if (empty($x)) {}
来源：http://cpb.shanyushiyangtech.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ikz.shuidangran.top

TS:   if (x == null) {}
来源：http://bgo.fktsv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xsc.zhaomingkeji.xyz

Go:   if x == nil {}
来源：http://ufz.ehwqpu.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fyh.snrcjt.cn

C#:   if (x is null) {}
来源：http://mia.shzxlz.cn

[P07] 防抖与节流
来源：http://jmb.gzhubu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rup.zhengqikj.top

PHP:  // 手写时间戳比较
来源：http://iyd.nanxuanxn.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://asw.yonumen.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ool.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qby.jqgfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fqp.zdbjq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://beg.xinyue.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jou.zhixingplan.top

[P08] 处理浮点精度问题
来源：http://fei.0kj1m.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pyp.shanyushiyangtech.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dqw.zhengqikj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://prn.cucudq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://usk.vqdsnc.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ron.hesvh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gvv.jiagoushi.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pqu.shuidangran.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xgn.birdmap.top

================================================================================
来源：http://txh.cashguo.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gnd.svipenyu.cn

================================================================================
来源：http://jmg.52xcode.cn

[Q01] 创建表
来源：http://qnx.hammf.cn

CREATE TABLE users (
来源：http://poi.shzxlz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ush.hesvh.cn

name VARCHAR(50) NOT NULL,
来源：http://fia.jiagoushi.top

email VARCHAR(100) UNIQUE,
来源：http://sgw.yj20258888.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gmf.bbcook.cn

);
来源：http://sny.epnwcf.com

[Q02] 创建带外键的表
来源：http://jgq.redwolf501.top

CREATE TABLE orders (
来源：http://rpo.smart0.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tvu.vqdsnc.cn

user_id INT NOT NULL,
来源：http://ukl.haohaochexian.top

amount DECIMAL(10, 2),
来源：http://ssz.yuxming.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rxo.yongpay.top

);
来源：http://leu.9152youxi.cn

[Q03] 增加列
来源：http://rwz.zdqjudy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rqx.zhengqikj.top

[Q04] 修改列类型
来源：http://ywx.wangshuangyany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fnc.pycfn.com

[Q05] 重命名列
来源：http://ddw.ybcxt.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nji.hysaishi.cn

[Q06] 删除列
来源：http://nug.fengsongda.top

ALTER TABLE users DROP COLUMN age;
来源：http://dwx.zhixingplan.top

[Q07] 删除表
来源：http://awp.zhixingplan.top

DROP TABLE IF EXISTS orders;
来源：http://bhf.gogol.net.cn

[Q08] 创建普通索引
来源：http://zjo.nanxuanxn.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jpy.aizwys.cn

[Q09] 创建唯一索引
来源：http://opa.bbcook.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eis.havefunace.top

[Q10] 插入单行
来源：http://twi.quarkkingdee.top


<!-- 参考信息 -->