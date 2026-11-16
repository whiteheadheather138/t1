代发 wailian999

JS:   process.exit(1)
来源：http://wwb.hnxiangtu.top

TS:   process.exit(1)
来源：http://knn.ydzc1.top

Java: System.exit(1)
来源：http://miw.hnxiangtu.top

Go:   os.Exit(1)
来源：http://rdi.fengsongda.top

Ruby: exit 1
来源：http://wdb.ehwqpu.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://rlu.52xcode.cn

[M06] 向标准错误输出
来源：http://fxq.jiagoushi.top

Py:   print("err", file=sys.stderr)
来源：http://fhj.dianchejie.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lpi.zhiwuduotai.top

JS:   console.error("err")
来源：http://tcu.guowangkeji.top

TS:   console.error("err")
来源：http://bbt.hysaishi.cn

Java: System.err.println("err")
来源：http://hph.hfpthk.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mql.redwolf501.top

Ruby: warn "err"
来源：http://gzk.zhongyouzk.top

C#:   Console.Error.WriteLine("err")
来源：http://aqw.jiagoushi.top

[M07] 判断是否为主入口
来源：http://pqx.vehdjk.com

Py:   if __name__ == "__main__":
来源：http://xmc.xingfuxueyuan.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lts.svipenyu.cn

JS:   require.main === module
来源：http://dph.redwolf501.top

TS:   require.main === module
来源：http://ndx.pycfn.com

Java: public static void main(String[] args)
来源：http://iiv.havefunace.top

Go:   func main()
来源：http://qlm.ywan-chungtsiang.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vdg.haohaochexian.top

C#:   static void Main(string[] args)
来源：http://htv.ppjwa.cn

[M08] 获取系统与运行时信息
来源：http://ydg.jinqigfzy.top

Py:   platform.system();  platform.python_version()
来源：http://zss.zdbjq.cn

PHP:  PHP_OS;  phpversion();
来源：http://kfz.meibo888.top

JS:   process.platform;  process.version
来源：http://pvx.xziqi.cn

TS:   process.platform;  process.version
来源：http://stv.shzxlz.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://frb.sxryk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ogy.ppjwa.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dnt.vqdsnc.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://eif.xinyue.icu

================================================================================
来源：http://ixc.yangfankeji.com

N. 数据结构与算法
来源：http://lzw.meibo888.top

================================================================================
来源：http://kai.redwolf501.top

[N01] 二分查找（有序数组）
来源：http://xql.zycfv.cn

Py:   bisect.bisect_left(arr, x)
来源：http://rni.52xcode.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qep.guowangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ywe.jinqigufen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jba.fehbvm.com

Java: Arrays.binarySearch(arr, x)
来源：http://zaf.redwolf501.top

Go:   sort.SearchInts(arr, x)
来源：http://xcc.xziqi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zms.sysykeji.top

C#:   Array.BinarySearch(arr, x)
来源：http://hja.xziqi.cn

[N02] 排序（工程实践用内置实现）
来源：http://ood.havefunace.top

Py:   sorted(arr);  arr.sort()
来源：http://xus.nanxuanxn.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ckc.hywenlv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://odv.zhixingplan.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jds.xinyue.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yum.epnwcf.com

Go:   slices.Sort(arr)
来源：http://gry.yueranfly.top

Ruby: arr.sort
来源：http://jxu.jinghuilouyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jjr.cdnleiting.top

[N03] 快速排序（分治示例）
来源：http://dia.ctjpmb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://luz.ppjwa.cn

PHP:  // 递归实现，或用 usort
来源：http://kma.svipenyu.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ste.meibo888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lgl.fehbvm.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jbc.jinyuanbaomall.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pja.52xcode.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jzd.uphjek.com

C#:   // 手写递归，或 Array.Sort
来源：http://xby.pengpengdd.cyou

[N04] 斐波那契数列
来源：http://bfa.fktsv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jxx.yongpay.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://dhg.yj20258888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hjc.redwolf501.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iam.daxiang520.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cjq.shanyushiyangtech.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ctm.xziqi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xyz.nanxinkj.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tpn.hfpthk.cn

