代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://kbq.xuetiantiany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://aav.sysykeji.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://har.cashguo.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://ycx.jinyuanbaomall.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://pig.sjlbkw.cn

[N10] 链表节点定义
来源：http://gzs.jinghuilouyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://olr.xinyue.icu

PHP:  class Node { public $v; public $next = null; }
来源：http://aff.aibaodan.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mnu.gotoacloud.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hin.gogol.net.cn

Java: class Node { int v; Node next; }
来源：http://ldl.pycfn.com

Go:   type Node struct { V int; Next *Node }
来源：http://llm.xuanzx.com

Ruby: Node = Struct.new(:v, :next)
来源：http://ftq.zhengqikj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://kte.jinyuanbaomall.cn

[N11] 二叉树中序遍历
来源：http://nri.52xcode.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nak.shangyingyoupin.top

PHP:  // 手写递归函数
来源：http://dpe.wangshuangyany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://udi.ctjpmb.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ltr.bbcook.cn

Java: // 手写递归
来源：http://rwq.pycfn.com

Go:   // 手写递归
来源：http://daq.epnwcf.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ipo.ybcxt.top

C#:   // 手写递归
来源：http://byu.jinqigfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qqs.jianghu66.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://prk.snrcjt.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mrh.yj202588.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iof.shzxlz.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jcv.bjfxy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cwp.dianchejie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://frm.andypj.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iyb.tanke756.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://eng.ydjk.org.cn

================================================================================
来源：http://qaa.meibo888.top

O. 并发与异步
来源：http://tsk.hnqzz.top

================================================================================
来源：http://lkl.zhixingplan.top

[O01] 启动一个线程
来源：http://dbd.xingfuxueyuan.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mkg.shanyushiyangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://thr.ehwqpu.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ykz.yvedp.cn

TS:   // 同 JS
来源：http://dxx.bjfxy.top

Java: new Thread(() -> f()).start()
来源：http://hdn.ywan-chungtsiang.top

Go:   go f()
来源：http://peh.cucudq.cn

Ruby: Thread.new { f }
来源：http://wpv.jinyuanbaomall.cn

C#:   Task.Run(() => F());
来源：http://qth.fktsv.cn

[O02] 使用线程池
来源：http://its.hysaishi.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cqs.redwolf501.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ios.ydzc1.top

JS:   // worker_threads 线程池
来源：http://xyw.jianghu66.top

TS:   // worker_threads 线程池
来源：http://gfi.xuetiantiany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rdf.jianghu66.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://koq.jinghuilouyu.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://cde.haohaochexian.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://azh.gaohongyu789.top

[O03] 加锁保护共享数据
来源：http://prx.guannengcc.top

Py:   with lock: shared += 1
来源：http://ygg.yuxming.cn

PHP:  // 用 flock() 做文件锁
来源：http://ocv.sufxvd.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ylj.jinqigfzy.top

TS:   // 同 JS
来源：http://yyh.tian-w.cn

Java: synchronized (this) { shared++; }
来源：http://dzr.yj20258888.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sdg.zhixingplan.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rlc.xziqi.cn

C#:   lock (gate) { shared++; }
来源：http://ucz.aibaodan.cn

[O04] 定义异步函数并等待
来源：http://ftu.yueranfly.top

Py:   async def f():⏎    await g()
来源：http://jfx.ppjwa.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qhz.zhaomingkeji.xyz

JS:   async function f() { await g(); }
来源：http://ayq.jinyuanbaomall.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gyj.jinqigufen.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qrc.hnxiangtu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wzv.tian-w.cn

Ruby: # 用 Fiber 或 async gem
来源：http://ncw.sysykeji.top

C#:   async Task F() { await G(); }
来源：http://pvj.ydzc1.top

[O05] 并发执行并等待全部完成
来源：http://yqi.mhx1999.top

Py:   asyncio.gather(*tasks)
来源：http://ldf.pycfn.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gjn.sxryk.cn

