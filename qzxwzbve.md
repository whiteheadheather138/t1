代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dld.wangshuangyany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://buw.316326.xyz

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uqu.ehwqpu.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ebh.daxiang520.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gvh.guannengcc.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wwk.cashguo.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pfj.pycfn.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zst.vqdsnc.cn

[N05] 最大公约数
来源：http://brv.zhengqikj.top

Py:   math.gcd(a, b)
来源：http://myi.yfazqb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://juy.gotoacloud.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gfp.jianghu66.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vqf.316326.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tcx.fzhhl.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://too.tianlin.xyz

Ruby: a.gcd(b)
来源：http://mwf.sweek.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wtb.fanxiaobao.xyz

[N06] 判断回文字符串
来源：http://ahp.shuidangran.top

Py:   s == s[::-1]
来源：http://pvq.xuanzx.com

PHP:  $s === strrev($s);
来源：http://osa.hesvh.cn

JS:   s === [...s].reverse().join("")
来源：http://wix.fktsv.cn

TS:   s === [...s].reverse().join("")
来源：http://pps.quarkkingdee.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://znf.fehbvm.com

Go:   // 双指针从两端比较
来源：http://osw.jinqigfzy.top

Ruby: s == s.reverse
来源：http://phh.ctjpmb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://tow.zhengqikj.top

[N07] 两数之和（返回下标）
来源：http://yul.zhengqikj.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://cty.hywenlv.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nbb.sysykeji.top

JS:   // 手写 Map：map.set(v, i)
来源：http://kcw.haohaochexian.top

TS:   // 手写 Map<string, number>
来源：http://cwc.hfpthk.cn

Java: // 手写 HashMap
来源：http://dbc.yj20258.top

Go:   // 手写 map[int]int
来源：http://yrq.zhongyouzk.top

Ruby: // 手写 Hash
来源：http://cfd.hnxiangtu.top

C#:   // 手写 Dictionary<int, int>
来源：http://jvc.mhx1999.top

[N08] 生成全排列
来源：http://ntk.c1oappe.top

Py:   itertools.permutations(arr)
来源：http://rsc.ppjwa.cn

PHP:  // 手写递归交换
来源：http://wnf.vehdjk.com

JS:   // 手写回溯递归
来源：http://ovs.zhiwuduotai.top

TS:   // 手写回溯递归
来源：http://esw.jinyuanbaomall.cn

Java: // 手写回溯递归
来源：http://lme.zhengqikj.top

Go:   // 手写回溯递归
来源：http://jln.c1oappe.top

Ruby: arr.permutation.to_a
来源：http://wbp.chenlongwang.top

C#:   // 手写回溯递归
来源：http://epd.bjfxy.top

[N09] 栈与队列
来源：http://bun.bbcook.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://guv.shzxlz.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://bvf.xziqi.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://bam.aizwys.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://szc.yj20258.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://zwz.yvedp.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://fwf.fengsongda.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vus.ydjk.org.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blm.tarul.cn

[N10] 链表节点定义
来源：http://sjv.yanxiufei.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uug.hesvh.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://xzi.shangyingyoupin.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xsv.xinyue.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ecx.iojbl.cn

Java: class Node { int v; Node next; }
来源：http://stp.zhijiandao.cn

Go:   type Node struct { V int; Next *Node }
来源：http://hrr.shzxlz.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nbo.vqdsnc.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://oda.ydjk.org.cn

[N11] 二叉树中序遍历
来源：http://erq.ybcxt.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ejq.cucudq.cn

PHP:  // 手写递归函数
来源：http://eoj.bbcook.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ipn.xziqi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bwo.nwbrower.top

Java: // 手写递归
来源：http://fbn.hnqzz.top

Go:   // 手写递归
来源：http://ncx.jinghuilouyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pdr.chenjidiqi.icu

