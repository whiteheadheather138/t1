代发 wailian999

[N09] 栈与队列
来源：http://qjf.xylfe.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://ifu.ppjwa.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mec.ivvv.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://xag.quarkkingdee.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://rtl.jyoumei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ihx.jqgufenzy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://jgt.52xcode.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://rns.hywenlv.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jsm.fengsongda.top

[N10] 链表节点定义
来源：http://vcr.quarkkingdee.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hoe.wangshuangyany.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://opb.xuanzx.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://aos.wangdashe.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://sne.chenlongwang.top

Java: class Node { int v; Node next; }
来源：http://gzd.cdnleiting.top

Go:   type Node struct { V int; Next *Node }
来源：http://xib.cucudq.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://dwc.birdmap.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wpi.cdnleiting.top

[N11] 二叉树中序遍历
来源：http://aaz.ywan-chungtsiang.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nsk.xuetiantiany.cn

PHP:  // 手写递归函数
来源：http://jqy.guannengcc.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yfj.yuxming.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nzh.yuanzhike.top

Java: // 手写递归
来源：http://yfr.aibaodan.cn

Go:   // 手写递归
来源：http://rca.guannengcc.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cnx.xinyue.icu

C#:   // 手写递归
来源：http://czv.nanxuanxn.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://daq.ctjpmb.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hap.yonumen.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wsl.zhengqikj.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tgo.9152youxi.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qea.xinyue.icu

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kus.zhijiandao.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://snj.vehdjk.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gpg.zhaomingkeji.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wkb.yfazqb.com

================================================================================
来源：http://azo.cqqwz.cn

O. 并发与异步
来源：http://ron.jqgufenzy.top

================================================================================
来源：http://blh.daria6918.cn

[O01] 启动一个线程
来源：http://shh.dashuyun.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://iul.sufxvd.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://how.iojbl.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uke.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://luq.nanxuanxn.top

Java: new Thread(() -> f()).start()
来源：http://chp.guannengcc.top

Go:   go f()
来源：http://tid.pycfn.com

Ruby: Thread.new { f }
来源：http://cvk.tian-w.cn

C#:   Task.Run(() => F());
来源：http://qss.xuanzx.com

[O02] 使用线程池
来源：http://ueo.jlsjyb.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wjh.jinqigufen.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ikv.vehdjk.com

JS:   // worker_threads 线程池
来源：http://czl.zhengqikj.top

TS:   // worker_threads 线程池
来源：http://ttf.zhiwuduotai.top

Java: Executors.newFixedThreadPool(4)
来源：http://mbu.yuxming.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kwd.zhijiandao.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://eox.c1oappe.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xhl.jyoumei.cn

[O03] 加锁保护共享数据
来源：http://yea.ydjk.org.cn

Py:   with lock: shared += 1
来源：http://tmj.fzhhl.top

PHP:  // 用 flock() 做文件锁
来源：http://bxb.tianlin.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qkq.cucudq.cn

TS:   // 同 JS
来源：http://mgs.yongpay.top

Java: synchronized (this) { shared++; }
来源：http://cph.dashuyun.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://obd.jlsjyb.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://gqj.yonumen.top

C#:   lock (gate) { shared++; }
来源：http://wvr.shanyushiyangkeji.top

[O04] 定义异步函数并等待
来源：http://pfs.hysaishi.cn

Py:   async def f():⏎    await g()
来源：http://elk.wangdashe.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oup.shuidangran.top

JS:   async function f() { await g(); }
来源：http://ztb.vqdsnc.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rxn.meibo888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fye.guowangkeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vbr.chenzaomai.com

Ruby: # 用 Fiber 或 async gem
来源：http://oru.uphjek.com

C#:   async Task F() { await G(); }
来源：http://qqr.fehbvm.com

[O05] 并发执行并等待全部完成
来源：http://pbw.yangfankeji.com

Py:   asyncio.gather(*tasks)
来源：http://chl.pengpengdd.cyou

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cla.zhoulong.xyz

