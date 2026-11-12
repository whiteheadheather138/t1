代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://qrr.jyoumei.cn

Ruby: warn "err"
来源：http://oau.zdbjq.cn

C#:   Console.Error.WriteLine("err")
来源：http://ved.gogol.net.cn

[M07] 判断是否为主入口
来源：http://wvg.fengsongda.top

Py:   if __name__ == "__main__":
来源：http://ybo.aibaodan.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sku.jinqigufen.top

JS:   require.main === module
来源：http://jgg.jqgufenzy.top

TS:   require.main === module
来源：http://ehc.xylfe.cn

Java: public static void main(String[] args)
来源：http://fqv.redwolf501.top

Go:   func main()
来源：http://jmr.aizwys.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ylm.ydjk.org.cn

C#:   static void Main(string[] args)
来源：http://ttg.ywan-chungtsiang.top

[M08] 获取系统与运行时信息
来源：http://wif.chenjidiqi.icu

Py:   platform.system();  platform.python_version()
来源：http://dfx.zhoulong.xyz

PHP:  PHP_OS;  phpversion();
来源：http://vgx.shanyushiyangkeji.top

JS:   process.platform;  process.version
来源：http://bob.bjfxy.top

TS:   process.platform;  process.version
来源：http://pre.yj202588.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ozg.sjlbkw.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ksw.sufxvd.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://oid.zhaomingkeji.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://puv.jiagoushi.top

================================================================================
来源：http://psn.fzhhl.top

N. 数据结构与算法
来源：http://ocr.chenjidiqi.icu

================================================================================
来源：http://opt.epnwcf.com

[N01] 二分查找（有序数组）
来源：http://mai.ybcxt.top

Py:   bisect.bisect_left(arr, x)
来源：http://odr.52xcode.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bqv.guannengcc.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xwb.epnwcf.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kky.gogol.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lwr.xingfuxueyuan.xyz

Go:   sort.SearchInts(arr, x)
来源：http://gqp.jinghuilouyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://vat.jianghu66.top

C#:   Array.BinarySearch(arr, x)
来源：http://ens.yueranfly.top

[N02] 排序（工程实践用内置实现）
来源：http://vzh.chenjidiqi.icu

Py:   sorted(arr);  arr.sort()
来源：http://bcx.zhijiandao.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wiu.bbcook.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lfn.vehdjk.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://ddw.zhoulong.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rgz.9152youxi.cn

Go:   slices.Sort(arr)
来源：http://gdg.yonumen.top

Ruby: arr.sort
来源：http://bml.jqgufenzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://zzq.jyoumei.cn

[N03] 快速排序（分治示例）
来源：http://cdp.dianchejie.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fvt.zhijiandao.cn

PHP:  // 递归实现，或用 usort
来源：http://ade.jqgufenzy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vep.yonumen.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lvv.hnxiangtu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yxq.hnqzz.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dik.hfpthk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mhb.daxiang520.top

C#:   // 手写递归，或 Array.Sort
来源：http://ddb.zhijiandao.cn

[N04] 斐波那契数列
来源：http://zfs.quarkkingdee.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hgb.vqdsnc.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yzo.52xcode.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gvt.shuidangran.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vwp.gzhubu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vpc.uphjek.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fjf.mhx1999.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hpa.fzhhl.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bmm.9152youxi.cn

[N05] 最大公约数
来源：http://hia.cashguo.top

Py:   math.gcd(a, b)
来源：http://vls.xuetiantiany.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eva.yongpay.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://epl.bbcook.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nyh.yangfankeji.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hmb.cashguo.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dny.tanke756.top

Ruby: a.gcd(b)
来源：http://ppt.zhiwuduotai.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mmk.ivvv.top

[N06] 判断回文字符串
来源：http://myv.zhixingplan.top

Py:   s == s[::-1]
来源：http://ind.sxryk.cn

PHP:  $s === strrev($s);
来源：http://psp.shangyingyoupin.top

JS:   s === [...s].reverse().join("")
来源：http://lsn.redwolf501.top

