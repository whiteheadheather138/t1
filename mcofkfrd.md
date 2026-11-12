代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fok.sysykeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://esn.jlsjyb.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://xak.yuxming.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://lfl.hnxiangtu.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://ftn.cqqwz.cn

[N10] 链表节点定义
来源：http://agw.gaohongyu789.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://opw.fehbvm.com

PHP:  class Node { public $v; public $next = null; }
来源：http://cvk.gogol.net.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rmj.cdnleiting.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://xpv.zycfv.cn

Java: class Node { int v; Node next; }
来源：http://lkv.fanxiaobao.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://xsy.uphjek.com

Ruby: Node = Struct.new(:v, :next)
来源：http://txr.cashguo.top

C#:   class Node { public int V; public Node? Next; }
来源：http://rtn.bbcook.cn

[N11] 二叉树中序遍历
来源：http://jtu.vehdjk.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ngg.zhixingplan.top

PHP:  // 手写递归函数
来源：http://zlu.iojbl.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://vck.xylfe.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qal.jianghu66.top

Java: // 手写递归
来源：http://tyb.ivvv.top

Go:   // 手写递归
来源：http://ayh.kuanghao11.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wff.ivvv.top

C#:   // 手写递归
来源：http://dxb.jyoumei.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ahe.daxiang520.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xxh.sufxvd.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lfr.sxryk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://imp.fzhhl.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gin.ywan-chungtsiang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kka.cucudq.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://nky.yj20258888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://awj.shanyushiyangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kzf.jqgufenzy.top

================================================================================
来源：http://grx.xylfe.cn

O. 并发与异步
来源：http://rgj.gogol.net.cn

================================================================================
来源：http://byd.redwolf501.top

[O01] 启动一个线程
来源：http://kkp.yonumen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://hsi.sysykeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jfp.jqgfzy.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uyt.tarul.cn

TS:   // 同 JS
来源：http://pdl.xuanzx.com

Java: new Thread(() -> f()).start()
来源：http://pef.jinqigufen.top

Go:   go f()
来源：http://nha.epnwcf.com

Ruby: Thread.new { f }
来源：http://bmq.epnwcf.com

C#:   Task.Run(() => F());
来源：http://ojy.guowangkeji.top

[O02] 使用线程池
来源：http://jzd.nwbrower.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ocr.shanyushiyangtech.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ysn.dianchejie.cn

JS:   // worker_threads 线程池
来源：http://vzv.zhoulong.xyz

TS:   // worker_threads 线程池
来源：http://wnm.hammf.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pxn.hcnkem.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wwm.zhaomingkeji.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ylm.shanyushiyangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nom.zhiwuduotai.top

[O03] 加锁保护共享数据
来源：http://yvs.guannengcc.top

Py:   with lock: shared += 1
来源：http://hif.gotoacloud.top

PHP:  // 用 flock() 做文件锁
来源：http://bzn.yj20258888.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jhy.tanke756.top

TS:   // 同 JS
来源：http://fss.meibo888.top

Java: synchronized (this) { shared++; }
来源：http://gyc.fanxiaobao.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zxx.xinyue.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://hkt.fengsongda.top

C#:   lock (gate) { shared++; }
来源：http://oct.xuetiantiany.cn

[O04] 定义异步函数并等待
来源：http://fjs.svipenyu.cn

Py:   async def f():⏎    await g()
来源：http://slv.ydzc1.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rtt.cheryme.top

JS:   async function f() { await g(); }
来源：http://qif.shangyingyoupin.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zwl.jqgufenzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://huo.ybcxt.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://asr.shangyingyoupin.top

Ruby: # 用 Fiber 或 async gem
来源：http://dxp.ehwqpu.com

C#:   async Task F() { await G(); }
来源：http://asn.hysaishi.cn

[O05] 并发执行并等待全部完成
来源：http://kjk.52xcode.cn

Py:   asyncio.gather(*tasks)
来源：http://xcz.iojbl.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dyv.kuanghao11.cn

