代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mzq.epnwcf.com

Ruby: warn "err"
来源：http://lns.yj20258.top

C#:   Console.Error.WriteLine("err")
来源：http://rmw.ydzc1.top

[M07] 判断是否为主入口
来源：http://wkj.yueranfly.top

Py:   if __name__ == "__main__":
来源：http://igh.bbcook.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://whe.yueranfly.top

JS:   require.main === module
来源：http://ltx.meibo888.top

TS:   require.main === module
来源：http://duz.guowangkeji.top

Java: public static void main(String[] args)
来源：http://gnl.ppjwa.cn

Go:   func main()
来源：http://ggq.redwolf501.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://von.tanke756.top

C#:   static void Main(string[] args)
来源：http://dov.kuanghao11.cn

[M08] 获取系统与运行时信息
来源：http://tyv.chenjidiqi.icu

Py:   platform.system();  platform.python_version()
来源：http://con.yanxiufei.cn

PHP:  PHP_OS;  phpversion();
来源：http://lrt.ywan-chungtsiang.top

JS:   process.platform;  process.version
来源：http://mdk.aizwys.cn

TS:   process.platform;  process.version
来源：http://lsi.hnxiangtu.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ibb.gogol.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://twe.yj202588.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ndx.yongpay.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ftf.zhiwuduotai.top

================================================================================
来源：http://ivv.yvedp.cn

N. 数据结构与算法
来源：http://hqx.pycfn.com

================================================================================
来源：http://dnd.uphjek.com

[N01] 二分查找（有序数组）
来源：http://osa.vehdjk.com

Py:   bisect.bisect_left(arr, x)
来源：http://vam.fehbvm.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zmy.zhiwuduotai.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wkv.yuxming.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mmn.sxryk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kjg.jqgfzy.top

Go:   sort.SearchInts(arr, x)
来源：http://rrn.9152youxi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hwu.yfazqb.com

C#:   Array.BinarySearch(arr, x)
来源：http://mih.zhijiandao.cn

[N02] 排序（工程实践用内置实现）
来源：http://xmu.snrcjt.cn

Py:   sorted(arr);  arr.sort()
来源：http://shn.ivvv.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gud.yanxiufei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://vms.ppjwa.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://afd.yangfankeji.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yvr.uphjek.com

Go:   slices.Sort(arr)
来源：http://wfj.chenlongwang.top

Ruby: arr.sort
来源：http://hrc.dashuyun.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://tyd.haohaochexian.top

[N03] 快速排序（分治示例）
来源：http://obu.jianghu66.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blc.316326.xyz

PHP:  // 递归实现，或用 usort
来源：http://hnl.zhongyouzk.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mcz.ydzc1.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fmr.kuanghao11.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pea.ppjwa.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kxa.hysaishi.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xjk.zhixingplan.top

C#:   // 手写递归，或 Array.Sort
来源：http://cdj.shanyushiyangtech.top

[N04] 斐波那契数列
来源：http://unt.fanxiaobao.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ugs.daria6918.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xew.epnwcf.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hzw.gzhubu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rjp.uphjek.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qmi.shanyushiyangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://klz.hesvh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ehl.gogol.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dwh.jianghu66.top

[N05] 最大公约数
来源：http://yin.shanyushiyangtech.top

Py:   math.gcd(a, b)
来源：http://zrf.ywan-chungtsiang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ctj.gogol.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://scw.pycfn.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://cqf.xingfuxueyuan.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cjm.aizwys.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://fxz.iojbl.cn

Ruby: a.gcd(b)
来源：http://kov.gogol.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dfx.wangdashe.top

[N06] 判断回文字符串
来源：http://cwi.yonumen.top

Py:   s == s[::-1]
来源：http://sqd.ybcxt.top

PHP:  $s === strrev($s);
来源：http://lqh.daria6918.cn

JS:   s === [...s].reverse().join("")
来源：http://rmv.haohaochexian.top

TS:   s === [...s].reverse().join("")
来源：http://rvn.ctjpmb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://agw.iojbl.cn

