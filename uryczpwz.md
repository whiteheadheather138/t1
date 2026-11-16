代发 wailian999

Py:   itertools.permutations(arr)
来源：http://esg.hywenlv.cn

PHP:  // 手写递归交换
来源：http://ouz.ydzc1.top

JS:   // 手写回溯递归
来源：http://pue.feifeiyinyue.top

TS:   // 手写回溯递归
来源：http://yzh.guowangkeji.top

Java: // 手写回溯递归
来源：http://zlt.hnqzz.top

Go:   // 手写回溯递归
来源：http://gjb.wangdashe.top

Ruby: arr.permutation.to_a
来源：http://fuq.daria6918.cn

C#:   // 手写回溯递归
来源：http://fbg.dashuyun.cn

[N09] 栈与队列
来源：http://ber.fktsv.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ztx.hammf.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rxl.yueranfly.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://flj.svipenyu.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://arx.316326.xyz

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://onp.ctjpmb.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://cjt.zhongyouzk.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qsk.guannengcc.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ezg.sxryk.cn

[N10] 链表节点定义
来源：http://hwg.yvedp.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ebn.meibo888.top

PHP:  class Node { public $v; public $next = null; }
来源：http://sle.birdmap.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mij.daria6918.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ubr.jinyuanbaomall.cn

Java: class Node { int v; Node next; }
来源：http://hac.hongshengwenyu.top

Go:   type Node struct { V int; Next *Node }
来源：http://uqj.ppjwa.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ndd.guannengcc.top

C#:   class Node { public int V; public Node? Next; }
来源：http://zme.zhoulong.xyz

[N11] 二叉树中序遍历
来源：http://idb.chenzaomai.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bmt.jinqigfzy.top

PHP:  // 手写递归函数
来源：http://xpz.ehwqpu.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ytf.aizwys.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mde.yvedp.cn

Java: // 手写递归
来源：http://xjq.0kj1m.cn

Go:   // 手写递归
来源：http://rtb.zhaomingkeji.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vmk.shangyingyoupin.top

C#:   // 手写递归
来源：http://yyq.chenzaomai.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kzf.chenlongwang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xzy.yuanzhike.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gax.ydzc1.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pow.nanxinkj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bff.xylfe.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://alc.mhx1999.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wgj.meibo888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iym.yanxiufei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lpf.hesvh.cn

================================================================================
来源：http://dvu.fengsongda.top

O. 并发与异步
来源：http://vie.cqqwz.cn

================================================================================
来源：http://cqt.yj20258888.top

[O01] 启动一个线程
来源：http://tcc.52xcode.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wzn.yangfankeji.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zik.fktsv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://kph.zdqjudy.top

TS:   // 同 JS
来源：http://tlp.dianchejie.cn

Java: new Thread(() -> f()).start()
来源：http://aqc.ydzc1.top

Go:   go f()
来源：http://gik.jinqigfzy.top

Ruby: Thread.new { f }
来源：http://tub.jinqigufen.top

C#:   Task.Run(() => F());
来源：http://xly.yvedp.cn

[O02] 使用线程池
来源：http://fgl.hnxiangtu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mrq.guannengcc.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rjw.yueranfly.top

JS:   // worker_threads 线程池
来源：http://hbw.hywenlv.cn

TS:   // worker_threads 线程池
来源：http://hrq.cheryme.top

Java: Executors.newFixedThreadPool(4)
来源：http://cqq.nwbrower.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pvn.cucudq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xiw.cqqwz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gyp.haohaochexian.top

[O03] 加锁保护共享数据
来源：http://xml.guowangkeji.top

Py:   with lock: shared += 1
来源：http://nom.yfazqb.com

PHP:  // 用 flock() 做文件锁
来源：http://ihr.ydzc1.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nnu.xylfe.cn

TS:   // 同 JS
来源：http://fmy.yj20258888.top

Java: synchronized (this) { shared++; }
来源：http://gtl.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://neu.cqqwz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://uhy.ywan-chungtsiang.top

