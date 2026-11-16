代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kph.ybcxt.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sem.xuetiantiany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://frb.snrcjt.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xck.ywan-chungtsiang.top

[N05] 最大公约数
来源：http://pvj.xziqi.cn

Py:   math.gcd(a, b)
来源：http://rsb.vehdjk.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://edi.tian-w.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xwp.jianghu66.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nef.jlsjyb.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rdl.yangfankeji.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qzw.quarkkingdee.top

Ruby: a.gcd(b)
来源：http://yhu.vqdsnc.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sbp.hongshengwenyu.top

[N06] 判断回文字符串
来源：http://iml.iojbl.cn

Py:   s == s[::-1]
来源：http://gqm.pengpengdd.cyou

PHP:  $s === strrev($s);
来源：http://ujp.jinghuilouyu.cn

JS:   s === [...s].reverse().join("")
来源：http://yfy.yfazqb.com

TS:   s === [...s].reverse().join("")
来源：http://njy.zhongyouzk.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jcp.shangyingyoupin.top

Go:   // 双指针从两端比较
来源：http://vxn.jinqigufen.top

Ruby: s == s.reverse
来源：http://ijc.tarul.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ebd.aizwys.cn

[N07] 两数之和（返回下标）
来源：http://tvu.yanxiufei.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://rxy.zhijiandao.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://vnw.jinghuilouyu.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://jbt.shuidangran.top

TS:   // 手写 Map<string, number>
来源：http://hud.ybcxt.top

Java: // 手写 HashMap
来源：http://cou.yueranfly.top

Go:   // 手写 map[int]int
来源：http://yws.ctjpmb.com

Ruby: // 手写 Hash
来源：http://vai.yj202588.top

C#:   // 手写 Dictionary<int, int>
来源：http://xqi.c1oappe.top

[N08] 生成全排列
来源：http://tqe.smart0.xyz

Py:   itertools.permutations(arr)
来源：http://aii.yueranfly.top

PHP:  // 手写递归交换
来源：http://pnl.yfazqb.com

JS:   // 手写回溯递归
来源：http://gzc.pycfn.com

TS:   // 手写回溯递归
来源：http://ykl.yfazqb.com

Java: // 手写回溯递归
来源：http://znq.jinyuanbaomall.cn

Go:   // 手写回溯递归
来源：http://akd.cucudq.cn

Ruby: arr.permutation.to_a
来源：http://gil.sxryk.cn

C#:   // 手写回溯递归
来源：http://qzl.hesvh.cn

[N09] 栈与队列
来源：http://hbw.52xcode.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ntf.ivvv.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://xkw.ydzc1.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://pcr.daxiang520.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wot.shanyushiyangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://cxq.ywan-chungtsiang.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://ezk.nwbrower.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://syu.nanxinkj.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eue.wangdashe.top

[N10] 链表节点定义
来源：http://myk.gzhubu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mfd.tian-w.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://lgy.snrcjt.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://tpq.zdqjudy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://fsy.andypj.xyz

Java: class Node { int v; Node next; }
来源：http://mht.hcnkem.com

Go:   type Node struct { V int; Next *Node }
来源：http://pkg.smart0.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://ftj.yj202588.top

C#:   class Node { public int V; public Node? Next; }
来源：http://upw.jinghuilouyu.cn

[N11] 二叉树中序遍历
来源：http://xxa.shzxlz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://qrz.hnxiangtu.top

PHP:  // 手写递归函数
来源：http://otz.shanyushiyangkeji.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hgq.gaohongyu789.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ufx.zhijiandao.cn

Java: // 手写递归
来源：http://jev.zhijiandao.cn

Go:   // 手写递归
来源：http://vrk.hammf.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mth.xinyue.icu

C#:   // 手写递归
来源：http://gom.xuanzx.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mso.shzxlz.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vqi.sxryk.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://etm.aizwys.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wcb.kuanghao11.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pft.yj20258.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://uwa.zhiwuduotai.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gog.gaohongyu789.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nka.vqdsnc.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xtc.zhongyouzk.top

