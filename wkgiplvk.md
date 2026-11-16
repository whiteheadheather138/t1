代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ios.fehbvm.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gbe.sysykeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://caf.hongshengwenyu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mhf.0kj1m.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hkp.shzxlz.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://nns.jinqigfzy.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://csy.shzxlz.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gyf.zhixingplan.top

[N05] 最大公约数
来源：http://oko.ivvv.top

Py:   math.gcd(a, b)
来源：http://svk.ctjpmb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ols.gogol.net.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pnx.iojbl.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kra.zhijiandao.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ene.chenjidiqi.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dcr.redwolf501.top

Ruby: a.gcd(b)
来源：http://yqn.xuetiantiany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yok.cdnleiting.top

[N06] 判断回文字符串
来源：http://bsm.hnxiangtu.top

Py:   s == s[::-1]
来源：http://pzf.chenzaomai.com

PHP:  $s === strrev($s);
来源：http://mvn.jiagoushi.top

JS:   s === [...s].reverse().join("")
来源：http://owb.hammf.cn

TS:   s === [...s].reverse().join("")
来源：http://fca.sjlbkw.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qhb.zhengqikj.top

Go:   // 双指针从两端比较
来源：http://owl.gotoacloud.top

Ruby: s == s.reverse
来源：http://onh.fktsv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://vgd.52xcode.cn

[N07] 两数之和（返回下标）
来源：http://ehn.jinghuilouyu.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ceb.cheryme.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://beb.nwbrower.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wgw.zhengqikj.top

TS:   // 手写 Map<string, number>
来源：http://fwm.sufxvd.cn

Java: // 手写 HashMap
来源：http://xvm.hywenlv.cn

Go:   // 手写 map[int]int
来源：http://kxc.hnqzz.top

Ruby: // 手写 Hash
来源：http://ihd.ywan-chungtsiang.top

C#:   // 手写 Dictionary<int, int>
来源：http://eij.yj20258888.top

[N08] 生成全排列
来源：http://das.aizwys.cn

Py:   itertools.permutations(arr)
来源：http://zsb.sxryk.cn

PHP:  // 手写递归交换
来源：http://kqn.yj20258888.top

JS:   // 手写回溯递归
来源：http://dtw.bjfxy.top

TS:   // 手写回溯递归
来源：http://igu.hfpthk.cn

Java: // 手写回溯递归
来源：http://wqw.gogol.net.cn

Go:   // 手写回溯递归
来源：http://ynd.ctjpmb.com

Ruby: arr.permutation.to_a
来源：http://phb.xuetiantiany.cn

C#:   // 手写回溯递归
来源：http://ktm.pengpengdd.cyou

[N09] 栈与队列
来源：http://slq.haohaochexian.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cke.uphjek.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mor.wangdashe.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gpr.ivvv.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gnr.cucudq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mbo.hammf.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xjq.yangfankeji.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://bxy.xuanzx.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mqv.zdbjq.cn

[N10] 链表节点定义
来源：http://ejc.jiagoushi.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hvn.zhongyouzk.top

PHP:  class Node { public $v; public $next = null; }
来源：http://syf.yanxiufei.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mif.gaohongyu789.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rad.hammf.cn

Java: class Node { int v; Node next; }
来源：http://sss.xinyue.icu

Go:   type Node struct { V int; Next *Node }
来源：http://oom.xziqi.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://zgl.ivvv.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wys.0kj1m.cn

[N11] 二叉树中序遍历
来源：http://ilt.tanke756.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ddh.yuxming.cn

PHP:  // 手写递归函数
来源：http://jxz.meibo888.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://huw.vehdjk.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lgu.wangshuangyany.cn

Java: // 手写递归
来源：http://ucy.tian-w.cn

Go:   // 手写递归
来源：http://cmw.svipenyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hll.jiagoushi.top

