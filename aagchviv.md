代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://klw.yj20258.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://vxe.guowangkeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://lut.nwbrower.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://brt.yuanzhike.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://eze.birdmap.top

[N10] 链表节点定义
来源：http://jpc.hnxiangtu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ucv.guannengcc.top

PHP:  class Node { public $v; public $next = null; }
来源：http://uvr.redwolf501.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gtu.xinyue.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://zea.cdnleiting.top

Java: class Node { int v; Node next; }
来源：http://qbp.yvedp.cn

Go:   type Node struct { V int; Next *Node }
来源：http://qbl.fehbvm.com

Ruby: Node = Struct.new(:v, :next)
来源：http://cqw.yfazqb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://ryj.fktsv.cn

[N11] 二叉树中序遍历
来源：http://prx.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://aaz.smart0.xyz

PHP:  // 手写递归函数
来源：http://shf.aibaodan.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://axf.zhongyouzk.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://klj.gogol.net.cn

Java: // 手写递归
来源：http://eib.yanxiufei.cn

Go:   // 手写递归
来源：http://oie.jqgfzy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://aio.jinyuanbaomall.cn

C#:   // 手写递归
来源：http://njz.svipenyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://cnh.jqgfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jjp.ehwqpu.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://tvz.9152youxi.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://poj.hfpthk.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fqs.shzxlz.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lax.ctjpmb.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://fqg.jinqigfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zop.shanyushiyangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ebr.zdbjq.cn

================================================================================
来源：http://gpl.jinyuanbaomall.cn

O. 并发与异步
来源：http://osi.yj20258888.top

================================================================================
来源：http://opr.epnwcf.com

[O01] 启动一个线程
来源：http://xai.zdbjq.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gvz.c1oappe.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://yrt.meibo888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tqs.yvedp.cn

TS:   // 同 JS
来源：http://gzh.hnxiangtu.top

Java: new Thread(() -> f()).start()
来源：http://can.ehwqpu.com

Go:   go f()
来源：http://kxy.zycfv.cn

Ruby: Thread.new { f }
来源：http://wpq.yj202588.top

C#:   Task.Run(() => F());
来源：http://mit.snrcjt.cn

[O02] 使用线程池
来源：http://gog.tianlin.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gax.ydzc1.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://zin.ivvv.top

JS:   // worker_threads 线程池
来源：http://zvk.wangdashe.top

TS:   // worker_threads 线程池
来源：http://jbx.hcnkem.com

Java: Executors.newFixedThreadPool(4)
来源：http://aqk.xinyue.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nrj.sjlbkw.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uvg.shangyingyoupin.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kzf.jqgufenzy.top

[O03] 加锁保护共享数据
来源：http://apf.yangfankeji.com

Py:   with lock: shared += 1
来源：http://hhc.kuanghao11.cn

PHP:  // 用 flock() 做文件锁
来源：http://jrv.ctjpmb.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rsn.yonumen.top

TS:   // 同 JS
来源：http://pse.svipenyu.cn

Java: synchronized (this) { shared++; }
来源：http://eam.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sfj.epnwcf.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://cox.nanxinkj.top

C#:   lock (gate) { shared++; }
来源：http://tzm.yuanzhike.top

[O04] 定义异步函数并等待
来源：http://upe.yvedp.cn

Py:   async def f():⏎    await g()
来源：http://xbq.ehwqpu.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hjb.cheryme.top

JS:   async function f() { await g(); }
来源：http://txp.andypj.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://owh.xingfuxueyuan.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sln.ppjwa.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jqx.jianghu66.top

Ruby: # 用 Fiber 或 async gem
来源：http://yjy.xinyue.icu

C#:   async Task F() { await G(); }
来源：http://ioe.zdbjq.cn

[O05] 并发执行并等待全部完成
来源：http://ygz.fengsongda.top

Py:   asyncio.gather(*tasks)
来源：http://grr.xziqi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dcu.cucudq.cn