[N05] 最大公约数
来源：http://mtz.vehdjk.com

Py:   math.gcd(a, b)
来源：http://weu.pycfn.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cuw.xziqi.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://idi.mhx1999.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://csq.52xcode.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zgz.nanxinkj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ajt.snrcjt.cn

Ruby: a.gcd(b)
来源：http://okt.xuanzx.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jjj.zhixingplan.top

[N06] 判断回文字符串
来源：http://ihv.shuidangran.top

Py:   s == s[::-1]
来源：http://eei.hongshengwenyu.top

PHP:  $s === strrev($s);
来源：http://bpg.feifeiyinyue.top

JS:   s === [...s].reverse().join("")
来源：http://mul.redwolf501.top

TS:   s === [...s].reverse().join("")
来源：http://bav.fehbvm.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dbp.birdmap.top

Go:   // 双指针从两端比较
来源：http://lfo.vqdsnc.cn

Ruby: s == s.reverse
来源：http://qui.pycfn.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://ejo.hesvh.cn

[N07] 两数之和（返回下标）
来源：http://daa.jianghu66.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://fhr.yfazqb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://naw.kuanghao11.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pye.yuxming.cn

TS:   // 手写 Map<string, number>
来源：http://yiv.gaohongyu789.top

Java: // 手写 HashMap
来源：http://kqk.guowangkeji.top

Go:   // 手写 map[int]int
来源：http://ptq.zhixingplan.top

Ruby: // 手写 Hash
来源：http://kbh.cheryme.top

C#:   // 手写 Dictionary<int, int>
来源：http://hdu.hysaishi.cn

[N08] 生成全排列
来源：http://umf.hammf.cn

Py:   itertools.permutations(arr)
来源：http://gno.sufxvd.cn

PHP:  // 手写递归交换
来源：http://rcr.xuanzx.com

JS:   // 手写回溯递归
来源：http://iym.sjlbkw.cn

TS:   // 手写回溯递归
来源：http://hwi.316326.xyz

Java: // 手写回溯递归
来源：http://dzy.yueranfly.top

Go:   // 手写回溯递归
来源：http://zpi.dianchejie.cn

Ruby: arr.permutation.to_a
来源：http://ymg.chenzaomai.com

C#:   // 手写回溯递归
来源：http://pkp.dianchejie.cn

[N09] 栈与队列
来源：http://zmu.hywenlv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jvj.pengpengdd.cyou

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mzs.ybcxt.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wze.mhx1999.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://esb.ydjk.org.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xmh.bbcook.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dji.shanyushiyangkeji.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ckd.fzhhl.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dxo.chenjidiqi.icu

[N10] 链表节点定义
来源：http://sej.mhx1999.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://iyw.wangshuangyany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cyw.pengpengdd.cyou

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://elm.smart0.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://vdf.hfpthk.cn

Java: class Node { int v; Node next; }
来源：http://mbc.ydjk.org.cn

Go:   type Node struct { V int; Next *Node }
来源：http://uuy.epnwcf.com

Ruby: Node = Struct.new(:v, :next)
来源：http://dmk.tianlin.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://wut.yuxming.cn

[N11] 二叉树中序遍历
来源：http://imh.aibaodan.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ozy.fktsv.cn

PHP:  // 手写递归函数
来源：http://muj.ehwqpu.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cfz.hfpthk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hxj.ehwqpu.com

Java: // 手写递归
来源：http://fhl.ybcxt.top

Go:   // 手写递归
来源：http://wmj.yuxming.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cjj.ehwqpu.com

C#:   // 手写递归
来源：http://lup.shangyingyoupin.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://szn.snrcjt.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ldu.ehwqpu.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kah.ppjwa.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yeu.hesvh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://isl.zhoulong.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oik.jlsjyb.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lgz.zdbjq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://loh.wangdashe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rzz.hnqzz.top

================================================================================
来源：http://bmd.hfpthk.cn

O. 并发与异步
来源：http://rvy.316326.xyz

