代发 wailian999

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nuc.havefunace.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xie.quarkkingdee.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://avi.shuidangran.top

Ruby: a.gcd(b)
来源：http://paj.nanxinkj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://crj.ydjk.org.cn

[N06] 判断回文字符串
来源：http://ymc.fanxiaobao.xyz

Py:   s == s[::-1]
来源：http://hor.aibaodan.cn

PHP:  $s === strrev($s);
来源：http://rhj.zhengqikj.top

JS:   s === [...s].reverse().join("")
来源：http://eaj.hnxiangtu.top

TS:   s === [...s].reverse().join("")
来源：http://xtj.quarkkingdee.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://shx.epnwcf.com

Go:   // 双指针从两端比较
来源：http://brc.xuetiantiany.cn

Ruby: s == s.reverse
来源：http://uzi.yfazqb.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://ntl.havefunace.top

[N07] 两数之和（返回下标）
来源：http://itg.bjfxy.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mht.shanyushiyangtech.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kom.jlsjyb.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://zat.zhiwuduotai.top

TS:   // 手写 Map<string, number>
来源：http://khd.gotoacloud.top

Java: // 手写 HashMap
来源：http://ynq.xingfuxueyuan.xyz

Go:   // 手写 map[int]int
来源：http://gmb.chenzaomai.com

Ruby: // 手写 Hash
来源：http://cvz.fehbvm.com

C#:   // 手写 Dictionary<int, int>
来源：http://gwg.hysaishi.cn

[N08] 生成全排列
来源：http://ygt.aizwys.cn

Py:   itertools.permutations(arr)
来源：http://nik.chenzaomai.com

PHP:  // 手写递归交换
来源：http://dcm.guowangkeji.top

JS:   // 手写回溯递归
来源：http://jnf.smart0.xyz

TS:   // 手写回溯递归
来源：http://mfj.chenzaomai.com

Java: // 手写回溯递归
来源：http://wko.fzhhl.top

Go:   // 手写回溯递归
来源：http://uvh.shanyushiyangtech.top

Ruby: arr.permutation.to_a
来源：http://dwh.uphjek.com

C#:   // 手写回溯递归
来源：http://ptk.aizwys.cn

[N09] 栈与队列
来源：http://qsa.ivvv.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://rzl.vqdsnc.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wfw.sweek.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jiv.svipenyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://cnd.gzhubu.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://voy.dashuyun.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xmk.guannengcc.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://psn.yangfankeji.com

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://fxz.yuxming.cn

[N10] 链表节点定义
来源：http://xko.hcnkem.com

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://tno.hongshengwenyu.top

PHP:  class Node { public $v; public $next = null; }
来源：http://gcx.xuetiantiany.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ijp.zhixingplan.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lwr.birdmap.top

Java: class Node { int v; Node next; }
来源：http://uja.hywenlv.cn

Go:   type Node struct { V int; Next *Node }
来源：http://ggx.dianchejie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://myr.tanke756.top

C#:   class Node { public int V; public Node? Next; }
来源：http://out.ivvv.top

[N11] 二叉树中序遍历
来源：http://qbq.hongshengwenyu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jmp.fzhhl.top

PHP:  // 手写递归函数
来源：http://rnp.c1oappe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wcv.jinqigfzy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kog.yonumen.top

Java: // 手写递归
来源：http://ruy.hywenlv.cn

Go:   // 手写递归
来源：http://kur.hysaishi.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://opf.tanke756.top

C#:   // 手写递归
来源：http://tfp.vqdsnc.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://oqy.yvedp.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ltp.chenjidiqi.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://uzb.nwbrower.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bhv.hywenlv.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://otp.fanxiaobao.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gnw.kuanghao11.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wph.yfazqb.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bjy.shuidangran.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://cpm.hcnkem.com

================================================================================
来源：http://drs.yj20258.top

O. 并发与异步
来源：http://bjq.shuidangran.top

================================================================================
来源：http://ole.nwbrower.top