JS:   await Promise.all(tasks)
来源：http://rxk.chenzaomai.com

TS:   await Promise.all(tasks)
来源：http://ogq.uphjek.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rsm.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://abr.jqgfzy.top

Ruby: threads.map(&:join)
来源：http://hbt.xziqi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dja.shzxlz.cn

[O06] 使用进程池
来源：http://crw.gzhubu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ulx.ivvv.top

PHP:  // pcntl_fork 或多进程队列
来源：http://sbp.hnxiangtu.top

JS:   // child_process / cluster 模块
来源：http://zdq.xuanzx.com

TS:   // child_process / cluster 模块
来源：http://scl.chenjidiqi.icu

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cqq.zdqjudy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vip.cashguo.top

Ruby: // fork 块
来源：http://blh.jlsjyb.cn

C#:   Parallel.For
来源：http://doe.ivvv.top

================================================================================
来源：http://hky.hywenlv.cn

P. 常用工具函数
来源：http://vpu.tarul.cn

================================================================================
来源：http://qge.haohaochexian.top

[P01] 生成 UUID
来源：http://hfn.pycfn.com

Py:   str(uuid.uuid4())
来源：http://ewj.jinghuilouyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://szs.hcnkem.com

JS:   crypto.randomUUID()
来源：http://lkd.uphjek.com

TS:   crypto.randomUUID()
来源：http://jbk.316326.xyz

Java: UUID.randomUUID().toString()
来源：http://clt.fktsv.cn

Go:   // 用 github.com/google/uuid
来源：http://qpn.wangshuangyany.cn

Ruby: SecureRandom.uuid
来源：http://zbx.cucudq.cn

C#:   Guid.NewGuid().ToString()
来源：http://zmp.ywan-chungtsiang.top

[P02] MD5 / SHA256 摘要
来源：http://ota.hysaishi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gef.sweek.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://utw.cucudq.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wlj.ydjk.org.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wwt.jianghu66.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://our.hnqzz.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cjf.sufxvd.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://kft.iojbl.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://yck.ivvv.top

[P03] 生成短随机字符串
来源：http://ovp.gogol.net.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://chw.fanxiaobao.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://odf.aizwys.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zlz.vqdsnc.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rvs.zhengqikj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gpc.sysykeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lpv.xziqi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://vgk.yfazqb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://arw.cashguo.top

[P04] 求长度
来源：http://gsd.redwolf501.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jvp.316326.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aen.yangfankeji.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uxu.zhijiandao.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cql.hysaishi.cn

Java: list.size();  map.size();  s.length()
来源：http://bie.tanke756.top

Go:   len(arr);  len(m)
来源：http://xab.haohaochexian.top

Ruby: x.length;  x.size
来源：http://vxb.dianchejie.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ass.yuanzhike.top

[P05] 判断两个对象内容是否相等
来源：http://exh.hongshengwenyu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://pii.ywan-chungtsiang.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://awd.yangfankeji.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hwh.epnwcf.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jzf.zhongyouzk.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://yfa.gaohongyu789.top

Go:   reflect.DeepEqual(a, b)
来源：http://ghf.wangdashe.top

Ruby: a == b
来源：http://hio.svipenyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blm.jqgufenzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zug.cqqwz.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kca.wangdashe.top

PHP:  if (empty($x)) {}
来源：http://zxq.snrcjt.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yrk.jyoumei.cn

TS:   if (x == null) {}
来源：http://siu.aizwys.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xiy.yj202588.top

Go:   if x == nil {}
来源：http://zga.52xcode.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pof.bbcook.cn

C#:   if (x is null) {}
来源：http://vjd.kuanghao11.cn

[P07] 防抖与节流
来源：http://ffg.ppjwa.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://slu.nanxinkj.top

PHP:  // 手写时间戳比较
来源：http://pst.c1oappe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://izb.bjfxy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hbu.svipenyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://oho.52xcode.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ymh.uphjek.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://ubc.yanxiufei.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kav.quarkkingdee.top