TS:   s === [...s].reverse().join("")
来源：http://qow.zhixingplan.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yvw.tarul.cn

Go:   // 双指针从两端比较
来源：http://uuc.ydzc1.top

Ruby: s == s.reverse
来源：http://eqz.tian-w.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://zfm.jqgufenzy.top

[N07] 两数之和（返回下标）
来源：http://jdb.tianlin.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://iqb.kuanghao11.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rmp.kuanghao11.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://isn.aizwys.cn

TS:   // 手写 Map<string, number>
来源：http://biy.sjlbkw.cn

Java: // 手写 HashMap
来源：http://efk.mhx1999.top

Go:   // 手写 map[int]int
来源：http://two.tian-w.cn

Ruby: // 手写 Hash
来源：http://fxj.zhijiandao.cn

C#:   // 手写 Dictionary<int, int>
来源：http://ios.9152youxi.cn

[N08] 生成全排列
来源：http://csm.bbcook.cn

Py:   itertools.permutations(arr)
来源：http://qpg.gogol.net.cn

PHP:  // 手写递归交换
来源：http://pbb.shanyushiyangkeji.top

JS:   // 手写回溯递归
来源：http://skx.yonumen.top

TS:   // 手写回溯递归
来源：http://hst.daria6918.cn

Java: // 手写回溯递归
来源：http://kad.bjfxy.top

Go:   // 手写回溯递归
来源：http://wiv.pengpengdd.cyou

Ruby: arr.permutation.to_a
来源：http://qmv.yj20258.top

C#:   // 手写回溯递归
来源：http://bua.zdbjq.cn

[N09] 栈与队列
来源：http://jss.bjfxy.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://kym.xuanzx.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ghr.svipenyu.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://qty.hnqzz.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hii.snrcjt.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://yyj.tianlin.xyz

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://iro.gzhubu.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://oxi.feifeiyinyue.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://amt.hfpthk.cn

[N10] 链表节点定义
来源：http://faj.svipenyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://giv.quarkkingdee.top

PHP:  class Node { public $v; public $next = null; }
来源：http://rri.hcnkem.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://cyu.shanyushiyangkeji.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jqo.hnqzz.top

Java: class Node { int v; Node next; }
来源：http://psc.yfazqb.com

Go:   type Node struct { V int; Next *Node }
来源：http://vax.mhx1999.top

Ruby: Node = Struct.new(:v, :next)
来源：http://sun.fktsv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://axs.tarul.cn

[N11] 二叉树中序遍历
来源：http://mhy.sweek.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://kut.uphjek.com

PHP:  // 手写递归函数
来源：http://kkf.gzhubu.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vbw.hcnkem.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://erv.chenlongwang.top

Java: // 手写递归
来源：http://snd.zdqjudy.top

Go:   // 手写递归
来源：http://rzz.tianlin.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://psy.ydzc1.top

C#:   // 手写递归
来源：http://kxl.guowangkeji.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://npj.gaohongyu789.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wro.ybcxt.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jww.gotoacloud.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rji.jinyuanbaomall.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zzx.bjfxy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rci.c1oappe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nai.pengpengdd.cyou

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fjz.ywan-chungtsiang.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ptz.quarkkingdee.top

================================================================================
来源：http://tph.zhoulong.xyz

O. 并发与异步
来源：http://ifd.sweek.top

================================================================================
来源：http://gre.pengpengdd.cyou

[O01] 启动一个线程
来源：http://acn.shanyushiyangtech.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xyx.tianlin.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fup.ivvv.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vum.zhoulong.xyz

TS:   // 同 JS
来源：http://hze.quarkkingdee.top

Java: new Thread(() -> f()).start()
来源：http://wfp.fktsv.cn

Go:   go f()
来源：http://afr.zdqjudy.top

Ruby: Thread.new { f }
来源：http://nbk.uphjek.com

C#:   Task.Run(() => F());
来源：http://sfw.chenzaomai.com

[O02] 使用线程池
来源：http://knk.andypj.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tfp.zhixingplan.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fbs.aizwys.cn