JS:   await Promise.all(tasks)
来源：http://cus.fktsv.cn

TS:   await Promise.all(tasks)
来源：http://brn.316326.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fog.yuanzhike.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yxk.tian-w.cn

Ruby: threads.map(&:join)
来源：http://gwl.dashuyun.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://oou.bjfxy.top

[O06] 使用进程池
来源：http://bzy.ehwqpu.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hnj.nanxinkj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://pey.jqgufenzy.top

JS:   // child_process / cluster 模块
来源：http://xya.bbcook.cn

TS:   // child_process / cluster 模块
来源：http://yaq.fanxiaobao.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ovn.ydjk.org.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xue.zhoulong.xyz

Ruby: // fork 块
来源：http://ipc.c1oappe.top

C#:   Parallel.For
来源：http://apw.fzhhl.top

================================================================================
来源：http://mwz.zhoulong.xyz

P. 常用工具函数
来源：http://utc.sufxvd.cn

================================================================================
来源：http://crk.quarkkingdee.top

[P01] 生成 UUID
来源：http://ugs.hysaishi.cn

Py:   str(uuid.uuid4())
来源：http://xtf.cheryme.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rjk.xingfuxueyuan.xyz

JS:   crypto.randomUUID()
来源：http://jgc.svipenyu.cn

TS:   crypto.randomUUID()
来源：http://ekd.hesvh.cn

Java: UUID.randomUUID().toString()
来源：http://oqo.xingfuxueyuan.xyz

Go:   // 用 github.com/google/uuid
来源：http://zqe.xingfuxueyuan.xyz

Ruby: SecureRandom.uuid
来源：http://zhs.jianghu66.top

C#:   Guid.NewGuid().ToString()
来源：http://cvo.ydjk.org.cn

[P02] MD5 / SHA256 摘要
来源：http://aid.ppjwa.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://svb.hnxiangtu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://pwy.tian-w.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jbm.chenlongwang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zkk.fengsongda.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xmv.fehbvm.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://gis.pengpengdd.cyou

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ogl.ivvv.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ahp.cheryme.top

[P03] 生成短随机字符串
来源：http://akq.fehbvm.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qiq.cqqwz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dtb.cqqwz.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dtb.jiagoushi.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gvh.jinyuanbaomall.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://quj.cdnleiting.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yqn.zhiwuduotai.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zhf.zhaomingkeji.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ncw.sysykeji.top

[P04] 求长度
来源：http://zeo.kuanghao11.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hsr.yanxiufei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xnz.bjfxy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ndm.xingfuxueyuan.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tya.sufxvd.cn

Java: list.size();  map.size();  s.length()
来源：http://rbr.yanxiufei.cn

Go:   len(arr);  len(m)
来源：http://rmi.yj20258.top

Ruby: x.length;  x.size
来源：http://zdr.yfazqb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://wii.meibo888.top

[P05] 判断两个对象内容是否相等
来源：http://fuo.shzxlz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://szd.aizwys.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wxm.vehdjk.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bki.zhijiandao.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://crf.9152youxi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fzj.daxiang520.top

Go:   reflect.DeepEqual(a, b)
来源：http://nhj.uphjek.com

Ruby: a == b
来源：http://xnc.zhijiandao.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://syd.yvedp.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sqt.guowangkeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zez.fzhhl.top

PHP:  if (empty($x)) {}
来源：http://pgl.fktsv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uxb.yangfankeji.com

TS:   if (x == null) {}
来源：http://wgy.zhijiandao.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://svx.yanxiufei.cn

Go:   if x == nil {}
来源：http://xad.c1oappe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hrd.chenzaomai.com

C#:   if (x is null) {}
来源：http://sfu.hywenlv.cn

[P07] 防抖与节流
来源：http://dym.meibo888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rlj.hesvh.cn

PHP:  // 手写时间戳比较
来源：http://xch.nanxinkj.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://igk.gzhubu.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bai.zdbjq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://owt.ctjpmb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://poe.zhoulong.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://krv.epnwcf.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vxe.tianlin.xyz