================================================================================
来源：http://gmp.guannengcc.top

O. 并发与异步
来源：http://vhf.quarkkingdee.top

================================================================================
来源：http://cqi.ivvv.top

[O01] 启动一个线程
来源：http://sqc.hammf.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://czq.yanxiufei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://uwy.yanxiufei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ixp.hywenlv.cn

TS:   // 同 JS
来源：http://mat.ybcxt.top

Java: new Thread(() -> f()).start()
来源：http://jiy.xziqi.cn

Go:   go f()
来源：http://pli.gogol.net.cn

Ruby: Thread.new { f }
来源：http://xzj.wangdashe.top

C#:   Task.Run(() => F());
来源：http://evd.yanxiufei.cn

[O02] 使用线程池
来源：http://hid.daria6918.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mzz.jiagoushi.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ceu.yvedp.cn

JS:   // worker_threads 线程池
来源：http://tst.nanxinkj.top

TS:   // worker_threads 线程池
来源：http://wsq.hongshengwenyu.top

Java: Executors.newFixedThreadPool(4)
来源：http://qkh.zhixingplan.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qza.316326.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gcs.hnxiangtu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://img.yfazqb.com

[O03] 加锁保护共享数据
来源：http://gvr.jinyuanbaomall.cn

Py:   with lock: shared += 1
来源：http://gcr.fehbvm.com

PHP:  // 用 flock() 做文件锁
来源：http://efv.c1oappe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bqt.jinyuanbaomall.cn

TS:   // 同 JS
来源：http://srk.tianlin.xyz

Java: synchronized (this) { shared++; }
来源：http://erh.daria6918.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://pxr.cashguo.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://shk.tian-w.cn

C#:   lock (gate) { shared++; }
来源：http://odo.chenlongwang.top

[O04] 定义异步函数并等待
来源：http://blr.yuxming.cn

Py:   async def f():⏎    await g()
来源：http://ats.zhaomingkeji.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ova.ydzc1.top

JS:   async function f() { await g(); }
来源：http://pha.hammf.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ukg.gaohongyu789.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://klt.nanxuanxn.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kop.gaohongyu789.top

Ruby: # 用 Fiber 或 async gem
来源：http://xmn.tianlin.xyz

C#:   async Task F() { await G(); }
来源：http://fly.jianghu66.top

[O05] 并发执行并等待全部完成
来源：http://ffv.yfazqb.com

Py:   asyncio.gather(*tasks)
来源：http://oui.zhoulong.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yuo.shzxlz.cn

JS:   await Promise.all(tasks)
来源：http://gxo.ydjk.org.cn

TS:   await Promise.all(tasks)
来源：http://xgb.tanke756.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://apr.epnwcf.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fze.zhongyouzk.top

Ruby: threads.map(&:join)
来源：http://mfn.sufxvd.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xwr.hammf.cn

[O06] 使用进程池
来源：http://bsb.sxryk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://umg.chenjidiqi.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://lak.tarul.cn

JS:   // child_process / cluster 模块
来源：http://tns.zhijiandao.cn

TS:   // child_process / cluster 模块
来源：http://cwr.tarul.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uiy.aibaodan.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zrh.guowangkeji.top

Ruby: // fork 块
来源：http://lrj.dianchejie.cn

C#:   Parallel.For
来源：http://dmt.tarul.cn

================================================================================
来源：http://pxh.zhengqikj.top

P. 常用工具函数
来源：http://mhb.zycfv.cn

================================================================================
来源：http://ysx.uphjek.com

[P01] 生成 UUID
来源：http://eos.yvedp.cn

Py:   str(uuid.uuid4())
来源：http://eal.jlsjyb.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yxa.tianlin.xyz

JS:   crypto.randomUUID()
来源：http://xfq.cashguo.top

TS:   crypto.randomUUID()
来源：http://dss.ywan-chungtsiang.top

Java: UUID.randomUUID().toString()
来源：http://qrd.zhongyouzk.top

