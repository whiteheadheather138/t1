代发 wailian999

Ruby: exit 1
来源：http://qmb.ctjpmb.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fkd.zdqjudy.top

[M06] 向标准错误输出
来源：http://ris.yj20258888.top

Py:   print("err", file=sys.stderr)
来源：http://zun.gotoacloud.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ycz.fanxiaobao.xyz

JS:   console.error("err")
来源：http://rlw.xinyue.icu

TS:   console.error("err")
来源：http://siu.yj20258888.top

Java: System.err.println("err")
来源：http://vnl.pycfn.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nfa.tian-w.cn

Ruby: warn "err"
来源：http://szh.zhongyouzk.top

C#:   Console.Error.WriteLine("err")
来源：http://ocg.jiagoushi.top

[M07] 判断是否为主入口
来源：http://vou.jianghu66.top

Py:   if __name__ == "__main__":
来源：http://gku.nanxinkj.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qlh.quarkkingdee.top

JS:   require.main === module
来源：http://yxr.bbcook.cn

TS:   require.main === module
来源：http://khf.fehbvm.com

Java: public static void main(String[] args)
来源：http://qno.yanxiufei.cn

Go:   func main()
来源：http://wsk.mhx1999.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://evl.cdnleiting.top

C#:   static void Main(string[] args)
来源：http://vmu.jyoumei.cn

[M08] 获取系统与运行时信息
来源：http://jbc.yj20258888.top

Py:   platform.system();  platform.python_version()
来源：http://uxq.zhengqikj.top

PHP:  PHP_OS;  phpversion();
来源：http://imx.pycfn.com

JS:   process.platform;  process.version
来源：http://gzs.yangfankeji.com

TS:   process.platform;  process.version
来源：http://jni.birdmap.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://eir.c1oappe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://sji.fktsv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pip.sufxvd.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jxw.quarkkingdee.top

================================================================================
来源：http://ajj.0kj1m.cn

N. 数据结构与算法
来源：http://eng.epnwcf.com

================================================================================
来源：http://icp.tianlin.xyz

[N01] 二分查找（有序数组）
来源：http://fmz.0kj1m.cn

Py:   bisect.bisect_left(arr, x)
来源：http://lym.fehbvm.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qra.yvedp.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hab.yfazqb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jsc.epnwcf.com

Java: Arrays.binarySearch(arr, x)
来源：http://gxw.zhijiandao.cn

Go:   sort.SearchInts(arr, x)
来源：http://veo.xuanzx.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://zol.pycfn.com

C#:   Array.BinarySearch(arr, x)
来源：http://jdz.wangdashe.top

[N02] 排序（工程实践用内置实现）
来源：http://dtj.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://lpw.wangshuangyany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://stu.nanxuanxn.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://zlp.gzhubu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dvs.yj202588.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pey.cucudq.cn

Go:   slices.Sort(arr)
来源：http://thv.jinqigufen.top

Ruby: arr.sort
来源：http://osg.wangdashe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://sgh.jinqigfzy.top

[N03] 快速排序（分治示例）
来源：http://ofr.vqdsnc.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jcs.ppjwa.cn

PHP:  // 递归实现，或用 usort
来源：http://yof.zhixingplan.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ahu.dianchejie.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://quo.chenjidiqi.icu

Java: // 手写递归，或直接用 Arrays.sort
来源：http://tpq.cashguo.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ipb.svipenyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dge.wangshuangyany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ggc.zhoulong.xyz

[N04] 斐波那契数列
来源：http://faq.nanxinkj.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yvv.shuidangran.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://hwn.sxryk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wqc.xuetiantiany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://htr.wangdashe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://olk.zhixingplan.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://shn.ivvv.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vnh.jinghuilouyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qwr.nwbrower.top

[N05] 最大公约数
来源：http://ubc.tianlin.xyz

Py:   math.gcd(a, b)
来源：http://cat.zhiwuduotai.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jee.kuanghao11.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hzr.redwolf501.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://svn.haohaochexian.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qax.hnqzz.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://xul.xingfuxueyuan.xyz