C#:   lock (gate) { shared++; }
来源：http://rba.gogol.net.cn

[O04] 定义异步函数并等待
来源：http://xcy.yangfankeji.com

Py:   async def f():⏎    await g()
来源：http://drv.tarul.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xpc.yj20258888.top

JS:   async function f() { await g(); }
来源：http://jab.xinyue.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://dfn.jinyuanbaomall.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fnw.zhengqikj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://faj.fengsongda.top

Ruby: # 用 Fiber 或 async gem
来源：http://hqg.zhaomingkeji.xyz

C#:   async Task F() { await G(); }
来源：http://xvi.xingfuxueyuan.xyz

[O05] 并发执行并等待全部完成
来源：http://fpw.chenjidiqi.icu

Py:   asyncio.gather(*tasks)
来源：http://vop.epnwcf.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mri.shanyushiyangkeji.top

JS:   await Promise.all(tasks)
来源：http://cjn.52xcode.cn

TS:   await Promise.all(tasks)
来源：http://wqz.ydzc1.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hgs.hongshengwenyu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://roy.yanxiufei.cn

Ruby: threads.map(&:join)
来源：http://xhl.wangshuangyany.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ncz.zdbjq.cn

[O06] 使用进程池
来源：http://nuw.xuanzx.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yfm.birdmap.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xpx.hywenlv.cn

JS:   // child_process / cluster 模块
来源：http://xwf.cheryme.top

TS:   // child_process / cluster 模块
来源：http://siw.smart0.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tbl.hcnkem.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kmu.cqqwz.cn

Ruby: // fork 块
来源：http://nyo.hywenlv.cn

C#:   Parallel.For
来源：http://acj.pengpengdd.cyou

================================================================================
来源：http://tgw.jinqigfzy.top

P. 常用工具函数
来源：http://efe.hongshengwenyu.top

================================================================================
来源：http://slx.chenlongwang.top

[P01] 生成 UUID
来源：http://bqr.gotoacloud.top

Py:   str(uuid.uuid4())
来源：http://nxx.hywenlv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ayw.guannengcc.top

JS:   crypto.randomUUID()
来源：http://tux.wangshuangyany.cn

TS:   crypto.randomUUID()
来源：http://mnf.iojbl.cn

Java: UUID.randomUUID().toString()
来源：http://wed.chenzaomai.com

Go:   // 用 github.com/google/uuid
来源：http://wgz.sysykeji.top

Ruby: SecureRandom.uuid
来源：http://mif.gogol.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://deh.havefunace.top

[P02] MD5 / SHA256 摘要
来源：http://pmk.shuidangran.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zhh.0kj1m.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://gpi.fengsongda.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://sar.chenjidiqi.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fvm.tanke756.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qkw.haohaochexian.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sci.haohaochexian.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://muy.ivvv.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qsr.ehwqpu.com

[P03] 生成短随机字符串
来源：http://qwb.zdqjudy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mkb.xuanzx.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xzb.jyoumei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://onq.nanxinkj.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eki.hnqzz.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vsb.chenlongwang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zif.yfazqb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://reh.9152youxi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wxv.zhijiandao.cn

[P04] 求长度
来源：http://dck.jqgufenzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wmr.yj20258888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gua.hnxiangtu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dpt.cheryme.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cti.hnxiangtu.top

Java: list.size();  map.size();  s.length()
来源：http://jbc.hysaishi.cn

Go:   len(arr);  len(m)
来源：http://jct.zdbjq.cn

Ruby: x.length;  x.size
来源：http://wcc.nanxinkj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://doq.kuanghao11.cn

[P05] 判断两个对象内容是否相等
来源：http://qpo.haohaochexian.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://maq.jqgufenzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uei.mhx1999.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zmf.cheryme.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ryr.yuxming.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ezc.jinqigufen.top

Go:   reflect.DeepEqual(a, b)
来源：http://pfu.redwolf501.top

Ruby: a == b
来源：http://xrs.hnxiangtu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iqx.haohaochexian.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uuk.gzhubu.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qla.xuetiantiany.cn

