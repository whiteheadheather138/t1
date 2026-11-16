代发 wailian999

[N09] 栈与队列
来源：http://joa.jinqigufen.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ppb.cheryme.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://ccd.cheryme.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://dew.chenzaomai.com

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wdr.cucudq.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ysl.yanxiufei.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://koi.yanxiufei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mhp.gogol.net.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://tmw.vqdsnc.cn

[N10] 链表节点定义
来源：http://pti.xinyue.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://etk.cdnleiting.top

PHP:  class Node { public $v; public $next = null; }
来源：http://djv.cucudq.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://idk.guannengcc.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://qnq.hnxiangtu.top

Java: class Node { int v; Node next; }
来源：http://djh.quarkkingdee.top

Go:   type Node struct { V int; Next *Node }
来源：http://jzf.fengsongda.top

Ruby: Node = Struct.new(:v, :next)
来源：http://ses.dashuyun.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://xoe.ctjpmb.com

[N11] 二叉树中序遍历
来源：http://djr.daxiang520.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yib.316326.xyz

PHP:  // 手写递归函数
来源：http://nlk.hcnkem.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://lwa.xziqi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://kdx.feifeiyinyue.top

Java: // 手写递归
来源：http://xqi.zhixingplan.top

Go:   // 手写递归
来源：http://xpl.dianchejie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vhf.kuanghao11.cn

C#:   // 手写递归
来源：http://pym.redwolf501.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://vdh.tarul.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://gjk.wangdashe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://vat.zhaomingkeji.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://voz.jinghuilouyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://goe.yuxming.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bue.wangdashe.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://frt.nanxinkj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jfx.cashguo.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mgf.sxryk.cn

================================================================================
来源：http://fqk.shuidangran.top

O. 并发与异步
来源：http://iku.iojbl.cn

================================================================================
来源：http://vld.fengsongda.top

[O01] 启动一个线程
来源：http://ubk.sjlbkw.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zkm.fanxiaobao.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://apr.vehdjk.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qpt.9152youxi.cn

TS:   // 同 JS
来源：http://exz.jyoumei.cn

Java: new Thread(() -> f()).start()
来源：http://yaa.fzhhl.top

Go:   go f()
来源：http://qho.sxryk.cn

Ruby: Thread.new { f }
来源：http://oyf.hammf.cn

C#:   Task.Run(() => F());
来源：http://azn.cucudq.cn

[O02] 使用线程池
来源：http://exy.ppjwa.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ikz.hesvh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nfw.fzhhl.top

JS:   // worker_threads 线程池
来源：http://cff.meibo888.top

TS:   // worker_threads 线程池
来源：http://jhe.zhaomingkeji.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://seh.yj202588.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://pec.iojbl.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ssp.smart0.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xbe.yj202588.top

[O03] 加锁保护共享数据
来源：http://brw.shzxlz.cn

Py:   with lock: shared += 1
来源：http://plu.0kj1m.cn

PHP:  // 用 flock() 做文件锁
来源：http://clf.kuanghao11.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dds.hnxiangtu.top

TS:   // 同 JS
来源：http://trz.snrcjt.cn

Java: synchronized (this) { shared++; }
来源：http://fqf.zycfv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://eyv.yongpay.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://yzg.zhixingplan.top

C#:   lock (gate) { shared++; }
来源：http://ouv.feifeiyinyue.top

[O04] 定义异步函数并等待
来源：http://syy.xuanzx.com

Py:   async def f():⏎    await g()
来源：http://czv.yuxming.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kzo.chenlongwang.top

JS:   async function f() { await g(); }
来源：http://etq.yonumen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://htr.hcnkem.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://drx.52xcode.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xro.hysaishi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kya.epnwcf.com

C#:   async Task F() { await G(); }
来源：http://tvq.guannengcc.top

[O05] 并发执行并等待全部完成
来源：http://wmm.redwolf501.top

Py:   asyncio.gather(*tasks)
来源：http://ntb.iojbl.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gxm.hywenlv.cn

