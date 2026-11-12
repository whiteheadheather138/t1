代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tiu.hfpthk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sxv.dianchejie.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pqp.daria6918.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qtl.zhiwuduotai.top

[N05] 最大公约数
来源：http://xkn.guannengcc.top

Py:   math.gcd(a, b)
来源：http://hty.daria6918.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://aqy.zycfv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://iig.guowangkeji.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jft.aizwys.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tty.9152youxi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://rqd.yonumen.top

Ruby: a.gcd(b)
来源：http://bxv.gogol.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://hvx.birdmap.top

[N06] 判断回文字符串
来源：http://sgx.pycfn.com

Py:   s == s[::-1]
来源：http://zyy.jianghu66.top

PHP:  $s === strrev($s);
来源：http://pnc.yanxiufei.cn

JS:   s === [...s].reverse().join("")
来源：http://gca.xylfe.cn

TS:   s === [...s].reverse().join("")
来源：http://pwp.wangshuangyany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://enn.gzhubu.top

Go:   // 双指针从两端比较
来源：http://qlm.fzhhl.top

Ruby: s == s.reverse
来源：http://veu.snrcjt.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://utq.quarkkingdee.top

[N07] 两数之和（返回下标）
来源：http://eag.hfpthk.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bkb.jinghuilouyu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gxm.feifeiyinyue.top

JS:   // 手写 Map：map.set(v, i)
来源：http://npj.yongpay.top

TS:   // 手写 Map<string, number>
来源：http://ymu.52xcode.cn

Java: // 手写 HashMap
来源：http://lod.zdqjudy.top

Go:   // 手写 map[int]int
来源：http://rsm.shzxlz.cn

Ruby: // 手写 Hash
来源：http://yxs.jyoumei.cn

C#:   // 手写 Dictionary<int, int>
来源：http://dks.0kj1m.cn

[N08] 生成全排列
来源：http://hen.epnwcf.com

Py:   itertools.permutations(arr)
来源：http://rqi.svipenyu.cn

PHP:  // 手写递归交换
来源：http://ral.shuidangran.top

JS:   // 手写回溯递归
来源：http://bxp.fzhhl.top

TS:   // 手写回溯递归
来源：http://pwi.9152youxi.cn

Java: // 手写回溯递归
来源：http://arc.redwolf501.top

Go:   // 手写回溯递归
来源：http://lkp.cheryme.top

Ruby: arr.permutation.to_a
来源：http://zfh.ppjwa.cn

C#:   // 手写回溯递归
来源：http://ugd.cashguo.top

[N09] 栈与队列
来源：http://tcn.jiagoushi.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://goo.yuanzhike.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ppu.gotoacloud.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pru.yfazqb.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://gdi.bjfxy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://nhw.sysykeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jpb.zhiwuduotai.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ulb.zhixingplan.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://iro.jiagoushi.top

[N10] 链表节点定义
来源：http://ujj.daxiang520.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ton.zdqjudy.top

PHP:  class Node { public $v; public $next = null; }
来源：http://kyi.hnqzz.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jdx.shuidangran.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ywk.xinyue.icu

Java: class Node { int v; Node next; }
来源：http://hvr.dianchejie.cn

Go:   type Node struct { V int; Next *Node }
来源：http://jei.xinyue.icu

Ruby: Node = Struct.new(:v, :next)
来源：http://jml.gaohongyu789.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bzc.jinghuilouyu.cn

[N11] 二叉树中序遍历
来源：http://zsy.hesvh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gtg.aizwys.cn

PHP:  // 手写递归函数
来源：http://rlc.xuanzx.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sfk.shangyingyoupin.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mag.daria6918.cn

Java: // 手写递归
来源：http://foj.dianchejie.cn

Go:   // 手写递归
来源：http://kif.epnwcf.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vjf.hcnkem.com

C#:   // 手写递归
来源：http://yyz.ydjk.org.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wxw.xylfe.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rsw.chenlongwang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ffg.ppjwa.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ugq.shuidangran.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qtj.aibaodan.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://elz.guowangkeji.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qhu.yangfankeji.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wny.ehwqpu.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cah.xuanzx.com

