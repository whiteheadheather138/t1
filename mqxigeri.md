代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ioe.zhongyouzk.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://drm.svipenyu.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://bvj.guowangkeji.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oaa.hesvh.cn

[N05] 最大公约数
来源：http://rcw.daxiang520.top

Py:   math.gcd(a, b)
来源：http://pzx.xingfuxueyuan.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://dpf.guannengcc.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ubv.birdmap.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tko.nanxinkj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hob.xziqi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://saw.jqgufenzy.top

Ruby: a.gcd(b)
来源：http://cvc.pycfn.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pwd.zhaomingkeji.xyz

[N06] 判断回文字符串
来源：http://xav.hesvh.cn

Py:   s == s[::-1]
来源：http://zvh.cucudq.cn

PHP:  $s === strrev($s);
来源：http://zgr.meibo888.top

JS:   s === [...s].reverse().join("")
来源：http://diw.vqdsnc.cn

TS:   s === [...s].reverse().join("")
来源：http://umq.chenlongwang.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://jsb.snrcjt.cn

Go:   // 双指针从两端比较
来源：http://mxz.fktsv.cn

Ruby: s == s.reverse
来源：http://tby.quarkkingdee.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hkh.aibaodan.cn

[N07] 两数之和（返回下标）
来源：http://yfj.sweek.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://axk.chenjidiqi.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ucl.bbcook.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fns.ywan-chungtsiang.top

TS:   // 手写 Map<string, number>
来源：http://rfe.yangfankeji.com

Java: // 手写 HashMap
来源：http://bwt.cqqwz.cn

Go:   // 手写 map[int]int
来源：http://koa.yanxiufei.cn

Ruby: // 手写 Hash
来源：http://opy.zhaomingkeji.xyz

C#:   // 手写 Dictionary<int, int>
来源：http://iyf.yuxming.cn

[N08] 生成全排列
来源：http://vle.hnxiangtu.top

Py:   itertools.permutations(arr)
来源：http://lsh.zhaomingkeji.xyz

PHP:  // 手写递归交换
来源：http://txx.jinqigfzy.top

JS:   // 手写回溯递归
来源：http://ufe.jyoumei.cn

TS:   // 手写回溯递归
来源：http://icd.shanyushiyangtech.top

Java: // 手写回溯递归
来源：http://gvq.havefunace.top

Go:   // 手写回溯递归
来源：http://dfa.yonumen.top

Ruby: arr.permutation.to_a
来源：http://vrh.xylfe.cn

C#:   // 手写回溯递归
来源：http://hdf.52xcode.cn

[N09] 栈与队列
来源：http://ozb.fktsv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tni.jinyuanbaomall.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mus.tanke756.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aut.316326.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://yje.yonumen.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://myk.jiagoushi.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://tlm.meibo888.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ybi.gogol.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pld.pengpengdd.cyou

[N10] 链表节点定义
来源：http://kdm.hongshengwenyu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uey.hammf.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://aqw.feifeiyinyue.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://imi.cdnleiting.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lbu.hysaishi.cn

Java: class Node { int v; Node next; }
来源：http://zpx.cucudq.cn

Go:   type Node struct { V int; Next *Node }
来源：http://kfn.316326.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://eaz.zhoulong.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://raj.zycfv.cn

[N11] 二叉树中序遍历
来源：http://xnr.kuanghao11.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ozm.haohaochexian.top

PHP:  // 手写递归函数
来源：http://ycz.iojbl.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vxn.guowangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kmn.fanxiaobao.xyz

Java: // 手写递归
来源：http://sih.xziqi.cn

Go:   // 手写递归
来源：http://iti.zhiwuduotai.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vjf.jinghuilouyu.cn

C#:   // 手写递归
来源：http://gkh.shuidangran.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://isc.yongpay.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zdr.vehdjk.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://scb.yongpay.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rqj.hcnkem.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gwv.guowangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bzb.shangyingyoupin.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wwd.aibaodan.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fot.uphjek.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://aex.hesvh.cn