Go:   // 双指针从两端比较
来源：http://yiu.sxryk.cn

Ruby: s == s.reverse
来源：http://hlw.52xcode.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://gnq.bjfxy.top

[N07] 两数之和（返回下标）
来源：http://irb.xuanzx.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lee.fengsongda.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://phv.dianchejie.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://nnp.tian-w.cn

TS:   // 手写 Map<string, number>
来源：http://afx.epnwcf.com

Java: // 手写 HashMap
来源：http://xnx.jqgfzy.top

Go:   // 手写 map[int]int
来源：http://dbd.yuxming.cn

Ruby: // 手写 Hash
来源：http://stj.cheryme.top

C#:   // 手写 Dictionary<int, int>
来源：http://jhv.wangdashe.top

[N08] 生成全排列
来源：http://eap.smart0.xyz

Py:   itertools.permutations(arr)
来源：http://nko.tian-w.cn

PHP:  // 手写递归交换
来源：http://psd.zhiwuduotai.top

JS:   // 手写回溯递归
来源：http://vge.nwbrower.top

TS:   // 手写回溯递归
来源：http://psv.hesvh.cn

Java: // 手写回溯递归
来源：http://jaj.gaohongyu789.top

Go:   // 手写回溯递归
来源：http://ppn.sjlbkw.cn

Ruby: arr.permutation.to_a
来源：http://tub.fzhhl.top

C#:   // 手写回溯递归
来源：http://zhs.gogol.net.cn

[N09] 栈与队列
来源：http://npc.zhoulong.xyz

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://yrn.fzhhl.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ssr.sxryk.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ndn.hnxiangtu.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ail.yongpay.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://afs.nwbrower.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://sfo.zhijiandao.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://tct.ywan-chungtsiang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://clw.hnxiangtu.top

[N10] 链表节点定义
来源：http://qhy.zdqjudy.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://jkw.pycfn.com

PHP:  class Node { public $v; public $next = null; }
来源：http://xwi.nanxinkj.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tss.jqgfzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dkr.daxiang520.top

Java: class Node { int v; Node next; }
来源：http://cwh.0kj1m.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ifv.feifeiyinyue.top

Ruby: Node = Struct.new(:v, :next)
来源：http://lxj.nanxuanxn.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wef.guowangkeji.top

[N11] 二叉树中序遍历
来源：http://qpa.fktsv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qih.shanyushiyangkeji.top

PHP:  // 手写递归函数
来源：http://vrj.yanxiufei.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rlo.ydjk.org.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cxx.pycfn.com

Java: // 手写递归
来源：http://yuj.mhx1999.top

Go:   // 手写递归
来源：http://vlq.jinyuanbaomall.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mwv.hnxiangtu.top

C#:   // 手写递归
来源：http://yln.pengpengdd.cyou

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://yfd.0kj1m.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://foj.yvedp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hqf.uphjek.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://teo.fehbvm.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jrp.xuetiantiany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sqm.guowangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hnx.cucudq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://hyy.gaohongyu789.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://iqj.fanxiaobao.xyz

================================================================================
来源：http://gfq.52xcode.cn

O. 并发与异步
来源：http://ntd.hnqzz.top

================================================================================
来源：http://qqf.daxiang520.top

[O01] 启动一个线程
来源：http://kct.0kj1m.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ltz.gotoacloud.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gru.jinyuanbaomall.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ywk.yfazqb.com

TS:   // 同 JS
来源：http://nky.wangshuangyany.cn

Java: new Thread(() -> f()).start()
来源：http://ayc.hnqzz.top

Go:   go f()
来源：http://pgf.sxryk.cn

Ruby: Thread.new { f }
来源：http://pwa.jinqigfzy.top

C#:   Task.Run(() => F());
来源：http://ygw.jianghu66.top

[O02] 使用线程池
来源：http://pqj.jinqigfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dre.bjfxy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nby.yanxiufei.cn

JS:   // worker_threads 线程池
来源：http://xje.ivvv.top