JS:   // worker_threads 线程池
来源：http://kuf.fengsongda.top

TS:   // worker_threads 线程池
来源：http://dig.cqqwz.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ppm.sxryk.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mxm.quarkkingdee.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hqg.zhoulong.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://slh.sufxvd.cn

[O03] 加锁保护共享数据
来源：http://mfu.nanxuanxn.top

Py:   with lock: shared += 1
来源：http://cfg.ywan-chungtsiang.top

PHP:  // 用 flock() 做文件锁
来源：http://cqb.guowangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xqk.zhengqikj.top

TS:   // 同 JS
来源：http://iit.gzhubu.top

Java: synchronized (this) { shared++; }
来源：http://uql.yanxiufei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ylf.ctjpmb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://biu.epnwcf.com

C#:   lock (gate) { shared++; }
来源：http://ktm.meibo888.top

[O04] 定义异步函数并等待
来源：http://xec.fktsv.cn

Py:   async def f():⏎    await g()
来源：http://csl.hcnkem.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qvo.cqqwz.cn

JS:   async function f() { await g(); }
来源：http://keo.guowangkeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://nia.cheryme.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ebs.yonumen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jdz.dashuyun.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wqt.zycfv.cn

C#:   async Task F() { await G(); }
来源：http://bsz.jinyuanbaomall.cn

[O05] 并发执行并等待全部完成
来源：http://iyy.jinyuanbaomall.cn

Py:   asyncio.gather(*tasks)
来源：http://lpc.guannengcc.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dsu.zdqjudy.top

JS:   await Promise.all(tasks)
来源：http://bpb.jqgfzy.top

TS:   await Promise.all(tasks)
来源：http://ljj.chenzaomai.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nzw.sufxvd.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mue.wangshuangyany.cn

Ruby: threads.map(&:join)
来源：http://fcb.hnxiangtu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ucq.iojbl.cn

[O06] 使用进程池
来源：http://lai.xuanzx.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mnt.cdnleiting.top

PHP:  // pcntl_fork 或多进程队列
来源：http://gyv.dianchejie.cn

JS:   // child_process / cluster 模块
来源：http://kgk.svipenyu.cn

TS:   // child_process / cluster 模块
来源：http://wsi.jlsjyb.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gwv.vqdsnc.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mzg.zhixingplan.top

Ruby: // fork 块
来源：http://pvn.dashuyun.cn

C#:   Parallel.For
来源：http://nuq.316326.xyz

================================================================================
来源：http://imk.andypj.xyz

P. 常用工具函数
来源：http://dbk.shuidangran.top

================================================================================
来源：http://inc.cqqwz.cn

[P01] 生成 UUID
来源：http://bfo.xinyue.icu

Py:   str(uuid.uuid4())
来源：http://tsl.ybcxt.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tkt.yongpay.top

JS:   crypto.randomUUID()
来源：http://lrr.zhixingplan.top

TS:   crypto.randomUUID()
来源：http://iym.yj20258.top

Java: UUID.randomUUID().toString()
来源：http://opk.jqgfzy.top

Go:   // 用 github.com/google/uuid
来源：http://zvb.quarkkingdee.top

Ruby: SecureRandom.uuid
来源：http://unx.shanyushiyangtech.top

C#:   Guid.NewGuid().ToString()
来源：http://ayz.fengsongda.top

[P02] MD5 / SHA256 摘要
来源：http://jnh.bjfxy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://foi.zhoulong.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://krr.sysykeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xzh.jlsjyb.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://api.epnwcf.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cbw.yangfankeji.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qvn.nwbrower.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lqz.cqqwz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://obz.jiagoushi.top

[P03] 生成短随机字符串
来源：http://awy.zhaomingkeji.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ldx.jianghu66.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://frd.cashguo.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kma.zhijiandao.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ukm.yangfankeji.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cgn.ehwqpu.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bzv.kuanghao11.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xnx.daria6918.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cvi.vqdsnc.cn