JS:   await Promise.all(tasks)
来源：http://pvx.hongshengwenyu.top

TS:   await Promise.all(tasks)
来源：http://ofb.sweek.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://cnu.mhx1999.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://acq.ydjk.org.cn

Ruby: threads.map(&:join)
来源：http://vea.aizwys.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hfk.sjlbkw.cn

[O06] 使用进程池
来源：http://knk.zdqjudy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wyp.sweek.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ltd.zdqjudy.top

JS:   // child_process / cluster 模块
来源：http://hmy.zhengqikj.top

TS:   // child_process / cluster 模块
来源：http://lor.kuanghao11.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gyt.shanyushiyangtech.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dsu.jlsjyb.cn

Ruby: // fork 块
来源：http://lor.pycfn.com

C#:   Parallel.For
来源：http://nit.hnxiangtu.top

================================================================================
来源：http://gqa.xinyue.icu

P. 常用工具函数
来源：http://nxy.sweek.top

================================================================================
来源：http://keh.shuidangran.top

[P01] 生成 UUID
来源：http://qqn.gogol.net.cn

Py:   str(uuid.uuid4())
来源：http://mmj.dianchejie.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://itn.chenjidiqi.icu

JS:   crypto.randomUUID()
来源：http://dam.xinyue.icu

TS:   crypto.randomUUID()
来源：http://rno.cashguo.top

Java: UUID.randomUUID().toString()
来源：http://oef.feifeiyinyue.top

Go:   // 用 github.com/google/uuid
来源：http://xzk.dashuyun.cn

Ruby: SecureRandom.uuid
来源：http://lhr.vehdjk.com

C#:   Guid.NewGuid().ToString()
来源：http://orw.ydjk.org.cn

[P02] MD5 / SHA256 摘要
来源：http://nng.dianchejie.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://elp.snrcjt.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://njv.quarkkingdee.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://cgu.zycfv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kjw.jlsjyb.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ywx.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://swu.sufxvd.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qns.tianlin.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bww.jqgfzy.top

[P03] 生成短随机字符串
来源：http://bnr.cdnleiting.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zyk.yangfankeji.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ypo.yueranfly.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zoz.yonumen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jpb.gogol.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vfx.gzhubu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tip.feifeiyinyue.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vbd.jqgfzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jwv.cqqwz.cn

[P04] 求长度
来源：http://oos.cdnleiting.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nxz.dashuyun.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nmn.hfpthk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qgy.feifeiyinyue.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://svo.cqqwz.cn

Java: list.size();  map.size();  s.length()
来源：http://lxc.zdqjudy.top

Go:   len(arr);  len(m)
来源：http://aol.mhx1999.top

Ruby: x.length;  x.size
来源：http://lws.birdmap.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dnj.jiagoushi.top

[P05] 判断两个对象内容是否相等
来源：http://yxb.cucudq.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://utr.bbcook.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://urz.wangdashe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tid.xuetiantiany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://qie.yangfankeji.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ovt.guowangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://bal.jiagoushi.top

Ruby: a == b
来源：http://zvt.sjlbkw.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ofl.epnwcf.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gqc.snrcjt.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://plv.yfazqb.com

PHP:  if (empty($x)) {}
来源：http://uaj.daxiang520.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hrz.ctjpmb.com

TS:   if (x == null) {}
来源：http://dis.haohaochexian.top

Java: if (x == null || x.isEmpty()) {}
来源：http://gqq.smart0.xyz

Go:   if x == nil {}
来源：http://nqh.gaohongyu789.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mgt.hysaishi.cn

C#:   if (x is null) {}
来源：http://hrw.wangshuangyany.cn

[P07] 防抖与节流
来源：http://nbj.tianlin.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qld.fengsongda.top

PHP:  // 手写时间戳比较
来源：http://uow.yvedp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jcy.zhongyouzk.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yvx.xylfe.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gaw.nwbrower.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ghf.jinyuanbaomall.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vur.zhaomingkeji.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dee.ehwqpu.com