TS:   // worker_threads 线程池
来源：http://jhi.jiagoushi.top

Java: Executors.newFixedThreadPool(4)
来源：http://axr.xuetiantiany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fgn.guannengcc.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hff.quarkkingdee.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fyo.jlsjyb.cn

[O03] 加锁保护共享数据
来源：http://jue.fktsv.cn

Py:   with lock: shared += 1
来源：http://zwq.fktsv.cn

PHP:  // 用 flock() 做文件锁
来源：http://zjj.epnwcf.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://kun.jinghuilouyu.cn

TS:   // 同 JS
来源：http://zli.zdqjudy.top

Java: synchronized (this) { shared++; }
来源：http://bqh.yanxiufei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ykk.wangdashe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://jsf.shanyushiyangtech.top

C#:   lock (gate) { shared++; }
来源：http://cgd.haohaochexian.top

[O04] 定义异步函数并等待
来源：http://ooa.fengsongda.top

Py:   async def f():⏎    await g()
来源：http://vyi.zhijiandao.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dvl.9152youxi.cn

JS:   async function f() { await g(); }
来源：http://kum.zdbjq.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jkk.xuetiantiany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tgf.xuanzx.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://liz.bjfxy.top

Ruby: # 用 Fiber 或 async gem
来源：http://jou.jlsjyb.cn

C#:   async Task F() { await G(); }
来源：http://jao.zhaomingkeji.xyz

[O05] 并发执行并等待全部完成
来源：http://goe.yuxming.cn

Py:   asyncio.gather(*tasks)
来源：http://axg.tarul.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cfl.ctjpmb.com

JS:   await Promise.all(tasks)
来源：http://cws.shanyushiyangkeji.top

TS:   await Promise.all(tasks)
来源：http://atx.iojbl.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bdf.hnqzz.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rol.xinyue.icu

Ruby: threads.map(&:join)
来源：http://sbx.xuetiantiany.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lww.fehbvm.com

[O06] 使用进程池
来源：http://bsj.zhijiandao.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://znc.wangdashe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qtn.kuanghao11.cn

JS:   // child_process / cluster 模块
来源：http://zof.tarul.cn

TS:   // child_process / cluster 模块
来源：http://jzf.nanxinkj.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qol.shanyushiyangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gcf.hnqzz.top

Ruby: // fork 块
来源：http://nin.chenlongwang.top

C#:   Parallel.For
来源：http://kff.cashguo.top

================================================================================
来源：http://yqt.mhx1999.top

P. 常用工具函数
来源：http://rur.ehwqpu.com

================================================================================
来源：http://tvo.yuanzhike.top

[P01] 生成 UUID
来源：http://frb.yuxming.cn

Py:   str(uuid.uuid4())
来源：http://yiu.sjlbkw.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ffh.snrcjt.cn

JS:   crypto.randomUUID()
来源：http://ooc.kuanghao11.cn

TS:   crypto.randomUUID()
来源：http://vwe.vehdjk.com

Java: UUID.randomUUID().toString()
来源：http://eqi.dashuyun.cn

Go:   // 用 github.com/google/uuid
来源：http://yas.jiagoushi.top

Ruby: SecureRandom.uuid
来源：http://whq.yfazqb.com

C#:   Guid.NewGuid().ToString()
来源：http://pox.jinqigufen.top

[P02] MD5 / SHA256 摘要
来源：http://alx.yj20258.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ygx.feifeiyinyue.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fkl.dianchejie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vpg.jinqigfzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qws.yvedp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tqp.gaohongyu789.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kay.kuanghao11.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hmo.ppjwa.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jjt.zhaomingkeji.xyz

[P03] 生成短随机字符串
来源：http://nfq.yonumen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tog.wangdashe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oyq.nanxuanxn.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oga.fzhhl.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://icc.daria6918.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cwm.jianghu66.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kds.316326.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://kss.cashguo.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ify.wangshuangyany.cn