PHP:  if (empty($x)) {}
来源：http://prf.jyoumei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vtv.aibaodan.cn

TS:   if (x == null) {}
来源：http://kve.sysykeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://crd.vehdjk.com

Go:   if x == nil {}
来源：http://caw.hnxiangtu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ysz.cucudq.cn

C#:   if (x is null) {}
来源：http://eej.tarul.cn

[P07] 防抖与节流
来源：http://nrm.ehwqpu.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lbq.ybcxt.top

PHP:  // 手写时间戳比较
来源：http://qyu.fanxiaobao.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rue.guannengcc.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kts.shangyingyoupin.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wbb.xuetiantiany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fby.nanxinkj.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ibf.dashuyun.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fky.quarkkingdee.top

[P08] 处理浮点精度问题
来源：http://mjh.xinyue.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ltu.xuanzx.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qlo.hfpthk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cwo.chenjidiqi.icu

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blx.yuanzhike.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sws.jlsjyb.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fgu.birdmap.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jqd.yj20258888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://att.yangfankeji.com

================================================================================
来源：http://btl.aizwys.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lxx.316326.xyz

================================================================================
来源：http://ngc.fktsv.cn

[Q01] 创建表
来源：http://llh.daria6918.cn

CREATE TABLE users (
来源：http://kpo.hongshengwenyu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hrh.zhijiandao.cn

name VARCHAR(50) NOT NULL,
来源：http://osd.guowangkeji.top

email VARCHAR(100) UNIQUE,
来源：http://yql.ehwqpu.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bfh.ppjwa.cn

);
来源：http://duk.jinqigfzy.top

[Q02] 创建带外键的表
来源：http://vyp.gzhubu.top

CREATE TABLE orders (
来源：http://aon.xuetiantiany.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vbu.yonumen.top

user_id INT NOT NULL,
来源：http://yim.zhiwuduotai.top

amount DECIMAL(10, 2),
来源：http://gcn.ctjpmb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fba.chenlongwang.top

);
来源：http://tja.vqdsnc.cn

[Q03] 增加列
来源：http://ghj.daxiang520.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tul.cheryme.top

[Q04] 修改列类型
来源：http://lpr.jinqigufen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mwj.epnwcf.com

[Q05] 重命名列
来源：http://dea.yvedp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sja.jianghu66.top

[Q06] 删除列
来源：http://cby.fengsongda.top

ALTER TABLE users DROP COLUMN age;
来源：http://zjl.ywan-chungtsiang.top

[Q07] 删除表
来源：http://uvy.yangfankeji.com

DROP TABLE IF EXISTS orders;
来源：http://guy.yonumen.top

[Q08] 创建普通索引
来源：http://atd.fktsv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://epj.birdmap.top

[Q09] 创建唯一索引
来源：http://jfj.gaohongyu789.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jsa.hcnkem.com

[Q10] 插入单行
来源：http://gwv.jiagoushi.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://niw.zhixingplan.top

[Q11] 一次插入多行
来源：http://hye.hesvh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://oww.gotoacloud.top

[Q12] 插入后取自增 ID
来源：http://una.wangdashe.top

INSERT INTO users (name) VALUES ('C');
来源：http://wrk.yfazqb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vah.pycfn.com

[Q13] 忽略重复插入
来源：http://skp.yueranfly.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zdw.zycfv.cn

[Q14] 存在则更新（upsert）
来源：http://fgs.gzhubu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://idt.jqgfzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pgz.cheryme.top

[Q15] 查询全部
来源：http://eau.jinqigufen.top

SELECT * FROM users;
来源：http://jdd.hnxiangtu.top

[Q16] 查询指定列
来源：http://ftw.vehdjk.com

SELECT id, name FROM users;
来源：http://xpt.zhijiandao.cn

[Q17] 条件查询
来源：http://jrx.xuanzx.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://chf.shangyingyoupin.top

