代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://oyt.tian-w.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://jdm.hywenlv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://uac.yj202588.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ltj.daria6918.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://sso.ydjk.org.cn

[N10] 链表节点定义
来源：http://rfl.ydzc1.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://gup.dashuyun.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://wfb.nwbrower.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gtl.jianghu66.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mcr.xziqi.cn

Java: class Node { int v; Node next; }
来源：http://kmc.gotoacloud.top

Go:   type Node struct { V int; Next *Node }
来源：http://umt.zdqjudy.top

Ruby: Node = Struct.new(:v, :next)
来源：http://npx.hnqzz.top

C#:   class Node { public int V; public Node? Next; }
来源：http://bjo.nanxinkj.top

[N11] 二叉树中序遍历
来源：http://tiv.fehbvm.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://gff.hywenlv.cn

PHP:  // 手写递归函数
来源：http://qar.yonumen.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mbp.jyoumei.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zvx.wangshuangyany.cn

Java: // 手写递归
来源：http://axe.fehbvm.com

Go:   // 手写递归
来源：http://mmt.ctjpmb.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://gej.guannengcc.top

C#:   // 手写递归
来源：http://wil.316326.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ghx.guannengcc.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://kys.fktsv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hho.hywenlv.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hnn.xuanzx.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tog.jianghu66.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pwl.cashguo.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://trt.hesvh.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ktt.yuxming.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qoo.shzxlz.cn

================================================================================
来源：http://tti.pengpengdd.cyou

O. 并发与异步
来源：http://csb.shanyushiyangtech.top

================================================================================
来源：http://zjk.uphjek.com

[O01] 启动一个线程
来源：http://goc.mhx1999.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zdo.aizwys.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bnb.nanxuanxn.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nsd.nanxuanxn.top

TS:   // 同 JS
来源：http://hls.c1oappe.top

Java: new Thread(() -> f()).start()
来源：http://nqn.zhijiandao.cn

Go:   go f()
来源：http://acf.hcnkem.com

Ruby: Thread.new { f }
来源：http://icx.fehbvm.com

C#:   Task.Run(() => F());
来源：http://wya.gogol.net.cn

[O02] 使用线程池
来源：http://hpy.cqqwz.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cjw.sxryk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://gmi.shuidangran.top

JS:   // worker_threads 线程池
来源：http://ljc.jqgufenzy.top

TS:   // worker_threads 线程池
来源：http://doj.hongshengwenyu.top

Java: Executors.newFixedThreadPool(4)
来源：http://ozd.jqgufenzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vlf.nanxuanxn.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bxp.yanxiufei.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://bte.ppjwa.cn

[O03] 加锁保护共享数据
来源：http://duz.aizwys.cn

Py:   with lock: shared += 1
来源：http://uol.meibo888.top

PHP:  // 用 flock() 做文件锁
来源：http://lel.daria6918.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lzd.yonumen.top

TS:   // 同 JS
来源：http://sne.zhengqikj.top

Java: synchronized (this) { shared++; }
来源：http://wdr.yj202588.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://idi.sysykeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://itz.zhaomingkeji.xyz

C#:   lock (gate) { shared++; }
来源：http://uor.gaohongyu789.top

[O04] 定义异步函数并等待
来源：http://blk.daria6918.cn

Py:   async def f():⏎    await g()
来源：http://gby.c1oappe.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pmf.fzhhl.top

JS:   async function f() { await g(); }
来源：http://qmt.fanxiaobao.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://wpp.ybcxt.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kri.chenjidiqi.icu

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gxh.zhaomingkeji.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://rww.jiagoushi.top

C#:   async Task F() { await G(); }
来源：http://fut.tarul.cn

[O05] 并发执行并等待全部完成
来源：http://wnk.cqqwz.cn

Py:   asyncio.gather(*tasks)
来源：http://vqo.tianlin.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hla.hammf.cn

JS:   await Promise.all(tasks)
来源：http://eyj.sysykeji.top