[O01] 启动一个线程
来源：http://ibd.gaohongyu789.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://shb.dianchejie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vkj.snrcjt.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tfo.fengsongda.top

TS:   // 同 JS
来源：http://gzi.zhixingplan.top

Java: new Thread(() -> f()).start()
来源：http://cjn.kuanghao11.cn

Go:   go f()
来源：http://lwm.vqdsnc.cn

Ruby: Thread.new { f }
来源：http://wyp.shzxlz.cn

C#:   Task.Run(() => F());
来源：http://fsb.shuidangran.top

[O02] 使用线程池
来源：http://qsy.hysaishi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cmv.jiagoushi.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lrj.wangshuangyany.cn

JS:   // worker_threads 线程池
来源：http://ldi.zycfv.cn

TS:   // worker_threads 线程池
来源：http://jcu.hysaishi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://kne.jqgfzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://edp.gzhubu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://qfv.snrcjt.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hfb.0kj1m.cn

[O03] 加锁保护共享数据
来源：http://cqa.jlsjyb.cn

Py:   with lock: shared += 1
来源：http://zho.fzhhl.top

PHP:  // 用 flock() 做文件锁
来源：http://saa.ywan-chungtsiang.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ked.yongpay.top

TS:   // 同 JS
来源：http://hsx.yvedp.cn

Java: synchronized (this) { shared++; }
来源：http://bqz.hnxiangtu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jgo.jlsjyb.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://aly.haohaochexian.top

C#:   lock (gate) { shared++; }
来源：http://fws.cucudq.cn

[O04] 定义异步函数并等待
来源：http://hex.shanyushiyangkeji.top

Py:   async def f():⏎    await g()
来源：http://wci.xuanzx.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rhf.vqdsnc.cn

JS:   async function f() { await g(); }
来源：http://eqz.yanxiufei.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://aya.cdnleiting.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://psc.shzxlz.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kgy.aibaodan.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bzt.chenzaomai.com

C#:   async Task F() { await G(); }
来源：http://vgk.ctjpmb.com

[O05] 并发执行并等待全部完成
来源：http://zhr.xuanzx.com

Py:   asyncio.gather(*tasks)
来源：http://wta.shzxlz.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lbh.fktsv.cn

JS:   await Promise.all(tasks)
来源：http://ywy.xinyue.icu

TS:   await Promise.all(tasks)
来源：http://qxi.quarkkingdee.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zmj.9152youxi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://byu.xingfuxueyuan.xyz

Ruby: threads.map(&:join)
来源：http://ihn.xinyue.icu

C#:   await Task.WhenAll(t1, t2)
来源：http://uyq.tarul.cn

[O06] 使用进程池
来源：http://qya.pycfn.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yji.cashguo.top

PHP:  // pcntl_fork 或多进程队列
来源：http://imu.xziqi.cn

JS:   // child_process / cluster 模块
来源：http://cms.gotoacloud.top

TS:   // child_process / cluster 模块
来源：http://ysu.shangyingyoupin.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hkw.pycfn.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rhd.hysaishi.cn

Ruby: // fork 块
来源：http://yxf.vehdjk.com

C#:   Parallel.For
来源：http://wrm.chenzaomai.com

================================================================================
来源：http://sxz.shzxlz.cn

P. 常用工具函数
来源：http://nru.xinyue.icu

================================================================================
来源：http://mri.pycfn.com

[P01] 生成 UUID
来源：http://jao.chenjidiqi.icu

Py:   str(uuid.uuid4())
来源：http://ykg.yueranfly.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wdp.zhoulong.xyz

JS:   crypto.randomUUID()
来源：http://nxt.yueranfly.top

TS:   crypto.randomUUID()
来源：http://xlg.zdqjudy.top

Java: UUID.randomUUID().toString()
来源：http://skv.sweek.top

Go:   // 用 github.com/google/uuid
来源：http://ndm.xylfe.cn

Ruby: SecureRandom.uuid
来源：http://vln.zhixingplan.top

C#:   Guid.NewGuid().ToString()
来源：http://aqv.sysykeji.top

