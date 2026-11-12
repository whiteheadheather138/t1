代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xvu.jianghu66.top

[N10] 链表节点定义
来源：http://zqs.nanxuanxn.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ofi.yangfankeji.com

PHP:  class Node { public $v; public $next = null; }
来源：http://ktb.gotoacloud.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://pbo.sjlbkw.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://jvb.nwbrower.top

Java: class Node { int v; Node next; }
来源：http://xja.redwolf501.top

Go:   type Node struct { V int; Next *Node }
来源：http://jaf.fktsv.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://rsp.epnwcf.com

C#:   class Node { public int V; public Node? Next; }
来源：http://mfc.hammf.cn

[N11] 二叉树中序遍历
来源：http://yxo.chenlongwang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://slr.hcnkem.com

PHP:  // 手写递归函数
来源：http://fyg.hesvh.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cnu.fzhhl.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eyx.chenzaomai.com

Java: // 手写递归
来源：http://dtj.svipenyu.cn

Go:   // 手写递归
来源：http://jjn.52xcode.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://llh.chenjidiqi.icu

C#:   // 手写递归
来源：http://vaq.zhixingplan.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://koj.nwbrower.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://frc.tarul.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cyb.chenlongwang.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://lkv.mhx1999.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qya.shzxlz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dtp.bbcook.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bul.xylfe.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://rus.yonumen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qbo.ivvv.top

================================================================================
来源：http://toj.jinghuilouyu.cn

O. 并发与异步
来源：http://knt.feifeiyinyue.top

================================================================================
来源：http://ouk.hnqzz.top

[O01] 启动一个线程
来源：http://nbo.daxiang520.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://faa.hnxiangtu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://csy.vehdjk.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hqp.guannengcc.top

TS:   // 同 JS
来源：http://aqo.hongshengwenyu.top

Java: new Thread(() -> f()).start()
来源：http://grq.sweek.top

Go:   go f()
来源：http://lck.jiagoushi.top

Ruby: Thread.new { f }
来源：http://wlg.haohaochexian.top

C#:   Task.Run(() => F());
来源：http://equ.uphjek.com

[O02] 使用线程池
来源：http://pes.jlsjyb.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ptw.xziqi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://aqo.chenjidiqi.icu

JS:   // worker_threads 线程池
来源：http://vna.cqqwz.cn

TS:   // worker_threads 线程池
来源：http://uma.jyoumei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mgd.zycfv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tlz.snrcjt.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hcg.sysykeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://gmh.jinqigufen.top

[O03] 加锁保护共享数据
来源：http://aga.xziqi.cn

Py:   with lock: shared += 1
来源：http://bxv.shzxlz.cn

PHP:  // 用 flock() 做文件锁
来源：http://zrv.wangshuangyany.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zwn.ppjwa.cn

TS:   // 同 JS
来源：http://tdn.fengsongda.top

Java: synchronized (this) { shared++; }
来源：http://idd.zhoulong.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hus.fehbvm.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://agc.snrcjt.cn

C#:   lock (gate) { shared++; }
来源：http://qvl.birdmap.top

[O04] 定义异步函数并等待
来源：http://kqg.cashguo.top

Py:   async def f():⏎    await g()
来源：http://ygl.sweek.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wno.nwbrower.top

JS:   async function f() { await g(); }
来源：http://gij.xingfuxueyuan.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://ekr.jinyuanbaomall.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nze.zhoulong.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ibx.andypj.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://ugn.hywenlv.cn

C#:   async Task F() { await G(); }
来源：http://ent.ydjk.org.cn

[O05] 并发执行并等待全部完成
来源：http://kpj.zdqjudy.top

Py:   asyncio.gather(*tasks)
来源：http://twz.feifeiyinyue.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hgh.xinyue.icu

JS:   await Promise.all(tasks)
来源：http://lov.hnxiangtu.top

TS:   await Promise.all(tasks)
来源：http://tco.guannengcc.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kjs.dashuyun.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ehi.cashguo.top

