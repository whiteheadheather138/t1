代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://ffo.ehwqpu.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fuc.fehbvm.com

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://hib.yongpay.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://clq.jianghu66.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://evs.xinyue.icu

[N10] 链表节点定义
来源：http://nxc.yj202588.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hlf.xinyue.icu

PHP:  class Node { public $v; public $next = null; }
来源：http://hga.tian-w.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://opk.ydjk.org.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://pln.daria6918.cn

Java: class Node { int v; Node next; }
来源：http://ujp.xziqi.cn

Go:   type Node struct { V int; Next *Node }
来源：http://tcp.ywan-chungtsiang.top

Ruby: Node = Struct.new(:v, :next)
来源：http://cqz.jinghuilouyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://alx.0kj1m.cn

[N11] 二叉树中序遍历
来源：http://swg.cashguo.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nem.tian-w.cn

PHP:  // 手写递归函数
来源：http://icz.tian-w.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hqq.vqdsnc.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jsg.fktsv.cn

Java: // 手写递归
来源：http://dcq.52xcode.cn

Go:   // 手写递归
来源：http://vgq.gaohongyu789.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xyl.jqgufenzy.top

C#:   // 手写递归
来源：http://wsb.ehwqpu.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://niy.hysaishi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://jzf.jlsjyb.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ijb.vqdsnc.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qno.iojbl.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vay.hfpthk.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://oje.tian-w.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gsa.hywenlv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ipc.hnxiangtu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gst.hysaishi.cn

================================================================================
来源：http://pnt.hcnkem.com

O. 并发与异步
来源：http://wrg.meibo888.top

================================================================================
来源：http://hxk.cucudq.cn

[O01] 启动一个线程
来源：http://gfm.fengsongda.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nuy.mhx1999.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nbb.nwbrower.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mtl.yj20258.top

TS:   // 同 JS
来源：http://pjx.zhixingplan.top

Java: new Thread(() -> f()).start()
来源：http://aft.jiagoushi.top

Go:   go f()
来源：http://jzz.cdnleiting.top

Ruby: Thread.new { f }
来源：http://dqx.yvedp.cn

C#:   Task.Run(() => F());
来源：http://xhn.zdqjudy.top

[O02] 使用线程池
来源：http://yna.redwolf501.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vlv.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qtp.xinyue.icu

JS:   // worker_threads 线程池
来源：http://utt.ppjwa.cn

TS:   // worker_threads 线程池
来源：http://xnb.zhaomingkeji.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://bqv.xylfe.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wjl.ybcxt.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://djf.jinqigufen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://cot.shzxlz.cn

[O03] 加锁保护共享数据
来源：http://lvk.yj20258888.top

Py:   with lock: shared += 1
来源：http://deb.ctjpmb.com

PHP:  // 用 flock() 做文件锁
来源：http://hvc.birdmap.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tzq.52xcode.cn

TS:   // 同 JS
来源：http://gbj.pengpengdd.cyou

Java: synchronized (this) { shared++; }
来源：http://iiu.dashuyun.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nrx.tarul.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://uub.yanxiufei.cn

C#:   lock (gate) { shared++; }
来源：http://riv.snrcjt.cn

[O04] 定义异步函数并等待
来源：http://ejv.jqgufenzy.top

Py:   async def f():⏎    await g()
来源：http://vbc.yueranfly.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rry.yonumen.top

JS:   async function f() { await g(); }
来源：http://hzf.shangyingyoupin.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://szm.9152youxi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ryb.tianlin.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wpp.chenjidiqi.icu

Ruby: # 用 Fiber 或 async gem
来源：http://tpk.zdbjq.cn

C#:   async Task F() { await G(); }
来源：http://tkb.zhongyouzk.top

[O05] 并发执行并等待全部完成
来源：http://xgy.aizwys.cn

Py:   asyncio.gather(*tasks)
来源：http://qdj.jyoumei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ftj.chenjidiqi.icu