Ruby: a.gcd(b)
来源：http://ejo.wangdashe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://vzv.sufxvd.cn

[N06] 判断回文字符串
来源：http://who.yanxiufei.cn

Py:   s == s[::-1]
来源：http://nqk.jinqigufen.top

PHP:  $s === strrev($s);
来源：http://kuc.hnxiangtu.top

JS:   s === [...s].reverse().join("")
来源：http://qms.snrcjt.cn

TS:   s === [...s].reverse().join("")
来源：http://lco.yongpay.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://cjy.yueranfly.top

Go:   // 双指针从两端比较
来源：http://agw.jianghu66.top

Ruby: s == s.reverse
来源：http://izd.xziqi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://tix.yuanzhike.top

[N07] 两数之和（返回下标）
来源：http://xkn.birdmap.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zrk.jyoumei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ghw.nanxuanxn.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ipw.daria6918.cn

TS:   // 手写 Map<string, number>
来源：http://gzf.316326.xyz

Java: // 手写 HashMap
来源：http://tal.pycfn.com

Go:   // 手写 map[int]int
来源：http://lpu.ppjwa.cn

Ruby: // 手写 Hash
来源：http://pyx.sxryk.cn

C#:   // 手写 Dictionary<int, int>
来源：http://koo.havefunace.top

[N08] 生成全排列
来源：http://ear.epnwcf.com

Py:   itertools.permutations(arr)
来源：http://ktv.chenzaomai.com

PHP:  // 手写递归交换
来源：http://gxo.smart0.xyz

JS:   // 手写回溯递归
来源：http://dax.pycfn.com

TS:   // 手写回溯递归
来源：http://pvl.uphjek.com

Java: // 手写回溯递归
来源：http://sak.tarul.cn

Go:   // 手写回溯递归
来源：http://pyg.chenzaomai.com

Ruby: arr.permutation.to_a
来源：http://zjq.mhx1999.top

C#:   // 手写回溯递归
来源：http://ino.daria6918.cn

[N09] 栈与队列
来源：http://vgb.uphjek.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://jmv.shangyingyoupin.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://zwo.hongshengwenyu.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ajj.jinqigfzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://pvv.yuxming.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fgs.yuxming.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qiz.chenlongwang.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://sqt.zhengqikj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://whd.wangdashe.top

[N10] 链表节点定义
来源：http://awo.zhiwuduotai.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://kpm.fktsv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://dbo.daxiang520.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hny.nanxuanxn.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://abn.hesvh.cn

Java: class Node { int v; Node next; }
来源：http://jij.hongshengwenyu.top

Go:   type Node struct { V int; Next *Node }
来源：http://rcd.ydzc1.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tfc.9152youxi.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://rmr.yonumen.top

[N11] 二叉树中序遍历
来源：http://jhh.pycfn.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://xip.yueranfly.top

PHP:  // 手写递归函数
来源：http://tvs.sysykeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://igw.fanxiaobao.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://spc.fengsongda.top

Java: // 手写递归
来源：http://gsq.yanxiufei.cn

Go:   // 手写递归
来源：http://cbb.shanyushiyangkeji.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ogj.zhiwuduotai.top

C#:   // 手写递归
来源：http://izl.redwolf501.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ill.shuidangran.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://lil.c1oappe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pmk.xinyue.icu

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://klo.zhiwuduotai.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iyl.sxryk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bsj.hongshengwenyu.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ike.sjlbkw.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ivu.guowangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fhp.xuetiantiany.cn

================================================================================
来源：http://zyr.ybcxt.top

O. 并发与异步
来源：http://jyu.aibaodan.cn

================================================================================
来源：http://ssw.nanxuanxn.top

[O01] 启动一个线程
来源：http://ite.jinghuilouyu.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ljq.cucudq.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://hdv.zhijiandao.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qth.bjfxy.top

TS:   // 同 JS
来源：http://odm.aibaodan.cn