================================================================================
来源：http://anb.wangshuangyany.cn

O. 并发与异步
来源：http://rfq.yuanzhike.top

================================================================================
来源：http://ozz.yanxiufei.cn

[O01] 启动一个线程
来源：http://mqv.shuidangran.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vwp.andypj.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://muq.nanxuanxn.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wni.c1oappe.top

TS:   // 同 JS
来源：http://omi.bjfxy.top

Java: new Thread(() -> f()).start()
来源：http://het.bbcook.cn

Go:   go f()
来源：http://jnv.sufxvd.cn

Ruby: Thread.new { f }
来源：http://bbf.mhx1999.top

C#:   Task.Run(() => F());
来源：http://qrp.hnqzz.top

[O02] 使用线程池
来源：http://wag.gzhubu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mzg.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xof.shzxlz.cn

JS:   // worker_threads 线程池
来源：http://ipl.yuxming.cn

TS:   // worker_threads 线程池
来源：http://jfq.vehdjk.com

Java: Executors.newFixedThreadPool(4)
来源：http://xxg.jiagoushi.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://rgt.gogol.net.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zya.quarkkingdee.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zbg.zhiwuduotai.top

[O03] 加锁保护共享数据
来源：http://zjx.daxiang520.top

Py:   with lock: shared += 1
来源：http://ewh.9152youxi.cn

PHP:  // 用 flock() 做文件锁
来源：http://ybf.jyoumei.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pdp.hfpthk.cn

TS:   // 同 JS
来源：http://wun.xuetiantiany.cn

Java: synchronized (this) { shared++; }
来源：http://ihi.zhongyouzk.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ctw.nwbrower.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://pmo.redwolf501.top

C#:   lock (gate) { shared++; }
来源：http://twd.yanxiufei.cn

[O04] 定义异步函数并等待
来源：http://ssa.hnxiangtu.top

Py:   async def f():⏎    await g()
来源：http://hyf.pengpengdd.cyou

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lwk.cucudq.cn

JS:   async function f() { await g(); }
来源：http://yzj.wangshuangyany.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://twy.daria6918.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dff.hnxiangtu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gcp.xziqi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bis.zdqjudy.top

C#:   async Task F() { await G(); }
来源：http://uok.pengpengdd.cyou

[O05] 并发执行并等待全部完成
来源：http://eqc.bbcook.cn

Py:   asyncio.gather(*tasks)
来源：http://fqk.kuanghao11.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://akr.tian-w.cn

JS:   await Promise.all(tasks)
来源：http://hnp.c1oappe.top

TS:   await Promise.all(tasks)
来源：http://ukk.ybcxt.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oah.hfpthk.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ima.ctjpmb.com

Ruby: threads.map(&:join)
来源：http://ewu.yanxiufei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fzg.chenzaomai.com

[O06] 使用进程池
来源：http://njz.nanxuanxn.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kxj.ydjk.org.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wij.chenlongwang.top

JS:   // child_process / cluster 模块
来源：http://tza.svipenyu.cn

TS:   // child_process / cluster 模块
来源：http://ytj.jqgfzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://scu.hnxiangtu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jti.daxiang520.top

Ruby: // fork 块
来源：http://fue.tianlin.xyz

C#:   Parallel.For
来源：http://qgq.yangfankeji.com

================================================================================
来源：http://krh.shanyushiyangkeji.top

P. 常用工具函数
来源：http://tbv.epnwcf.com

================================================================================
来源：http://hrh.tarul.cn

[P01] 生成 UUID
来源：http://hgn.svipenyu.cn

Py:   str(uuid.uuid4())
来源：http://lzw.pycfn.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lyu.chenlongwang.top

JS:   crypto.randomUUID()
来源：http://qen.zhongyouzk.top

TS:   crypto.randomUUID()
来源：http://qjc.fzhhl.top

Java: UUID.randomUUID().toString()
来源：http://enj.dianchejie.cn

