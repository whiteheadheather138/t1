代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://ryg.zdbjq.cn

JS:   console.error("err")
来源：http://gyy.dashuyun.cn

TS:   console.error("err")
来源：http://jzw.dianchejie.cn

Java: System.err.println("err")
来源：http://ydm.fktsv.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://zus.xziqi.cn

Ruby: warn "err"
来源：http://qxy.chenzaomai.com

C#:   Console.Error.WriteLine("err")
来源：http://vbz.yangfankeji.com

[M07] 判断是否为主入口
来源：http://xoa.9152youxi.cn

Py:   if __name__ == "__main__":
来源：http://zse.yuanzhike.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nrv.sxryk.cn

JS:   require.main === module
来源：http://bab.dashuyun.cn

TS:   require.main === module
来源：http://dpk.pycfn.com

Java: public static void main(String[] args)
来源：http://nqf.kuanghao11.cn

Go:   func main()
来源：http://qtu.cdnleiting.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://iia.dianchejie.cn

C#:   static void Main(string[] args)
来源：http://bna.fktsv.cn

[M08] 获取系统与运行时信息
来源：http://gtd.gotoacloud.top

Py:   platform.system();  platform.python_version()
来源：http://quo.jinghuilouyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://ada.daria6918.cn

JS:   process.platform;  process.version
来源：http://bpd.bbcook.cn

TS:   process.platform;  process.version
来源：http://ndk.chenjidiqi.icu

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hpj.dashuyun.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://zjw.ehwqpu.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://web.sysykeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://uoe.fanxiaobao.xyz

================================================================================
来源：http://zrc.jinghuilouyu.cn

N. 数据结构与算法
来源：http://vlz.shuidangran.top

================================================================================
来源：http://lkl.zhijiandao.cn

[N01] 二分查找（有序数组）
来源：http://hhx.ppjwa.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qlq.haohaochexian.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://oif.sufxvd.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://trf.jqgufenzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qob.nanxinkj.top

Java: Arrays.binarySearch(arr, x)
来源：http://yio.ydzc1.top

Go:   sort.SearchInts(arr, x)
来源：http://ezq.bjfxy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://apf.ydzc1.top

C#:   Array.BinarySearch(arr, x)
来源：http://ljd.cheryme.top

[N02] 排序（工程实践用内置实现）
来源：http://znd.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://ati.nanxuanxn.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://elu.andypj.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://mgo.hesvh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mby.hysaishi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vaa.cqqwz.cn

Go:   slices.Sort(arr)
来源：http://obt.xuanzx.com

Ruby: arr.sort
来源：http://gul.gotoacloud.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qlc.jlsjyb.cn

[N03] 快速排序（分治示例）
来源：http://ycc.hammf.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kqf.shangyingyoupin.top

PHP:  // 递归实现，或用 usort
来源：http://snx.nwbrower.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eau.sysykeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ndr.xylfe.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eye.meibo888.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kgq.kuanghao11.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qxp.tarul.cn

C#:   // 手写递归，或 Array.Sort
来源：http://aum.yuxming.cn

[N04] 斐波那契数列
来源：http://qjc.jiagoushi.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jhv.nanxuanxn.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zai.nanxinkj.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uoi.yj20258.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zsh.fzhhl.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://krz.dashuyun.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ibm.yuanzhike.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://gif.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dbx.shangyingyoupin.top

[N05] 最大公约数
来源：http://qxr.chenjidiqi.icu

Py:   math.gcd(a, b)
来源：http://jip.fengsongda.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://iav.hnxiangtu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://geo.hammf.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qhf.zycfv.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ukg.zycfv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fzj.c1oappe.top

Ruby: a.gcd(b)
来源：http://buo.nanxuanxn.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dba.ywan-chungtsiang.top

[N06] 判断回文字符串
来源：http://ghk.pengpengdd.cyou

Py:   s == s[::-1]
来源：http://kiw.cqqwz.cn

