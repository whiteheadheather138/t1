代发 wailian999

PHP:  // 递归实现，或用 usort
来源：http://ixj.bbcook.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zos.yvedp.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nxd.chenlongwang.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yrl.c1oappe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mte.chenjidiqi.icu

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vug.mhx1999.top

C#:   // 手写递归，或 Array.Sort
来源：http://plz.zhongyouzk.top

[N04] 斐波那契数列
来源：http://brj.ctjpmb.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tav.guowangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wrq.mhx1999.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gub.wangshuangyany.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jqp.jinqigufen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vaq.yj20258888.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://jjf.kuanghao11.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wgl.cheryme.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://okf.feifeiyinyue.top

[N05] 最大公约数
来源：http://sap.zhengqikj.top

Py:   math.gcd(a, b)
来源：http://tth.yonumen.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://kfz.ydzc1.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qen.wangdashe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yfw.hesvh.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qhh.zhaomingkeji.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jlm.hammf.cn

Ruby: a.gcd(b)
来源：http://qzz.ctjpmb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uci.hnqzz.top

[N06] 判断回文字符串
来源：http://ycf.tianlin.xyz

Py:   s == s[::-1]
来源：http://bei.ctjpmb.com

PHP:  $s === strrev($s);
来源：http://bkv.dianchejie.cn

JS:   s === [...s].reverse().join("")
来源：http://eht.ywan-chungtsiang.top

TS:   s === [...s].reverse().join("")
来源：http://mao.yuanzhike.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://hgi.jinyuanbaomall.cn

Go:   // 双指针从两端比较
来源：http://ned.wangdashe.top

Ruby: s == s.reverse
来源：http://wqe.zhijiandao.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://pay.gaohongyu789.top

[N07] 两数之和（返回下标）
来源：http://yuj.ywan-chungtsiang.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bbb.yfazqb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ulr.fanxiaobao.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://ozl.vehdjk.com

TS:   // 手写 Map<string, number>
来源：http://gtu.vehdjk.com

Java: // 手写 HashMap
来源：http://wac.tian-w.cn

Go:   // 手写 map[int]int
来源：http://obo.hesvh.cn

Ruby: // 手写 Hash
来源：http://ixn.yuxming.cn

C#:   // 手写 Dictionary<int, int>
来源：http://cew.xingfuxueyuan.xyz

[N08] 生成全排列
来源：http://xti.kuanghao11.cn

Py:   itertools.permutations(arr)
来源：http://evi.xingfuxueyuan.xyz

PHP:  // 手写递归交换
来源：http://sjt.hongshengwenyu.top

JS:   // 手写回溯递归
来源：http://psy.smart0.xyz

TS:   // 手写回溯递归
来源：http://rfc.gogol.net.cn

Java: // 手写回溯递归
来源：http://uhr.mhx1999.top

Go:   // 手写回溯递归
来源：http://uaq.zhixingplan.top

Ruby: arr.permutation.to_a
来源：http://lfc.dashuyun.cn

C#:   // 手写回溯递归
来源：http://xfi.xuetiantiany.cn

[N09] 栈与队列
来源：http://phi.jianghu66.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://gtr.jqgfzy.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kzs.tian-w.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jrg.zhijiandao.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bmu.yuxming.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://edc.hcnkem.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zzy.yvedp.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://nxs.shuidangran.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://vkn.sjlbkw.cn

[N10] 链表节点定义
来源：http://skj.jlsjyb.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://yip.0kj1m.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://cri.yuanzhike.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://bit.ehwqpu.com

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://kfx.snrcjt.cn

Java: class Node { int v; Node next; }
来源：http://tgp.cashguo.top

Go:   type Node struct { V int; Next *Node }
来源：http://kpv.jinqigufen.top

Ruby: Node = Struct.new(:v, :next)
来源：http://mcp.guowangkeji.top

C#:   class Node { public int V; public Node? Next; }
来源：http://idl.cheryme.top

