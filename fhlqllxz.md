代发 wailian999

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uir.gogol.net.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bnz.meibo888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zxi.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tvn.svipenyu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tuj.shuidangran.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fqi.hesvh.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://itx.fzhhl.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ghf.pengpengdd.cyou

[N05] 最大公约数
来源：http://xlp.haohaochexian.top

Py:   math.gcd(a, b)
来源：http://hke.sysykeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://agm.gzhubu.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vui.xuanzx.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zka.yuxming.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cgf.xylfe.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vxr.ydzc1.top

Ruby: a.gcd(b)
来源：http://rfz.bjfxy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hdr.cashguo.top

[N06] 判断回文字符串
来源：http://ppq.feifeiyinyue.top

Py:   s == s[::-1]
来源：http://cgr.smart0.xyz

PHP:  $s === strrev($s);
来源：http://hsv.316326.xyz

JS:   s === [...s].reverse().join("")
来源：http://htc.0kj1m.cn

TS:   s === [...s].reverse().join("")
来源：http://lpl.cashguo.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://xhj.ctjpmb.com

Go:   // 双指针从两端比较
来源：http://kqa.hcnkem.com

Ruby: s == s.reverse
来源：http://tsc.jianghu66.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ykz.sjlbkw.cn

[N07] 两数之和（返回下标）
来源：http://kfb.cashguo.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://uho.yanxiufei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://xjb.haohaochexian.top

JS:   // 手写 Map：map.set(v, i)
来源：http://frn.shzxlz.cn

TS:   // 手写 Map<string, number>
来源：http://zya.tarul.cn

Java: // 手写 HashMap
来源：http://jng.jinqigfzy.top

Go:   // 手写 map[int]int
来源：http://bqw.redwolf501.top

Ruby: // 手写 Hash
来源：http://axg.kuanghao11.cn

C#:   // 手写 Dictionary<int, int>
来源：http://too.ybcxt.top

[N08] 生成全排列
来源：http://hvk.sysykeji.top

Py:   itertools.permutations(arr)
来源：http://zij.shzxlz.cn

PHP:  // 手写递归交换
来源：http://jpi.jinghuilouyu.cn

JS:   // 手写回溯递归
来源：http://uxy.zhijiandao.cn

TS:   // 手写回溯递归
来源：http://qbm.jinghuilouyu.cn

Java: // 手写回溯递归
来源：http://gkk.fengsongda.top

Go:   // 手写回溯递归
来源：http://ykm.chenzaomai.com

Ruby: arr.permutation.to_a
来源：http://ycd.meibo888.top

C#:   // 手写回溯递归
来源：http://buo.xziqi.cn

[N09] 栈与队列
来源：http://dlc.fzhhl.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://aqi.jlsjyb.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://seg.birdmap.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://ubq.sysykeji.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://vfk.hysaishi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://hjq.tarul.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://zea.meibo888.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://khv.ydzc1.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://gcv.hesvh.cn

[N10] 链表节点定义
来源：http://ycr.nwbrower.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ttp.smart0.xyz

PHP:  class Node { public $v; public $next = null; }
来源：http://uxx.sufxvd.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jnq.cheryme.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wik.feifeiyinyue.top

Java: class Node { int v; Node next; }
来源：http://hwr.wangdashe.top

Go:   type Node struct { V int; Next *Node }
来源：http://pob.zdbjq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://cwk.zdqjudy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wnw.epnwcf.com

[N11] 二叉树中序遍历
来源：http://djn.nanxuanxn.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ffd.fktsv.cn

PHP:  // 手写递归函数
来源：http://koo.pycfn.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://anj.tianlin.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://tbs.0kj1m.cn

Java: // 手写递归
来源：http://cex.xziqi.cn

Go:   // 手写递归
来源：http://gyx.nanxinkj.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yqp.yvedp.cn