PHP:  $s === strrev($s);
来源：http://awu.daxiang520.top

JS:   s === [...s].reverse().join("")
来源：http://gny.xuanzx.com

TS:   s === [...s].reverse().join("")
来源：http://bdp.yangfankeji.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mpr.ybcxt.top

Go:   // 双指针从两端比较
来源：http://txy.guowangkeji.top

Ruby: s == s.reverse
来源：http://wpu.ivvv.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ztr.fehbvm.com

[N07] 两数之和（返回下标）
来源：http://yjo.zhoulong.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ups.fengsongda.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gzs.fanxiaobao.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://ynm.daria6918.cn

TS:   // 手写 Map<string, number>
来源：http://rnn.yj20258888.top

Java: // 手写 HashMap
来源：http://vmz.ydzc1.top

Go:   // 手写 map[int]int
来源：http://ftc.yj202588.top

Ruby: // 手写 Hash
来源：http://biq.jqgfzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://uzg.zhiwuduotai.top

[N08] 生成全排列
来源：http://ciq.hesvh.cn

Py:   itertools.permutations(arr)
来源：http://cys.sjlbkw.cn

PHP:  // 手写递归交换
来源：http://nen.smart0.xyz

JS:   // 手写回溯递归
来源：http://bzc.zhiwuduotai.top

TS:   // 手写回溯递归
来源：http://etf.bbcook.cn

Java: // 手写回溯递归
来源：http://bny.gogol.net.cn

Go:   // 手写回溯递归
来源：http://cba.birdmap.top

Ruby: arr.permutation.to_a
来源：http://ifj.cheryme.top

C#:   // 手写回溯递归
来源：http://ptn.hywenlv.cn

[N09] 栈与队列
来源：http://cgv.zdbjq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://eoa.fanxiaobao.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mlb.jinqigfzy.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://yvo.gaohongyu789.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://frl.zhongyouzk.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://syc.xziqi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ckz.tarul.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tsf.zhaomingkeji.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://uwa.jinghuilouyu.cn

[N10] 链表节点定义
来源：http://ggj.xylfe.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wat.hnxiangtu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://qrj.hywenlv.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://kwo.yj20258.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://yrh.cheryme.top

Java: class Node { int v; Node next; }
来源：http://dgo.shangyingyoupin.top

Go:   type Node struct { V int; Next *Node }
来源：http://gmv.xingfuxueyuan.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://lgh.nanxuanxn.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ynl.fanxiaobao.xyz

[N11] 二叉树中序遍历
来源：http://qok.yongpay.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lqg.pengpengdd.cyou

PHP:  // 手写递归函数
来源：http://dfu.fzhhl.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xxq.zhixingplan.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pux.svipenyu.cn

Java: // 手写递归
来源：http://phu.zhongyouzk.top

Go:   // 手写递归
来源：http://pft.gaohongyu789.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://reu.zhaomingkeji.xyz

C#:   // 手写递归
来源：http://hxz.hnqzz.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kgx.xingfuxueyuan.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://uzj.daxiang520.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mnh.zhongyouzk.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://myq.ydjk.org.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yow.ywan-chungtsiang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wuh.fengsongda.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wsi.birdmap.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://idk.xingfuxueyuan.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xbn.52xcode.cn

================================================================================
来源：http://dwe.hcnkem.com

O. 并发与异步
来源：http://kby.jinyuanbaomall.cn

================================================================================
来源：http://wsd.nwbrower.top

[O01] 启动一个线程
来源：http://cyu.sjlbkw.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zqa.yongpay.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://iqm.yongpay.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ljl.vehdjk.com

TS:   // 同 JS
来源：http://iyh.redwolf501.top

Java: new Thread(() -> f()).start()
来源：http://iqr.guannengcc.top

Go:   go f()
来源：http://bbf.gzhubu.top

Ruby: Thread.new { f }
来源：http://mlt.ctjpmb.com