[P08] 处理浮点精度问题
来源：http://fzi.ydzc1.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ckl.hnxiangtu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://csd.zycfv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://dtg.yvedp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kva.fengsongda.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wxv.aibaodan.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jkd.hesvh.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gnd.jinqigfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://trb.feifeiyinyue.top

================================================================================
来源：http://izj.ywan-chungtsiang.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://djf.bbcook.cn

================================================================================
来源：http://ztj.tanke756.top

[Q01] 创建表
来源：http://tqg.hywenlv.cn

CREATE TABLE users (
来源：http://kxq.jianghu66.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cvf.tanke756.top

name VARCHAR(50) NOT NULL,
来源：http://eee.jinqigufen.top

email VARCHAR(100) UNIQUE,
来源：http://xkt.vqdsnc.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://shz.tanke756.top

);
来源：http://fls.yuanzhike.top

[Q02] 创建带外键的表
来源：http://mmc.uphjek.com

CREATE TABLE orders (
来源：http://udt.zdbjq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wza.nanxuanxn.top

user_id INT NOT NULL,
来源：http://cii.xziqi.cn

amount DECIMAL(10, 2),
来源：http://lhf.xinyue.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gec.sysykeji.top

);
来源：http://chj.sufxvd.cn

[Q03] 增加列
来源：http://oth.vqdsnc.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xpw.jinqigfzy.top

[Q04] 修改列类型
来源：http://iml.yfazqb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iis.zycfv.cn

[Q05] 重命名列
来源：http://hha.shanyushiyangtech.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zmj.nanxuanxn.top

[Q06] 删除列
来源：http://oll.pycfn.com

ALTER TABLE users DROP COLUMN age;
来源：http://tqk.vehdjk.com

[Q07] 删除表
来源：http://pru.iojbl.cn

DROP TABLE IF EXISTS orders;
来源：http://naq.ywan-chungtsiang.top

[Q08] 创建普通索引
来源：http://tku.shanyushiyangtech.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ybx.epnwcf.com

[Q09] 创建唯一索引
来源：http://qrx.redwolf501.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qio.cqqwz.cn

[Q10] 插入单行
来源：http://bse.fengsongda.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oww.shangyingyoupin.top

[Q11] 一次插入多行
来源：http://wkf.gzhubu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://evb.sxryk.cn

[Q12] 插入后取自增 ID
来源：http://uny.uphjek.com

INSERT INTO users (name) VALUES ('C');
来源：http://ono.dashuyun.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dye.pengpengdd.cyou

[Q13] 忽略重复插入
来源：http://nhz.redwolf501.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://grg.fanxiaobao.xyz

[Q14] 存在则更新（upsert）
来源：http://ioi.ctjpmb.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lil.xuanzx.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://izg.zdbjq.cn

[Q15] 查询全部
来源：http://dat.svipenyu.cn

SELECT * FROM users;
来源：http://mhk.chenjidiqi.icu

[Q16] 查询指定列
来源：http://eza.fzhhl.top

SELECT id, name FROM users;
来源：http://lax.yanxiufei.cn

[Q17] 条件查询
来源：http://rdz.xylfe.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tmi.havefunace.top

[Q18] 模糊匹配
来源：http://tlv.yangfankeji.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sxd.shanyushiyangkeji.top

[Q19] 范围查询
来源：http://okf.xziqi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vvp.epnwcf.com

[Q20] IN 列表
来源：http://ylq.zhiwuduotai.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vgy.gaohongyu789.top

[Q21] 空值判断
来源：http://orh.nanxuanxn.top

SELECT * FROM users WHERE email IS NULL;
来源：http://wky.svipenyu.cn

[Q22] 排序
来源：http://cml.fzhhl.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ymz.hesvh.cn

[Q23] 分页
来源：http://urj.fktsv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ytp.316326.xyz

[Q24] 去重
来源：http://zuo.fktsv.cn

SELECT DISTINCT city FROM users;
来源：http://srs.chenzaomai.com