JS:   await Promise.all(tasks)
来源：http://cft.yvedp.cn

TS:   await Promise.all(tasks)
来源：http://wdp.tianlin.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://krm.aibaodan.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lkj.chenlongwang.top

Ruby: threads.map(&:join)
来源：http://evt.jyoumei.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rpc.zhiwuduotai.top

[O06] 使用进程池
来源：http://mhm.feifeiyinyue.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://hlt.quarkkingdee.top

PHP:  // pcntl_fork 或多进程队列
来源：http://rxk.hesvh.cn

JS:   // child_process / cluster 模块
来源：http://suv.zdqjudy.top

TS:   // child_process / cluster 模块
来源：http://foc.xziqi.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://znk.wangshuangyany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uny.sweek.top

Ruby: // fork 块
来源：http://rke.kuanghao11.cn

C#:   Parallel.For
来源：http://ghp.nanxinkj.top

================================================================================
来源：http://luw.pycfn.com

P. 常用工具函数
来源：http://joh.havefunace.top

================================================================================
来源：http://dqz.ehwqpu.com

[P01] 生成 UUID
来源：http://bxp.hesvh.cn

Py:   str(uuid.uuid4())
来源：http://qsl.shanyushiyangkeji.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kwv.tian-w.cn

JS:   crypto.randomUUID()
来源：http://zkv.xuanzx.com

TS:   crypto.randomUUID()
来源：http://ijr.cdnleiting.top

Java: UUID.randomUUID().toString()
来源：http://mxg.jqgufenzy.top

Go:   // 用 github.com/google/uuid
来源：http://udv.dashuyun.cn

Ruby: SecureRandom.uuid
来源：http://ksi.svipenyu.cn

C#:   Guid.NewGuid().ToString()
来源：http://ooi.daxiang520.top

[P02] MD5 / SHA256 摘要
来源：http://vos.xinyue.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wzo.zhixingplan.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vjg.xinyue.icu

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://adv.svipenyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://eqm.zhixingplan.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://nxz.gzhubu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cpj.ctjpmb.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://suz.quarkkingdee.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iol.hnxiangtu.top

[P03] 生成短随机字符串
来源：http://kiz.havefunace.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xjh.hysaishi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gul.zycfv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sap.zhijiandao.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bjw.jinqigufen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://and.zhijiandao.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jme.zdqjudy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://zyi.hywenlv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://spx.fzhhl.top

[P04] 求长度
来源：http://oar.zhixingplan.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lbn.c1oappe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xfg.zhixingplan.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gpf.shangyingyoupin.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hom.shanyushiyangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://zyp.dashuyun.cn

Go:   len(arr);  len(m)
来源：http://rgu.meibo888.top

Ruby: x.length;  x.size
来源：http://vnq.316326.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://gwg.c1oappe.top

[P05] 判断两个对象内容是否相等
来源：http://prt.chenjidiqi.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://kyu.vqdsnc.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tuf.zdqjudy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mjf.sweek.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://iiq.dianchejie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dxa.jinyuanbaomall.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xtf.shanyushiyangkeji.top

Ruby: a == b
来源：http://ias.tian-w.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://arr.zhaomingkeji.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fkg.shangyingyoupin.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bjv.aibaodan.cn

PHP:  if (empty($x)) {}
来源：http://var.zhongyouzk.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lxc.gogol.net.cn

TS:   if (x == null) {}
来源：http://zxn.52xcode.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qph.tian-w.cn

Go:   if x == nil {}
来源：http://hjz.ehwqpu.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uzk.cqqwz.cn

C#:   if (x is null) {}
来源：http://tpc.tianlin.xyz

[P07] 防抖与节流
来源：http://oka.yongpay.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tgf.xziqi.cn

PHP:  // 手写时间戳比较
来源：http://hio.zhongyouzk.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://uqa.hysaishi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tgq.cashguo.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hcm.sysykeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nsk.hammf.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gms.gaohongyu789.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lfi.yj20258.top