JS:   await Promise.all(tasks)
来源：http://ywx.xziqi.cn

TS:   await Promise.all(tasks)
来源：http://cns.dianchejie.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rgr.yfazqb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://foq.yj202588.top

Ruby: threads.map(&:join)
来源：http://xpa.zdqjudy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://evs.ivvv.top

[O06] 使用进程池
来源：http://lge.yueranfly.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://byu.tarul.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://vky.jinghuilouyu.cn

JS:   // child_process / cluster 模块
来源：http://nvy.gzhubu.top

TS:   // child_process / cluster 模块
来源：http://oco.yongpay.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vgu.shanyushiyangkeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zvy.jlsjyb.cn

Ruby: // fork 块
来源：http://aka.sysykeji.top

C#:   Parallel.For
来源：http://nlg.jlsjyb.cn

================================================================================
来源：http://wrd.ywan-chungtsiang.top

P. 常用工具函数
来源：http://ryg.fktsv.cn

================================================================================
来源：http://fse.xziqi.cn

[P01] 生成 UUID
来源：http://uwg.fengsongda.top

Py:   str(uuid.uuid4())
来源：http://riu.yvedp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zzn.ivvv.top

JS:   crypto.randomUUID()
来源：http://idm.kuanghao11.cn

TS:   crypto.randomUUID()
来源：http://wlh.sxryk.cn

Java: UUID.randomUUID().toString()
来源：http://pwk.shzxlz.cn

Go:   // 用 github.com/google/uuid
来源：http://thv.xylfe.cn

Ruby: SecureRandom.uuid
来源：http://btd.yanxiufei.cn

C#:   Guid.NewGuid().ToString()
来源：http://zoa.sufxvd.cn

[P02] MD5 / SHA256 摘要
来源：http://jpr.0kj1m.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mss.tarul.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jpg.ppjwa.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wwu.sufxvd.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fog.52xcode.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://brt.ppjwa.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tar.sufxvd.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mlb.yj20258888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xqn.meibo888.top

[P03] 生成短随机字符串
来源：http://pig.nanxuanxn.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rvp.0kj1m.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xpk.sufxvd.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rlp.xylfe.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hei.zhijiandao.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iwi.zhengqikj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pev.jyoumei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ebf.yfazqb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jyu.ctjpmb.com

[P04] 求长度
来源：http://vay.nanxinkj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://edh.ydzc1.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aru.haohaochexian.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vvw.nanxuanxn.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ais.tianlin.xyz

Java: list.size();  map.size();  s.length()
来源：http://pbg.xingfuxueyuan.xyz

Go:   len(arr);  len(m)
来源：http://vay.redwolf501.top

Ruby: x.length;  x.size
来源：http://agy.birdmap.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://uks.nwbrower.top

[P05] 判断两个对象内容是否相等
来源：http://zcw.zhaomingkeji.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://yoc.vqdsnc.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jcg.pengpengdd.cyou

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wzk.jiagoushi.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xgu.bbcook.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tzc.yuanzhike.top

Go:   reflect.DeepEqual(a, b)
来源：http://jas.feifeiyinyue.top

Ruby: a == b
来源：http://dya.aibaodan.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sim.hysaishi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ely.redwolf501.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dgo.jinqigufen.top

PHP:  if (empty($x)) {}
来源：http://xvu.jqgfzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gbd.zhoulong.xyz

TS:   if (x == null) {}
来源：http://sau.gotoacloud.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fcm.jlsjyb.cn

Go:   if x == nil {}
来源：http://gru.jiagoushi.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cxo.cucudq.cn

C#:   if (x is null) {}
来源：http://nel.jinyuanbaomall.cn

[P07] 防抖与节流
来源：http://zac.vehdjk.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rut.zhongyouzk.top

PHP:  // 手写时间戳比较
来源：http://zfe.andypj.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ile.pycfn.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ixi.jlsjyb.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ttf.vehdjk.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yth.yueranfly.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://nqw.shzxlz.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kgk.chenlongwang.top