TS:   await Promise.all(tasks)
来源：http://ttx.gotoacloud.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xam.cqqwz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://phh.andypj.xyz

Ruby: threads.map(&:join)
来源：http://nfj.fehbvm.com

C#:   await Task.WhenAll(t1, t2)
来源：http://dqq.zdqjudy.top

[O06] 使用进程池
来源：http://nep.yueranfly.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://duh.shangyingyoupin.top

PHP:  // pcntl_fork 或多进程队列
来源：http://jww.daxiang520.top

JS:   // child_process / cluster 模块
来源：http://cjm.pengpengdd.cyou

TS:   // child_process / cluster 模块
来源：http://wsp.yj20258.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ner.hesvh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mwl.yuxming.cn

Ruby: // fork 块
来源：http://lqg.zhixingplan.top

C#:   Parallel.For
来源：http://svp.haohaochexian.top

================================================================================
来源：http://nju.aizwys.cn

P. 常用工具函数
来源：http://stu.meibo888.top

================================================================================
来源：http://qgb.yanxiufei.cn

[P01] 生成 UUID
来源：http://wxx.iojbl.cn

Py:   str(uuid.uuid4())
来源：http://ghi.pycfn.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mcr.yonumen.top

JS:   crypto.randomUUID()
来源：http://ouo.guowangkeji.top

TS:   crypto.randomUUID()
来源：http://bwi.mhx1999.top

Java: UUID.randomUUID().toString()
来源：http://ysy.quarkkingdee.top

Go:   // 用 github.com/google/uuid
来源：http://emt.guannengcc.top

Ruby: SecureRandom.uuid
来源：http://dhl.ehwqpu.com

C#:   Guid.NewGuid().ToString()
来源：http://mao.xuetiantiany.cn

[P02] MD5 / SHA256 摘要
来源：http://ckr.ywan-chungtsiang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fec.tian-w.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://eal.vqdsnc.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ryb.hongshengwenyu.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://kam.hywenlv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mtr.hnxiangtu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ipa.cqqwz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fme.gogol.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://imb.0kj1m.cn

[P03] 生成短随机字符串
来源：http://lxx.daxiang520.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jml.fktsv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vpe.tanke756.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bph.gaohongyu789.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mby.shuidangran.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qsp.chenzaomai.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jyo.hywenlv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tsd.c1oappe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://kxh.chenjidiqi.icu

[P04] 求长度
来源：http://vzx.daxiang520.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uwo.yongpay.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jxs.hnxiangtu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lzi.vehdjk.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wob.yvedp.cn

Java: list.size();  map.size();  s.length()
来源：http://kcf.zycfv.cn

Go:   len(arr);  len(m)
来源：http://cpe.nanxinkj.top

Ruby: x.length;  x.size
来源：http://tfo.wangdashe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://iae.fengsongda.top

[P05] 判断两个对象内容是否相等
来源：http://ccg.hammf.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://agj.9152youxi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rnz.pycfn.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vxq.xuetiantiany.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xjz.sufxvd.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ajf.epnwcf.com

Go:   reflect.DeepEqual(a, b)
来源：http://jpw.fehbvm.com

Ruby: a == b
来源：http://qrb.cqqwz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sak.tanke756.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hkl.jianghu66.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xae.shangyingyoupin.top

PHP:  if (empty($x)) {}
来源：http://qkx.yj20258888.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tlj.sxryk.cn

TS:   if (x == null) {}
来源：http://gov.fzhhl.top

Java: if (x == null || x.isEmpty()) {}
来源：http://usv.shanyushiyangkeji.top

Go:   if x == nil {}
来源：http://tzn.hysaishi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ghh.hesvh.cn

C#:   if (x is null) {}
来源：http://ozv.yj20258.top

[P07] 防抖与节流
来源：http://qky.fzhhl.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://afg.52xcode.cn

PHP:  // 手写时间戳比较
来源：http://ino.yj20258.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pyn.xingfuxueyuan.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://viu.zycfv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://edb.hnxiangtu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hce.dianchejie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wov.sxryk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mzj.yuanzhike.top