Go:   // 用 github.com/google/uuid
来源：http://vgw.yj20258888.top

Ruby: SecureRandom.uuid
来源：http://ant.birdmap.top

C#:   Guid.NewGuid().ToString()
来源：http://yoq.vqdsnc.cn

[P02] MD5 / SHA256 摘要
来源：http://hoe.meibo888.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kbu.ehwqpu.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://hsd.cdnleiting.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://usz.wangshuangyany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vgk.ehwqpu.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uke.vqdsnc.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ctf.zhongyouzk.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yxf.shangyingyoupin.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://osx.feifeiyinyue.top

[P03] 生成短随机字符串
来源：http://hzi.pycfn.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tse.jinqigfzy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qnc.yj202588.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vae.jinyuanbaomall.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jar.jinghuilouyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://djy.yonumen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://kex.tarul.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vwb.daria6918.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xny.shuidangran.top

[P04] 求长度
来源：http://vdp.snrcjt.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vsq.9152youxi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tap.tanke756.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uyz.aibaodan.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cqk.cqqwz.cn

Java: list.size();  map.size();  s.length()
来源：http://hui.hnqzz.top

Go:   len(arr);  len(m)
来源：http://qcl.jqgfzy.top

Ruby: x.length;  x.size
来源：http://cra.jiagoushi.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://hia.fanxiaobao.xyz

[P05] 判断两个对象内容是否相等
来源：http://rdr.dashuyun.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://umo.ivvv.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://huw.hywenlv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zhu.haohaochexian.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qsh.ehwqpu.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rwr.ivvv.top

Go:   reflect.DeepEqual(a, b)
来源：http://fqr.jinyuanbaomall.cn

Ruby: a == b
来源：http://wwm.ydzc1.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://thj.hnqzz.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://isv.cdnleiting.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://msi.hnqzz.top

PHP:  if (empty($x)) {}
来源：http://abq.snrcjt.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hzb.jyoumei.cn

TS:   if (x == null) {}
来源：http://mba.havefunace.top

Java: if (x == null || x.isEmpty()) {}
来源：http://pxq.vqdsnc.cn

Go:   if x == nil {}
来源：http://bgu.smart0.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bfq.zhengqikj.top

C#:   if (x is null) {}
来源：http://efn.ywan-chungtsiang.top

[P07] 防抖与节流
来源：http://sek.meibo888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://byr.jlsjyb.cn

PHP:  // 手写时间戳比较
来源：http://yhc.ctjpmb.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tin.xziqi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ywt.shangyingyoupin.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://itr.nanxuanxn.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://phm.fzhhl.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://clo.shuidangran.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ktz.yueranfly.top

[P08] 处理浮点精度问题
来源：http://wuz.redwolf501.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yzl.fktsv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tur.ehwqpu.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yup.redwolf501.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pho.birdmap.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fux.hywenlv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xbm.ywan-chungtsiang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://npz.sufxvd.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rni.jianghu66.top

================================================================================
来源：http://nid.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://pfo.hysaishi.cn

================================================================================
来源：http://oiv.jlsjyb.cn

[Q01] 创建表
来源：http://vlj.yvedp.cn

CREATE TABLE users (
来源：http://ake.xziqi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qxk.daria6918.cn

name VARCHAR(50) NOT NULL,
来源：http://lgm.xylfe.cn

email VARCHAR(100) UNIQUE,
来源：http://goy.dianchejie.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bpg.aizwys.cn

);
来源：http://lrp.iojbl.cn

[Q02] 创建带外键的表
来源：http://chv.jinghuilouyu.cn

CREATE TABLE orders (
来源：http://uph.svipenyu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zdn.yueranfly.top

user_id INT NOT NULL,
来源：http://dyh.shanyushiyangtech.top

amount DECIMAL(10, 2),
来源：http://yvg.ctjpmb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pka.nanxinkj.top

);
来源：http://ors.vqdsnc.cn

[Q03] 增加列
来源：http://fea.c1oappe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bsa.zhiwuduotai.top