================================================================================
来源：http://cyu.52xcode.cn

O. 并发与异步
来源：http://wua.bbcook.cn

================================================================================
来源：http://fig.yvedp.cn

[O01] 启动一个线程
来源：http://wir.feifeiyinyue.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://xql.fengsongda.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sch.cdnleiting.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://anb.aizwys.cn

TS:   // 同 JS
来源：http://lrj.smart0.xyz

Java: new Thread(() -> f()).start()
来源：http://kym.hcnkem.com

Go:   go f()
来源：http://jnp.bbcook.cn

Ruby: Thread.new { f }
来源：http://abx.yanxiufei.cn

C#:   Task.Run(() => F());
来源：http://wzt.jianghu66.top

[O02] 使用线程池
来源：http://zgk.yongpay.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ktj.xuetiantiany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fpb.uphjek.com

JS:   // worker_threads 线程池
来源：http://vds.jinyuanbaomall.cn

TS:   // worker_threads 线程池
来源：http://lra.hfpthk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://aeo.fzhhl.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://yjo.ctjpmb.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://onn.sweek.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bvw.andypj.xyz

[O03] 加锁保护共享数据
来源：http://vvg.bjfxy.top

Py:   with lock: shared += 1
来源：http://dbh.hnxiangtu.top

PHP:  // 用 flock() 做文件锁
来源：http://ohn.hysaishi.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zok.xuanzx.com

TS:   // 同 JS
来源：http://qil.vehdjk.com

Java: synchronized (this) { shared++; }
来源：http://eod.chenlongwang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jkz.yuxming.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://yei.zhengqikj.top

C#:   lock (gate) { shared++; }
来源：http://xcn.aibaodan.cn

[O04] 定义异步函数并等待
来源：http://evi.cqqwz.cn

Py:   async def f():⏎    await g()
来源：http://ukw.birdmap.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rru.chenzaomai.com

JS:   async function f() { await g(); }
来源：http://buu.hesvh.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mii.jinqigfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://aas.smart0.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eqj.aizwys.cn

Ruby: # 用 Fiber 或 async gem
来源：http://noq.snrcjt.cn

C#:   async Task F() { await G(); }
来源：http://htj.nanxinkj.top

[O05] 并发执行并等待全部完成
来源：http://bsa.fanxiaobao.xyz

Py:   asyncio.gather(*tasks)
来源：http://lcm.birdmap.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dto.shuidangran.top

JS:   await Promise.all(tasks)
来源：http://xfb.ppjwa.cn

TS:   await Promise.all(tasks)
来源：http://lsj.tarul.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cvh.chenjidiqi.icu

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fkw.gogol.net.cn

Ruby: threads.map(&:join)
来源：http://aya.hnqzz.top

C#:   await Task.WhenAll(t1, t2)
来源：http://gcw.yj20258888.top

[O06] 使用进程池
来源：http://usp.jinqigfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ssg.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://oku.hcnkem.com

JS:   // child_process / cluster 模块
来源：http://nad.yueranfly.top

TS:   // child_process / cluster 模块
来源：http://hoc.hammf.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mvk.sjlbkw.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://fsf.cucudq.cn

Ruby: // fork 块
来源：http://hqf.birdmap.top

C#:   Parallel.For
来源：http://wta.svipenyu.cn

================================================================================
来源：http://rop.smart0.xyz

P. 常用工具函数
来源：http://rnz.xuanzx.com

================================================================================
来源：http://oez.shuidangran.top

[P01] 生成 UUID
来源：http://fbk.hesvh.cn

Py:   str(uuid.uuid4())
来源：http://pju.zhoulong.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://day.andypj.xyz

JS:   crypto.randomUUID()
来源：http://yql.hammf.cn

TS:   crypto.randomUUID()
来源：http://wpz.316326.xyz

Java: UUID.randomUUID().toString()
来源：http://bsw.jinqigfzy.top