[P08] 处理浮点精度问题
来源：http://zzx.0kj1m.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ayz.jqgufenzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dyx.sysykeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jok.zhoulong.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://esd.shuidangran.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://evk.xuetiantiany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://uux.yanxiufei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://njc.hcnkem.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ooa.xziqi.cn

================================================================================
来源：http://yqn.xinyue.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tze.xinyue.icu

================================================================================
来源：http://vfn.yfazqb.com

[Q01] 创建表
来源：http://kzc.9152youxi.cn

CREATE TABLE users (
来源：http://evt.smart0.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://iqo.vehdjk.com

name VARCHAR(50) NOT NULL,
来源：http://arq.shanyushiyangtech.top

email VARCHAR(100) UNIQUE,
来源：http://jum.ehwqpu.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cto.zycfv.cn

);
来源：http://jna.cdnleiting.top

[Q02] 创建带外键的表
来源：http://cle.wangshuangyany.cn

CREATE TABLE orders (
来源：http://adw.fktsv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cbp.jinqigfzy.top

user_id INT NOT NULL,
来源：http://vyy.jinqigfzy.top

amount DECIMAL(10, 2),
来源：http://itl.ctjpmb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pyj.zycfv.cn

);
来源：http://soe.dashuyun.cn

[Q03] 增加列
来源：http://cxi.yj202588.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ubg.xylfe.cn

[Q04] 修改列类型
来源：http://wnt.ybcxt.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wrm.zhijiandao.cn

[Q05] 重命名列
来源：http://itt.shanyushiyangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://iup.zhengqikj.top

[Q06] 删除列
来源：http://frg.tian-w.cn

ALTER TABLE users DROP COLUMN age;
来源：http://agg.wangdashe.top

[Q07] 删除表
来源：http://fal.gzhubu.top

DROP TABLE IF EXISTS orders;
来源：http://zsr.zhijiandao.cn

[Q08] 创建普通索引
来源：http://oko.chenlongwang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qfl.jqgufenzy.top

[Q09] 创建唯一索引
来源：http://hga.tianlin.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dwe.pycfn.com

[Q10] 插入单行
来源：http://oic.52xcode.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hma.hysaishi.cn

[Q11] 一次插入多行
来源：http://kkc.cqqwz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://flt.zdqjudy.top

[Q12] 插入后取自增 ID
来源：http://bey.vehdjk.com

INSERT INTO users (name) VALUES ('C');
来源：http://oko.yfazqb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xtr.jiagoushi.top

[Q13] 忽略重复插入
来源：http://ini.yj20258.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dng.yueranfly.top

[Q14] 存在则更新（upsert）
来源：http://lmm.yj20258.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nbw.shanyushiyangtech.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gje.zhixingplan.top

[Q15] 查询全部
来源：http://cyp.xuanzx.com

SELECT * FROM users;
来源：http://crz.cdnleiting.top

[Q16] 查询指定列
来源：http://ejz.jqgufenzy.top

SELECT id, name FROM users;
来源：http://kbq.xziqi.cn

[Q17] 条件查询
来源：http://gjb.zhixingplan.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sed.daria6918.cn

[Q18] 模糊匹配
来源：http://vva.daxiang520.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jtk.cdnleiting.top

[Q19] 范围查询
来源：http://fnt.fengsongda.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://yzr.wangdashe.top

[Q20] IN 列表
来源：http://tqc.gogol.net.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cat.smart0.xyz

[Q21] 空值判断
来源：http://qik.aizwys.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ryb.tanke756.top

[Q22] 排序
来源：http://naa.yj20258888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fmg.bjfxy.top

[Q23] 分页
来源：http://rzr.jiagoushi.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tib.svipenyu.cn

[Q24] 去重
来源：http://crg.dianchejie.cn

SELECT DISTINCT city FROM users;
来源：http://rii.birdmap.top

[Q25] 只取前 N 条
来源：http://uyf.ctjpmb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ukk.zhoulong.xyz