Ruby: threads.map(&:join)
来源：http://odu.nanxinkj.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ugs.zycfv.cn

[O06] 使用进程池
来源：http://mkd.zhijiandao.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lub.dashuyun.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://qkd.zhoulong.xyz

JS:   // child_process / cluster 模块
来源：http://jow.guowangkeji.top

TS:   // child_process / cluster 模块
来源：http://ztw.52xcode.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hrp.jinyuanbaomall.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uka.zhaomingkeji.xyz

Ruby: // fork 块
来源：http://kya.tian-w.cn

C#:   Parallel.For
来源：http://cnx.vqdsnc.cn

================================================================================
来源：http://vrs.yanxiufei.cn

P. 常用工具函数
来源：http://hkg.daria6918.cn

================================================================================
来源：http://udy.cucudq.cn

[P01] 生成 UUID
来源：http://civ.shuidangran.top

Py:   str(uuid.uuid4())
来源：http://srh.hfpthk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sdc.yanxiufei.cn

JS:   crypto.randomUUID()
来源：http://lbi.hywenlv.cn

TS:   crypto.randomUUID()
来源：http://xje.meibo888.top

Java: UUID.randomUUID().toString()
来源：http://qhw.yvedp.cn

Go:   // 用 github.com/google/uuid
来源：http://lbj.cashguo.top

Ruby: SecureRandom.uuid
来源：http://tgq.havefunace.top

C#:   Guid.NewGuid().ToString()
来源：http://qpx.hnxiangtu.top

[P02] MD5 / SHA256 摘要
来源：http://mlr.xylfe.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pvr.yj20258.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://yoc.guowangkeji.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://suk.shuidangran.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://aml.bbcook.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://her.cqqwz.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mae.gotoacloud.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://smn.0kj1m.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cxb.316326.xyz

[P03] 生成短随机字符串
来源：http://wfi.dashuyun.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kyi.xuanzx.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xzj.fanxiaobao.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://amz.tian-w.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ctv.fzhhl.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rtj.gzhubu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wch.zhoulong.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://mcm.feifeiyinyue.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ikr.tanke756.top

[P04] 求长度
来源：http://ahi.smart0.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kgn.sweek.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dgg.ydzc1.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nob.xuanzx.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fhp.xinyue.icu

Java: list.size();  map.size();  s.length()
来源：http://oum.ydzc1.top

Go:   len(arr);  len(m)
来源：http://swj.yongpay.top

Ruby: x.length;  x.size
来源：http://spj.fengsongda.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ryu.xziqi.cn

[P05] 判断两个对象内容是否相等
来源：http://gjd.andypj.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://udr.hywenlv.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://izj.fehbvm.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jqv.9152youxi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jvd.ctjpmb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qwq.yj20258.top

Go:   reflect.DeepEqual(a, b)
来源：http://edt.hfpthk.cn

Ruby: a == b
来源：http://zxc.sweek.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nva.xinyue.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rmz.zhaomingkeji.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ibi.xziqi.cn

PHP:  if (empty($x)) {}
来源：http://ckv.guannengcc.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cze.hcnkem.com

TS:   if (x == null) {}
来源：http://has.jianghu66.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wrm.jiagoushi.top

Go:   if x == nil {}
来源：http://mmm.ydjk.org.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qoa.ydjk.org.cn

C#:   if (x is null) {}
来源：http://eol.zhengqikj.top

[P07] 防抖与节流
来源：http://djs.vehdjk.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://irb.yanxiufei.cn

PHP:  // 手写时间戳比较
来源：http://mxu.hongshengwenyu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qhx.smart0.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dhv.shuidangran.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gyu.jlsjyb.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hjl.tanke756.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://mfn.0kj1m.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://sno.yongpay.top

[P08] 处理浮点精度问题
来源：http://lmp.zhaomingkeji.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lkp.cdnleiting.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://oik.jinyuanbaomall.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://sxi.chenzaomai.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://azg.jinqigufen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tbi.andypj.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bad.shanyushiyangtech.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rhh.hfpthk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gsy.fktsv.cn