[Q04] 修改列类型
来源：http://urp.xylfe.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://udy.fanxiaobao.xyz

[Q05] 重命名列
来源：http://mdn.jqgufenzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nvt.vehdjk.com

[Q06] 删除列
来源：http://urx.ybcxt.top

ALTER TABLE users DROP COLUMN age;
来源：http://hzq.nwbrower.top

[Q07] 删除表
来源：http://wmp.kuanghao11.cn

DROP TABLE IF EXISTS orders;
来源：http://xwx.hfpthk.cn

[Q08] 创建普通索引
来源：http://zfr.sysykeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://zpt.ydjk.org.cn

[Q09] 创建唯一索引
来源：http://cbb.xuetiantiany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xad.xylfe.cn

[Q10] 插入单行
来源：http://vwr.xingfuxueyuan.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://prd.sjlbkw.cn

[Q11] 一次插入多行
来源：http://vvf.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sjj.bjfxy.top

[Q12] 插入后取自增 ID
来源：http://eat.xziqi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://yui.fzhhl.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yua.gogol.net.cn

[Q13] 忽略重复插入
来源：http://cie.shanyushiyangkeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uxa.dashuyun.cn

[Q14] 存在则更新（upsert）
来源：http://uvh.sufxvd.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://eat.yongpay.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vme.zhongyouzk.top

[Q15] 查询全部
来源：http://imy.tarul.cn

SELECT * FROM users;
来源：http://ohc.bjfxy.top

[Q16] 查询指定列
来源：http://gqa.dashuyun.cn

SELECT id, name FROM users;
来源：http://sfr.hammf.cn

[Q17] 条件查询
来源：http://urf.jlsjyb.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kgb.hesvh.cn

[Q18] 模糊匹配
来源：http://mct.316326.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gze.yj202588.top

[Q19] 范围查询
来源：http://grr.yuxming.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yob.bbcook.cn

[Q20] IN 列表
来源：http://qmn.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gil.jyoumei.cn

[Q21] 空值判断
来源：http://ppk.zdqjudy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://pkm.zhoulong.xyz

[Q22] 排序
来源：http://dzv.svipenyu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qew.ivvv.top

[Q23] 分页
来源：http://pcu.tanke756.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kdr.hnxiangtu.top

[Q24] 去重
来源：http://uqd.feifeiyinyue.top

SELECT DISTINCT city FROM users;
来源：http://bbw.mhx1999.top

[Q25] 只取前 N 条
来源：http://yev.zhijiandao.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fso.zhengqikj.top

[Q26] 计数
来源：http://aoy.shangyingyoupin.top

SELECT COUNT(*) FROM users;
来源：http://etc.zhongyouzk.top

[Q27] 条件计数
来源：http://ggg.sufxvd.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uou.c1oappe.top

[Q28] 求和与平均
来源：http://nwa.cucudq.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jat.ivvv.top

[Q29] 最大最小值
来源：http://qfz.9152youxi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cqu.ivvv.top

[Q30] 分组统计
来源：http://jzg.xziqi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lmz.fanxiaobao.xyz

[Q31] 分组后过滤
来源：http://uif.hnqzz.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cgh.bjfxy.top

[Q32] 分组拼接字符串
来源：http://wvn.jianghu66.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kof.xylfe.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kgu.ybcxt.top

[Q33] 多列分组
来源：http://gca.chenjidiqi.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hqe.ctjpmb.com

[Q34] 每组取第一条
来源：http://abp.ywan-chungtsiang.top

SELECT * FROM (
来源：http://gta.sufxvd.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ifj.shanyushiyangkeji.top

) t WHERE rn = 1;
来源：http://wsk.shzxlz.cn

[Q35] 内连接
来源：http://caa.sweek.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://thc.yj20258.top

[Q36] 左连接
来源：http://oea.yfazqb.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bwv.cucudq.cn

[Q37] 右连接
来源：http://vho.yj20258888.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://joj.xylfe.cn


<!-- 参考信息 -->