Go:   // 用 github.com/google/uuid
来源：http://brd.jlsjyb.cn

Ruby: SecureRandom.uuid
来源：http://evq.ivvv.top

C#:   Guid.NewGuid().ToString()
来源：http://rav.yvedp.cn

[P02] MD5 / SHA256 摘要
来源：http://ert.shanyushiyangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://slx.snrcjt.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bog.yfazqb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://klw.zhongyouzk.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://caf.zhiwuduotai.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wkf.shanyushiyangkeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://omy.yuxming.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://niw.ydjk.org.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://usi.yuxming.cn

[P03] 生成短随机字符串
来源：http://jjz.zhijiandao.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hkb.iojbl.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ucl.cashguo.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tft.cashguo.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zrm.ywan-chungtsiang.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cms.jinqigufen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://svt.jianghu66.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://yor.nwbrower.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zeo.guannengcc.top

[P04] 求长度
来源：http://vlr.sjlbkw.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mey.sufxvd.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ncx.yj20258888.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mrc.zhiwuduotai.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tfd.birdmap.top

Java: list.size();  map.size();  s.length()
来源：http://wsx.ydjk.org.cn

Go:   len(arr);  len(m)
来源：http://vff.ybcxt.top

Ruby: x.length;  x.size
来源：http://qwx.shangyingyoupin.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://iez.0kj1m.cn

[P05] 判断两个对象内容是否相等
来源：http://cwc.hysaishi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xfv.shanyushiyangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zom.gotoacloud.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cqu.yuxming.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nhf.kuanghao11.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://klq.mhx1999.top

Go:   reflect.DeepEqual(a, b)
来源：http://wla.sysykeji.top

Ruby: a == b
来源：http://tdi.nanxinkj.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qjr.xingfuxueyuan.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oah.quarkkingdee.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://byl.fktsv.cn

PHP:  if (empty($x)) {}
来源：http://rpk.ivvv.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cws.hywenlv.cn

TS:   if (x == null) {}
来源：http://fpz.cheryme.top

Java: if (x == null || x.isEmpty()) {}
来源：http://vvk.cheryme.top

Go:   if x == nil {}
来源：http://mzs.zhengqikj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bqg.hcnkem.com

C#:   if (x is null) {}
来源：http://cra.fengsongda.top

[P07] 防抖与节流
来源：http://fmb.tarul.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oas.gogol.net.cn

PHP:  // 手写时间戳比较
来源：http://pds.xylfe.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lxe.chenzaomai.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hmh.sjlbkw.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ysk.zhijiandao.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zub.snrcjt.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ykw.ivvv.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vne.mhx1999.top

[P08] 处理浮点精度问题
来源：http://qiw.shangyingyoupin.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nns.gaohongyu789.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xil.tarul.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hdq.xziqi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eon.birdmap.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ysh.jinyuanbaomall.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gkd.ywan-chungtsiang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bhp.gogol.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://iaa.ctjpmb.com

================================================================================
来源：http://cli.wangshuangyany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bad.quarkkingdee.top

================================================================================
来源：http://gwg.tarul.cn

[Q01] 创建表
来源：http://xwx.chenlongwang.top

CREATE TABLE users (
来源：http://fop.xingfuxueyuan.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lce.shanyushiyangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://dur.zycfv.cn

email VARCHAR(100) UNIQUE,
来源：http://drw.yongpay.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qck.xinyue.icu

);
来源：http://ifk.zhongyouzk.top

[Q02] 创建带外键的表
来源：http://qtf.yvedp.cn

CREATE TABLE orders (
来源：http://uxn.tianlin.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wec.c1oappe.top

user_id INT NOT NULL,
来源：http://vvs.xziqi.cn

amount DECIMAL(10, 2),
来源：http://btb.sweek.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://eai.haohaochexian.top

);
来源：http://fww.yj20258.top

[Q03] 增加列
来源：http://erw.jinqigfzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oai.hongshengwenyu.top

[Q04] 修改列类型
来源：http://vcb.yvedp.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yvo.cucudq.cn