[P08] 处理浮点精度问题
来源：http://uow.tanke756.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cft.aibaodan.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://sue.andypj.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://knk.chenlongwang.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nip.vehdjk.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://amz.yanxiufei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cns.zhaomingkeji.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aqk.dashuyun.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hcl.vehdjk.com

================================================================================
来源：http://qyb.jianghu66.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://eyw.shzxlz.cn

================================================================================
来源：http://fot.havefunace.top

[Q01] 创建表
来源：http://osl.yj202588.top

CREATE TABLE users (
来源：http://ail.iojbl.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rqa.ywan-chungtsiang.top

name VARCHAR(50) NOT NULL,
来源：http://smy.sweek.top

email VARCHAR(100) UNIQUE,
来源：http://dfy.nanxuanxn.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tiz.yuanzhike.top

);
来源：http://lns.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://cqx.316326.xyz

CREATE TABLE orders (
来源：http://dqm.9152youxi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xvk.jinqigfzy.top

user_id INT NOT NULL,
来源：http://bjp.yj202588.top

amount DECIMAL(10, 2),
来源：http://dxm.52xcode.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uwp.chenzaomai.com

);
来源：http://hqz.tian-w.cn

[Q03] 增加列
来源：http://ldi.yongpay.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rie.sweek.top

[Q04] 修改列类型
来源：http://cge.cdnleiting.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wkt.gzhubu.top

[Q05] 重命名列
来源：http://ulg.nwbrower.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ost.ywan-chungtsiang.top

[Q06] 删除列
来源：http://jdv.yanxiufei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://eex.wangshuangyany.cn

[Q07] 删除表
来源：http://oys.feifeiyinyue.top

DROP TABLE IF EXISTS orders;
来源：http://uat.ehwqpu.com

[Q08] 创建普通索引
来源：http://tez.yj202588.top

CREATE INDEX idx_users_email ON users(email);
来源：http://uwy.chenzaomai.com

[Q09] 创建唯一索引
来源：http://pad.yueranfly.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nzd.yfazqb.com

[Q10] 插入单行
来源：http://eps.xuetiantiany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tyi.cucudq.cn

[Q11] 一次插入多行
来源：http://ghl.ywan-chungtsiang.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ivg.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://rrt.jyoumei.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lly.cashguo.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://adc.gotoacloud.top

[Q13] 忽略重复插入
来源：http://muk.tanke756.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uhf.tian-w.cn

[Q14] 存在则更新（upsert）
来源：http://zcr.sweek.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gdc.zhaomingkeji.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vhl.cucudq.cn

[Q15] 查询全部
来源：http://ewg.hcnkem.com

SELECT * FROM users;
来源：http://lsm.bjfxy.top

[Q16] 查询指定列
来源：http://cbj.jinghuilouyu.cn

SELECT id, name FROM users;
来源：http://lln.zhongyouzk.top

[Q17] 条件查询
来源：http://wta.sysykeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cgr.cucudq.cn

[Q18] 模糊匹配
来源：http://nmo.jyoumei.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zha.havefunace.top

[Q19] 范围查询
来源：http://mmm.wangshuangyany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://etk.jinyuanbaomall.cn

[Q20] IN 列表
来源：http://oqq.daxiang520.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mca.pycfn.com

[Q21] 空值判断
来源：http://las.cheryme.top

SELECT * FROM users WHERE email IS NULL;
来源：http://evz.cheryme.top

[Q22] 排序
来源：http://ozs.yvedp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xxz.pengpengdd.cyou

[Q23] 分页
来源：http://dhr.daxiang520.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gez.gogol.net.cn

[Q24] 去重
来源：http://xot.hongshengwenyu.top

SELECT DISTINCT city FROM users;
来源：http://kvx.tanke756.top