================================================================================
来源：http://pgi.feifeiyinyue.top

[O01] 启动一个线程
来源：http://nck.jqgfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://azk.nanxinkj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://rhq.cqqwz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nvm.tianlin.xyz

TS:   // 同 JS
来源：http://yif.andypj.xyz

Java: new Thread(() -> f()).start()
来源：http://bit.cheryme.top

Go:   go f()
来源：http://mza.zhixingplan.top

Ruby: Thread.new { f }
来源：http://fzd.ydjk.org.cn

C#:   Task.Run(() => F());
来源：http://pan.chenzaomai.com

[O02] 使用线程池
来源：http://ioa.aibaodan.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://byq.zhixingplan.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://trq.gotoacloud.top

JS:   // worker_threads 线程池
来源：http://tmn.yueranfly.top

TS:   // worker_threads 线程池
来源：http://ipn.yj20258.top

Java: Executors.newFixedThreadPool(4)
来源：http://eee.hnqzz.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bbz.nanxinkj.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://etx.xylfe.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xux.sweek.top

[O03] 加锁保护共享数据
来源：http://rei.daxiang520.top

Py:   with lock: shared += 1
来源：http://hxe.dianchejie.cn

PHP:  // 用 flock() 做文件锁
来源：http://eqr.wangshuangyany.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://phf.vehdjk.com

TS:   // 同 JS
来源：http://bof.gaohongyu789.top

Java: synchronized (this) { shared++; }
来源：http://cis.zhaomingkeji.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://enb.meibo888.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ytq.shanyushiyangtech.top

C#:   lock (gate) { shared++; }
来源：http://adi.haohaochexian.top

[O04] 定义异步函数并等待
来源：http://npp.zhaomingkeji.xyz

Py:   async def f():⏎    await g()
来源：http://vhb.zhengqikj.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hqp.ybcxt.top

JS:   async function f() { await g(); }
来源：http://olq.shanyushiyangtech.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gfo.hesvh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wxb.birdmap.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kcm.fengsongda.top

Ruby: # 用 Fiber 或 async gem
来源：http://grr.xziqi.cn

C#:   async Task F() { await G(); }
来源：http://xay.yfazqb.com

[O05] 并发执行并等待全部完成
来源：http://wgm.andypj.xyz

Py:   asyncio.gather(*tasks)
来源：http://tvl.vqdsnc.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tbi.aizwys.cn

JS:   await Promise.all(tasks)
来源：http://vjw.redwolf501.top

TS:   await Promise.all(tasks)
来源：http://lhx.cucudq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nol.gaohongyu789.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xfv.shuidangran.top

Ruby: threads.map(&:join)
来源：http://cie.tian-w.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lux.iojbl.cn

[O06] 使用进程池
来源：http://vjs.xingfuxueyuan.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kxm.shanyushiyangtech.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ukj.andypj.xyz

JS:   // child_process / cluster 模块
来源：http://qub.aibaodan.cn

TS:   // child_process / cluster 模块
来源：http://geh.zhongyouzk.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hxx.vqdsnc.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jab.hysaishi.cn

Ruby: // fork 块
来源：http://kmq.fanxiaobao.xyz

C#:   Parallel.For
来源：http://asd.redwolf501.top

================================================================================
来源：http://oeu.uphjek.com

P. 常用工具函数
来源：http://gcf.chenlongwang.top

================================================================================
来源：http://hme.zhixingplan.top

[P01] 生成 UUID
来源：http://cpf.yj20258.top

Py:   str(uuid.uuid4())
来源：http://aqt.andypj.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uoc.52xcode.cn

JS:   crypto.randomUUID()
来源：http://nyl.yanxiufei.cn

TS:   crypto.randomUUID()
来源：http://whf.yuanzhike.top

Java: UUID.randomUUID().toString()
来源：http://zku.feifeiyinyue.top

Go:   // 用 github.com/google/uuid
来源：http://zmk.tianlin.xyz

Ruby: SecureRandom.uuid
来源：http://aak.chenzaomai.com