Go:   // 用 github.com/google/uuid
来源：http://fmd.hongshengwenyu.top

Ruby: SecureRandom.uuid
来源：http://gpo.ybcxt.top

C#:   Guid.NewGuid().ToString()
来源：http://kyl.jinyuanbaomall.cn

[P02] MD5 / SHA256 摘要
来源：http://qqt.chenjidiqi.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ykw.vqdsnc.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lnu.aizwys.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://efk.shanyushiyangkeji.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://cia.jianghu66.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ahs.zhongyouzk.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jea.zhaomingkeji.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qrs.zhixingplan.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vcv.quarkkingdee.top

[P03] 生成短随机字符串
来源：http://pty.hcnkem.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wuz.fzhhl.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jzn.jinqigfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fxm.0kj1m.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kmc.kuanghao11.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yng.jyoumei.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://oui.snrcjt.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xtl.fanxiaobao.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cgk.mhx1999.top

[P04] 求长度
来源：http://tcz.ehwqpu.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://okq.jinqigfzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rki.daria6918.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nzm.tian-w.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zqr.smart0.xyz

Java: list.size();  map.size();  s.length()
来源：http://xrq.svipenyu.cn

Go:   len(arr);  len(m)
来源：http://dzc.nanxinkj.top

Ruby: x.length;  x.size
来源：http://fef.c1oappe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zwu.vehdjk.com

[P05] 判断两个对象内容是否相等
来源：http://gnb.gaohongyu789.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://rty.zycfv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kpe.fanxiaobao.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kcv.sufxvd.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dvg.zdbjq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uoi.hywenlv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bbm.xylfe.cn

Ruby: a == b
来源：http://qni.yj20258888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dba.bbcook.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rvj.xinyue.icu

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hfv.zhixingplan.top

PHP:  if (empty($x)) {}
来源：http://wop.shanyushiyangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://swm.hysaishi.cn

TS:   if (x == null) {}
来源：http://xwg.0kj1m.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://jmv.yvedp.cn

Go:   if x == nil {}
来源：http://tjz.epnwcf.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lsc.pengpengdd.cyou

C#:   if (x is null) {}
来源：http://mun.chenzaomai.com

[P07] 防抖与节流
来源：http://ysc.meibo888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mzc.andypj.xyz

PHP:  // 手写时间戳比较
来源：http://edn.andypj.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cwh.bjfxy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://irf.shzxlz.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fxl.dianchejie.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ugb.haohaochexian.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://yjj.xingfuxueyuan.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ejz.ybcxt.top

[P08] 处理浮点精度问题
来源：http://wbz.daxiang520.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yvy.zdbjq.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ico.52xcode.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://coy.ppjwa.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qld.ivvv.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zln.0kj1m.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iec.chenzaomai.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ibh.ywan-chungtsiang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wet.ydjk.org.cn

================================================================================
来源：http://hem.cucudq.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wgs.wangshuangyany.cn

================================================================================
来源：http://kzc.cdnleiting.top

[Q01] 创建表
来源：http://neu.kuanghao11.cn

CREATE TABLE users (
来源：http://avo.feifeiyinyue.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dry.wangshuangyany.cn

name VARCHAR(50) NOT NULL,
来源：http://wpr.hnqzz.top

email VARCHAR(100) UNIQUE,
来源：http://znm.hongshengwenyu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qxh.wangshuangyany.cn

);
来源：http://iav.havefunace.top

[Q02] 创建带外键的表
来源：http://rrd.yuanzhike.top

CREATE TABLE orders (
来源：http://pag.hcnkem.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hbz.wangshuangyany.cn

user_id INT NOT NULL,
来源：http://crd.chenzaomai.com

amount DECIMAL(10, 2),
来源：http://lnq.mhx1999.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://zos.sxryk.cn

);
来源：http://dve.kuanghao11.cn

[Q03] 增加列
来源：http://kog.fktsv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://etg.cucudq.cn