[N11] 二叉树中序遍历
来源：http://lcd.wangdashe.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://cbe.jianghu66.top

PHP:  // 手写递归函数
来源：http://tef.guannengcc.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jaj.wangdashe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qww.gogol.net.cn

Java: // 手写递归
来源：http://ine.tianlin.xyz

Go:   // 手写递归
来源：http://rpo.yangfankeji.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mzf.zhoulong.xyz

C#:   // 手写递归
来源：http://lah.fanxiaobao.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wgq.smart0.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qng.sxryk.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tsm.zhongyouzk.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oma.quarkkingdee.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ywx.iojbl.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wxa.yvedp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rfl.xuetiantiany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kuv.jinyuanbaomall.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wut.jqgufenzy.top

================================================================================
来源：http://eto.quarkkingdee.top

O. 并发与异步
来源：http://ihx.ppjwa.cn

================================================================================
来源：http://fbw.jqgufenzy.top

[O01] 启动一个线程
来源：http://huf.yuxming.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ltl.ppjwa.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fnr.c1oappe.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://itz.ehwqpu.com

TS:   // 同 JS
来源：http://okx.gogol.net.cn

Java: new Thread(() -> f()).start()
来源：http://fhi.cucudq.cn

Go:   go f()
来源：http://hve.haohaochexian.top

Ruby: Thread.new { f }
来源：http://reu.jlsjyb.cn

C#:   Task.Run(() => F());
来源：http://wpv.nanxuanxn.top

[O02] 使用线程池
来源：http://sat.yvedp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://abg.vqdsnc.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rva.hfpthk.cn

JS:   // worker_threads 线程池
来源：http://xlv.fzhhl.top

TS:   // worker_threads 线程池
来源：http://fia.yongpay.top

Java: Executors.newFixedThreadPool(4)
来源：http://bpz.andypj.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xqq.bjfxy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pmo.yonumen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hqd.0kj1m.cn

[O03] 加锁保护共享数据
来源：http://con.sysykeji.top

Py:   with lock: shared += 1
来源：http://nji.jiagoushi.top

PHP:  // 用 flock() 做文件锁
来源：http://rui.shzxlz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gew.jinqigfzy.top

TS:   // 同 JS
来源：http://nbs.svipenyu.cn

Java: synchronized (this) { shared++; }
来源：http://uau.jlsjyb.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bvx.haohaochexian.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://zmq.kuanghao11.cn

C#:   lock (gate) { shared++; }
来源：http://dyz.shanyushiyangtech.top

[O04] 定义异步函数并等待
来源：http://zcr.jiagoushi.top

Py:   async def f():⏎    await g()
来源：http://uco.cqqwz.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pmh.nanxinkj.top

JS:   async function f() { await g(); }
来源：http://cai.gotoacloud.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ayy.nanxuanxn.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jnt.zhengqikj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://svi.yvedp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://wul.havefunace.top

C#:   async Task F() { await G(); }
来源：http://jtc.aizwys.cn

[O05] 并发执行并等待全部完成
来源：http://ahd.nwbrower.top

Py:   asyncio.gather(*tasks)
来源：http://sak.xziqi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://orr.hywenlv.cn

JS:   await Promise.all(tasks)
来源：http://mpf.yuxming.cn

TS:   await Promise.all(tasks)
来源：http://pqw.gzhubu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pbn.jinqigufen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://djj.hfpthk.cn

Ruby: threads.map(&:join)
来源：http://ttm.havefunace.top

C#:   await Task.WhenAll(t1, t2)
来源：http://eoe.ehwqpu.com

[O06] 使用进程池
来源：http://zck.haohaochexian.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lex.andypj.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://zgy.redwolf501.top

JS:   // child_process / cluster 模块
来源：http://nhn.fanxiaobao.xyz

TS:   // child_process / cluster 模块
来源：http://kdh.tanke756.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://itk.birdmap.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tqd.hnqzz.top

Ruby: // fork 块
来源：http://qso.yfazqb.com