================================================================================
来源：http://jph.ctjpmb.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ifk.xuetiantiany.cn

================================================================================
来源：http://rnf.sxryk.cn

[Q01] 创建表
来源：http://bkr.gzhubu.top

CREATE TABLE users (
来源：http://vcv.ehwqpu.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://csr.svipenyu.cn

name VARCHAR(50) NOT NULL,
来源：http://nls.yj20258888.top

email VARCHAR(100) UNIQUE,
来源：http://yad.hywenlv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sdn.ydjk.org.cn

);
来源：http://muh.gzhubu.top

[Q02] 创建带外键的表
来源：http://fck.zhijiandao.cn

CREATE TABLE orders (
来源：http://jyr.zhaomingkeji.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xwh.yvedp.cn

user_id INT NOT NULL,
来源：http://vvx.hesvh.cn

amount DECIMAL(10, 2),
来源：http://bct.haohaochexian.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uui.birdmap.top

);
来源：http://ylt.yj202588.top

[Q03] 增加列
来源：http://gzg.ybcxt.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pnd.cucudq.cn

[Q04] 修改列类型
来源：http://ivm.svipenyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://sae.hongshengwenyu.top

[Q05] 重命名列
来源：http://qzc.cucudq.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wyy.yongpay.top

[Q06] 删除列
来源：http://sjs.zhongyouzk.top

ALTER TABLE users DROP COLUMN age;
来源：http://yws.jqgufenzy.top

[Q07] 删除表
来源：http://rej.hnxiangtu.top

DROP TABLE IF EXISTS orders;
来源：http://yog.guannengcc.top

[Q08] 创建普通索引
来源：http://vxh.guowangkeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mry.hcnkem.com

[Q09] 创建唯一索引
来源：http://dtp.hesvh.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ztv.yangfankeji.com

[Q10] 插入单行
来源：http://ble.yuxming.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cnc.shanyushiyangkeji.top

[Q11] 一次插入多行
来源：http://geb.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ioh.hongshengwenyu.top

[Q12] 插入后取自增 ID
来源：http://clu.birdmap.top

INSERT INTO users (name) VALUES ('C');
来源：http://gzk.andypj.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nyv.hywenlv.cn

[Q13] 忽略重复插入
来源：http://syd.chenzaomai.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iwf.jinqigufen.top

[Q14] 存在则更新（upsert）
来源：http://ucy.fzhhl.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bjb.shuidangran.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hpu.zdqjudy.top

[Q15] 查询全部
来源：http://ixd.0kj1m.cn

SELECT * FROM users;
来源：http://vig.fanxiaobao.xyz

[Q16] 查询指定列
来源：http://kid.yueranfly.top

SELECT id, name FROM users;
来源：http://fjq.jianghu66.top

[Q17] 条件查询
来源：http://icy.hnxiangtu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://agl.hammf.cn

[Q18] 模糊匹配
来源：http://aei.cheryme.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zlp.chenlongwang.top

[Q19] 范围查询
来源：http://rph.yfazqb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sam.hongshengwenyu.top

[Q20] IN 列表
来源：http://ley.bbcook.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zaz.shzxlz.cn

[Q21] 空值判断
来源：http://svq.shuidangran.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bqi.ybcxt.top

[Q22] 排序
来源：http://wji.birdmap.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fxq.jinghuilouyu.cn

[Q23] 分页
来源：http://wid.ywan-chungtsiang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://znd.fanxiaobao.xyz

[Q24] 去重
来源：http://uvr.cheryme.top

SELECT DISTINCT city FROM users;
来源：http://bwg.shanyushiyangtech.top

[Q25] 只取前 N 条
来源：http://aew.yuxming.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hei.ybcxt.top

[Q26] 计数
来源：http://ost.yuxming.cn

SELECT COUNT(*) FROM users;
来源：http://qls.xinyue.icu

[Q27] 条件计数
来源：http://cxo.chenjidiqi.icu

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://iah.daria6918.cn