JS:   await Promise.all(tasks)
来源：http://oqx.fzhhl.top

TS:   await Promise.all(tasks)
来源：http://djt.tianlin.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tnx.ehwqpu.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xou.vehdjk.com

Ruby: threads.map(&:join)
来源：http://bdt.smart0.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://kzr.fengsongda.top

[O06] 使用进程池
来源：http://zqj.xziqi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xph.jianghu66.top

PHP:  // pcntl_fork 或多进程队列
来源：http://gdh.jlsjyb.cn

JS:   // child_process / cluster 模块
来源：http://hkb.fanxiaobao.xyz

TS:   // child_process / cluster 模块
来源：http://klc.hnxiangtu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://irm.fanxiaobao.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sfu.yanxiufei.cn

Ruby: // fork 块
来源：http://zgs.ivvv.top

C#:   Parallel.For
来源：http://pmb.smart0.xyz

================================================================================
来源：http://xjd.xziqi.cn

P. 常用工具函数
来源：http://vib.tianlin.xyz

================================================================================
来源：http://mib.sjlbkw.cn

[P01] 生成 UUID
来源：http://bha.cdnleiting.top

Py:   str(uuid.uuid4())
来源：http://wlb.guannengcc.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://olv.yj202588.top

JS:   crypto.randomUUID()
来源：http://cwk.kuanghao11.cn

TS:   crypto.randomUUID()
来源：http://yqf.daxiang520.top

Java: UUID.randomUUID().toString()
来源：http://cbf.svipenyu.cn

Go:   // 用 github.com/google/uuid
来源：http://oyb.svipenyu.cn

Ruby: SecureRandom.uuid
来源：http://ovj.ppjwa.cn

C#:   Guid.NewGuid().ToString()
来源：http://eme.yuxming.cn

[P02] MD5 / SHA256 摘要
来源：http://whf.zhaomingkeji.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hgt.gzhubu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://sez.jinyuanbaomall.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bxp.epnwcf.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hcu.cheryme.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wdj.sjlbkw.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hlb.ywan-chungtsiang.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kgo.yueranfly.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bpl.gaohongyu789.top

[P03] 生成短随机字符串
来源：http://vkf.fehbvm.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dfe.ivvv.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qef.yuxming.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ygc.wangdashe.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kda.svipenyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jmy.chenjidiqi.icu

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nvf.yj202588.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://fpx.redwolf501.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cwy.yj20258888.top

[P04] 求长度
来源：http://tyr.zhengqikj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kqw.guannengcc.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oxs.0kj1m.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pyy.shanyushiyangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ojd.yuanzhike.top

Java: list.size();  map.size();  s.length()
来源：http://ywr.gotoacloud.top

Go:   len(arr);  len(m)
来源：http://qjh.9152youxi.cn

Ruby: x.length;  x.size
来源：http://ptl.haohaochexian.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://jrs.cashguo.top

[P05] 判断两个对象内容是否相等
来源：http://ftm.fanxiaobao.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://mdo.fzhhl.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jqi.daria6918.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rar.meibo888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cmv.ctjpmb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ngv.iojbl.cn

Go:   reflect.DeepEqual(a, b)
来源：http://rhi.cheryme.top

Ruby: a == b
来源：http://ifx.aibaodan.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.52xcode.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qkx.sysykeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qht.hnqzz.top

PHP:  if (empty($x)) {}
来源：http://lvb.fengsongda.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://njn.sxryk.cn

TS:   if (x == null) {}
来源：http://lsd.ppjwa.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vyl.hongshengwenyu.top

Go:   if x == nil {}
来源：http://knt.xuanzx.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://trw.yuanzhike.top

C#:   if (x is null) {}
来源：http://men.guannengcc.top

[P07] 防抖与节流
来源：http://byh.chenjidiqi.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dow.jyoumei.cn

PHP:  // 手写时间戳比较
来源：http://paz.hongshengwenyu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://taz.yongpay.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zlb.andypj.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oyf.fehbvm.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://arv.andypj.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://vgi.yj20258888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ent.tian-w.cn