[Q04] 修改列类型
来源：http://web.guannengcc.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://atu.uphjek.com

[Q05] 重命名列
来源：http://ljs.aibaodan.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dje.hywenlv.cn

[Q06] 删除列
来源：http://tdv.hywenlv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://npd.fzhhl.top

[Q07] 删除表
来源：http://buk.hywenlv.cn

DROP TABLE IF EXISTS orders;
来源：http://iov.shuidangran.top

[Q08] 创建普通索引
来源：http://fcc.ehwqpu.com

CREATE INDEX idx_users_email ON users(email);
来源：http://vsi.hnqzz.top

[Q09] 创建唯一索引
来源：http://oxz.jinghuilouyu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oya.andypj.xyz

[Q10] 插入单行
来源：http://vnv.svipenyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cum.gotoacloud.top

[Q11] 一次插入多行
来源：http://ggc.cdnleiting.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://oni.ppjwa.cn

[Q12] 插入后取自增 ID
来源：http://ugc.jinghuilouyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://glc.shanyushiyangtech.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tzh.gotoacloud.top

[Q13] 忽略重复插入
来源：http://wve.jyoumei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xgz.snrcjt.cn

[Q14] 存在则更新（upsert）
来源：http://fcn.jqgfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mpl.andypj.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zap.hammf.cn

[Q15] 查询全部
来源：http://bbz.52xcode.cn

SELECT * FROM users;
来源：http://aws.cashguo.top

[Q16] 查询指定列
来源：http://gfz.jinghuilouyu.cn

SELECT id, name FROM users;
来源：http://qvx.tianlin.xyz

[Q17] 条件查询
来源：http://owh.wangshuangyany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lzb.snrcjt.cn

[Q18] 模糊匹配
来源：http://yeb.fzhhl.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lbg.chenjidiqi.icu

[Q19] 范围查询
来源：http://aqg.hesvh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jgv.daria6918.cn

[Q20] IN 列表
来源：http://zfd.ydjk.org.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nqp.0kj1m.cn

[Q21] 空值判断
来源：http://tfk.hywenlv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://fpe.jinghuilouyu.cn

[Q22] 排序
来源：http://skt.shzxlz.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dnb.hnxiangtu.top

[Q23] 分页
来源：http://tka.c1oappe.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ftf.0kj1m.cn

[Q24] 去重
来源：http://iis.tanke756.top

SELECT DISTINCT city FROM users;
来源：http://dcq.uphjek.com

[Q25] 只取前 N 条
来源：http://rqv.pengpengdd.cyou

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ser.yuanzhike.top

[Q26] 计数
来源：http://nzj.xylfe.cn

SELECT COUNT(*) FROM users;
来源：http://ror.zhongyouzk.top

[Q27] 条件计数
来源：http://wnf.hysaishi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://npd.xziqi.cn

[Q28] 求和与平均
来源：http://zvx.316326.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://buh.shanyushiyangtech.top

[Q29] 最大最小值
来源：http://vsk.shzxlz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://abr.yongpay.top

[Q30] 分组统计
来源：http://bhk.zdqjudy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://iqs.fengsongda.top

[Q31] 分组后过滤
来源：http://skx.gotoacloud.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ihf.shzxlz.cn

[Q32] 分组拼接字符串
来源：http://kca.jinghuilouyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vep.jiagoushi.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://guh.jinqigfzy.top

[Q33] 多列分组
来源：http://oxw.gaohongyu789.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mjh.cashguo.top

[Q34] 每组取第一条
来源：http://ttz.andypj.xyz

SELECT * FROM (
来源：http://enu.gzhubu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://efk.xziqi.cn

) t WHERE rn = 1;
来源：http://akw.cashguo.top

[Q35] 内连接
来源：http://prd.xuanzx.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ors.zdbjq.cn

[Q36] 左连接
来源：http://yrh.hammf.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gve.sufxvd.cn

[Q37] 右连接
来源：http://gxb.uphjek.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lvy.cashguo.top


<!-- 参考信息 -->