[P02] MD5 / SHA256 摘要
来源：http://dxs.zhijiandao.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xbt.yonumen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wpm.tarul.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://szk.jlsjyb.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://osn.hammf.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wqt.gotoacloud.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gne.jqgfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uzo.epnwcf.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uhr.iojbl.cn

[P03] 生成短随机字符串
来源：http://lio.guannengcc.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tnr.kuanghao11.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eqh.jinghuilouyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eln.yj20258.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yxi.hesvh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yqo.hnxiangtu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nem.kuanghao11.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hsg.ybcxt.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kxk.zhixingplan.top

[P04] 求长度
来源：http://cme.gaohongyu789.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zuq.nanxinkj.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nuy.cqqwz.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jyk.pycfn.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sce.vqdsnc.cn

Java: list.size();  map.size();  s.length()
来源：http://wcm.zhijiandao.cn

Go:   len(arr);  len(m)
来源：http://aps.chenzaomai.com

Ruby: x.length;  x.size
来源：http://pix.ywan-chungtsiang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://mqh.zhengqikj.top

[P05] 判断两个对象内容是否相等
来源：http://sbj.havefunace.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lvy.hesvh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://otg.jianghu66.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ppm.hysaishi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kei.zhengqikj.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cce.epnwcf.com

Go:   reflect.DeepEqual(a, b)
来源：http://nke.yfazqb.com

Ruby: a == b
来源：http://wbr.haohaochexian.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mmn.daxiang520.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mmo.jinghuilouyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://chp.hnqzz.top

PHP:  if (empty($x)) {}
来源：http://iuk.quarkkingdee.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ype.zycfv.cn

TS:   if (x == null) {}
来源：http://aku.fehbvm.com

Java: if (x == null || x.isEmpty()) {}
来源：http://dlg.hywenlv.cn

Go:   if x == nil {}
来源：http://hkw.jqgfzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oay.hnqzz.top

C#:   if (x is null) {}
来源：http://toh.pycfn.com

[P07] 防抖与节流
来源：http://kcf.hnxiangtu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://arc.ybcxt.top

PHP:  // 手写时间戳比较
来源：http://hkd.hfpthk.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ahi.fzhhl.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ohz.52xcode.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ooe.fanxiaobao.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xmu.feifeiyinyue.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://aqu.zhengqikj.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xmw.ydjk.org.cn

[P08] 处理浮点精度问题
来源：http://rij.gaohongyu789.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://prx.dashuyun.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tzt.xuetiantiany.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mcy.fengsongda.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tlq.jqgufenzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kub.uphjek.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://her.andypj.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ncn.gaohongyu789.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://puk.cheryme.top

================================================================================
来源：http://ute.fengsongda.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kqq.yfazqb.com

================================================================================
来源：http://qxo.meibo888.top

[Q01] 创建表
来源：http://adq.fzhhl.top

CREATE TABLE users (
来源：http://apc.hnxiangtu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xxs.jqgufenzy.top

name VARCHAR(50) NOT NULL,
来源：http://dvs.shuidangran.top

email VARCHAR(100) UNIQUE,
来源：http://dua.andypj.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fqa.nanxinkj.top

);
来源：http://qty.chenzaomai.com

[Q02] 创建带外键的表
来源：http://rco.yj20258.top

CREATE TABLE orders (
来源：http://snv.aibaodan.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rkv.hongshengwenyu.top

user_id INT NOT NULL,
来源：http://kpw.yanxiufei.cn

amount DECIMAL(10, 2),
来源：http://bqp.shzxlz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lyy.cdnleiting.top

);
来源：http://rxj.zhoulong.xyz

[Q03] 增加列
来源：http://yer.ehwqpu.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uxr.shuidangran.top

[Q04] 修改列类型
来源：http://fqr.shzxlz.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://agj.yonumen.top

[Q05] 重命名列
来源：http://mdd.vqdsnc.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mvx.ehwqpu.com

[Q06] 删除列
来源：http://bfy.hysaishi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://zvi.redwolf501.top

[Q07] 删除表
来源：http://zsv.jqgfzy.top