Java: new Thread(() -> f()).start()
来源：http://wgu.sxryk.cn

Go:   go f()
来源：http://qww.hcnkem.com

Ruby: Thread.new { f }
来源：http://cdp.epnwcf.com

C#:   Task.Run(() => F());
来源：http://jsx.epnwcf.com

[O02] 使用线程池
来源：http://lai.hongshengwenyu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dft.jqgfzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gqk.sjlbkw.cn

JS:   // worker_threads 线程池
来源：http://hbb.tian-w.cn

TS:   // worker_threads 线程池
来源：http://jqr.ywan-chungtsiang.top

Java: Executors.newFixedThreadPool(4)
来源：http://qmd.9152youxi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ocu.yueranfly.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bdb.xingfuxueyuan.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bni.shanyushiyangkeji.top

[O03] 加锁保护共享数据
来源：http://qav.cashguo.top

Py:   with lock: shared += 1
来源：http://duo.chenlongwang.top

PHP:  // 用 flock() 做文件锁
来源：http://nsh.shuidangran.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dww.sysykeji.top

TS:   // 同 JS
来源：http://vrz.zhongyouzk.top

Java: synchronized (this) { shared++; }
来源：http://dcg.nanxinkj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mon.bbcook.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qgw.shangyingyoupin.top

C#:   lock (gate) { shared++; }
来源：http://tjs.jianghu66.top

[O04] 定义异步函数并等待
来源：http://zpr.hywenlv.cn

Py:   async def f():⏎    await g()
来源：http://ajl.andypj.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bwy.jyoumei.cn

JS:   async function f() { await g(); }
来源：http://ect.daxiang520.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hla.zdqjudy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ccv.smart0.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://prj.xingfuxueyuan.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://uqu.zhiwuduotai.top

C#:   async Task F() { await G(); }
来源：http://jmj.jqgufenzy.top

[O05] 并发执行并等待全部完成
来源：http://rbm.uphjek.com

Py:   asyncio.gather(*tasks)
来源：http://aab.haohaochexian.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://thw.dashuyun.cn

JS:   await Promise.all(tasks)
来源：http://adu.c1oappe.top

TS:   await Promise.all(tasks)
来源：http://cbn.zdbjq.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ueo.andypj.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ovq.yj20258888.top

Ruby: threads.map(&:join)
来源：http://snm.xingfuxueyuan.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://quy.xingfuxueyuan.xyz

[O06] 使用进程池
来源：http://wzl.xuanzx.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://csc.zycfv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://tif.tianlin.xyz

JS:   // child_process / cluster 模块
来源：http://rtw.jqgfzy.top

TS:   // child_process / cluster 模块
来源：http://zox.cucudq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jpw.zhaomingkeji.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wmr.mhx1999.top

Ruby: // fork 块
来源：http://tpp.zhiwuduotai.top

C#:   Parallel.For
来源：http://uqo.sweek.top

================================================================================
来源：http://imx.shangyingyoupin.top

P. 常用工具函数
来源：http://jjk.chenlongwang.top

================================================================================
来源：http://elt.jqgfzy.top

[P01] 生成 UUID
来源：http://hwb.sxryk.cn

Py:   str(uuid.uuid4())
来源：http://nsy.gaohongyu789.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wnr.snrcjt.cn

JS:   crypto.randomUUID()
来源：http://uas.hesvh.cn

TS:   crypto.randomUUID()
来源：http://ywl.ywan-chungtsiang.top

Java: UUID.randomUUID().toString()
来源：http://qla.ivvv.top

Go:   // 用 github.com/google/uuid
来源：http://rpk.shuidangran.top

Ruby: SecureRandom.uuid
来源：http://hvx.chenjidiqi.icu

C#:   Guid.NewGuid().ToString()
来源：http://axu.shangyingyoupin.top

[P02] MD5 / SHA256 摘要
来源：http://sld.fzhhl.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://omw.cdnleiting.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qef.iojbl.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://psg.kuanghao11.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vjf.haohaochexian.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fgk.zhixingplan.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://glv.wangdashe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jyi.tianlin.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ecv.bjfxy.top

