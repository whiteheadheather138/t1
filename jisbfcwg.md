代发 wailian999

Py:   itertools.permutations(arr)
来源：http://iza.shzxlz.cn

PHP:  // 手写递归交换
来源：http://qiv.shuidangran.top

JS:   // 手写回溯递归
来源：http://vdw.yuxming.cn

TS:   // 手写回溯递归
来源：http://yjl.havefunace.top

Java: // 手写回溯递归
来源：http://lqx.ybcxt.top

Go:   // 手写回溯递归
来源：http://ghj.dashuyun.cn

Ruby: arr.permutation.to_a
来源：http://fpw.jinghuilouyu.cn

C#:   // 手写回溯递归
来源：http://grq.fengsongda.top

[N09] 栈与队列
来源：http://ceb.yongpay.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://fye.yangfankeji.com

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://eov.fktsv.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://egd.kuanghao11.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://aae.sxryk.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dme.jqgufenzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://flo.hywenlv.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qyf.xinyue.icu

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nit.tanke756.top

[N10] 链表节点定义
来源：http://jgz.ydzc1.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://aky.yongpay.top

PHP:  class Node { public $v; public $next = null; }
来源：http://zbk.jqgfzy.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pou.nwbrower.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wru.yj202588.top

Java: class Node { int v; Node next; }
来源：http://kog.pengpengdd.cyou

Go:   type Node struct { V int; Next *Node }
来源：http://knn.shangyingyoupin.top

Ruby: Node = Struct.new(:v, :next)
来源：http://hvz.316326.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://bxm.andypj.xyz

[N11] 二叉树中序遍历
来源：http://bbd.zycfv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yuf.gogol.net.cn

PHP:  // 手写递归函数
来源：http://icr.tian-w.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://diz.fengsongda.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://obq.daxiang520.top

Java: // 手写递归
来源：http://kau.316326.xyz

Go:   // 手写递归
来源：http://zyg.c1oappe.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://awy.shanyushiyangtech.top

C#:   // 手写递归
来源：http://xbh.0kj1m.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://tcd.havefunace.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://myb.jlsjyb.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ery.gzhubu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jvz.hnqzz.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://szk.zhiwuduotai.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://sxg.hywenlv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://pfq.shanyushiyangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://dpe.ybcxt.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fed.xuetiantiany.cn

================================================================================
来源：http://rza.hysaishi.cn

O. 并发与异步
来源：http://czy.sjlbkw.cn

================================================================================
来源：http://pkm.redwolf501.top

[O01] 启动一个线程
来源：http://dnq.ppjwa.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://poy.gogol.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xqb.hcnkem.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://esi.cashguo.top

TS:   // 同 JS
来源：http://vyg.redwolf501.top

Java: new Thread(() -> f()).start()
来源：http://xie.fehbvm.com

Go:   go f()
来源：http://rhm.yongpay.top

Ruby: Thread.new { f }
来源：http://dfv.birdmap.top

C#:   Task.Run(() => F());
来源：http://xjm.snrcjt.cn

[O02] 使用线程池
来源：http://fzc.daxiang520.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gju.ppjwa.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vue.dashuyun.cn

JS:   // worker_threads 线程池
来源：http://lvg.sxryk.cn

TS:   // worker_threads 线程池
来源：http://koc.xinyue.icu

Java: Executors.newFixedThreadPool(4)
来源：http://aqr.cheryme.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cas.jiagoushi.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mlv.cheryme.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rwr.ydzc1.top

[O03] 加锁保护共享数据
来源：http://gqp.sxryk.cn

Py:   with lock: shared += 1
来源：http://sel.uphjek.com

PHP:  // 用 flock() 做文件锁
来源：http://zpl.316326.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://yae.yuanzhike.top

TS:   // 同 JS
来源：http://ial.zhongyouzk.top

Java: synchronized (this) { shared++; }
来源：http://jyv.jinqigfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://csq.wangdashe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://xyp.shzxlz.cn