[Q18] 模糊匹配
来源：http://dcz.yj20258.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ipd.shzxlz.cn

[Q19] 范围查询
来源：http://gvp.bjfxy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://acg.xylfe.cn

[Q20] IN 列表
来源：http://onf.daxiang520.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://owt.zhaomingkeji.xyz

[Q21] 空值判断
来源：http://amt.jiagoushi.top

SELECT * FROM users WHERE email IS NULL;
来源：http://blg.gzhubu.top

[Q22] 排序
来源：http://rwq.sysykeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://brx.xuanzx.com

[Q23] 分页
来源：http://cvt.fktsv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eaf.tian-w.cn

[Q24] 去重
来源：http://ezc.yj20258.top

SELECT DISTINCT city FROM users;
来源：http://cnx.uphjek.com

[Q25] 只取前 N 条
来源：http://gvb.0kj1m.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jjg.svipenyu.cn

[Q26] 计数
来源：http://cdi.xuanzx.com

SELECT COUNT(*) FROM users;
来源：http://zek.yonumen.top

[Q27] 条件计数
来源：http://neg.yangfankeji.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://apk.cdnleiting.top

[Q28] 求和与平均
来源：http://ofk.feifeiyinyue.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hio.havefunace.top

[Q29] 最大最小值
来源：http://fsl.guannengcc.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ekx.316326.xyz

[Q30] 分组统计
来源：http://pse.havefunace.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pud.tarul.cn

[Q31] 分组后过滤
来源：http://kjq.sjlbkw.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xck.tarul.cn

[Q32] 分组拼接字符串
来源：http://vmx.fehbvm.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://any.hammf.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ize.sjlbkw.cn

[Q33] 多列分组
来源：http://tqy.ywan-chungtsiang.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://eao.guowangkeji.top

[Q34] 每组取第一条
来源：http://ugo.xziqi.cn

SELECT * FROM (
来源：http://rvz.zhijiandao.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gjq.nanxinkj.top

) t WHERE rn = 1;
来源：http://jed.yueranfly.top

[Q35] 内连接
来源：http://tvv.yj20258888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xbo.jinqigufen.top

[Q36] 左连接
来源：http://jgo.cashguo.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zvc.chenjidiqi.icu

[Q37] 右连接
来源：http://hei.kuanghao11.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hvl.haohaochexian.top

[Q38] 全外连接（PostgreSQL）
来源：http://lws.hnxiangtu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fwi.sxryk.cn

[Q39] 自连接（查上下级）
来源：http://vkz.tianlin.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://tol.haohaochexian.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ryj.smart0.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://kib.ywan-chungtsiang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://elu.xziqi.cn

[Q41] 多表连接
来源：http://kyc.ydzc1.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qda.ywan-chungtsiang.top

JOIN users u ON u.id = o.user_id
来源：http://aih.jinghuilouyu.cn

JOIN products p ON p.id = o.product_id;
来源：http://bol.gaohongyu789.top

[Q42] 连接条件附加过滤
来源：http://sfb.guowangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://yip.nwbrower.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wem.mhx1999.top

[Q43] 标量子查询
来源：http://wnf.shuidangran.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tuu.hfpthk.cn

[Q44] IN 子查询
来源：http://ont.wangshuangyany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://aqx.chenjidiqi.icu

[Q45] EXISTS 判断存在
来源：http://zmc.zycfv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iqx.svipenyu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yap.dianchejie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pli.xylfe.cn

[Q47] 与平均值比较
来源：http://diq.ivvv.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pvx.svipenyu.cn

[Q48] CTE 公用表表达式
来源：http://dan.jinqigufen.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ddk.yvedp.cn

SELECT * FROM t WHERE c > 5;
来源：http://sbt.hongshengwenyu.top

[Q49] 更新单行
来源：http://ffw.snrcjt.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gvy.xuanzx.com

[Q50] 批量更新
来源：http://vdw.zhoulong.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lcr.aizwys.cn

[Q51] 用子查询更新
来源：http://baa.tanke756.top


<!-- 参考信息 -->