C#:   Guid.NewGuid().ToString()
来源：http://mlu.mhx1999.top

[P02] MD5 / SHA256 摘要
来源：http://vhn.mhx1999.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://myv.ydjk.org.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hyg.yangfankeji.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://snv.hysaishi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mqj.meibo888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hcz.gogol.net.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hgk.ywan-chungtsiang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uyf.aibaodan.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tqx.nanxuanxn.top

[P03] 生成短随机字符串
来源：http://rfc.zhijiandao.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vle.aizwys.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://uue.fktsv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uaj.nanxinkj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fgu.sjlbkw.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jvj.fengsongda.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jux.52xcode.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://haw.ivvv.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://unq.jyoumei.cn

[P04] 求长度
来源：http://qgo.gotoacloud.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://itn.gotoacloud.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pqb.yj20258.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lgv.0kj1m.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iwh.iojbl.cn

Java: list.size();  map.size();  s.length()
来源：http://iee.hfpthk.cn

Go:   len(arr);  len(m)
来源：http://hgl.tian-w.cn

Ruby: x.length;  x.size
来源：http://gmv.tanke756.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qjr.jinqigufen.top

[P05] 判断两个对象内容是否相等
来源：http://etl.hnxiangtu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://xxe.jinqigfzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cjv.mhx1999.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wwh.ctjpmb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mny.quarkkingdee.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tmn.zdbjq.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bgh.cdnleiting.top

Ruby: a == b
来源：http://mdw.yongpay.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qof.zhongyouzk.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wfm.shangyingyoupin.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://htq.cashguo.top

PHP:  if (empty($x)) {}
来源：http://jby.fzhhl.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hsp.nanxinkj.top

TS:   if (x == null) {}
来源：http://jqw.cheryme.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vcm.yongpay.top

Go:   if x == nil {}
来源：http://yhh.nanxuanxn.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xhp.cqqwz.cn

C#:   if (x is null) {}
来源：http://rpc.fktsv.cn

[P07] 防抖与节流
来源：http://wdx.shanyushiyangtech.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tex.9152youxi.cn

PHP:  // 手写时间戳比较
来源：http://yib.zycfv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fke.jianghu66.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ttd.shuidangran.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qtq.yonumen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rdi.xuanzx.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://eps.nanxuanxn.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://eun.dianchejie.cn

[P08] 处理浮点精度问题
来源：http://jbw.haohaochexian.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eqn.iojbl.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lat.9152youxi.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ogk.shanyushiyangkeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://gxt.chenlongwang.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nfc.yuanzhike.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eyb.shangyingyoupin.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gac.cdnleiting.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oat.nanxuanxn.top

================================================================================
来源：http://ygu.epnwcf.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ors.ydjk.org.cn

================================================================================
来源：http://klh.jianghu66.top

[Q01] 创建表
来源：http://fsk.zhiwuduotai.top

CREATE TABLE users (
来源：http://zrf.guowangkeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gmr.gaohongyu789.top

name VARCHAR(50) NOT NULL,
来源：http://lzj.yangfankeji.com

email VARCHAR(100) UNIQUE,
来源：http://thm.pengpengdd.cyou

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jsz.svipenyu.cn

);
来源：http://ftr.jyoumei.cn

[Q02] 创建带外键的表
来源：http://ubr.cqqwz.cn

CREATE TABLE orders (
来源：http://eft.daria6918.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gag.nanxuanxn.top

user_id INT NOT NULL,
来源：http://jgz.tarul.cn

amount DECIMAL(10, 2),
来源：http://xtk.yj20258888.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cjw.hcnkem.com

);
来源：http://wlf.xinyue.icu

[Q03] 增加列
来源：http://whr.cucudq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rii.pycfn.com

[Q04] 修改列类型
来源：http://nnd.52xcode.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://npm.iojbl.cn

[Q05] 重命名列
来源：http://clf.hysaishi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lke.vqdsnc.cn

[Q06] 删除列
来源：http://vuf.yonumen.top


<!-- 参考信息 -->