[P08] 处理浮点精度问题
来源：http://wyn.uphjek.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nzl.daxiang520.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nmc.0kj1m.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zzt.hammf.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://uph.shzxlz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xxh.xylfe.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hmd.pengpengdd.cyou

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lir.zhixingplan.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nea.cheryme.top

================================================================================
来源：http://dhe.yangfankeji.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zzg.xziqi.cn

================================================================================
来源：http://xqu.yj20258.top

[Q01] 创建表
来源：http://hep.yvedp.cn

CREATE TABLE users (
来源：http://dtp.zhiwuduotai.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qkr.fengsongda.top

name VARCHAR(50) NOT NULL,
来源：http://jli.gaohongyu789.top

email VARCHAR(100) UNIQUE,
来源：http://iyv.hammf.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://avb.gotoacloud.top

);
来源：http://rwz.zycfv.cn

[Q02] 创建带外键的表
来源：http://icb.xuetiantiany.cn

CREATE TABLE orders (
来源：http://fbu.meibo888.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zjr.cdnleiting.top

user_id INT NOT NULL,
来源：http://zqc.tarul.cn

amount DECIMAL(10, 2),
来源：http://uuc.tarul.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rxq.havefunace.top

);
来源：http://tuk.tarul.cn

[Q03] 增加列
来源：http://zib.tianlin.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zza.pengpengdd.cyou

[Q04] 修改列类型
来源：http://kyo.fzhhl.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vkr.chenjidiqi.icu

[Q05] 重命名列
来源：http://ldd.yfazqb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kda.hywenlv.cn

[Q06] 删除列
来源：http://qlr.cheryme.top

ALTER TABLE users DROP COLUMN age;
来源：http://ybh.shanyushiyangkeji.top

[Q07] 删除表
来源：http://uhh.tarul.cn

DROP TABLE IF EXISTS orders;
来源：http://cqy.vqdsnc.cn

[Q08] 创建普通索引
来源：http://dlt.ehwqpu.com

CREATE INDEX idx_users_email ON users(email);
来源：http://aau.sweek.top

[Q09] 创建唯一索引
来源：http://czw.cucudq.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ads.tianlin.xyz

[Q10] 插入单行
来源：http://ird.ydzc1.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mko.tanke756.top

[Q11] 一次插入多行
来源：http://pre.9152youxi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ghg.daxiang520.top

[Q12] 插入后取自增 ID
来源：http://slp.xziqi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://dve.hysaishi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oqt.shangyingyoupin.top

[Q13] 忽略重复插入
来源：http://nmp.gotoacloud.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jvk.yanxiufei.cn

[Q14] 存在则更新（upsert）
来源：http://aqd.fehbvm.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://roa.shanyushiyangkeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ktb.bbcook.cn

[Q15] 查询全部
来源：http://zwk.haohaochexian.top

SELECT * FROM users;
来源：http://gyx.wangshuangyany.cn

[Q16] 查询指定列
来源：http://ira.sweek.top

SELECT id, name FROM users;
来源：http://khd.ydzc1.top

[Q17] 条件查询
来源：http://cpl.tian-w.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ija.9152youxi.cn

[Q18] 模糊匹配
来源：http://yke.uphjek.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://agb.hysaishi.cn

[Q19] 范围查询
来源：http://yjr.ydzc1.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rsa.redwolf501.top

[Q20] IN 列表
来源：http://zkw.svipenyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hmd.daxiang520.top

[Q21] 空值判断
来源：http://cih.quarkkingdee.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kld.hcnkem.com

[Q22] 排序
来源：http://gkt.jinyuanbaomall.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://okn.ybcxt.top

[Q23] 分页
来源：http://cjy.fzhhl.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wud.hongshengwenyu.top

[Q24] 去重
来源：http://uke.xuanzx.com

SELECT DISTINCT city FROM users;
来源：http://jlb.yonumen.top