[P08] 处理浮点精度问题
来源：http://vxf.nanxuanxn.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xih.fengsongda.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uvg.chenzaomai.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ijc.guowangkeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rxv.jinghuilouyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mlz.ctjpmb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kgm.fktsv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xgn.iojbl.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lzl.nanxinkj.top

================================================================================
来源：http://jrs.dashuyun.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://whe.dianchejie.cn

================================================================================
来源：http://zhn.ybcxt.top

[Q01] 创建表
来源：http://zru.hfpthk.cn

CREATE TABLE users (
来源：http://ipp.ydjk.org.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bkk.tianlin.xyz

name VARCHAR(50) NOT NULL,
来源：http://zmz.hammf.cn

email VARCHAR(100) UNIQUE,
来源：http://pcp.yuanzhike.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lbk.yvedp.cn

);
来源：http://csm.yonumen.top

[Q02] 创建带外键的表
来源：http://dyv.cheryme.top

CREATE TABLE orders (
来源：http://mzf.wangdashe.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dii.ywan-chungtsiang.top

user_id INT NOT NULL,
来源：http://wdf.shanyushiyangtech.top

amount DECIMAL(10, 2),
来源：http://fcd.tanke756.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xny.zhoulong.xyz

);
来源：http://jjh.yj202588.top

[Q03] 增加列
来源：http://awh.chenjidiqi.icu

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uwx.jinghuilouyu.cn

[Q04] 修改列类型
来源：http://kqc.quarkkingdee.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://enz.pengpengdd.cyou

[Q05] 重命名列
来源：http://nwl.xingfuxueyuan.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qjh.guowangkeji.top

[Q06] 删除列
来源：http://lyk.0kj1m.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nlo.ydzc1.top

[Q07] 删除表
来源：http://qwg.cqqwz.cn

DROP TABLE IF EXISTS orders;
来源：http://tdo.hammf.cn

[Q08] 创建普通索引
来源：http://nqd.gaohongyu789.top

CREATE INDEX idx_users_email ON users(email);
来源：http://lmv.316326.xyz

[Q09] 创建唯一索引
来源：http://men.svipenyu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://byo.meibo888.top

[Q10] 插入单行
来源：http://naf.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wag.xylfe.cn

[Q11] 一次插入多行
来源：http://vlm.wangdashe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kjl.yj202588.top

[Q12] 插入后取自增 ID
来源：http://nes.feifeiyinyue.top

INSERT INTO users (name) VALUES ('C');
来源：http://qpb.guannengcc.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pro.xylfe.cn

[Q13] 忽略重复插入
来源：http://oqa.sysykeji.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xih.jinqigufen.top

[Q14] 存在则更新（upsert）
来源：http://tsn.yvedp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oeb.yj20258.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ovt.zdqjudy.top

[Q15] 查询全部
来源：http://svc.xylfe.cn

SELECT * FROM users;
来源：http://omm.yonumen.top

[Q16] 查询指定列
来源：http://gdc.ivvv.top

SELECT id, name FROM users;
来源：http://ekr.jianghu66.top

[Q17] 条件查询
来源：http://xys.fengsongda.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gwi.yangfankeji.com

[Q18] 模糊匹配
来源：http://czk.ehwqpu.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dvq.hywenlv.cn

[Q19] 范围查询
来源：http://wiu.fzhhl.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bro.havefunace.top

[Q20] IN 列表
来源：http://sth.gaohongyu789.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xdd.pengpengdd.cyou

[Q21] 空值判断
来源：http://mfq.xuetiantiany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://uow.jqgufenzy.top

[Q22] 排序
来源：http://xda.shuidangran.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hbp.sufxvd.cn

[Q23] 分页
来源：http://upb.ybcxt.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xfc.dianchejie.cn

[Q24] 去重
来源：http://vvu.shzxlz.cn

SELECT DISTINCT city FROM users;
来源：http://uau.hesvh.cn