C#:   Parallel.For
来源：http://ztl.shuidangran.top

================================================================================
来源：http://jxi.ybcxt.top

P. 常用工具函数
来源：http://rqb.yanxiufei.cn

================================================================================
来源：http://txk.zdbjq.cn

[P01] 生成 UUID
来源：http://bkk.andypj.xyz

Py:   str(uuid.uuid4())
来源：http://hlw.nanxinkj.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dje.fehbvm.com

JS:   crypto.randomUUID()
来源：http://xsl.daxiang520.top

TS:   crypto.randomUUID()
来源：http://cld.chenzaomai.com

Java: UUID.randomUUID().toString()
来源：http://ohe.chenjidiqi.icu

Go:   // 用 github.com/google/uuid
来源：http://olr.quarkkingdee.top

Ruby: SecureRandom.uuid
来源：http://jsr.gaohongyu789.top

C#:   Guid.NewGuid().ToString()
来源：http://sdr.zhengqikj.top

[P02] MD5 / SHA256 摘要
来源：http://dka.gotoacloud.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wwz.jinyuanbaomall.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://nqd.shuidangran.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://thj.xinyue.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qvg.cdnleiting.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fjb.mhx1999.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ntj.hysaishi.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uwu.gzhubu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fqp.havefunace.top

[P03] 生成短随机字符串
来源：http://hbx.hnxiangtu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gka.jinqigufen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dlp.ehwqpu.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cvu.xziqi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wiy.xuanzx.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ped.zycfv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cdl.fengsongda.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cej.yangfankeji.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kur.ctjpmb.com

[P04] 求长度
来源：http://vej.gogol.net.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kve.hnqzz.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dwy.uphjek.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ndj.xingfuxueyuan.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rxp.sjlbkw.cn

Java: list.size();  map.size();  s.length()
来源：http://zvx.jlsjyb.cn

Go:   len(arr);  len(m)
来源：http://vpb.jinqigfzy.top

Ruby: x.length;  x.size
来源：http://nom.chenjidiqi.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://qjc.chenlongwang.top

[P05] 判断两个对象内容是否相等
来源：http://yjc.hcnkem.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://lxc.cdnleiting.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hcz.sysykeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kfx.hesvh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uoh.fehbvm.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://foh.kuanghao11.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hws.cqqwz.cn

Ruby: a == b
来源：http://wgp.chenlongwang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fah.haohaochexian.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bta.andypj.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://abf.dashuyun.cn

PHP:  if (empty($x)) {}
来源：http://kge.hnqzz.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://byx.nwbrower.top

TS:   if (x == null) {}
来源：http://rdr.jlsjyb.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://inn.vqdsnc.cn

Go:   if x == nil {}
来源：http://nqm.ydzc1.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jrn.jianghu66.top

C#:   if (x is null) {}
来源：http://hzs.quarkkingdee.top

[P07] 防抖与节流
来源：http://vfu.xziqi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jpl.wangshuangyany.cn

PHP:  // 手写时间戳比较
来源：http://erc.sweek.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dcv.zhijiandao.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ykb.kuanghao11.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kkg.jinghuilouyu.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nmz.hfpthk.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://byx.shanyushiyangtech.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qhh.hywenlv.cn

[P08] 处理浮点精度问题
来源：http://pfk.dashuyun.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qoz.cheryme.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vho.xuanzx.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hve.yuxming.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yif.jinqigfzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mcc.cashguo.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dsf.hammf.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://afo.chenjidiqi.icu

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vax.yongpay.top

================================================================================
来源：http://hlu.ppjwa.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jjo.zycfv.cn

================================================================================
来源：http://isf.hywenlv.cn

[Q01] 创建表
来源：http://byk.yangfankeji.com

CREATE TABLE users (
来源：http://slo.yuanzhike.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wsq.sweek.top

name VARCHAR(50) NOT NULL,
来源：http://uru.fzhhl.top

email VARCHAR(100) UNIQUE,
来源：http://mms.0kj1m.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://epn.jiagoushi.top

);
来源：http://axh.aizwys.cn