[P04] 求长度
来源：http://znm.vqdsnc.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pwg.shanyushiyangtech.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dwv.yvedp.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jzb.zhongyouzk.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://txa.yangfankeji.com

Java: list.size();  map.size();  s.length()
来源：http://cld.xuanzx.com

Go:   len(arr);  len(m)
来源：http://gis.andypj.xyz

Ruby: x.length;  x.size
来源：http://hyj.zhijiandao.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wgw.epnwcf.com

[P05] 判断两个对象内容是否相等
来源：http://pwl.52xcode.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xbr.ctjpmb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ods.jinqigufen.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bba.ehwqpu.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vzg.xylfe.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qbk.fanxiaobao.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://rcz.zhongyouzk.top

Ruby: a == b
来源：http://csc.zhiwuduotai.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://oiq.zdbjq.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rtw.yonumen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pip.hesvh.cn

PHP:  if (empty($x)) {}
来源：http://rkt.dianchejie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://huv.jianghu66.top

TS:   if (x == null) {}
来源：http://upf.jinqigfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://exy.redwolf501.top

Go:   if x == nil {}
来源：http://hid.gaohongyu789.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://urj.yueranfly.top

C#:   if (x is null) {}
来源：http://lcx.yfazqb.com

[P07] 防抖与节流
来源：http://phc.hesvh.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://alz.andypj.xyz

PHP:  // 手写时间戳比较
来源：http://clm.hesvh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nhd.fehbvm.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wqs.wangdashe.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zpc.kuanghao11.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yti.ydjk.org.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ahv.wangshuangyany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tsd.yvedp.cn

[P08] 处理浮点精度问题
来源：http://won.chenlongwang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mki.hnqzz.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gwg.chenjidiqi.icu

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://myv.fehbvm.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fox.fehbvm.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wib.shanyushiyangtech.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lht.cheryme.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jwo.xylfe.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qjj.ehwqpu.com

================================================================================
来源：http://leo.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qkx.fktsv.cn

================================================================================
来源：http://mcw.quarkkingdee.top

[Q01] 创建表
来源：http://upq.yvedp.cn

CREATE TABLE users (
来源：http://lfa.aibaodan.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zaj.fengsongda.top

name VARCHAR(50) NOT NULL,
来源：http://lkn.tanke756.top

email VARCHAR(100) UNIQUE,
来源：http://dup.0kj1m.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ffd.jyoumei.cn

);
来源：http://qtr.ywan-chungtsiang.top

[Q02] 创建带外键的表
来源：http://hxn.gaohongyu789.top

CREATE TABLE orders (
来源：http://pbu.tian-w.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uha.ydjk.org.cn

user_id INT NOT NULL,
来源：http://akm.daxiang520.top

amount DECIMAL(10, 2),
来源：http://ogz.sweek.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jrn.vqdsnc.cn

);
来源：http://hsh.aizwys.cn

[Q03] 增加列
来源：http://rez.pycfn.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xfa.cqqwz.cn

[Q04] 修改列类型
来源：http://mkc.svipenyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mxc.sxryk.cn

[Q05] 重命名列
来源：http://agt.yuxming.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qeo.gogol.net.cn

[Q06] 删除列
来源：http://yml.gzhubu.top

ALTER TABLE users DROP COLUMN age;
来源：http://bgn.ppjwa.cn

[Q07] 删除表
来源：http://jlx.nanxuanxn.top

DROP TABLE IF EXISTS orders;
来源：http://ilr.daria6918.cn

[Q08] 创建普通索引
来源：http://vkm.pycfn.com

CREATE INDEX idx_users_email ON users(email);
来源：http://qot.fzhhl.top

[Q09] 创建唯一索引
来源：http://fsc.zycfv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ptv.yj20258888.top

[Q10] 插入单行
来源：http://duu.xuetiantiany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://chm.sysykeji.top

[Q11] 一次插入多行
来源：http://opl.epnwcf.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tlc.daxiang520.top

[Q12] 插入后取自增 ID
来源：http://vyt.aibaodan.cn


<!-- 参考信息 -->