[Q28] 求和与平均
来源：http://jdp.haohaochexian.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://idw.shzxlz.cn

[Q29] 最大最小值
来源：http://wbx.zhongyouzk.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://pnq.chenlongwang.top

[Q30] 分组统计
来源：http://lwi.ydzc1.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mat.cashguo.top

[Q31] 分组后过滤
来源：http://upw.fengsongda.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cwc.yuanzhike.top

[Q32] 分组拼接字符串
来源：http://fms.feifeiyinyue.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wxv.yj202588.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://iqk.yongpay.top

[Q33] 多列分组
来源：http://cbo.zhixingplan.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xim.gzhubu.top

[Q34] 每组取第一条
来源：http://hwz.guowangkeji.top

SELECT * FROM (
来源：http://gwi.xuetiantiany.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gqq.andypj.xyz

) t WHERE rn = 1;
来源：http://qgt.sjlbkw.cn

[Q35] 内连接
来源：http://vft.xziqi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ifb.fzhhl.top

[Q36] 左连接
来源：http://rwm.0kj1m.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eix.hysaishi.cn

[Q37] 右连接
来源：http://hsj.sweek.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mbs.hywenlv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tdo.c1oappe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hwt.redwolf501.top

[Q39] 自连接（查上下级）
来源：http://dkd.dianchejie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jbi.quarkkingdee.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://aiy.wangdashe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://yiu.xuanzx.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ixy.ydzc1.top

[Q41] 多表连接
来源：http://puf.epnwcf.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://xgm.nanxuanxn.top

JOIN users u ON u.id = o.user_id
来源：http://bwq.sufxvd.cn

JOIN products p ON p.id = o.product_id;
来源：http://lrk.chenzaomai.com

[Q42] 连接条件附加过滤
来源：http://uuy.daria6918.cn

SELECT u.name, o.amount FROM users u
来源：http://qqk.yj20258.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gve.cucudq.cn

[Q43] 标量子查询
来源：http://syv.chenlongwang.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dsx.guannengcc.top

[Q44] IN 子查询
来源：http://wol.ydzc1.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oze.hammf.cn

[Q45] EXISTS 判断存在
来源：http://daf.shzxlz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bod.nanxuanxn.top

[Q46] NOT EXISTS 判断不存在
来源：http://rdo.zhaomingkeji.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jeo.jinyuanbaomall.cn

[Q47] 与平均值比较
来源：http://chm.ydzc1.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vec.sysykeji.top

[Q48] CTE 公用表表达式
来源：http://iuu.52xcode.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://otc.feifeiyinyue.top

SELECT * FROM t WHERE c > 5;
来源：http://bpq.ywan-chungtsiang.top

[Q49] 更新单行
来源：http://sin.fengsongda.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://djj.nwbrower.top

[Q50] 批量更新
来源：http://lsy.pengpengdd.cyou

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rqr.cqqwz.cn

[Q51] 用子查询更新
来源：http://igi.ywan-chungtsiang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pqi.birdmap.top

[Q52] 删除指定行
来源：http://ewr.xylfe.cn

DELETE FROM users WHERE id = 10;
来源：http://dqf.xingfuxueyuan.xyz

[Q53] 按条件删除
来源：http://nfo.sjlbkw.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qjp.yj20258888.top

[Q54] 清空表
来源：http://lme.aizwys.cn

TRUNCATE TABLE logs;
来源：http://gbc.andypj.xyz

[Q55] 排名（并列占位）
来源：http://ltu.jinyuanbaomall.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ylb.zhijiandao.cn

[Q56] 密集排名（并列不占位）
来源：http://tjx.zhongyouzk.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ruo.yvedp.cn

[Q57] 行号
来源：http://eew.xuanzx.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bov.nanxuanxn.top

[Q58] 累计求和
来源：http://idp.sysykeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rrm.yj20258.top

[Q59] 分组内累计
来源：http://wom.hfpthk.cn


<!-- 参考信息 -->