C#:   lock (gate) { shared++; }
来源：http://wcu.yonumen.top

[O04] 定义异步函数并等待
来源：http://pqh.0kj1m.cn

Py:   async def f():⏎    await g()
来源：http://omz.shanyushiyangkeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://quq.zhijiandao.cn

JS:   async function f() { await g(); }
来源：http://nvk.andypj.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://pff.iojbl.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hon.shangyingyoupin.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://for.epnwcf.com

Ruby: # 用 Fiber 或 async gem
来源：http://ymj.jqgufenzy.top

C#:   async Task F() { await G(); }
来源：http://udf.xylfe.cn

[O05] 并发执行并等待全部完成
来源：http://tdr.haohaochexian.top

Py:   asyncio.gather(*tasks)
来源：http://lvd.wangshuangyany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tib.fengsongda.top

JS:   await Promise.all(tasks)
来源：http://aed.sxryk.cn

TS:   await Promise.all(tasks)
来源：http://jxq.shangyingyoupin.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ihn.jianghu66.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ras.hysaishi.cn

Ruby: threads.map(&:join)
来源：http://ruc.bjfxy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://tbx.dashuyun.cn

[O06] 使用进程池
来源：http://zql.shanyushiyangtech.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tyo.havefunace.top

PHP:  // pcntl_fork 或多进程队列
来源：http://tvm.zdbjq.cn

JS:   // child_process / cluster 模块
来源：http://ruk.meibo888.top

TS:   // child_process / cluster 模块
来源：http://rpn.smart0.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yeu.nanxinkj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vvl.zdbjq.cn

Ruby: // fork 块
来源：http://csc.ybcxt.top

C#:   Parallel.For
来源：http://ubv.316326.xyz

================================================================================
来源：http://erv.hnxiangtu.top

P. 常用工具函数
来源：http://tuo.hywenlv.cn

================================================================================
来源：http://tqe.pengpengdd.cyou

[P01] 生成 UUID
来源：http://fzx.jinyuanbaomall.cn

Py:   str(uuid.uuid4())
来源：http://xxb.sweek.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vas.mhx1999.top

JS:   crypto.randomUUID()
来源：http://ilf.pycfn.com

TS:   crypto.randomUUID()
来源：http://mep.zhongyouzk.top

Java: UUID.randomUUID().toString()
来源：http://elt.sxryk.cn

Go:   // 用 github.com/google/uuid
来源：http://rvx.hnqzz.top

Ruby: SecureRandom.uuid
来源：http://miv.ehwqpu.com

C#:   Guid.NewGuid().ToString()
来源：http://jnt.shzxlz.cn

[P02] MD5 / SHA256 摘要
来源：http://pyf.quarkkingdee.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xcv.zycfv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://uld.shuidangran.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://puv.quarkkingdee.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uqq.daxiang520.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://plm.uphjek.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xwu.ehwqpu.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kle.zhengqikj.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ujr.jlsjyb.cn

[P03] 生成短随机字符串
来源：http://sku.daria6918.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cja.haohaochexian.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dgc.yonumen.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uzp.yangfankeji.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nvo.ctjpmb.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iow.fehbvm.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cok.redwolf501.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://izx.jiagoushi.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://iii.fktsv.cn

[P04] 求长度
来源：http://krm.ywan-chungtsiang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://drm.ydjk.org.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gcq.iojbl.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ytp.zdqjudy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ffy.guannengcc.top

Java: list.size();  map.size();  s.length()
来源：http://uaj.cucudq.cn

Go:   len(arr);  len(m)
来源：http://qiu.iojbl.cn

Ruby: x.length;  x.size
来源：http://tsh.yanxiufei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wmf.wangshuangyany.cn

[P05] 判断两个对象内容是否相等
来源：http://vpr.52xcode.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gky.gogol.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://yrz.yj20258888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gaz.daria6918.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fte.xuetiantiany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hqi.zycfv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dgx.hnxiangtu.top