[Q26] 计数
来源：http://bve.cdnleiting.top

SELECT COUNT(*) FROM users;
来源：http://pso.tianlin.xyz

[Q27] 条件计数
来源：http://bot.chenzaomai.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ncj.zhixingplan.top

[Q28] 求和与平均
来源：http://rgl.yueranfly.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sdf.tarul.cn

[Q29] 最大最小值
来源：http://lxh.chenzaomai.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://lnp.hywenlv.cn

[Q30] 分组统计
来源：http://sos.hfpthk.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ykz.chenzaomai.com

[Q31] 分组后过滤
来源：http://fqd.gzhubu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hnq.ydjk.org.cn

[Q32] 分组拼接字符串
来源：http://fui.sjlbkw.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://twr.sweek.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cih.jlsjyb.cn

[Q33] 多列分组
来源：http://ukk.xingfuxueyuan.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sbx.xylfe.cn

[Q34] 每组取第一条
来源：http://unn.nanxuanxn.top

SELECT * FROM (
来源：http://sbt.quarkkingdee.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ich.xylfe.cn

) t WHERE rn = 1;
来源：http://uex.fktsv.cn

[Q35] 内连接
来源：http://qtt.cashguo.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lgz.yuxming.cn

[Q36] 左连接
来源：http://ier.birdmap.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hgl.jyoumei.cn

[Q37] 右连接
来源：http://xcy.jinqigufen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ret.zhaomingkeji.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://iqk.tian-w.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xgz.tianlin.xyz

[Q39] 自连接（查上下级）
来源：http://osm.yuanzhike.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://sdv.tanke756.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://knl.zhoulong.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://qnt.sxryk.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wwf.ybcxt.top

[Q41] 多表连接
来源：http://njj.9152youxi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://sds.zhiwuduotai.top

JOIN users u ON u.id = o.user_id
来源：http://uya.hesvh.cn

JOIN products p ON p.id = o.product_id;
来源：http://sgn.fengsongda.top

[Q42] 连接条件附加过滤
来源：http://dph.feifeiyinyue.top

SELECT u.name, o.amount FROM users u
来源：http://xkn.tarul.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://eol.chenzaomai.com

[Q43] 标量子查询
来源：http://vsd.52xcode.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nsz.xuetiantiany.cn

[Q44] IN 子查询
来源：http://xni.zhiwuduotai.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pjn.jyoumei.cn

[Q45] EXISTS 判断存在
来源：http://ivh.shuidangran.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nip.ywan-chungtsiang.top

[Q46] NOT EXISTS 判断不存在
来源：http://xjc.hysaishi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bou.hywenlv.cn

[Q47] 与平均值比较
来源：http://hdm.uphjek.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://itl.0kj1m.cn

[Q48] CTE 公用表表达式
来源：http://kdc.shzxlz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xzk.gaohongyu789.top

SELECT * FROM t WHERE c > 5;
来源：http://kbi.yuxming.cn

[Q49] 更新单行
来源：http://nzw.sysykeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://agi.fzhhl.top

[Q50] 批量更新
来源：http://nyn.xinyue.icu

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xmu.jinghuilouyu.cn

[Q51] 用子查询更新
来源：http://zgd.guannengcc.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jbb.aibaodan.cn

[Q52] 删除指定行
来源：http://ovi.hesvh.cn

DELETE FROM users WHERE id = 10;
来源：http://dkn.sufxvd.cn

[Q53] 按条件删除
来源：http://ipt.wangdashe.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mbi.dianchejie.cn

[Q54] 清空表
来源：http://eiy.yvedp.cn

TRUNCATE TABLE logs;
来源：http://isp.jqgfzy.top

[Q55] 排名（并列占位）
来源：http://fxi.sysykeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://twm.yanxiufei.cn

[Q56] 密集排名（并列不占位）
来源：http://aue.nanxinkj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cka.hammf.cn

[Q57] 行号
来源：http://nxo.nanxuanxn.top


<!-- 参考信息 -->