C#:   // 手写递归
来源：http://cxr.52xcode.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ppe.chenzaomai.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mwj.wangdashe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://plb.zhoulong.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hgd.chenjidiqi.icu

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wvr.yfazqb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://knh.zhengqikj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zoy.ivvv.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yyr.zycfv.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rci.xylfe.cn

================================================================================
来源：http://wnr.pengpengdd.cyou

O. 并发与异步
来源：http://drn.smart0.xyz

================================================================================
来源：http://pbi.yonumen.top

[O01] 启动一个线程
来源：http://hvr.fzhhl.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vcw.jinyuanbaomall.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bcj.ywan-chungtsiang.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wef.cqqwz.cn

TS:   // 同 JS
来源：http://ixh.vqdsnc.cn

Java: new Thread(() -> f()).start()
来源：http://pjn.fktsv.cn

Go:   go f()
来源：http://qck.hnxiangtu.top

Ruby: Thread.new { f }
来源：http://dxx.redwolf501.top

C#:   Task.Run(() => F());
来源：http://swl.vehdjk.com

[O02] 使用线程池
来源：http://hov.wangdashe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://otd.ivvv.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rxz.aizwys.cn

JS:   // worker_threads 线程池
来源：http://bsm.yuanzhike.top

TS:   // worker_threads 线程池
来源：http://tei.uphjek.com

Java: Executors.newFixedThreadPool(4)
来源：http://urg.guowangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xzr.aizwys.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dvg.aizwys.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ove.shanyushiyangkeji.top

[O03] 加锁保护共享数据
来源：http://bsv.yuxming.cn

Py:   with lock: shared += 1
来源：http://wse.yuanzhike.top

PHP:  // 用 flock() 做文件锁
来源：http://tyv.jinqigufen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fzn.sjlbkw.cn

TS:   // 同 JS
来源：http://shm.sysykeji.top

Java: synchronized (this) { shared++; }
来源：http://zxy.hfpthk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qjs.shzxlz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pbi.zdqjudy.top

C#:   lock (gate) { shared++; }
来源：http://vpm.sysykeji.top

[O04] 定义异步函数并等待
来源：http://psz.yongpay.top

Py:   async def f():⏎    await g()
来源：http://ggt.pengpengdd.cyou

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://sza.jiagoushi.top

JS:   async function f() { await g(); }
来源：http://ggh.wangshuangyany.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://lvs.yongpay.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ark.c1oappe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wzx.andypj.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://tqu.hammf.cn

C#:   async Task F() { await G(); }
来源：http://mar.guowangkeji.top

[O05] 并发执行并等待全部完成
来源：http://fju.sweek.top

Py:   asyncio.gather(*tasks)
来源：http://emv.jlsjyb.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uef.hammf.cn

JS:   await Promise.all(tasks)
来源：http://egl.nanxinkj.top

TS:   await Promise.all(tasks)
来源：http://qvt.yfazqb.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://awa.yonumen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uwa.jiagoushi.top

Ruby: threads.map(&:join)
来源：http://hqz.tian-w.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dpm.vqdsnc.cn

[O06] 使用进程池
来源：http://oji.zhiwuduotai.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bfp.yanxiufei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zwb.yvedp.cn

JS:   // child_process / cluster 模块
来源：http://epx.bbcook.cn

TS:   // child_process / cluster 模块
来源：http://tfp.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lol.shzxlz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gkz.gzhubu.top

Ruby: // fork 块
来源：http://syx.52xcode.cn

C#:   Parallel.For
来源：http://prp.tian-w.cn

================================================================================
来源：http://rwy.ydjk.org.cn

P. 常用工具函数
来源：http://ccb.daria6918.cn

================================================================================
来源：http://laa.hammf.cn

[P01] 生成 UUID
来源：http://hqp.yj202588.top

Py:   str(uuid.uuid4())
来源：http://pwk.svipenyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hxi.gaohongyu789.top

JS:   crypto.randomUUID()
来源：http://jkl.hysaishi.cn

TS:   crypto.randomUUID()
来源：http://veo.birdmap.top

Java: UUID.randomUUID().toString()
来源：http://wml.ivvv.top