[P08] 处理浮点精度问题
来源：http://csa.redwolf501.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vhv.zycfv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wem.yueranfly.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qqg.jinqigufen.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hov.xuetiantiany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rqy.gaohongyu789.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kav.daria6918.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nbz.xuanzx.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nyp.jiagoushi.top

================================================================================
来源：http://mji.9152youxi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zqk.yfazqb.com

================================================================================
来源：http://slq.zhiwuduotai.top

[Q01] 创建表
来源：http://ikm.fanxiaobao.xyz

CREATE TABLE users (
来源：http://ala.kuanghao11.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ovg.zhijiandao.cn

name VARCHAR(50) NOT NULL,
来源：http://nfn.hammf.cn

email VARCHAR(100) UNIQUE,
来源：http://hjo.zhongyouzk.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fmb.yfazqb.com

);
来源：http://zfh.zhengqikj.top

[Q02] 创建带外键的表
来源：http://jjd.shzxlz.cn

CREATE TABLE orders (
来源：http://cgi.hysaishi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ybc.tian-w.cn

user_id INT NOT NULL,
来源：http://wwh.havefunace.top

amount DECIMAL(10, 2),
来源：http://euq.dashuyun.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xcs.zhaomingkeji.xyz

);
来源：http://qoe.9152youxi.cn

[Q03] 增加列
来源：http://tjd.yfazqb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://arj.daxiang520.top

[Q04] 修改列类型
来源：http://edy.fktsv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ezb.jqgufenzy.top

[Q05] 重命名列
来源：http://mvt.nanxinkj.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ios.svipenyu.cn

[Q06] 删除列
来源：http://joy.jqgfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://lhc.jinqigfzy.top

[Q07] 删除表
来源：http://xvc.andypj.xyz

DROP TABLE IF EXISTS orders;
来源：http://vkz.ctjpmb.com

[Q08] 创建普通索引
来源：http://wye.fehbvm.com

CREATE INDEX idx_users_email ON users(email);
来源：http://rka.yj202588.top

[Q09] 创建唯一索引
来源：http://gww.sjlbkw.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ndm.quarkkingdee.top

[Q10] 插入单行
来源：http://tfo.snrcjt.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fcu.tian-w.cn

[Q11] 一次插入多行
来源：http://lqb.gogol.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qdr.svipenyu.cn

[Q12] 插入后取自增 ID
来源：http://mlc.dianchejie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://uiy.fehbvm.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jfe.jinyuanbaomall.cn

[Q13] 忽略重复插入
来源：http://sag.zhixingplan.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dzx.chenjidiqi.icu

[Q14] 存在则更新（upsert）
来源：http://pgp.dashuyun.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://apu.nanxinkj.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://och.9152youxi.cn

[Q15] 查询全部
来源：http://fti.hywenlv.cn

SELECT * FROM users;
来源：http://gxe.cqqwz.cn

[Q16] 查询指定列
来源：http://hmx.yfazqb.com

SELECT id, name FROM users;
来源：http://sdk.yueranfly.top

[Q17] 条件查询
来源：http://jsl.xylfe.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mtu.hnqzz.top

[Q18] 模糊匹配
来源：http://tju.cqqwz.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rkq.hcnkem.com

[Q19] 范围查询
来源：http://stn.uphjek.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mcl.zhengqikj.top

[Q20] IN 列表
来源：http://oxn.tanke756.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gzq.chenlongwang.top

[Q21] 空值判断
来源：http://dsc.feifeiyinyue.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ofl.snrcjt.cn

[Q22] 排序
来源：http://qdy.tian-w.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yfj.cashguo.top

[Q23] 分页
来源：http://ygt.pycfn.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://idm.guannengcc.top

[Q24] 去重
来源：http://zir.jyoumei.cn

SELECT DISTINCT city FROM users;
来源：http://mvv.ivvv.top

[Q25] 只取前 N 条
来源：http://agb.zhengqikj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://klg.yueranfly.top

