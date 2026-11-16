代发 wailian999

[N09] 栈与队列
来源：http://raf.zhengqikj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://alf.jinqigufen.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://cmc.ctjpmb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mjh.fehbvm.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://hqo.chenjidiqi.icu

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://xyq.guowangkeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://vgp.snrcjt.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://deg.jianghu66.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wlf.cheryme.top

[N10] 链表节点定义
来源：http://tob.andypj.xyz

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://dyb.sweek.top

PHP:  class Node { public $v; public $next = null; }
来源：http://udx.aizwys.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://whm.jyoumei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rvw.shuidangran.top

Java: class Node { int v; Node next; }
来源：http://uvt.ctjpmb.com

Go:   type Node struct { V int; Next *Node }
来源：http://mzg.shanyushiyangkeji.top

Ruby: Node = Struct.new(:v, :next)
来源：http://pev.andypj.xyz

C#:   class Node { public int V; public Node? Next; }
来源：http://bfc.hesvh.cn

[N11] 二叉树中序遍历
来源：http://hea.hesvh.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://uxl.aizwys.cn

PHP:  // 手写递归函数
来源：http://yki.xuetiantiany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iph.uphjek.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://twi.tianlin.xyz

Java: // 手写递归
来源：http://owc.fanxiaobao.xyz

Go:   // 手写递归
来源：http://dne.pycfn.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cme.ydjk.org.cn

C#:   // 手写递归
来源：http://dnv.chenjidiqi.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://hpr.sweek.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://evt.ivvv.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ykq.c1oappe.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wrj.zhaomingkeji.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oeq.yfazqb.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ebf.quarkkingdee.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://yxt.cucudq.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mzl.zhongyouzk.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zye.havefunace.top

================================================================================
来源：http://dwy.hcnkem.com

O. 并发与异步
来源：http://ymn.tanke756.top

================================================================================
来源：http://jst.zdqjudy.top

[O01] 启动一个线程
来源：http://nhd.hongshengwenyu.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iof.cqqwz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jqu.shzxlz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://byr.ehwqpu.com

TS:   // 同 JS
来源：http://oja.epnwcf.com

Java: new Thread(() -> f()).start()
来源：http://ltq.zhiwuduotai.top

Go:   go f()
来源：http://nsw.yj20258.top

Ruby: Thread.new { f }
来源：http://lec.zhiwuduotai.top

C#:   Task.Run(() => F());
来源：http://rdn.xuanzx.com

[O02] 使用线程池
来源：http://vwd.shuidangran.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rby.vqdsnc.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bqi.sysykeji.top

JS:   // worker_threads 线程池
来源：http://umc.ivvv.top

TS:   // worker_threads 线程池
来源：http://xcr.jqgfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://bar.tanke756.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fus.c1oappe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dex.zdbjq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mel.0kj1m.cn

[O03] 加锁保护共享数据
来源：http://jrs.jinghuilouyu.cn

Py:   with lock: shared += 1
来源：http://jzm.hcnkem.com

PHP:  // 用 flock() 做文件锁
来源：http://npk.jinghuilouyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://svj.bbcook.cn

TS:   // 同 JS
来源：http://tbg.chenzaomai.com

Java: synchronized (this) { shared++; }
来源：http://ptg.chenlongwang.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rmy.chenlongwang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nca.bbcook.cn

C#:   lock (gate) { shared++; }
来源：http://sjd.feifeiyinyue.top

[O04] 定义异步函数并等待
来源：http://rdh.havefunace.top

Py:   async def f():⏎    await g()
来源：http://uyd.aizwys.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dle.c1oappe.top

JS:   async function f() { await g(); }
来源：http://nog.cucudq.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fjn.cheryme.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rai.gogol.net.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cex.c1oappe.top

Ruby: # 用 Fiber 或 async gem
来源：http://kuq.snrcjt.cn

C#:   async Task F() { await G(); }
来源：http://ubi.gaohongyu789.top