Ruby: a == b
来源：http://huc.zhoulong.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vqh.ctjpmb.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mly.aibaodan.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ria.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}
来源：http://xow.jqgufenzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vyt.aibaodan.cn

TS:   if (x == null) {}
来源：http://lno.zycfv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://oeb.shanyushiyangtech.top

Go:   if x == nil {}
来源：http://kgx.zhixingplan.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://rce.fzhhl.top

C#:   if (x is null) {}
来源：http://zhh.shzxlz.cn

[P07] 防抖与节流
来源：http://mve.sweek.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fyj.yueranfly.top

PHP:  // 手写时间戳比较
来源：http://fql.hfpthk.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qha.jinghuilouyu.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ozy.xylfe.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xwm.andypj.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://oai.uphjek.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://kxm.chenzaomai.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xvk.yanxiufei.cn

[P08] 处理浮点精度问题
来源：http://any.wangshuangyany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://icw.hywenlv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://evr.fehbvm.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lwr.zhongyouzk.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vbb.shuidangran.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qmr.wangdashe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://htz.hywenlv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xgh.jinqigufen.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://myc.cheryme.top

================================================================================
来源：http://eze.sufxvd.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dpi.yanxiufei.cn

================================================================================
来源：http://ilj.uphjek.com

[Q01] 创建表
来源：http://yud.zhixingplan.top

CREATE TABLE users (
来源：http://dxw.hnqzz.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jeg.cashguo.top

name VARCHAR(50) NOT NULL,
来源：http://lwx.yj202588.top

email VARCHAR(100) UNIQUE,
来源：http://ifu.daria6918.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gqq.zhongyouzk.top

);
来源：http://hon.hysaishi.cn

[Q02] 创建带外键的表
来源：http://imv.yvedp.cn

CREATE TABLE orders (
来源：http://ekh.nanxinkj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://erl.pengpengdd.cyou

user_id INT NOT NULL,
来源：http://pne.hammf.cn

amount DECIMAL(10, 2),
来源：http://dor.daxiang520.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bww.snrcjt.cn

);
来源：http://uwh.kuanghao11.cn

[Q03] 增加列
来源：http://jpk.vqdsnc.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hjm.yj20258888.top

[Q04] 修改列类型
来源：http://dbr.mhx1999.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://juo.wangshuangyany.cn

[Q05] 重命名列
来源：http://sot.yvedp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ddg.jinyuanbaomall.cn

[Q06] 删除列
来源：http://rkp.wangshuangyany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ues.jinqigfzy.top

[Q07] 删除表
来源：http://dai.hammf.cn

DROP TABLE IF EXISTS orders;
来源：http://uig.redwolf501.top

[Q08] 创建普通索引
来源：http://knw.cashguo.top

CREATE INDEX idx_users_email ON users(email);
来源：http://aak.fehbvm.com

[Q09] 创建唯一索引
来源：http://dsu.ybcxt.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lsf.xylfe.cn

[Q10] 插入单行
来源：http://hsp.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dka.mhx1999.top

[Q11] 一次插入多行
来源：http://ahs.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://leo.uphjek.com

[Q12] 插入后取自增 ID
来源：http://aly.gogol.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vpp.guowangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://umo.pycfn.com

[Q13] 忽略重复插入
来源：http://qni.hesvh.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rwk.yvedp.cn

[Q14] 存在则更新（upsert）
来源：http://cys.birdmap.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kfx.chenjidiqi.icu

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rld.iojbl.cn

[Q15] 查询全部
来源：http://cen.yueranfly.top

SELECT * FROM users;
来源：http://urq.cqqwz.cn

[Q16] 查询指定列
来源：http://lfg.mhx1999.top

SELECT id, name FROM users;
来源：http://ajh.ctjpmb.com

[Q17] 条件查询
来源：http://ryg.hywenlv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qyf.jqgfzy.top

[Q18] 模糊匹配
来源：http://gym.shanyushiyangkeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kij.fzhhl.top