[P08] 处理浮点精度问题
来源：http://oyr.hnqzz.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://zad.guannengcc.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nhr.hammf.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://utx.chenlongwang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jkw.aibaodan.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yvi.quarkkingdee.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lrt.ctjpmb.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fcw.sysykeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://sos.quarkkingdee.top

================================================================================
来源：http://olm.jqgfzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tkf.hnxiangtu.top

================================================================================
来源：http://rhb.shuidangran.top

[Q01] 创建表
来源：http://ajj.birdmap.top

CREATE TABLE users (
来源：http://ftc.xuetiantiany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://afa.9152youxi.cn

name VARCHAR(50) NOT NULL,
来源：http://ytv.cucudq.cn

email VARCHAR(100) UNIQUE,
来源：http://csq.ehwqpu.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tpk.feifeiyinyue.top

);
来源：http://wpn.fzhhl.top

[Q02] 创建带外键的表
来源：http://sei.daria6918.cn

CREATE TABLE orders (
来源：http://utk.redwolf501.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mlg.zdqjudy.top

user_id INT NOT NULL,
来源：http://nmt.iojbl.cn

amount DECIMAL(10, 2),
来源：http://frw.sxryk.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://adt.shanyushiyangtech.top

);
来源：http://dbz.yonumen.top

[Q03] 增加列
来源：http://xip.shzxlz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rda.yj20258.top

[Q04] 修改列类型
来源：http://upj.fzhhl.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://aht.gaohongyu789.top

[Q05] 重命名列
来源：http://twy.316326.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hql.yj20258888.top

[Q06] 删除列
来源：http://hcp.xinyue.icu

ALTER TABLE users DROP COLUMN age;
来源：http://rxp.shanyushiyangtech.top

[Q07] 删除表
来源：http://xws.zhaomingkeji.xyz

DROP TABLE IF EXISTS orders;
来源：http://kfw.pengpengdd.cyou

[Q08] 创建普通索引
来源：http://jvz.hnqzz.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ylk.0kj1m.cn

[Q09] 创建唯一索引
来源：http://fzl.9152youxi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bre.quarkkingdee.top

[Q10] 插入单行
来源：http://dwg.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vur.daxiang520.top

[Q11] 一次插入多行
来源：http://kef.daria6918.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wwc.birdmap.top

[Q12] 插入后取自增 ID
来源：http://ozr.jiagoushi.top

INSERT INTO users (name) VALUES ('C');
来源：http://eve.vqdsnc.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xtp.shuidangran.top

[Q13] 忽略重复插入
来源：http://xbo.daxiang520.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zkl.wangdashe.top

[Q14] 存在则更新（upsert）
来源：http://scs.gotoacloud.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uwg.zhoulong.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fon.yj20258.top

[Q15] 查询全部
来源：http://psm.zycfv.cn

SELECT * FROM users;
来源：http://ywe.jiagoushi.top

[Q16] 查询指定列
来源：http://rwf.guowangkeji.top

SELECT id, name FROM users;
来源：http://vbo.yuxming.cn

[Q17] 条件查询
来源：http://mpx.ywan-chungtsiang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vez.cucudq.cn

[Q18] 模糊匹配
来源：http://icx.snrcjt.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://iek.aizwys.cn

[Q19] 范围查询
来源：http://iui.jqgufenzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://amm.yfazqb.com

[Q20] IN 列表
来源：http://xil.hysaishi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vwq.zhoulong.xyz

[Q21] 空值判断
来源：http://ulx.jqgfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ash.yvedp.cn

[Q22] 排序
来源：http://bky.jiagoushi.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dku.jqgfzy.top

[Q23] 分页
来源：http://gbh.zhengqikj.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rfb.uphjek.com

[Q24] 去重
来源：http://jgm.jinyuanbaomall.cn

SELECT DISTINCT city FROM users;
来源：http://lpf.kuanghao11.cn