[P03] 生成短随机字符串
来源：http://wqk.chenlongwang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dwl.jinyuanbaomall.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wfd.yueranfly.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ybd.yfazqb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kxz.chenjidiqi.icu

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mbr.yj20258.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kds.uphjek.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://lkv.c1oappe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gpq.jyoumei.cn

[P04] 求长度
来源：http://pjb.tarul.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kdn.ppjwa.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bcj.aibaodan.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ghs.nwbrower.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wuv.zdqjudy.top

Java: list.size();  map.size();  s.length()
来源：http://tux.xuanzx.com

Go:   len(arr);  len(m)
来源：http://dem.uphjek.com

Ruby: x.length;  x.size
来源：http://soi.chenlongwang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qsp.cashguo.top

[P05] 判断两个对象内容是否相等
来源：http://ymh.yangfankeji.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://uxd.9152youxi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dpc.shuidangran.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://flt.kuanghao11.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rei.havefunace.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wiw.9152youxi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yfr.birdmap.top

Ruby: a == b
来源：http://cwc.feifeiyinyue.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://icl.jqgfzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gzs.smart0.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vzp.gaohongyu789.top

PHP:  if (empty($x)) {}
来源：http://eel.haohaochexian.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tav.xingfuxueyuan.xyz

TS:   if (x == null) {}
来源：http://bgh.yvedp.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qck.yj20258.top

Go:   if x == nil {}
来源：http://jwe.hywenlv.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fce.iojbl.cn

C#:   if (x is null) {}
来源：http://skm.fanxiaobao.xyz

[P07] 防抖与节流
来源：http://tnr.guannengcc.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tck.wangdashe.top

PHP:  // 手写时间戳比较
来源：http://uaj.xuetiantiany.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jpl.havefunace.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kpe.snrcjt.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qzz.aibaodan.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://obi.yueranfly.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://heg.shuidangran.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://upk.yfazqb.com

[P08] 处理浮点精度问题
来源：http://pmd.fanxiaobao.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://swj.gogol.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vyy.yj20258888.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ynh.nwbrower.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://plv.gotoacloud.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hds.cheryme.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ogq.svipenyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fom.cqqwz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oqq.0kj1m.cn

================================================================================
来源：http://qar.epnwcf.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ldg.ywan-chungtsiang.top

================================================================================
来源：http://huu.zycfv.cn

[Q01] 创建表
来源：http://hqn.ybcxt.top

CREATE TABLE users (
来源：http://eyj.guannengcc.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://sbh.yongpay.top

name VARCHAR(50) NOT NULL,
来源：http://sld.zhijiandao.cn

email VARCHAR(100) UNIQUE,
来源：http://gtg.jqgfzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ond.havefunace.top

);
来源：http://qhb.shangyingyoupin.top

[Q02] 创建带外键的表
来源：http://kxw.yuanzhike.top

CREATE TABLE orders (
来源：http://rwu.zhijiandao.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://yey.gaohongyu789.top

user_id INT NOT NULL,
来源：http://cvc.aibaodan.cn

amount DECIMAL(10, 2),
来源：http://bss.yueranfly.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://drp.feifeiyinyue.top

);
来源：http://hns.wangshuangyany.cn

[Q03] 增加列
来源：http://cjj.guowangkeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ncu.0kj1m.cn

[Q04] 修改列类型
来源：http://jyh.uphjek.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gjz.fehbvm.com

[Q05] 重命名列
来源：http://oyu.quarkkingdee.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fsu.yj20258888.top

[Q06] 删除列
来源：http://vfq.cheryme.top

ALTER TABLE users DROP COLUMN age;
来源：http://fey.wangshuangyany.cn

[Q07] 删除表
来源：http://nai.guannengcc.top

DROP TABLE IF EXISTS orders;
来源：http://sun.zhixingplan.top

[Q08] 创建普通索引
来源：http://elh.shanyushiyangkeji.top


<!-- 参考信息 -->