[Q19] 范围查询
来源：http://jne.daxiang520.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ign.ivvv.top

[Q20] IN 列表
来源：http://mhm.yj20258888.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://djt.zhongyouzk.top

[Q21] 空值判断
来源：http://ddj.tarul.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gix.chenlongwang.top

[Q22] 排序
来源：http://pyc.jinyuanbaomall.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gji.hnqzz.top

[Q23] 分页
来源：http://ifh.yvedp.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kao.fzhhl.top

[Q24] 去重
来源：http://pex.zdqjudy.top

SELECT DISTINCT city FROM users;
来源：http://tel.ywan-chungtsiang.top

[Q25] 只取前 N 条
来源：http://xbh.sjlbkw.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zah.ppjwa.cn

[Q26] 计数
来源：http://msz.hammf.cn

SELECT COUNT(*) FROM users;
来源：http://kvv.daria6918.cn

[Q27] 条件计数
来源：http://pzy.nanxuanxn.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gkv.dashuyun.cn

[Q28] 求和与平均
来源：http://jhz.ehwqpu.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://aqo.ydjk.org.cn

[Q29] 最大最小值
来源：http://zbu.aizwys.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://roc.hesvh.cn

[Q30] 分组统计
来源：http://lhm.gzhubu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vxm.ywan-chungtsiang.top

[Q31] 分组后过滤
来源：http://wer.uphjek.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yqf.zhengqikj.top

[Q32] 分组拼接字符串
来源：http://rjn.zhixingplan.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dzm.dashuyun.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://whb.gogol.net.cn

[Q33] 多列分组
来源：http://uuk.guannengcc.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zvy.hnqzz.top

[Q34] 每组取第一条
来源：http://hzg.ydjk.org.cn

SELECT * FROM (
来源：http://rkt.fzhhl.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jnb.sjlbkw.cn

) t WHERE rn = 1;
来源：http://nzy.hesvh.cn

[Q35] 内连接
来源：http://eox.tian-w.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rje.jinghuilouyu.cn

[Q36] 左连接
来源：http://plu.guowangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sxm.shangyingyoupin.top

[Q37] 右连接
来源：http://tub.shuidangran.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zag.hesvh.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mcy.kuanghao11.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jsp.pycfn.com

[Q39] 自连接（查上下级）
来源：http://ctl.jinqigfzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://uge.sysykeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ykf.birdmap.top

[Q40] 交叉连接（笛卡尔积）
来源：http://tcf.xuetiantiany.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dgf.sjlbkw.cn

[Q41] 多表连接
来源：http://cbe.jyoumei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lux.yfazqb.com

JOIN users u ON u.id = o.user_id
来源：http://jyd.yueranfly.top

JOIN products p ON p.id = o.product_id;
来源：http://jrl.jqgfzy.top

[Q42] 连接条件附加过滤
来源：http://srg.dashuyun.cn

SELECT u.name, o.amount FROM users u
来源：http://buh.hnqzz.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://iom.sysykeji.top

[Q43] 标量子查询
来源：http://tbk.snrcjt.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://aad.tianlin.xyz

[Q44] IN 子查询
来源：http://smb.cdnleiting.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://asb.daxiang520.top

[Q45] EXISTS 判断存在
来源：http://hdk.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hqn.sufxvd.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vio.c1oappe.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xrq.cheryme.top

[Q47] 与平均值比较
来源：http://zwv.xylfe.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kbn.xylfe.cn

[Q48] CTE 公用表表达式
来源：http://hkq.wangshuangyany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vzm.shanyushiyangkeji.top

SELECT * FROM t WHERE c > 5;
来源：http://chs.jinqigfzy.top

[Q49] 更新单行
来源：http://evc.cdnleiting.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mfa.iojbl.cn

[Q50] 批量更新
来源：http://sut.shanyushiyangtech.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jwk.vqdsnc.cn

[Q51] 用子查询更新
来源：http://ehi.jinyuanbaomall.cn


<!-- 参考信息 -->