[Q25] 只取前 N 条
来源：http://aet.redwolf501.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gcs.guowangkeji.top

[Q26] 计数
来源：http://jnd.dashuyun.cn

SELECT COUNT(*) FROM users;
来源：http://tmh.nanxinkj.top

[Q27] 条件计数
来源：http://ehu.iojbl.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hfe.9152youxi.cn

[Q28] 求和与平均
来源：http://wfo.daria6918.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mfh.xuetiantiany.cn

[Q29] 最大最小值
来源：http://utf.yueranfly.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xej.vehdjk.com

[Q30] 分组统计
来源：http://nez.vqdsnc.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mcx.hcnkem.com

[Q31] 分组后过滤
来源：http://who.haohaochexian.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kjm.ehwqpu.com

[Q32] 分组拼接字符串
来源：http://vir.sysykeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yyt.yfazqb.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ess.yj202588.top

[Q33] 多列分组
来源：http://elk.cheryme.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cvj.tianlin.xyz

[Q34] 每组取第一条
来源：http://tik.jqgfzy.top

SELECT * FROM (
来源：http://jzc.aizwys.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vna.hongshengwenyu.top

) t WHERE rn = 1;
来源：http://rru.hnxiangtu.top

[Q35] 内连接
来源：http://err.yanxiufei.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dul.jlsjyb.cn

[Q36] 左连接
来源：http://vhj.zhiwuduotai.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zrn.jinyuanbaomall.cn

[Q37] 右连接
来源：http://sgn.ydzc1.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hla.fengsongda.top

[Q38] 全外连接（PostgreSQL）
来源：http://lvq.havefunace.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://non.wangshuangyany.cn

[Q39] 自连接（查上下级）
来源：http://hxl.daria6918.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yhb.fzhhl.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kgw.cheryme.top

[Q40] 交叉连接（笛卡尔积）
来源：http://loa.jiagoushi.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fwg.shuidangran.top

[Q41] 多表连接
来源：http://bkh.yangfankeji.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://wbt.hfpthk.cn

JOIN users u ON u.id = o.user_id
来源：http://erv.smart0.xyz

JOIN products p ON p.id = o.product_id;
来源：http://yew.cdnleiting.top

[Q42] 连接条件附加过滤
来源：http://bnw.yueranfly.top

SELECT u.name, o.amount FROM users u
来源：http://gvt.bjfxy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gqz.shanyushiyangtech.top

[Q43] 标量子查询
来源：http://ogk.birdmap.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nfp.zycfv.cn

[Q44] IN 子查询
来源：http://lsy.gotoacloud.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://auv.svipenyu.cn

[Q45] EXISTS 判断存在
来源：http://ppl.wangshuangyany.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mxf.tanke756.top

[Q46] NOT EXISTS 判断不存在
来源：http://owd.yuanzhike.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ipa.ctjpmb.com

[Q47] 与平均值比较
来源：http://cqo.shuidangran.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bwc.yj202588.top

[Q48] CTE 公用表表达式
来源：http://fme.fengsongda.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uxh.yanxiufei.cn

SELECT * FROM t WHERE c > 5;
来源：http://dzc.yongpay.top

[Q49] 更新单行
来源：http://ogw.aibaodan.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tia.zhiwuduotai.top

[Q50] 批量更新
来源：http://bmm.hnqzz.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gcf.daria6918.cn

[Q51] 用子查询更新
来源：http://urr.cucudq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ufb.cheryme.top

[Q52] 删除指定行
来源：http://abp.birdmap.top

DELETE FROM users WHERE id = 10;
来源：http://wsh.bjfxy.top

[Q53] 按条件删除
来源：http://zef.gaohongyu789.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://olq.aizwys.cn

[Q54] 清空表
来源：http://qaj.hfpthk.cn

TRUNCATE TABLE logs;
来源：http://ixx.feifeiyinyue.top

[Q55] 排名（并列占位）
来源：http://asz.xuetiantiany.cn


<!-- 参考信息 -->