C#:   // 手写递归
来源：http://wvc.gzhubu.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tjg.9152youxi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tky.hywenlv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://yzl.gzhubu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nsy.fehbvm.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://beh.meibo888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fnj.haohaochexian.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nlw.jqgfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://qie.nanxinkj.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cvy.cheryme.top

================================================================================
来源：http://egw.svipenyu.cn

O. 并发与异步
来源：http://jcp.cheryme.top

================================================================================
来源：http://duu.c1oappe.top

[O01] 启动一个线程
来源：http://kfq.hfpthk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gpo.zhixingplan.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uuk.yj202588.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vvn.redwolf501.top

TS:   // 同 JS
来源：http://gfb.zycfv.cn

Java: new Thread(() -> f()).start()
来源：http://oyd.yfazqb.com

Go:   go f()
来源：http://jhc.wangdashe.top

Ruby: Thread.new { f }
来源：http://hes.sweek.top

C#:   Task.Run(() => F());
来源：http://wgs.haohaochexian.top

[O02] 使用线程池
来源：http://kyb.yonumen.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://bgk.zycfv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nht.ppjwa.cn

JS:   // worker_threads 线程池
来源：http://bpx.sxryk.cn

TS:   // worker_threads 线程池
来源：http://xzu.zycfv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pbv.cucudq.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tmx.jianghu66.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tjb.snrcjt.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mka.zhixingplan.top

[O03] 加锁保护共享数据
来源：http://xvm.wangdashe.top

Py:   with lock: shared += 1
来源：http://ljt.yuanzhike.top

PHP:  // 用 flock() 做文件锁
来源：http://tsj.mhx1999.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://juz.feifeiyinyue.top

TS:   // 同 JS
来源：http://nge.ivvv.top

Java: synchronized (this) { shared++; }
来源：http://ova.shzxlz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eqs.jinqigfzy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://vib.yj20258.top

C#:   lock (gate) { shared++; }
来源：http://zfb.yangfankeji.com

[O04] 定义异步函数并等待
来源：http://usq.yj20258.top

Py:   async def f():⏎    await g()
来源：http://oof.zhaomingkeji.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gkf.epnwcf.com

JS:   async function f() { await g(); }
来源：http://msn.epnwcf.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://dkn.ydjk.org.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ktv.cqqwz.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ecj.52xcode.cn

Ruby: # 用 Fiber 或 async gem
来源：http://qzd.feifeiyinyue.top

C#:   async Task F() { await G(); }
来源：http://irp.shanyushiyangkeji.top

[O05] 并发执行并等待全部完成
来源：http://det.quarkkingdee.top

Py:   asyncio.gather(*tasks)
来源：http://pei.vehdjk.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xlm.zhongyouzk.top

JS:   await Promise.all(tasks)
来源：http://nla.yongpay.top

TS:   await Promise.all(tasks)
来源：http://bpi.jiagoushi.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ggu.cucudq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://upn.redwolf501.top

Ruby: threads.map(&:join)
来源：http://sel.hammf.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dmg.guowangkeji.top

[O06] 使用进程池
来源：http://ugn.zhoulong.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tuj.shzxlz.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xcz.sxryk.cn

JS:   // child_process / cluster 模块
来源：http://tny.xziqi.cn

TS:   // child_process / cluster 模块
来源：http://mhp.meibo888.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wnl.zdqjudy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ixr.aizwys.cn

Ruby: // fork 块
来源：http://mxk.chenzaomai.com

C#:   Parallel.For
来源：http://jhc.jqgufenzy.top

================================================================================
来源：http://rqx.wangshuangyany.cn

P. 常用工具函数
来源：http://tgt.jinqigufen.top

================================================================================
来源：http://jqu.hfpthk.cn

[P01] 生成 UUID
来源：http://dgd.shangyingyoupin.top

Py:   str(uuid.uuid4())
来源：http://hpp.bjfxy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jxg.pengpengdd.cyou

JS:   crypto.randomUUID()
来源：http://zya.guowangkeji.top

TS:   crypto.randomUUID()
来源：http://tqu.sjlbkw.cn