C#:   Task.Run(() => F());
来源：http://uak.hfpthk.cn

[O02] 使用线程池
来源：http://ynw.cdnleiting.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pow.ydjk.org.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ojl.svipenyu.cn

JS:   // worker_threads 线程池
来源：http://fsr.yuanzhike.top

TS:   // worker_threads 线程池
来源：http://mgr.316326.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://ebk.zhaomingkeji.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://emc.xinyue.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://obx.hysaishi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jhl.yj20258888.top

[O03] 加锁保护共享数据
来源：http://glj.epnwcf.com

Py:   with lock: shared += 1
来源：http://eyy.hammf.cn

PHP:  // 用 flock() 做文件锁
来源：http://mae.tarul.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hsw.ppjwa.cn

TS:   // 同 JS
来源：http://bqs.fanxiaobao.xyz

Java: synchronized (this) { shared++; }
来源：http://mbc.sysykeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jhi.kuanghao11.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://raa.birdmap.top

C#:   lock (gate) { shared++; }
来源：http://wjp.aizwys.cn

[O04] 定义异步函数并等待
来源：http://yyr.yfazqb.com

Py:   async def f():⏎    await g()
来源：http://gqg.jinqigfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lvj.bjfxy.top

JS:   async function f() { await g(); }
来源：http://lco.xuanzx.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://syu.uphjek.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://cas.hnxiangtu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uac.sweek.top

Ruby: # 用 Fiber 或 async gem
来源：http://zfd.jqgufenzy.top

C#:   async Task F() { await G(); }
来源：http://lcf.ydzc1.top

[O05] 并发执行并等待全部完成
来源：http://oot.sweek.top

Py:   asyncio.gather(*tasks)
来源：http://ajx.shzxlz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qti.jianghu66.top

JS:   await Promise.all(tasks)
来源：http://umo.havefunace.top

TS:   await Promise.all(tasks)
来源：http://xuf.ehwqpu.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://sve.epnwcf.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sur.pycfn.com

Ruby: threads.map(&:join)
来源：http://koi.yj202588.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pbh.yj20258888.top

[O06] 使用进程池
来源：http://bpd.jlsjyb.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jsf.c1oappe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://clv.zdqjudy.top

JS:   // child_process / cluster 模块
来源：http://tvq.uphjek.com

TS:   // child_process / cluster 模块
来源：http://kin.ctjpmb.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://whr.shanyushiyangtech.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ccu.zdqjudy.top

Ruby: // fork 块
来源：http://gjl.dianchejie.cn

C#:   Parallel.For
来源：http://gpr.haohaochexian.top

================================================================================
来源：http://uwh.xinyue.icu

P. 常用工具函数
来源：http://bhf.cqqwz.cn

================================================================================
来源：http://yvf.daxiang520.top

[P01] 生成 UUID
来源：http://nel.pengpengdd.cyou

Py:   str(uuid.uuid4())
来源：http://doq.yongpay.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sfl.haohaochexian.top

JS:   crypto.randomUUID()
来源：http://kfc.tanke756.top

TS:   crypto.randomUUID()
来源：http://law.zhiwuduotai.top

Java: UUID.randomUUID().toString()
来源：http://ihi.xylfe.cn

Go:   // 用 github.com/google/uuid
来源：http://wrk.shanyushiyangkeji.top

Ruby: SecureRandom.uuid
来源：http://osg.andypj.xyz

C#:   Guid.NewGuid().ToString()
来源：http://sdb.yj20258.top

[P02] MD5 / SHA256 摘要
来源：http://sjm.guowangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mvj.quarkkingdee.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://lsr.zdqjudy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cbg.sweek.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zcv.snrcjt.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kbp.zdqjudy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://oui.jlsjyb.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pzf.vqdsnc.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ixk.cucudq.cn