[Q26] 计数
来源：http://uod.yj202588.top

SELECT COUNT(*) FROM users;
来源：http://gru.wangshuangyany.cn

[Q27] 条件计数
来源：http://ess.pycfn.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://krx.cashguo.top

[Q28] 求和与平均
来源：http://qjh.zhoulong.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uae.jqgfzy.top

[Q29] 最大最小值
来源：http://eha.cqqwz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cut.xuanzx.com

[Q30] 分组统计
来源：http://vvd.xuetiantiany.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pdo.jinqigfzy.top

[Q31] 分组后过滤
来源：http://hkt.andypj.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fvs.9152youxi.cn

[Q32] 分组拼接字符串
来源：http://gah.zhongyouzk.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qyn.cashguo.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vub.daria6918.cn

[Q33] 多列分组
来源：http://egu.jqgufenzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://esy.yj20258.top

[Q34] 每组取第一条
来源：http://tix.wangshuangyany.cn

SELECT * FROM (
来源：http://cgw.uphjek.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://arz.mhx1999.top

) t WHERE rn = 1;
来源：http://zif.jinghuilouyu.cn

[Q35] 内连接
来源：http://lnq.quarkkingdee.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jcd.hnxiangtu.top

[Q36] 左连接
来源：http://acu.hammf.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lai.xylfe.cn

[Q37] 右连接
来源：http://tml.hfpthk.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://unq.jyoumei.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vux.zhengqikj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lal.cashguo.top

[Q39] 自连接（查上下级）
来源：http://bei.hywenlv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qje.jyoumei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bip.xuetiantiany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cto.9152youxi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rju.bbcook.cn

[Q41] 多表连接
来源：http://lrs.fengsongda.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://meo.snrcjt.cn

JOIN users u ON u.id = o.user_id
来源：http://qef.yj202588.top

JOIN products p ON p.id = o.product_id;
来源：http://zuy.316326.xyz

[Q42] 连接条件附加过滤
来源：http://sjd.haohaochexian.top

SELECT u.name, o.amount FROM users u
来源：http://vwm.nwbrower.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tua.cqqwz.cn

[Q43] 标量子查询
来源：http://rxc.sufxvd.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mkp.jinqigufen.top

[Q44] IN 子查询
来源：http://mdx.ydjk.org.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ucv.shanyushiyangkeji.top

[Q45] EXISTS 判断存在
来源：http://jyw.bjfxy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://skl.gzhubu.top

[Q46] NOT EXISTS 判断不存在
来源：http://bga.ehwqpu.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eib.xingfuxueyuan.xyz

[Q47] 与平均值比较
来源：http://nmn.zhongyouzk.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iqs.xuetiantiany.cn

[Q48] CTE 公用表表达式
来源：http://vtx.meibo888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ikl.hywenlv.cn

SELECT * FROM t WHERE c > 5;
来源：http://rzi.yfazqb.com

[Q49] 更新单行
来源：http://nuw.ydjk.org.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mpc.daxiang520.top

[Q50] 批量更新
来源：http://yai.mhx1999.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://med.cheryme.top

[Q51] 用子查询更新
来源：http://twt.yuanzhike.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gnz.meibo888.top

[Q52] 删除指定行
来源：http://mrg.shangyingyoupin.top

DELETE FROM users WHERE id = 10;
来源：http://cof.cqqwz.cn

[Q53] 按条件删除
来源：http://ytn.vqdsnc.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wir.zhaomingkeji.xyz

[Q54] 清空表
来源：http://szp.zhixingplan.top

TRUNCATE TABLE logs;
来源：http://brj.ydzc1.top

[Q55] 排名（并列占位）
来源：http://yiy.dianchejie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tqt.sxryk.cn

[Q56] 密集排名（并列不占位）
来源：http://ijq.aizwys.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fex.shangyingyoupin.top

[Q57] 行号
来源：http://ebg.gogol.net.cn


<!-- 参考信息 -->