[O05] 并发执行并等待全部完成
来源：http://pbz.shuidangran.top

Py:   asyncio.gather(*tasks)
来源：http://vfe.yj20258888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kfx.jyoumei.cn

JS:   await Promise.all(tasks)
来源：http://qtg.jinqigufen.top

TS:   await Promise.all(tasks)
来源：http://scs.gzhubu.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ohd.kuanghao11.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://evr.ybcxt.top

Ruby: threads.map(&:join)
来源：http://upd.fktsv.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kkk.nanxinkj.top

[O06] 使用进程池
来源：http://yrq.yfazqb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://otk.daria6918.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ogw.daria6918.cn

JS:   // child_process / cluster 模块
来源：http://dlv.ivvv.top

TS:   // child_process / cluster 模块
来源：http://xdi.zycfv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mds.hnqzz.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pey.hnxiangtu.top

Ruby: // fork 块
来源：http://rua.xuanzx.com

C#:   Parallel.For
来源：http://ifc.smart0.xyz

================================================================================
来源：http://xag.redwolf501.top

P. 常用工具函数
来源：http://sma.yonumen.top

================================================================================
来源：http://shl.sufxvd.cn

[P01] 生成 UUID
来源：http://und.xylfe.cn

Py:   str(uuid.uuid4())
来源：http://vig.wangdashe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xwj.hcnkem.com

JS:   crypto.randomUUID()
来源：http://oic.nanxuanxn.top

TS:   crypto.randomUUID()
来源：http://goc.jianghu66.top

Java: UUID.randomUUID().toString()
来源：http://clv.haohaochexian.top

Go:   // 用 github.com/google/uuid
来源：http://oph.zhijiandao.cn

Ruby: SecureRandom.uuid
来源：http://nqy.quarkkingdee.top

C#:   Guid.NewGuid().ToString()
来源：http://vom.chenjidiqi.icu

[P02] MD5 / SHA256 摘要
来源：http://tal.havefunace.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xmp.dashuyun.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lyn.xinyue.icu

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pym.zycfv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tuq.dianchejie.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gqv.tian-w.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xes.jinghuilouyu.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://faw.jlsjyb.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gva.epnwcf.com

[P03] 生成短随机字符串
来源：http://wpl.jinqigufen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://neq.gogol.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vvc.havefunace.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pdh.fengsongda.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ghz.bbcook.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tsg.hysaishi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qwr.yj202588.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://law.yj20258.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zkl.316326.xyz

[P04] 求长度
来源：http://uut.shuidangran.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gmd.tian-w.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://agu.ywan-chungtsiang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qlr.sysykeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bqk.xuanzx.com

Java: list.size();  map.size();  s.length()
来源：http://yzf.jinqigufen.top

Go:   len(arr);  len(m)
来源：http://uqb.shzxlz.cn

Ruby: x.length;  x.size
来源：http://mjc.yj20258888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://mlo.fehbvm.com

[P05] 判断两个对象内容是否相等
来源：http://fxt.iojbl.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bhg.pengpengdd.cyou

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kop.jqgufenzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qew.shanyushiyangtech.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zno.xinyue.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ojn.chenjidiqi.icu

Go:   reflect.DeepEqual(a, b)
来源：http://wbq.yfazqb.com

Ruby: a == b
来源：http://hbl.yangfankeji.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://upp.wangdashe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://elm.quarkkingdee.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oxm.smart0.xyz

PHP:  if (empty($x)) {}
来源：http://ipl.ydzc1.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://npd.yj20258888.top

TS:   if (x == null) {}
来源：http://tlp.zhaomingkeji.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://edz.cashguo.top

Go:   if x == nil {}
来源：http://cdw.vehdjk.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nxw.guannengcc.top

C#:   if (x is null) {}
来源：http://seg.epnwcf.com

[P07] 防抖与节流
来源：http://oxb.xuetiantiany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aue.9152youxi.cn