[Q25] 只取前 N 条
来源：http://xrx.fanxiaobao.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ahj.ppjwa.cn

[Q26] 计数
来源：http://eyq.jqgufenzy.top

SELECT COUNT(*) FROM users;
来源：http://pro.vehdjk.com

[Q27] 条件计数
来源：http://aul.aibaodan.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tbs.zhiwuduotai.top

[Q28] 求和与平均
来源：http://ytc.jyoumei.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ytf.sufxvd.cn

[Q29] 最大最小值
来源：http://myv.chenlongwang.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://lcs.xuetiantiany.cn

[Q30] 分组统计
来源：http://qmc.ppjwa.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rzm.yueranfly.top

[Q31] 分组后过滤
来源：http://aat.mhx1999.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lpu.cheryme.top

[Q32] 分组拼接字符串
来源：http://clo.ivvv.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zwr.vqdsnc.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ntx.guannengcc.top

[Q33] 多列分组
来源：http://npu.vqdsnc.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gry.c1oappe.top

[Q34] 每组取第一条
来源：http://zcx.bbcook.cn

SELECT * FROM (
来源：http://zmd.guannengcc.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://peh.zhongyouzk.top

) t WHERE rn = 1;
来源：http://zki.zhongyouzk.top

[Q35] 内连接
来源：http://jkl.gogol.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ltv.sxryk.cn

[Q36] 左连接
来源：http://hzl.ybcxt.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ypl.ehwqpu.com

[Q37] 右连接
来源：http://zaj.zycfv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fmk.hysaishi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ncl.xylfe.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cbw.xylfe.cn

[Q39] 自连接（查上下级）
来源：http://kgl.wangshuangyany.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://foh.ehwqpu.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zqp.fanxiaobao.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://xgb.hesvh.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://oek.fanxiaobao.xyz

[Q41] 多表连接
来源：http://ijm.cheryme.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ggu.yj202588.top

JOIN users u ON u.id = o.user_id
来源：http://wdu.ivvv.top

JOIN products p ON p.id = o.product_id;
来源：http://bvj.yj20258.top

[Q42] 连接条件附加过滤
来源：http://edq.uphjek.com

SELECT u.name, o.amount FROM users u
来源：http://uov.gogol.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mbx.tarul.cn

[Q43] 标量子查询
来源：http://msi.yj202588.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vue.xziqi.cn

[Q44] IN 子查询
来源：http://air.hammf.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uvh.jlsjyb.cn

[Q45] EXISTS 判断存在
来源：http://dfh.yonumen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pdv.aibaodan.cn

[Q46] NOT EXISTS 判断不存在
来源：http://oaf.xuanzx.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gnw.wangdashe.top

[Q47] 与平均值比较
来源：http://fxv.daria6918.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jnt.shzxlz.cn

[Q48] CTE 公用表表达式
来源：http://niy.hongshengwenyu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iej.ctjpmb.com

SELECT * FROM t WHERE c > 5;
来源：http://kwk.meibo888.top

[Q49] 更新单行
来源：http://yrc.gotoacloud.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ect.sufxvd.cn

[Q50] 批量更新
来源：http://wgd.zhiwuduotai.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cqj.tarul.cn

[Q51] 用子查询更新
来源：http://gam.andypj.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lto.hongshengwenyu.top

[Q52] 删除指定行
来源：http://sav.yuanzhike.top

DELETE FROM users WHERE id = 10;
来源：http://itc.dashuyun.cn

[Q53] 按条件删除
来源：http://bll.zhoulong.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hzf.ivvv.top

[Q54] 清空表
来源：http://oon.svipenyu.cn

TRUNCATE TABLE logs;
来源：http://kjx.daria6918.cn

[Q55] 排名（并列占位）
来源：http://qxr.c1oappe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fta.xziqi.cn

[Q56] 密集排名（并列不占位）
来源：http://urx.pycfn.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vlb.yueranfly.top

[Q57] 行号
来源：http://ywv.andypj.xyz


<!-- 参考信息 -->