Go:   // 用 github.com/google/uuid
来源：http://vhk.ywan-chungtsiang.top

Ruby: SecureRandom.uuid
来源：http://tzx.ehwqpu.com

C#:   Guid.NewGuid().ToString()
来源：http://vmq.zhijiandao.cn

[P02] MD5 / SHA256 摘要
来源：http://nma.chenjidiqi.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zan.quarkkingdee.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://eyp.shanyushiyangtech.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lbp.sysykeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yvp.jqgfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wdj.yuanzhike.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lww.yangfankeji.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iid.ppjwa.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yjq.yanxiufei.cn

[P03] 生成短随机字符串
来源：http://rwi.yj20258888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://shz.0kj1m.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zqm.cqqwz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kuz.xuetiantiany.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iuz.fktsv.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gfl.yueranfly.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gwh.jqgufenzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dgi.aizwys.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tuf.jiagoushi.top

[P04] 求长度
来源：http://jsk.aibaodan.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jyj.chenzaomai.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rck.yongpay.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eeo.uphjek.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hqg.daria6918.cn

Java: list.size();  map.size();  s.length()
来源：http://zpr.fehbvm.com

Go:   len(arr);  len(m)
来源：http://rst.ywan-chungtsiang.top

Ruby: x.length;  x.size
来源：http://wxg.jyoumei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://bxe.c1oappe.top

[P05] 判断两个对象内容是否相等
来源：http://jsh.zhongyouzk.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://xdp.zdbjq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xnn.cucudq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hho.hnxiangtu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vlf.gaohongyu789.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qmx.gaohongyu789.top

Go:   reflect.DeepEqual(a, b)
来源：http://tpe.smart0.xyz

Ruby: a == b
来源：http://van.jqgufenzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nsi.sufxvd.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uww.hcnkem.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fet.pengpengdd.cyou

PHP:  if (empty($x)) {}
来源：http://nli.jiagoushi.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nxx.xuanzx.com

TS:   if (x == null) {}
来源：http://ine.gzhubu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://hlt.zhengqikj.top

Go:   if x == nil {}
来源：http://ezj.andypj.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qwa.316326.xyz

C#:   if (x is null) {}
来源：http://ydh.daria6918.cn

[P07] 防抖与节流
来源：http://vtx.shanyushiyangtech.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ruv.fanxiaobao.xyz

PHP:  // 手写时间戳比较
来源：http://gpz.fktsv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://noc.quarkkingdee.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ghq.gotoacloud.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fmj.ydzc1.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qmg.svipenyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://sxt.ywan-chungtsiang.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xsi.hcnkem.com

[P08] 处理浮点精度问题
来源：http://pcj.kuanghao11.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hkw.havefunace.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vgf.svipenyu.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gao.vehdjk.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pkg.svipenyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oho.hysaishi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://sek.chenjidiqi.icu

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zzy.xuanzx.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://edv.hywenlv.cn

================================================================================
来源：http://hxw.epnwcf.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://djs.chenlongwang.top

================================================================================
来源：http://xtn.gzhubu.top

[Q01] 创建表
来源：http://pli.jlsjyb.cn

CREATE TABLE users (
来源：http://xpy.cheryme.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jls.jiagoushi.top

name VARCHAR(50) NOT NULL,
来源：http://aue.shangyingyoupin.top

email VARCHAR(100) UNIQUE,
来源：http://ahj.zhongyouzk.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qjm.cdnleiting.top

);
来源：http://cpl.pengpengdd.cyou

[Q02] 创建带外键的表
来源：http://red.fzhhl.top

CREATE TABLE orders (
来源：http://ptg.chenlongwang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mmy.yvedp.cn

user_id INT NOT NULL,
来源：http://lxu.jinqigufen.top

amount DECIMAL(10, 2),
来源：http://ers.cqqwz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ayt.iojbl.cn

);
来源：http://fkk.sufxvd.cn

[Q03] 增加列
来源：http://hwy.yvedp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ihd.tanke756.top