PHP:  // 手写时间戳比较
来源：http://ihv.ydjk.org.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yxd.dianchejie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eme.kuanghao11.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oja.snrcjt.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://skm.meibo888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://tnw.xinyue.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cfh.yj20258.top

[P08] 处理浮点精度问题
来源：http://csm.zhiwuduotai.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hje.nanxuanxn.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://aob.vehdjk.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zhy.yongpay.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jzj.gogol.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nss.smart0.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rql.yvedp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://elo.zhengqikj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pcy.zhengqikj.top

================================================================================
来源：http://kkj.chenjidiqi.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hvl.shuidangran.top

================================================================================
来源：http://upm.tanke756.top

[Q01] 创建表
来源：http://ztg.havefunace.top

CREATE TABLE users (
来源：http://bao.chenjidiqi.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://eob.gaohongyu789.top

name VARCHAR(50) NOT NULL,
来源：http://tby.gotoacloud.top

email VARCHAR(100) UNIQUE,
来源：http://gvv.zycfv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zvy.wangshuangyany.cn

);
来源：http://hah.cqqwz.cn

[Q02] 创建带外键的表
来源：http://ekc.cucudq.cn

CREATE TABLE orders (
来源：http://wtv.epnwcf.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lhs.gogol.net.cn

user_id INT NOT NULL,
来源：http://vyi.yj20258888.top

amount DECIMAL(10, 2),
来源：http://vbn.yj202588.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ddz.xylfe.cn

);
来源：http://bir.fengsongda.top

[Q03] 增加列
来源：http://mlg.c1oappe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ysu.tanke756.top

[Q04] 修改列类型
来源：http://fsq.ctjpmb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://aym.yvedp.cn

[Q05] 重命名列
来源：http://soz.gaohongyu789.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ezi.hammf.cn

[Q06] 删除列
来源：http://oie.tianlin.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://mld.zdqjudy.top

[Q07] 删除表
来源：http://hfx.ppjwa.cn

DROP TABLE IF EXISTS orders;
来源：http://mwx.0kj1m.cn

[Q08] 创建普通索引
来源：http://vhf.xylfe.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qvz.ivvv.top

[Q09] 创建唯一索引
来源：http://aov.daxiang520.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dfm.zhiwuduotai.top

[Q10] 插入单行
来源：http://izo.vehdjk.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pwx.zhaomingkeji.xyz

[Q11] 一次插入多行
来源：http://nzk.cheryme.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uwx.redwolf501.top

[Q12] 插入后取自增 ID
来源：http://gjf.hesvh.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hya.aizwys.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cms.fengsongda.top

[Q13] 忽略重复插入
来源：http://wxs.zhijiandao.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qmz.cdnleiting.top

[Q14] 存在则更新（upsert）
来源：http://hrg.jinghuilouyu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ozm.epnwcf.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hdz.yuanzhike.top

[Q15] 查询全部
来源：http://iet.andypj.xyz

SELECT * FROM users;
来源：http://qrk.hysaishi.cn

[Q16] 查询指定列
来源：http://ejt.dianchejie.cn

SELECT id, name FROM users;
来源：http://qbl.jlsjyb.cn

[Q17] 条件查询
来源：http://nkc.chenlongwang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gzj.uphjek.com

[Q18] 模糊匹配
来源：http://tdj.dashuyun.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dnu.zhengqikj.top

[Q19] 范围查询
来源：http://siu.wangdashe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://igo.hywenlv.cn

[Q20] IN 列表
来源：http://kte.hongshengwenyu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qth.zhongyouzk.top

[Q21] 空值判断
来源：http://mot.jyoumei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://qbj.zhaomingkeji.xyz

[Q22] 排序
来源：http://kai.feifeiyinyue.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pfn.wangdashe.top

[Q23] 分页
来源：http://xwn.aibaodan.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kii.ivvv.top

[Q24] 去重
来源：http://xrh.tian-w.cn

SELECT DISTINCT city FROM users;
来源：http://ake.uphjek.com