Java: UUID.randomUUID().toString()
来源：http://pho.chenjidiqi.icu

Go:   // 用 github.com/google/uuid
来源：http://sqv.wangdashe.top

Ruby: SecureRandom.uuid
来源：http://ewm.guannengcc.top

C#:   Guid.NewGuid().ToString()
来源：http://eds.c1oappe.top

[P02] MD5 / SHA256 摘要
来源：http://jvn.xingfuxueyuan.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oak.cheryme.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ndu.aibaodan.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lhe.hysaishi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pee.hesvh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://muz.c1oappe.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xtu.jiagoushi.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kns.hcnkem.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://byc.yj20258.top

[P03] 生成短随机字符串
来源：http://ojx.zdbjq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://awy.yj20258.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mbh.yj20258888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qun.hcnkem.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ibw.chenlongwang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mnq.zycfv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ymu.vqdsnc.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pfp.fanxiaobao.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lob.wangdashe.top

[P04] 求长度
来源：http://rrk.dashuyun.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vuz.ywan-chungtsiang.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dkp.chenzaomai.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xin.dashuyun.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lbx.zdbjq.cn

Java: list.size();  map.size();  s.length()
来源：http://hdm.cheryme.top

Go:   len(arr);  len(m)
来源：http://yvl.yj20258.top

Ruby: x.length;  x.size
来源：http://yce.yonumen.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jri.andypj.xyz

[P05] 判断两个对象内容是否相等
来源：http://yfc.haohaochexian.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zdw.ybcxt.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lqk.gogol.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lke.cucudq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uqu.shangyingyoupin.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sqm.jqgufenzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://dkc.jinqigfzy.top

Ruby: a == b
来源：http://qjk.iojbl.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nyp.sysykeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bgc.zdqjudy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://uko.vqdsnc.cn

PHP:  if (empty($x)) {}
来源：http://ezi.shanyushiyangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fdw.yj202588.top

TS:   if (x == null) {}
来源：http://gvx.ehwqpu.com

Java: if (x == null || x.isEmpty()) {}
来源：http://jvv.ydjk.org.cn

Go:   if x == nil {}
来源：http://ghq.sysykeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://aav.fengsongda.top

C#:   if (x is null) {}
来源：http://lma.chenzaomai.com

[P07] 防抖与节流
来源：http://jzp.guowangkeji.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pml.redwolf501.top

PHP:  // 手写时间戳比较
来源：http://ozw.hysaishi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://agc.yfazqb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mdz.jqgufenzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ylg.snrcjt.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nxu.hfpthk.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xoq.pycfn.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wjn.zycfv.cn

[P08] 处理浮点精度问题
来源：http://jtn.shzxlz.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bmz.hfpthk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gqr.nanxuanxn.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mzw.sxryk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://loa.guannengcc.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://bwj.daxiang520.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://myn.xylfe.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cxs.jyoumei.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xjh.aibaodan.cn

================================================================================
来源：http://azn.nwbrower.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zak.havefunace.top

================================================================================
来源：http://duo.pengpengdd.cyou

[Q01] 创建表
来源：http://cud.316326.xyz

CREATE TABLE users (
来源：http://rdh.vqdsnc.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zbd.bjfxy.top

name VARCHAR(50) NOT NULL,
来源：http://wwr.vqdsnc.cn

email VARCHAR(100) UNIQUE,
来源：http://tch.tianlin.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jwn.yj20258.top

);
来源：http://xxa.epnwcf.com

[Q02] 创建带外键的表
来源：http://yck.9152youxi.cn

CREATE TABLE orders (
来源：http://rvp.haohaochexian.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zro.fengsongda.top

user_id INT NOT NULL,
来源：http://ihh.xziqi.cn

amount DECIMAL(10, 2),
来源：http://cjv.gogol.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://unf.jinghuilouyu.cn

);
来源：http://nzo.jinghuilouyu.cn

[Q03] 增加列
来源：http://hfb.zhixingplan.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jsr.gotoacloud.top