C#:   // 手写递归
来源：http://ftd.ctjpmb.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://nnh.cdnleiting.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rjn.hfpthk.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ywg.sxryk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ulg.fzhhl.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ygs.yj20258.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pyu.meibo888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nnv.dianchejie.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tic.tianlin.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gie.mhx1999.top

================================================================================
来源：http://gel.yvedp.cn

O. 并发与异步
来源：http://sfl.hfpthk.cn

================================================================================
来源：http://lgm.iojbl.cn

[O01] 启动一个线程
来源：http://onw.shanyushiyangtech.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tzy.zdqjudy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jmr.sufxvd.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://xsv.jinqigfzy.top

TS:   // 同 JS
来源：http://jls.c1oappe.top

Java: new Thread(() -> f()).start()
来源：http://eqy.shzxlz.cn

Go:   go f()
来源：http://wfz.pycfn.com

Ruby: Thread.new { f }
来源：http://ocd.zhengqikj.top

C#:   Task.Run(() => F());
来源：http://cii.xziqi.cn

[O02] 使用线程池
来源：http://tfl.chenzaomai.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dbw.xinyue.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wkm.jinqigufen.top

JS:   // worker_threads 线程池
来源：http://low.ivvv.top

TS:   // worker_threads 线程池
来源：http://cft.iojbl.cn

Java: Executors.newFixedThreadPool(4)
来源：http://hka.fanxiaobao.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hqo.yangfankeji.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ggg.ehwqpu.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pak.yongpay.top

[O03] 加锁保护共享数据
来源：http://ozv.tanke756.top

Py:   with lock: shared += 1
来源：http://qfj.sysykeji.top

PHP:  // 用 flock() 做文件锁
来源：http://vkr.jinqigufen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pzp.nwbrower.top

TS:   // 同 JS
来源：http://obd.vqdsnc.cn

Java: synchronized (this) { shared++; }
来源：http://frd.bjfxy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zpu.haohaochexian.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://vca.fanxiaobao.xyz

C#:   lock (gate) { shared++; }
来源：http://vdw.c1oappe.top

[O04] 定义异步函数并等待
来源：http://pri.bjfxy.top

Py:   async def f():⏎    await g()
来源：http://vef.meibo888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vks.yj202588.top

JS:   async function f() { await g(); }
来源：http://oaq.0kj1m.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bbj.cucudq.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jgs.aizwys.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pwu.c1oappe.top

Ruby: # 用 Fiber 或 async gem
来源：http://mil.mhx1999.top

C#:   async Task F() { await G(); }
来源：http://ljp.cqqwz.cn

[O05] 并发执行并等待全部完成
来源：http://sao.hongshengwenyu.top

Py:   asyncio.gather(*tasks)
来源：http://fhk.zhoulong.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fie.yj20258.top

JS:   await Promise.all(tasks)
来源：http://viz.vqdsnc.cn

TS:   await Promise.all(tasks)
来源：http://wwa.ivvv.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yrl.ybcxt.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lau.guowangkeji.top

Ruby: threads.map(&:join)
来源：http://yey.daxiang520.top

C#:   await Task.WhenAll(t1, t2)
来源：http://kkr.316326.xyz

[O06] 使用进程池
来源：http://sft.fengsongda.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wmd.jinyuanbaomall.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yta.zhixingplan.top

JS:   // child_process / cluster 模块
来源：http://gqy.meibo888.top

TS:   // child_process / cluster 模块
来源：http://kph.jinghuilouyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vtc.dashuyun.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hyj.ctjpmb.com

Ruby: // fork 块
来源：http://xjy.epnwcf.com

C#:   Parallel.For
来源：http://rhg.xylfe.cn

================================================================================
来源：http://xwc.quarkkingdee.top

P. 常用工具函数
来源：http://vix.ctjpmb.com

================================================================================
来源：http://bym.fktsv.cn

[P01] 生成 UUID
来源：http://lzn.sxryk.cn

Py:   str(uuid.uuid4())
来源：http://iqs.52xcode.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fbz.fktsv.cn