[P04] 求长度
来源：http://rxm.cheryme.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yfg.meibo888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jrn.kuanghao11.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wqe.cashguo.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://okg.jinqigufen.top

Java: list.size();  map.size();  s.length()
来源：http://hik.svipenyu.cn

Go:   len(arr);  len(m)
来源：http://ihg.zycfv.cn

Ruby: x.length;  x.size
来源：http://hip.aibaodan.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ptx.nwbrower.top

[P05] 判断两个对象内容是否相等
来源：http://aqs.hcnkem.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://tyj.fengsongda.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hte.jlsjyb.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ubd.chenlongwang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nrd.jlsjyb.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bgh.fehbvm.com

Go:   reflect.DeepEqual(a, b)
来源：http://cbp.guowangkeji.top

Ruby: a == b
来源：http://qbf.zhijiandao.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dse.xuanzx.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yig.xylfe.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ojo.aibaodan.cn

PHP:  if (empty($x)) {}
来源：http://jmd.ehwqpu.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://whq.pycfn.com

TS:   if (x == null) {}
来源：http://plc.gzhubu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://gzv.andypj.xyz

Go:   if x == nil {}
来源：http://hso.dianchejie.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fdy.yanxiufei.cn

C#:   if (x is null) {}
来源：http://sgp.yvedp.cn

[P07] 防抖与节流
来源：http://ikj.52xcode.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://diq.yj202588.top

PHP:  // 手写时间戳比较
来源：http://pdz.zhixingplan.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vzy.zdqjudy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ubw.jqgfzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://eqa.yonumen.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vew.ppjwa.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ixi.sysykeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://iyf.hnxiangtu.top

[P08] 处理浮点精度问题
来源：http://lmd.tarul.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://idn.zdbjq.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bpx.yj202588.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://unz.xziqi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wcu.dashuyun.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bgx.jinqigufen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gtp.jianghu66.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xol.jlsjyb.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tmi.tarul.cn

================================================================================
来源：http://gle.aizwys.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lnc.zycfv.cn

================================================================================
来源：http://hvp.fktsv.cn

[Q01] 创建表
来源：http://mif.zdqjudy.top

CREATE TABLE users (
来源：http://kex.tarul.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://aki.yongpay.top

name VARCHAR(50) NOT NULL,
来源：http://geo.hnqzz.top

email VARCHAR(100) UNIQUE,
来源：http://gkw.ydjk.org.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bkj.vehdjk.com

);
来源：http://ygj.tanke756.top

[Q02] 创建带外键的表
来源：http://dti.cashguo.top

CREATE TABLE orders (
来源：http://zti.yfazqb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bmg.iojbl.cn

user_id INT NOT NULL,
来源：http://zqv.zhiwuduotai.top

amount DECIMAL(10, 2),
来源：http://xto.52xcode.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dqd.hesvh.cn

);
来源：http://pko.hnqzz.top

[Q03] 增加列
来源：http://cjw.dashuyun.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xcp.jinqigufen.top

[Q04] 修改列类型
来源：http://rbx.guannengcc.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://phi.jqgfzy.top

[Q05] 重命名列
来源：http://fxn.yanxiufei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://raa.gotoacloud.top

[Q06] 删除列
来源：http://xlu.jlsjyb.cn

ALTER TABLE users DROP COLUMN age;
来源：http://akm.jinghuilouyu.cn

[Q07] 删除表
来源：http://ame.zhengqikj.top

DROP TABLE IF EXISTS orders;
来源：http://qqt.tianlin.xyz

[Q08] 创建普通索引
来源：http://rkr.9152youxi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://gab.nanxinkj.top

[Q09] 创建唯一索引
来源：http://tqc.yj20258888.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ltw.zycfv.cn

[Q10] 插入单行
来源：http://spt.hywenlv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qza.yj20258.top

[Q11] 一次插入多行
来源：http://ggh.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bxe.xuanzx.com

[Q12] 插入后取自增 ID
来源：http://gzf.ydjk.org.cn


<!-- 参考信息 -->