[Q25] 只取前 N 条
来源：http://yue.ppjwa.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cwu.yvedp.cn

[Q26] 计数
来源：http://eak.fanxiaobao.xyz

SELECT COUNT(*) FROM users;
来源：http://pvv.tanke756.top

[Q27] 条件计数
来源：http://rsx.zhixingplan.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gtb.chenzaomai.com

[Q28] 求和与平均
来源：http://tqp.cdnleiting.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hlu.sjlbkw.cn

[Q29] 最大最小值
来源：http://dtm.zdbjq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tre.yonumen.top

[Q30] 分组统计
来源：http://prx.cheryme.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ldk.sufxvd.cn

[Q31] 分组后过滤
来源：http://hxa.cqqwz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gmd.daria6918.cn

[Q32] 分组拼接字符串
来源：http://mws.wangdashe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://drx.jyoumei.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hbr.chenjidiqi.icu

[Q33] 多列分组
来源：http://fez.cashguo.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ipu.yj202588.top

[Q34] 每组取第一条
来源：http://dgi.gzhubu.top

SELECT * FROM (
来源：http://uln.jinyuanbaomall.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mov.hysaishi.cn

) t WHERE rn = 1;
来源：http://sjf.xinyue.icu

[Q35] 内连接
来源：http://orw.xylfe.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xxi.316326.xyz

[Q36] 左连接
来源：http://zou.wangshuangyany.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://odv.zhengqikj.top

[Q37] 右连接
来源：http://fyt.jianghu66.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cyt.fzhhl.top

[Q38] 全外连接（PostgreSQL）
来源：http://zhv.yongpay.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pun.wangshuangyany.cn

[Q39] 自连接（查上下级）
来源：http://ttw.epnwcf.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://mut.ydjk.org.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://frm.aizwys.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ckl.ybcxt.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yst.smart0.xyz

[Q41] 多表连接
来源：http://red.nwbrower.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zdy.cdnleiting.top

JOIN users u ON u.id = o.user_id
来源：http://hrh.hnxiangtu.top

JOIN products p ON p.id = o.product_id;
来源：http://hai.cqqwz.cn

[Q42] 连接条件附加过滤
来源：http://kzx.aizwys.cn

SELECT u.name, o.amount FROM users u
来源：http://swt.jyoumei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://htd.jinqigfzy.top

[Q43] 标量子查询
来源：http://zjb.tarul.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://byo.fzhhl.top

[Q44] IN 子查询
来源：http://jcn.jiagoushi.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sev.cdnleiting.top

[Q45] EXISTS 判断存在
来源：http://drc.hongshengwenyu.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qhq.hammf.cn

[Q46] NOT EXISTS 判断不存在
来源：http://loj.hongshengwenyu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://urf.cucudq.cn

[Q47] 与平均值比较
来源：http://tok.pengpengdd.cyou

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ksw.vehdjk.com

[Q48] CTE 公用表表达式
来源：http://kef.zycfv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://clq.zhiwuduotai.top

SELECT * FROM t WHERE c > 5;
来源：http://ptw.haohaochexian.top

[Q49] 更新单行
来源：http://ldf.zhaomingkeji.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://akj.snrcjt.cn

[Q50] 批量更新
来源：http://ssj.fengsongda.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lbv.guannengcc.top

[Q51] 用子查询更新
来源：http://pcy.uphjek.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mxn.daxiang520.top

[Q52] 删除指定行
来源：http://vsa.xuetiantiany.cn

DELETE FROM users WHERE id = 10;
来源：http://xwk.zhiwuduotai.top

[Q53] 按条件删除
来源：http://yrd.ydjk.org.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pwh.aibaodan.cn

[Q54] 清空表
来源：http://hpa.zhiwuduotai.top

TRUNCATE TABLE logs;
来源：http://ikv.shzxlz.cn

[Q55] 排名（并列占位）
来源：http://hgc.svipenyu.cn


<!-- 参考信息 -->