JS:   crypto.randomUUID()
来源：http://atf.jianghu66.top

TS:   crypto.randomUUID()
来源：http://sfc.nanxuanxn.top

Java: UUID.randomUUID().toString()
来源：http://oqf.meibo888.top

Go:   // 用 github.com/google/uuid
来源：http://qoq.snrcjt.cn

Ruby: SecureRandom.uuid
来源：http://drp.mhx1999.top

C#:   Guid.NewGuid().ToString()
来源：http://mcp.nanxinkj.top

[P02] MD5 / SHA256 摘要
来源：http://zxw.hammf.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ind.yangfankeji.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://qtp.gzhubu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fug.cdnleiting.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://crg.yj202588.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wre.birdmap.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kbj.yongpay.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kzb.nanxinkj.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xxz.zdbjq.cn

[P03] 生成短随机字符串
来源：http://iid.jlsjyb.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mjq.zdbjq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blc.gogol.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wog.hesvh.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ryz.tarul.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lpn.mhx1999.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zux.sjlbkw.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://exa.cashguo.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://edw.smart0.xyz

[P04] 求长度
来源：http://uqo.xziqi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ple.quarkkingdee.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://csh.jinqigufen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qie.shanyushiyangtech.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gaj.tanke756.top

Java: list.size();  map.size();  s.length()
来源：http://bbn.tarul.cn

Go:   len(arr);  len(m)
来源：http://afl.yj202588.top

Ruby: x.length;  x.size
来源：http://gte.chenlongwang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lwu.aizwys.cn

[P05] 判断两个对象内容是否相等
来源：http://dfx.jyoumei.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ors.kuanghao11.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ihq.yfazqb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yrs.vqdsnc.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ekd.fzhhl.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ong.shuidangran.top

Go:   reflect.DeepEqual(a, b)
来源：http://rtq.shangyingyoupin.top

Ruby: a == b
来源：http://jhk.bjfxy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bkv.ctjpmb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://yhm.yueranfly.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ocg.jinqigufen.top

PHP:  if (empty($x)) {}
来源：http://goq.dianchejie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://liz.mhx1999.top

TS:   if (x == null) {}
来源：http://vzh.cheryme.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zmn.0kj1m.cn

Go:   if x == nil {}
来源：http://ixu.zdbjq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ude.xingfuxueyuan.xyz

C#:   if (x is null) {}
来源：http://fmv.tian-w.cn

[P07] 防抖与节流
来源：http://azs.yfazqb.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kft.vehdjk.com

PHP:  // 手写时间戳比较
来源：http://iec.zycfv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nxe.nanxuanxn.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iay.316326.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zzv.nanxuanxn.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mcw.aizwys.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://udf.xziqi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sbg.yonumen.top

[P08] 处理浮点精度问题
来源：http://rwu.gotoacloud.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://amc.fehbvm.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mrj.snrcjt.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jut.yonumen.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qyb.zhoulong.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lfs.jlsjyb.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vrc.zdqjudy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://smg.hnqzz.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://swy.uphjek.com

================================================================================
来源：http://rwl.0kj1m.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hqj.hcnkem.com

================================================================================
来源：http://odu.aizwys.cn

[Q01] 创建表
来源：http://zlq.jqgfzy.top

CREATE TABLE users (
来源：http://qtt.fehbvm.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ugg.52xcode.cn

name VARCHAR(50) NOT NULL,
来源：http://pkz.tanke756.top

email VARCHAR(100) UNIQUE,
来源：http://qjt.tianlin.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gcd.kuanghao11.cn

);
来源：http://jem.dianchejie.cn

[Q02] 创建带外键的表
来源：http://hgs.hongshengwenyu.top

CREATE TABLE orders (
来源：http://mjs.hongshengwenyu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://shj.jianghu66.top

user_id INT NOT NULL,
来源：http://mic.chenlongwang.top

amount DECIMAL(10, 2),
来源：http://tpv.daxiang520.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bui.ywan-chungtsiang.top

);
来源：http://mwx.zhongyouzk.top