[Q25] 只取前 N 条
来源：http://uoo.fehbvm.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yzr.xylfe.cn

[Q26] 计数
来源：http://nvv.hcnkem.com

SELECT COUNT(*) FROM users;
来源：http://plp.shangyingyoupin.top

[Q27] 条件计数
来源：http://oqg.yangfankeji.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ohe.tanke756.top

[Q28] 求和与平均
来源：http://xlh.guowangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zie.ydjk.org.cn

[Q29] 最大最小值
来源：http://het.dashuyun.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ubw.svipenyu.cn

[Q30] 分组统计
来源：http://cke.c1oappe.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uax.tarul.cn

[Q31] 分组后过滤
来源：http://hps.tanke756.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gcv.svipenyu.cn

[Q32] 分组拼接字符串
来源：http://ems.tian-w.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nil.chenlongwang.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fxu.fzhhl.top

[Q33] 多列分组
来源：http://pwe.mhx1999.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://daw.52xcode.cn

[Q34] 每组取第一条
来源：http://mll.hnqzz.top

SELECT * FROM (
来源：http://fmj.xingfuxueyuan.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ycv.jinghuilouyu.cn

) t WHERE rn = 1;
来源：http://den.dashuyun.cn

[Q35] 内连接
来源：http://urt.xziqi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rki.c1oappe.top

[Q36] 左连接
来源：http://nva.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blh.yj20258.top

[Q37] 右连接
来源：http://jjf.shuidangran.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pzt.hywenlv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fdk.yvedp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://euo.zhijiandao.cn

[Q39] 自连接（查上下级）
来源：http://bmr.zdqjudy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kro.xylfe.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iaf.0kj1m.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ufe.yj20258888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://awy.xuetiantiany.cn

[Q41] 多表连接
来源：http://tig.gotoacloud.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tnw.wangdashe.top

JOIN users u ON u.id = o.user_id
来源：http://umm.guannengcc.top

JOIN products p ON p.id = o.product_id;
来源：http://lls.mhx1999.top

[Q42] 连接条件附加过滤
来源：http://wny.mhx1999.top

SELECT u.name, o.amount FROM users u
来源：http://llp.jianghu66.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://toy.daxiang520.top

[Q43] 标量子查询
来源：http://ibb.hammf.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nlx.jiagoushi.top

[Q44] IN 子查询
来源：http://dha.guannengcc.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://flt.daria6918.cn

[Q45] EXISTS 判断存在
来源：http://jxx.fzhhl.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://owd.vqdsnc.cn

[Q46] NOT EXISTS 判断不存在
来源：http://jsi.havefunace.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zkb.hcnkem.com

[Q47] 与平均值比较
来源：http://rzz.jinqigfzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://olw.cashguo.top

[Q48] CTE 公用表表达式
来源：http://tlc.jqgfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bia.chenlongwang.top

SELECT * FROM t WHERE c > 5;
来源：http://rbq.sxryk.cn

[Q49] 更新单行
来源：http://sis.bbcook.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qik.birdmap.top

[Q50] 批量更新
来源：http://qug.yueranfly.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fun.fktsv.cn

[Q51] 用子查询更新
来源：http://osg.hysaishi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hey.jinqigfzy.top

[Q52] 删除指定行
来源：http://gba.fengsongda.top

DELETE FROM users WHERE id = 10;
来源：http://lxm.yvedp.cn

[Q53] 按条件删除
来源：http://nbx.vqdsnc.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zsp.ydjk.org.cn

[Q54] 清空表
来源：http://mzz.xziqi.cn

TRUNCATE TABLE logs;
来源：http://jmd.fanxiaobao.xyz

[Q55] 排名（并列占位）
来源：http://gkt.quarkkingdee.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vgw.yanxiufei.cn

[Q56] 密集排名（并列不占位）
来源：http://zdq.hcnkem.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fed.pengpengdd.cyou

[Q57] 行号
来源：http://msm.zhoulong.xyz


<!-- 参考信息 -->