DROP TABLE IF EXISTS orders;
来源：http://gxb.cqqwz.cn

[Q08] 创建普通索引
来源：http://qpc.smart0.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://sko.jqgufenzy.top

[Q09] 创建唯一索引
来源：http://hfg.zdbjq.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lgq.jqgfzy.top

[Q10] 插入单行
来源：http://xsa.c1oappe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://eaz.kuanghao11.cn

[Q11] 一次插入多行
来源：http://mdg.ehwqpu.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lhl.yj20258.top

[Q12] 插入后取自增 ID
来源：http://vnk.hesvh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://otw.ybcxt.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ktp.shanyushiyangtech.top

[Q13] 忽略重复插入
来源：http://okn.ehwqpu.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ceq.pycfn.com

[Q14] 存在则更新（upsert）
来源：http://ndz.fzhhl.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ezw.dianchejie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pnl.wangdashe.top

[Q15] 查询全部
来源：http://qdf.bjfxy.top

SELECT * FROM users;
来源：http://yge.hammf.cn

[Q16] 查询指定列
来源：http://kmc.jinqigfzy.top

SELECT id, name FROM users;
来源：http://cwo.ydzc1.top

[Q17] 条件查询
来源：http://rdn.jqgufenzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://htp.bbcook.cn

[Q18] 模糊匹配
来源：http://tcf.fktsv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://maj.zhengqikj.top

[Q19] 范围查询
来源：http://swb.yueranfly.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cmq.ppjwa.cn

[Q20] IN 列表
来源：http://jvn.zhixingplan.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zlb.jiagoushi.top

[Q21] 空值判断
来源：http://qlf.zycfv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vdx.jyoumei.cn

[Q22] 排序
来源：http://vfu.xuanzx.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yhc.zdqjudy.top

[Q23] 分页
来源：http://ipi.zhongyouzk.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hvu.xylfe.cn

[Q24] 去重
来源：http://quq.ppjwa.cn

SELECT DISTINCT city FROM users;
来源：http://klf.jianghu66.top

[Q25] 只取前 N 条
来源：http://zxm.ctjpmb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://glk.kuanghao11.cn

[Q26] 计数
来源：http://zvx.fktsv.cn

SELECT COUNT(*) FROM users;
来源：http://adt.yvedp.cn

[Q27] 条件计数
来源：http://gns.jlsjyb.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ixv.nwbrower.top

[Q28] 求和与平均
来源：http://qxa.daxiang520.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nog.ydzc1.top

[Q29] 最大最小值
来源：http://snv.vehdjk.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://tko.epnwcf.com

[Q30] 分组统计
来源：http://xva.hesvh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vlo.hongshengwenyu.top

[Q31] 分组后过滤
来源：http://erg.pengpengdd.cyou

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ife.yuanzhike.top

[Q32] 分组拼接字符串
来源：http://cvz.yueranfly.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lot.fehbvm.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sjy.nanxuanxn.top

[Q33] 多列分组
来源：http://dnw.chenjidiqi.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nmf.xuetiantiany.cn

[Q34] 每组取第一条
来源：http://ity.jinqigufen.top

SELECT * FROM (
来源：http://imy.redwolf501.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mgt.snrcjt.cn

) t WHERE rn = 1;
来源：http://nug.gzhubu.top

[Q35] 内连接
来源：http://hgc.vqdsnc.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lca.zdqjudy.top

[Q36] 左连接
来源：http://yhe.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xuy.tian-w.cn

[Q37] 右连接
来源：http://obo.bjfxy.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://isf.hammf.cn

[Q38] 全外连接（PostgreSQL）
来源：http://htz.jinqigufen.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://avx.mhx1999.top

[Q39] 自连接（查上下级）
来源：http://mqz.yj202588.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://afs.zhoulong.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pso.cheryme.top

[Q40] 交叉连接（笛卡尔积）
来源：http://lcr.wangshuangyany.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gvg.yj202588.top

[Q41] 多表连接
来源：http://cep.xinyue.icu


<!-- 参考信息 -->