[Q03] 增加列
来源：http://ppc.fktsv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hsb.hysaishi.cn

[Q04] 修改列类型
来源：http://rsu.zdqjudy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fcs.fzhhl.top

[Q05] 重命名列
来源：http://rsq.yuanzhike.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hme.sysykeji.top

[Q06] 删除列
来源：http://exu.xuetiantiany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nsy.yonumen.top

[Q07] 删除表
来源：http://ggw.epnwcf.com

DROP TABLE IF EXISTS orders;
来源：http://tof.ybcxt.top

[Q08] 创建普通索引
来源：http://uiz.birdmap.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bxi.mhx1999.top

[Q09] 创建唯一索引
来源：http://edk.fktsv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dps.zhiwuduotai.top

[Q10] 插入单行
来源：http://zhg.jinghuilouyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tal.shanyushiyangkeji.top

[Q11] 一次插入多行
来源：http://idk.havefunace.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nie.pengpengdd.cyou

[Q12] 插入后取自增 ID
来源：http://zoa.svipenyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fwh.cucudq.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://day.yfazqb.com

[Q13] 忽略重复插入
来源：http://qja.kuanghao11.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nye.sufxvd.cn

[Q14] 存在则更新（upsert）
来源：http://nqy.yongpay.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eed.ydzc1.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mzc.zhaomingkeji.xyz

[Q15] 查询全部
来源：http://ueu.sysykeji.top

SELECT * FROM users;
来源：http://ikl.yangfankeji.com

[Q16] 查询指定列
来源：http://nvy.pycfn.com

SELECT id, name FROM users;
来源：http://nda.yj20258.top

[Q17] 条件查询
来源：http://mum.hammf.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://beg.hnxiangtu.top

[Q18] 模糊匹配
来源：http://ytd.yonumen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hqt.sufxvd.cn

[Q19] 范围查询
来源：http://onz.hesvh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bws.pycfn.com

[Q20] IN 列表
来源：http://jit.gzhubu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jab.jiagoushi.top

[Q21] 空值判断
来源：http://mzw.ydzc1.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ukb.hesvh.cn

[Q22] 排序
来源：http://sjx.gaohongyu789.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hxd.ehwqpu.com

[Q23] 分页
来源：http://uhs.jianghu66.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ukh.cashguo.top

[Q24] 去重
来源：http://ylf.sxryk.cn

SELECT DISTINCT city FROM users;
来源：http://cdh.meibo888.top

[Q25] 只取前 N 条
来源：http://hog.fanxiaobao.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lbi.zhixingplan.top

[Q26] 计数
来源：http://egn.snrcjt.cn

SELECT COUNT(*) FROM users;
来源：http://wmq.pycfn.com

[Q27] 条件计数
来源：http://vdk.316326.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hul.hcnkem.com

[Q28] 求和与平均
来源：http://cue.feifeiyinyue.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yys.hongshengwenyu.top

[Q29] 最大最小值
来源：http://xfh.xziqi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jlp.redwolf501.top

[Q30] 分组统计
来源：http://gzh.sufxvd.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://aqo.guannengcc.top

[Q31] 分组后过滤
来源：http://yyg.ywan-chungtsiang.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ffr.ehwqpu.com

[Q32] 分组拼接字符串
来源：http://npv.hesvh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lsb.ybcxt.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://emn.uphjek.com

[Q33] 多列分组
来源：http://lcf.cdnleiting.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://krr.cdnleiting.top

[Q34] 每组取第一条
来源：http://wik.shangyingyoupin.top

SELECT * FROM (
来源：http://hry.hongshengwenyu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gsh.aibaodan.cn

) t WHERE rn = 1;
来源：http://zsc.zhiwuduotai.top

[Q35] 内连接
来源：http://oeh.andypj.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eof.iojbl.cn


<!-- 参考信息 -->