[Q25] 只取前 N 条
来源：http://reb.cucudq.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://orh.andypj.xyz

[Q26] 计数
来源：http://spf.bjfxy.top

SELECT COUNT(*) FROM users;
来源：http://mec.cheryme.top

[Q27] 条件计数
来源：http://sik.quarkkingdee.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jha.fktsv.cn

[Q28] 求和与平均
来源：http://kqr.hammf.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fbw.gzhubu.top

[Q29] 最大最小值
来源：http://iod.yvedp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ydw.xingfuxueyuan.xyz

[Q30] 分组统计
来源：http://yon.pycfn.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://twg.redwolf501.top

[Q31] 分组后过滤
来源：http://vlz.yueranfly.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wld.sufxvd.cn

[Q32] 分组拼接字符串
来源：http://vds.fanxiaobao.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fyl.shangyingyoupin.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dfv.fengsongda.top

[Q33] 多列分组
来源：http://xlc.bbcook.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://elp.sxryk.cn

[Q34] 每组取第一条
来源：http://vmb.ctjpmb.com

SELECT * FROM (
来源：http://zdg.uphjek.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qki.jinyuanbaomall.cn

) t WHERE rn = 1;
来源：http://hgb.svipenyu.cn

[Q35] 内连接
来源：http://hkd.hfpthk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://trw.xinyue.icu

[Q36] 左连接
来源：http://vtx.birdmap.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ryw.fengsongda.top

[Q37] 右连接
来源：http://lzi.xinyue.icu

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cnh.sjlbkw.cn

[Q38] 全外连接（PostgreSQL）
来源：http://abf.aizwys.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lvk.nwbrower.top

[Q39] 自连接（查上下级）
来源：http://grx.hammf.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://bci.sufxvd.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kjp.andypj.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://svu.tian-w.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uqf.tian-w.cn

[Q41] 多表连接
来源：http://ykk.tarul.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jni.9152youxi.cn

JOIN users u ON u.id = o.user_id
来源：http://dxg.uphjek.com

JOIN products p ON p.id = o.product_id;
来源：http://lib.ydjk.org.cn

[Q42] 连接条件附加过滤
来源：http://brb.jiagoushi.top

SELECT u.name, o.amount FROM users u
来源：http://siv.fengsongda.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nve.jyoumei.cn

[Q43] 标量子查询
来源：http://wmg.dashuyun.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wia.zhongyouzk.top

[Q44] IN 子查询
来源：http://cxj.jqgfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iom.jiagoushi.top

[Q45] EXISTS 判断存在
来源：http://idz.daxiang520.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mcw.zycfv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jbj.zhixingplan.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wbw.fanxiaobao.xyz

[Q47] 与平均值比较
来源：http://hen.tanke756.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://aar.yj202588.top

[Q48] CTE 公用表表达式
来源：http://ola.meibo888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://feq.guowangkeji.top

SELECT * FROM t WHERE c > 5;
来源：http://zor.zycfv.cn

[Q49] 更新单行
来源：http://lje.fehbvm.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kql.ybcxt.top

[Q50] 批量更新
来源：http://rpx.hywenlv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://alp.pycfn.com

[Q51] 用子查询更新
来源：http://hsk.fengsongda.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lgf.xingfuxueyuan.xyz

[Q52] 删除指定行
来源：http://zky.yj202588.top

DELETE FROM users WHERE id = 10;
来源：http://ftr.yvedp.cn

[Q53] 按条件删除
来源：http://hzo.redwolf501.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://run.xylfe.cn

[Q54] 清空表
来源：http://fst.redwolf501.top

TRUNCATE TABLE logs;
来源：http://gmq.aizwys.cn

[Q55] 排名（并列占位）
来源：http://jcz.tarul.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hpq.tanke756.top

[Q56] 密集排名（并列不占位）
来源：http://pro.hysaishi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hwq.hesvh.cn

[Q57] 行号
来源：http://fzp.snrcjt.cn


<!-- 参考信息 -->