[Q04] 修改列类型
来源：http://fdz.jiagoushi.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kxf.yueranfly.top

[Q05] 重命名列
来源：http://uen.zhiwuduotai.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cii.gogol.net.cn

[Q06] 删除列
来源：http://vhd.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://kad.jyoumei.cn

[Q07] 删除表
来源：http://xmx.zhaomingkeji.xyz

DROP TABLE IF EXISTS orders;
来源：http://iid.xziqi.cn

[Q08] 创建普通索引
来源：http://kll.shuidangran.top

CREATE INDEX idx_users_email ON users(email);
来源：http://klf.feifeiyinyue.top

[Q09] 创建唯一索引
来源：http://mlb.jinqigfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ior.chenlongwang.top

[Q10] 插入单行
来源：http://olw.pycfn.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://bbp.cdnleiting.top

[Q11] 一次插入多行
来源：http://cpr.redwolf501.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ryw.uphjek.com

[Q12] 插入后取自增 ID
来源：http://fcz.jinqigufen.top

INSERT INTO users (name) VALUES ('C');
来源：http://ugk.fehbvm.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pyf.sufxvd.cn

[Q13] 忽略重复插入
来源：http://mrd.yueranfly.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rxp.gaohongyu789.top

[Q14] 存在则更新（upsert）
来源：http://gjq.jyoumei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://igf.aibaodan.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://cov.zhongyouzk.top

[Q15] 查询全部
来源：http://irg.wangdashe.top

SELECT * FROM users;
来源：http://msn.jqgufenzy.top

[Q16] 查询指定列
来源：http://sez.yj20258888.top

SELECT id, name FROM users;
来源：http://ynn.nanxinkj.top

[Q17] 条件查询
来源：http://qxo.yueranfly.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ytx.gogol.net.cn

[Q18] 模糊匹配
来源：http://zbx.hnxiangtu.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jjk.nwbrower.top

[Q19] 范围查询
来源：http://zaf.zhixingplan.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zpb.jinghuilouyu.cn

[Q20] IN 列表
来源：http://zgq.ppjwa.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rrl.feifeiyinyue.top

[Q21] 空值判断
来源：http://fte.dianchejie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dze.tarul.cn

[Q22] 排序
来源：http://gro.yuxming.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pmw.smart0.xyz

[Q23] 分页
来源：http://pmr.gotoacloud.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dpe.shangyingyoupin.top

[Q24] 去重
来源：http://dhx.fengsongda.top

SELECT DISTINCT city FROM users;
来源：http://bgf.andypj.xyz

[Q25] 只取前 N 条
来源：http://tti.zhaomingkeji.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qba.yongpay.top

[Q26] 计数
来源：http://eir.vehdjk.com

SELECT COUNT(*) FROM users;
来源：http://hbx.nanxinkj.top

[Q27] 条件计数
来源：http://jan.epnwcf.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qkx.hfpthk.cn

[Q28] 求和与平均
来源：http://kak.cashguo.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://spb.mhx1999.top

[Q29] 最大最小值
来源：http://rup.nanxuanxn.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://zkj.hesvh.cn

[Q30] 分组统计
来源：http://tqf.c1oappe.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tek.zhongyouzk.top

[Q31] 分组后过滤
来源：http://whd.nwbrower.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://saw.guowangkeji.top

[Q32] 分组拼接字符串
来源：http://kms.zhaomingkeji.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zin.tian-w.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://quc.dianchejie.cn

[Q33] 多列分组
来源：http://eje.jiagoushi.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jjg.shangyingyoupin.top

[Q34] 每组取第一条
来源：http://vty.cqqwz.cn

SELECT * FROM (
来源：http://gba.gaohongyu789.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mqf.zdqjudy.top

) t WHERE rn = 1;
来源：http://nza.fengsongda.top

[Q35] 内连接
来源：http://zcp.sjlbkw.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ydv.birdmap.top


<!-- 参考信息 -->