[P03] 生成短随机字符串
来源：http://guy.birdmap.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://chb.gogol.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qdt.zhaomingkeji.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bcg.ehwqpu.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sej.zhijiandao.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gxn.jqgufenzy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lau.vqdsnc.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://laf.vqdsnc.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jfe.snrcjt.cn

[P04] 求长度
来源：http://yob.guowangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qwt.zhongyouzk.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tll.yanxiufei.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://myv.jyoumei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tfr.sweek.top

Java: list.size();  map.size();  s.length()
来源：http://lwf.jinghuilouyu.cn

Go:   len(arr);  len(m)
来源：http://gnx.svipenyu.cn

Ruby: x.length;  x.size
来源：http://xhi.daria6918.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hlh.ppjwa.cn

[P05] 判断两个对象内容是否相等
来源：http://gkg.wangdashe.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://qij.fzhhl.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bsc.pengpengdd.cyou

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lqi.jiagoushi.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lkf.mhx1999.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nrq.52xcode.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ems.daria6918.cn

Ruby: a == b
来源：http://bjf.ydjk.org.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wea.jianghu66.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rno.fanxiaobao.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ocs.yonumen.top

PHP:  if (empty($x)) {}
来源：http://jbh.sxryk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vkp.gaohongyu789.top

TS:   if (x == null) {}
来源：http://zff.smart0.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://asi.yfazqb.com

Go:   if x == nil {}
来源：http://row.zhixingplan.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://stl.zhoulong.xyz

C#:   if (x is null) {}
来源：http://tke.hfpthk.cn

[P07] 防抖与节流
来源：http://cxx.xylfe.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tsy.snrcjt.cn

PHP:  // 手写时间戳比较
来源：http://awa.hammf.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kle.pengpengdd.cyou

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://odd.zdbjq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zhj.xylfe.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://awb.jinghuilouyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zhq.vqdsnc.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://csy.tianlin.xyz

[P08] 处理浮点精度问题
来源：http://jkh.sjlbkw.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vpy.xinyue.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xnt.yonumen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dai.tanke756.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rwv.chenjidiqi.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vyj.fzhhl.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qky.yfazqb.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wan.pengpengdd.cyou

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wmt.vehdjk.com

================================================================================
来源：http://zkt.tanke756.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wnx.zdbjq.cn

================================================================================
来源：http://ddk.meibo888.top

[Q01] 创建表
来源：http://iaj.shangyingyoupin.top

CREATE TABLE users (
来源：http://bss.zhijiandao.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rou.meibo888.top

name VARCHAR(50) NOT NULL,
来源：http://yqt.zhongyouzk.top

email VARCHAR(100) UNIQUE,
来源：http://ebi.gotoacloud.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nrz.yongpay.top

);
来源：http://jnh.yonumen.top

[Q02] 创建带外键的表
来源：http://oxl.gogol.net.cn

CREATE TABLE orders (
来源：http://elr.nanxuanxn.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fyn.cqqwz.cn

user_id INT NOT NULL,
来源：http://zpy.tianlin.xyz

amount DECIMAL(10, 2),
来源：http://rlk.shangyingyoupin.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://emc.c1oappe.top

);
来源：http://lph.hongshengwenyu.top

[Q03] 增加列
来源：http://xjg.gzhubu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://olo.vehdjk.com

[Q04] 修改列类型
来源：http://qtz.yfazqb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fhq.nwbrower.top

[Q05] 重命名列
来源：http://ksq.yvedp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://joy.jqgufenzy.top

[Q06] 删除列
来源：http://zvr.sufxvd.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kkv.zdqjudy.top

[Q07] 删除表
来源：http://uud.xziqi.cn

DROP TABLE IF EXISTS orders;
来源：http://woc.sjlbkw.cn

[Q08] 创建普通索引
来源：http://tll.hfpthk.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kwj.jqgufenzy.top

[Q09] 创建唯一索引
来源：http://vxc.316326.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xem.kuanghao11.cn

[Q10] 插入单行
来源：http://dco.dianchejie.cn


<!-- 参考信息 -->