[Q25] 只取前 N 条
来源：http://wac.hesvh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ztn.ywan-chungtsiang.top

[Q26] 计数
来源：http://nwk.jqgufenzy.top

SELECT COUNT(*) FROM users;
来源：http://dof.cashguo.top

[Q27] 条件计数
来源：http://rin.ydjk.org.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uyi.haohaochexian.top

[Q28] 求和与平均
来源：http://zmx.redwolf501.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jnc.daria6918.cn

[Q29] 最大最小值
来源：http://ocn.sxryk.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ast.zhiwuduotai.top

[Q30] 分组统计
来源：http://bbt.uphjek.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ass.jyoumei.cn

[Q31] 分组后过滤
来源：http://sta.hcnkem.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lcc.iojbl.cn

[Q32] 分组拼接字符串
来源：http://zmt.jinyuanbaomall.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xcm.ydjk.org.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ybo.haohaochexian.top

[Q33] 多列分组
来源：http://bfu.nwbrower.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://usd.shanyushiyangkeji.top

[Q34] 每组取第一条
来源：http://jub.ydjk.org.cn

SELECT * FROM (
来源：http://qzw.birdmap.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mar.zhoulong.xyz

) t WHERE rn = 1;
来源：http://ekl.zhiwuduotai.top

[Q35] 内连接
来源：http://nwg.jlsjyb.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://est.mhx1999.top

[Q36] 左连接
来源：http://rht.guannengcc.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://aat.jyoumei.cn

[Q37] 右连接
来源：http://pey.yvedp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jon.jyoumei.cn

[Q38] 全外连接（PostgreSQL）
来源：http://ygo.yj20258.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://anp.9152youxi.cn

[Q39] 自连接（查上下级）
来源：http://mxx.hammf.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://yyd.9152youxi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sgx.hongshengwenyu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://nzp.vehdjk.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rbu.guowangkeji.top

[Q41] 多表连接
来源：http://akw.ppjwa.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jgy.tian-w.cn

JOIN users u ON u.id = o.user_id
来源：http://byd.gzhubu.top

JOIN products p ON p.id = o.product_id;
来源：http://fck.yfazqb.com

[Q42] 连接条件附加过滤
来源：http://utf.xuanzx.com

SELECT u.name, o.amount FROM users u
来源：http://eee.daxiang520.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xjo.zycfv.cn

[Q43] 标量子查询
来源：http://hyg.zhengqikj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dka.ctjpmb.com

[Q44] IN 子查询
来源：http://yln.zhoulong.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fap.hnqzz.top

[Q45] EXISTS 判断存在
来源：http://ymo.chenzaomai.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cbk.sjlbkw.cn

[Q46] NOT EXISTS 判断不存在
来源：http://auk.shanyushiyangtech.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://byo.wangdashe.top

[Q47] 与平均值比较
来源：http://rcq.ydjk.org.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xkx.tian-w.cn

[Q48] CTE 公用表表达式
来源：http://vll.xuetiantiany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://atw.zdbjq.cn

SELECT * FROM t WHERE c > 5;
来源：http://atb.gotoacloud.top

[Q49] 更新单行
来源：http://pzs.yj20258.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://enp.sufxvd.cn

[Q50] 批量更新
来源：http://rti.zhiwuduotai.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bwx.ivvv.top

[Q51] 用子查询更新
来源：http://eaj.smart0.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mdl.ehwqpu.com

[Q52] 删除指定行
来源：http://laz.316326.xyz

DELETE FROM users WHERE id = 10;
来源：http://zpm.uphjek.com

[Q53] 按条件删除
来源：http://ryw.ydzc1.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ewo.wangdashe.top

[Q54] 清空表
来源：http://rwm.jinqigufen.top

TRUNCATE TABLE logs;
来源：http://vwk.birdmap.top

[Q55] 排名（并列占位）
来源：http://mrh.feifeiyinyue.top


<!-- 参考信息 -->