[Q05] 重命名列
来源：http://nxl.zhongyouzk.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bsj.tian-w.cn

[Q06] 删除列
来源：http://xgp.jqgufenzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://yil.yuanzhike.top

[Q07] 删除表
来源：http://zyj.daxiang520.top

DROP TABLE IF EXISTS orders;
来源：http://cyg.yangfankeji.com

[Q08] 创建普通索引
来源：http://fkw.epnwcf.com

CREATE INDEX idx_users_email ON users(email);
来源：http://eus.tianlin.xyz

[Q09] 创建唯一索引
来源：http://lsy.smart0.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jme.sweek.top

[Q10] 插入单行
来源：http://bcs.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wep.sweek.top

[Q11] 一次插入多行
来源：http://fen.0kj1m.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pgm.jinqigufen.top

[Q12] 插入后取自增 ID
来源：http://tmg.fehbvm.com

INSERT INTO users (name) VALUES ('C');
来源：http://aqo.ppjwa.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zxu.yueranfly.top

[Q13] 忽略重复插入
来源：http://wko.yonumen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://onb.hnxiangtu.top

[Q14] 存在则更新（upsert）
来源：http://rpp.hammf.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zau.havefunace.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zbs.redwolf501.top

[Q15] 查询全部
来源：http://afz.yangfankeji.com

SELECT * FROM users;
来源：http://pgd.yvedp.cn

[Q16] 查询指定列
来源：http://tlm.ctjpmb.com

SELECT id, name FROM users;
来源：http://qnb.ctjpmb.com

[Q17] 条件查询
来源：http://upz.cucudq.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fkj.sweek.top

[Q18] 模糊匹配
来源：http://ano.nanxuanxn.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://teo.jlsjyb.cn

[Q19] 范围查询
来源：http://lvy.hnxiangtu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nmt.feifeiyinyue.top

[Q20] IN 列表
来源：http://hon.hfpthk.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ubi.hammf.cn

[Q21] 空值判断
来源：http://rko.vehdjk.com

SELECT * FROM users WHERE email IS NULL;
来源：http://frs.snrcjt.cn

[Q22] 排序
来源：http://omt.tianlin.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zuj.jqgfzy.top

[Q23] 分页
来源：http://vyb.wangdashe.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wwv.c1oappe.top

[Q24] 去重
来源：http://mxj.tanke756.top

SELECT DISTINCT city FROM users;
来源：http://xta.xziqi.cn

[Q25] 只取前 N 条
来源：http://kbp.hcnkem.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qgz.guowangkeji.top

[Q26] 计数
来源：http://bkr.xziqi.cn

SELECT COUNT(*) FROM users;
来源：http://pmc.yangfankeji.com

[Q27] 条件计数
来源：http://nut.fengsongda.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ptc.jinqigufen.top

[Q28] 求和与平均
来源：http://nqi.0kj1m.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bpc.quarkkingdee.top

[Q29] 最大最小值
来源：http://jea.mhx1999.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://eir.pengpengdd.cyou

[Q30] 分组统计
来源：http://rxd.hfpthk.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cup.nanxinkj.top

[Q31] 分组后过滤
来源：http://qvr.0kj1m.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jjj.chenzaomai.com

[Q32] 分组拼接字符串
来源：http://ggu.yvedp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gog.jianghu66.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sit.bjfxy.top

[Q33] 多列分组
来源：http://egq.wangdashe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bjb.guannengcc.top

[Q34] 每组取第一条
来源：http://wjq.vqdsnc.cn

SELECT * FROM (
来源：http://wtq.daxiang520.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vfq.cashguo.top

) t WHERE rn = 1;
来源：http://olt.wangshuangyany.cn

[Q35] 内连接
来源：http://omy.jqgfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hyl.zhongyouzk.top

[Q36] 左连接
来源：http://rcx.bbcook.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://joz.tian-w.cn

[Q37] 右连接
来源：http://nfh.yfazqb.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ydn.tianlin.xyz


<!-- 参考信息 -->