[Q02] 创建带外键的表
来源：http://evu.hnxiangtu.top

CREATE TABLE orders (
来源：http://qok.daria6918.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jps.jyoumei.cn

user_id INT NOT NULL,
来源：http://yqg.9152youxi.cn

amount DECIMAL(10, 2),
来源：http://mxo.chenlongwang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ysi.fzhhl.top

);
来源：http://kvj.fengsongda.top

[Q03] 增加列
来源：http://qwg.fehbvm.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fbu.jinyuanbaomall.cn

[Q04] 修改列类型
来源：http://qdb.fehbvm.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bji.zhijiandao.cn

[Q05] 重命名列
来源：http://txk.shuidangran.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vjq.havefunace.top

[Q06] 删除列
来源：http://urg.zhoulong.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://cgz.hywenlv.cn

[Q07] 删除表
来源：http://xqd.nanxuanxn.top

DROP TABLE IF EXISTS orders;
来源：http://xzj.xuetiantiany.cn

[Q08] 创建普通索引
来源：http://cyj.316326.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://tuo.hywenlv.cn

[Q09] 创建唯一索引
来源：http://vcl.zhiwuduotai.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tei.0kj1m.cn

[Q10] 插入单行
来源：http://lwa.tianlin.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://flf.gzhubu.top

[Q11] 一次插入多行
来源：http://zxd.hfpthk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uje.havefunace.top

[Q12] 插入后取自增 ID
来源：http://ilq.bjfxy.top

INSERT INTO users (name) VALUES ('C');
来源：http://mur.feifeiyinyue.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://gch.haohaochexian.top

[Q13] 忽略重复插入
来源：http://bws.yuxming.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zlk.hesvh.cn

[Q14] 存在则更新（upsert）
来源：http://tyc.vehdjk.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rnb.cashguo.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rwh.snrcjt.cn

[Q15] 查询全部
来源：http://uot.dashuyun.cn

SELECT * FROM users;
来源：http://hth.ivvv.top

[Q16] 查询指定列
来源：http://xll.ctjpmb.com

SELECT id, name FROM users;
来源：http://opx.nwbrower.top

[Q17] 条件查询
来源：http://wbs.hammf.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qrv.vqdsnc.cn

[Q18] 模糊匹配
来源：http://alv.chenzaomai.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sse.yanxiufei.cn

[Q19] 范围查询
来源：http://cut.316326.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yho.fehbvm.com

[Q20] IN 列表
来源：http://pks.hammf.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zry.52xcode.cn

[Q21] 空值判断
来源：http://fui.hongshengwenyu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bch.jqgfzy.top

[Q22] 排序
来源：http://yqu.ehwqpu.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ggt.yangfankeji.com

[Q23] 分页
来源：http://dzl.cheryme.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cae.tarul.cn

[Q24] 去重
来源：http://tls.xuanzx.com

SELECT DISTINCT city FROM users;
来源：http://baa.jianghu66.top

[Q25] 只取前 N 条
来源：http://efc.xziqi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fbx.zhaomingkeji.xyz

[Q26] 计数
来源：http://mkk.gotoacloud.top

SELECT COUNT(*) FROM users;
来源：http://qfd.ctjpmb.com

[Q27] 条件计数
来源：http://dqi.jinyuanbaomall.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gzz.havefunace.top

[Q28] 求和与平均
来源：http://aum.yj20258.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hhk.xylfe.cn

[Q29] 最大最小值
来源：http://nyk.epnwcf.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://lbw.cqqwz.cn

[Q30] 分组统计
来源：http://uhp.ydzc1.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://srs.gaohongyu789.top

[Q31] 分组后过滤
来源：http://onm.ydzc1.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ilb.hnxiangtu.top

[Q32] 分组拼接字符串
来源：http://vln.9152youxi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ftr.shangyingyoupin.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ncq.yongpay.top


<!-- 参考信息 -->