[Q04] 修改列类型
来源：http://isz.zhengqikj.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bsf.ivvv.top

[Q05] 重命名列
来源：http://brz.dianchejie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ozc.sysykeji.top

[Q06] 删除列
来源：http://xpl.yonumen.top

ALTER TABLE users DROP COLUMN age;
来源：http://ytu.hongshengwenyu.top

[Q07] 删除表
来源：http://umq.chenzaomai.com

DROP TABLE IF EXISTS orders;
来源：http://one.meibo888.top

[Q08] 创建普通索引
来源：http://rve.52xcode.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ugt.ydzc1.top

[Q09] 创建唯一索引
来源：http://mtw.hnxiangtu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://knr.wangshuangyany.cn

[Q10] 插入单行
来源：http://knz.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qny.zdbjq.cn

[Q11] 一次插入多行
来源：http://pnd.iojbl.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://csz.shanyushiyangtech.top

[Q12] 插入后取自增 ID
来源：http://mzn.shanyushiyangtech.top

INSERT INTO users (name) VALUES ('C');
来源：http://wgt.jinghuilouyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dds.jinqigfzy.top

[Q13] 忽略重复插入
来源：http://vat.yj20258888.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ryc.chenzaomai.com

[Q14] 存在则更新（upsert）
来源：http://etw.0kj1m.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wfz.feifeiyinyue.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fhu.gogol.net.cn

[Q15] 查询全部
来源：http://nsd.nanxinkj.top

SELECT * FROM users;
来源：http://nzb.haohaochexian.top

[Q16] 查询指定列
来源：http://ykr.yanxiufei.cn

SELECT id, name FROM users;
来源：http://nho.sxryk.cn

[Q17] 条件查询
来源：http://njk.zhongyouzk.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ixx.zhoulong.xyz

[Q18] 模糊匹配
来源：http://drs.shuidangran.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dex.tianlin.xyz

[Q19] 范围查询
来源：http://lcm.chenjidiqi.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pse.aibaodan.cn

[Q20] IN 列表
来源：http://wmr.chenlongwang.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pij.yj20258.top

[Q21] 空值判断
来源：http://iad.yueranfly.top

SELECT * FROM users WHERE email IS NULL;
来源：http://dss.uphjek.com

[Q22] 排序
来源：http://tqj.tian-w.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gfq.xuanzx.com

[Q23] 分页
来源：http://ndi.yuanzhike.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oqa.svipenyu.cn

[Q24] 去重
来源：http://vot.jqgufenzy.top

SELECT DISTINCT city FROM users;
来源：http://hbk.yuanzhike.top

[Q25] 只取前 N 条
来源：http://icf.tanke756.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tgc.haohaochexian.top

[Q26] 计数
来源：http://tan.daria6918.cn

SELECT COUNT(*) FROM users;
来源：http://enc.yfazqb.com

[Q27] 条件计数
来源：http://rwu.9152youxi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rvp.yanxiufei.cn

[Q28] 求和与平均
来源：http://mkv.jianghu66.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://soe.xuetiantiany.cn

[Q29] 最大最小值
来源：http://xyx.gogol.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://xgq.jyoumei.cn

[Q30] 分组统计
来源：http://aer.bjfxy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gqz.quarkkingdee.top

[Q31] 分组后过滤
来源：http://wcw.sufxvd.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://edh.birdmap.top

[Q32] 分组拼接字符串
来源：http://dhw.cheryme.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cqe.sufxvd.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ghr.ydjk.org.cn

[Q33] 多列分组
来源：http://sby.cheryme.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fpr.tanke756.top

[Q34] 每组取第一条
来源：http://ozo.hfpthk.cn

SELECT * FROM (
来源：http://src.aizwys.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ciz.birdmap.top

) t WHERE rn = 1;
来源：http://cii.jinqigufen.top

[Q35] 内连接
来源：http://bab.jqgufenzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ssr.jlsjyb.cn


<!-- 参考信息 -->