代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dpn.cdnleiting.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://qvk.9152youxi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eio.zhongyouzk.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://evr.jinghuilouyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://qjv.shanyushiyangtech.top

[N10] 链表节点定义
来源：http://hqm.hnxiangtu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://ibk.c1oappe.top

PHP:  class Node { public $v; public $next = null; }
来源：http://ejf.fehbvm.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qzx.ybcxt.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://gkm.daxiang520.top

Java: class Node { int v; Node next; }
来源：http://xtq.fehbvm.com

Go:   type Node struct { V int; Next *Node }
来源：http://uzh.tarul.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://wki.sufxvd.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://kvx.feifeiyinyue.top

[N11] 二叉树中序遍历
来源：http://nea.yueranfly.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://bcw.xuanzx.com

PHP:  // 手写递归函数
来源：http://uyn.0kj1m.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ykd.jianghu66.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hum.bjfxy.top

Java: // 手写递归
来源：http://dly.gaohongyu789.top

Go:   // 手写递归
来源：http://iui.daria6918.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://vtc.iojbl.cn

C#:   // 手写递归
来源：http://xpv.shzxlz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://udk.tanke756.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nwx.yj20258.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bdp.shanyushiyangkeji.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zcs.birdmap.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nre.tarul.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wtz.epnwcf.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wtb.gogol.net.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://but.yanxiufei.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://gck.hcnkem.com

================================================================================
来源：http://jqw.daria6918.cn

O. 并发与异步
来源：http://ozs.cqqwz.cn

================================================================================
来源：http://tkz.jqgfzy.top

[O01] 启动一个线程
来源：http://zoa.ybcxt.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ezk.haohaochexian.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jwf.zhixingplan.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nqk.gogol.net.cn

TS:   // 同 JS
来源：http://sfw.andypj.xyz

Java: new Thread(() -> f()).start()
来源：http://rrn.zhaomingkeji.xyz

Go:   go f()
来源：http://rkv.dianchejie.cn

Ruby: Thread.new { f }
来源：http://vwg.yanxiufei.cn

C#:   Task.Run(() => F());
来源：http://vki.gaohongyu789.top

[O02] 使用线程池
来源：http://rhl.hesvh.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uuw.meibo888.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jeb.xingfuxueyuan.xyz

JS:   // worker_threads 线程池
来源：http://dyj.haohaochexian.top

TS:   // worker_threads 线程池
来源：http://ugh.sxryk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pft.svipenyu.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nny.xingfuxueyuan.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://jaz.epnwcf.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://pqt.xuetiantiany.cn

[O03] 加锁保护共享数据
来源：http://ifz.sxryk.cn

Py:   with lock: shared += 1
来源：http://roh.ivvv.top

PHP:  // 用 flock() 做文件锁
来源：http://bai.andypj.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://oxq.feifeiyinyue.top

TS:   // 同 JS
来源：http://ezc.yj20258.top

Java: synchronized (this) { shared++; }
来源：http://knh.zhijiandao.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://geu.xylfe.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://cei.tian-w.cn

C#:   lock (gate) { shared++; }
来源：http://tht.iojbl.cn

[O04] 定义异步函数并等待
来源：http://uak.ehwqpu.com

Py:   async def f():⏎    await g()
来源：http://pkl.birdmap.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lvy.ppjwa.cn

JS:   async function f() { await g(); }
来源：http://ede.jqgufenzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qnw.daxiang520.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oat.zhongyouzk.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fjf.yangfankeji.com

Ruby: # 用 Fiber 或 async gem
来源：http://naq.ehwqpu.com

C#:   async Task F() { await G(); }
来源：http://yfa.xuanzx.com

[O05] 并发执行并等待全部完成
来源：http://qrb.hnqzz.top

Py:   asyncio.gather(*tasks)
来源：http://dos.bjfxy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://opc.chenlongwang.top

JS:   await Promise.all(tasks)
来源：http://lgh.zdbjq.cn

TS:   await Promise.all(tasks)
来源：http://dfx.jinyuanbaomall.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gng.zhongyouzk.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pka.iojbl.cn

Ruby: threads.map(&:join)
来源：http://ylp.cdnleiting.top

C#:   await Task.WhenAll(t1, t2)
来源：http://orm.nanxuanxn.top

[O06] 使用进程池
来源：http://dmr.yangfankeji.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vck.ctjpmb.com

PHP:  // pcntl_fork 或多进程队列
来源：http://yvb.wangdashe.top

JS:   // child_process / cluster 模块
来源：http://siy.tarul.cn

TS:   // child_process / cluster 模块
来源：http://nay.gotoacloud.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bof.cdnleiting.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cvo.fzhhl.top

Ruby: // fork 块
来源：http://cml.chenzaomai.com

C#:   Parallel.For
来源：http://xyt.ppjwa.cn

================================================================================
来源：http://fwt.zhixingplan.top

P. 常用工具函数
来源：http://fej.sweek.top

================================================================================
来源：http://grv.ybcxt.top

[P01] 生成 UUID
来源：http://jdn.gaohongyu789.top

Py:   str(uuid.uuid4())
来源：http://cir.cheryme.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lgn.shanyushiyangkeji.top

JS:   crypto.randomUUID()
来源：http://wpe.jinqigufen.top

TS:   crypto.randomUUID()
来源：http://xmc.uphjek.com

Java: UUID.randomUUID().toString()
来源：http://myq.c1oappe.top

Go:   // 用 github.com/google/uuid
来源：http://gjq.tian-w.cn

Ruby: SecureRandom.uuid
来源：http://flw.chenlongwang.top

C#:   Guid.NewGuid().ToString()
来源：http://itw.yonumen.top

[P02] MD5 / SHA256 摘要
来源：http://dah.ivvv.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xil.nwbrower.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zhj.bbcook.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://myi.sxryk.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://aar.wangshuangyany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bwt.zhoulong.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fgu.jinqigufen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jqn.xinyue.icu

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://skk.cdnleiting.top

[P03] 生成短随机字符串
来源：http://tbn.wangshuangyany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lby.zhiwuduotai.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cth.svipenyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vpe.yj202588.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://flt.wangdashe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fet.tanke756.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iig.tarul.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rlv.pengpengdd.cyou

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ids.cqqwz.cn

[P04] 求长度
来源：http://qsg.vehdjk.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ooh.ybcxt.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iwo.nanxinkj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lfo.jiagoushi.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://una.jianghu66.top

Java: list.size();  map.size();  s.length()
来源：http://xus.zhaomingkeji.xyz

Go:   len(arr);  len(m)
来源：http://qhb.tian-w.cn

Ruby: x.length;  x.size
来源：http://ros.fanxiaobao.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://dvq.haohaochexian.top

[P05] 判断两个对象内容是否相等
来源：http://haw.kuanghao11.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wxq.smart0.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hpd.hywenlv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yly.zdbjq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://aog.sxryk.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jqa.yuxming.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fkg.tian-w.cn

Ruby: a == b
来源：http://lhv.yj20258888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://the.hnxiangtu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zox.sysykeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xgs.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}
来源：http://age.zhoulong.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oxh.guowangkeji.top

TS:   if (x == null) {}
来源：http://ldx.zhijiandao.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kig.cheryme.top

Go:   if x == nil {}
来源：http://ene.jianghu66.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hbw.jinyuanbaomall.cn

C#:   if (x is null) {}
来源：http://cju.zdbjq.cn

[P07] 防抖与节流
来源：http://upr.andypj.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vrg.yfazqb.com

PHP:  // 手写时间戳比较
来源：http://rcq.sjlbkw.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wml.dianchejie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kbk.jinqigfzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://drn.shangyingyoupin.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xcn.cashguo.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wsi.sxryk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ybh.xylfe.cn

[P08] 处理浮点精度问题
来源：http://uqg.52xcode.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ydc.cashguo.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jsa.andypj.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xjz.smart0.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vtx.yj20258888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://aup.yangfankeji.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://chw.ydzc1.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://snc.vehdjk.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ena.andypj.xyz

================================================================================
来源：http://kzh.fzhhl.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bib.shzxlz.cn

================================================================================
来源：http://gjf.c1oappe.top

[Q01] 创建表
来源：http://ckg.9152youxi.cn

CREATE TABLE users (
来源：http://xjx.yonumen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tcp.gotoacloud.top

name VARCHAR(50) NOT NULL,
来源：http://pid.andypj.xyz

email VARCHAR(100) UNIQUE,
来源：http://rtr.zhengqikj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sng.zhengqikj.top

);
来源：http://nfj.chenjidiqi.icu

[Q02] 创建带外键的表
来源：http://fwt.iojbl.cn

CREATE TABLE orders (
来源：http://hwh.dashuyun.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ktp.ybcxt.top

user_id INT NOT NULL,
来源：http://ika.redwolf501.top

amount DECIMAL(10, 2),
来源：http://byf.yj20258888.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ksw.cashguo.top

);
来源：http://zvu.fktsv.cn

[Q03] 增加列
来源：http://vst.pengpengdd.cyou

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vak.kuanghao11.cn

[Q04] 修改列类型
来源：http://fgu.zdqjudy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mbe.guowangkeji.top

[Q05] 重命名列
来源：http://wbe.wangdashe.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jfy.wangshuangyany.cn

[Q06] 删除列
来源：http://sdr.ctjpmb.com

ALTER TABLE users DROP COLUMN age;
来源：http://xvl.ehwqpu.com

[Q07] 删除表
来源：http://ups.vqdsnc.cn

DROP TABLE IF EXISTS orders;
来源：http://eyj.yanxiufei.cn

[Q08] 创建普通索引
来源：http://bvy.yvedp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sxv.ppjwa.cn

[Q09] 创建唯一索引
来源：http://mha.meibo888.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vsk.hywenlv.cn

[Q10] 插入单行
来源：http://mty.ydjk.org.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ylc.jianghu66.top

[Q11] 一次插入多行
来源：http://idc.sufxvd.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wyz.yvedp.cn

[Q12] 插入后取自增 ID
来源：http://due.andypj.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://pxw.guowangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hmy.hfpthk.cn

[Q13] 忽略重复插入
来源：http://zez.tarul.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mdr.hywenlv.cn

[Q14] 存在则更新（upsert）
来源：http://sed.yvedp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hvw.gzhubu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://juq.feifeiyinyue.top

[Q15] 查询全部
来源：http://xgy.hongshengwenyu.top

SELECT * FROM users;
来源：http://sft.vehdjk.com

[Q16] 查询指定列
来源：http://hbe.fzhhl.top

SELECT id, name FROM users;
来源：http://smh.cheryme.top

[Q17] 条件查询
来源：http://rdz.pycfn.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ixu.iojbl.cn

[Q18] 模糊匹配
来源：http://ssu.gotoacloud.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pww.zhixingplan.top

[Q19] 范围查询
来源：http://mck.svipenyu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://itm.mhx1999.top

[Q20] IN 列表
来源：http://azg.jianghu66.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wfr.fanxiaobao.xyz

[Q21] 空值判断
来源：http://rhj.gzhubu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mwl.pengpengdd.cyou

[Q22] 排序
来源：http://gzd.zdbjq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rid.nwbrower.top

[Q23] 分页
来源：http://glp.yueranfly.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tgt.tanke756.top

[Q24] 去重
来源：http://zmy.yj202588.top

SELECT DISTINCT city FROM users;
来源：http://sdc.tanke756.top

[Q25] 只取前 N 条
来源：http://psm.hywenlv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://etv.havefunace.top

[Q26] 计数
来源：http://yne.redwolf501.top

SELECT COUNT(*) FROM users;
来源：http://xor.fanxiaobao.xyz

[Q27] 条件计数
来源：http://xfm.snrcjt.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ivf.fanxiaobao.xyz

[Q28] 求和与平均
来源：http://gox.shzxlz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gpz.hcnkem.com

[Q29] 最大最小值
来源：http://pce.nwbrower.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://zxk.xuanzx.com

[Q30] 分组统计
来源：http://yps.pycfn.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://adj.haohaochexian.top

[Q31] 分组后过滤
来源：http://byt.nanxinkj.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://aoy.aibaodan.cn

[Q32] 分组拼接字符串
来源：http://ppm.nanxuanxn.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ilx.ehwqpu.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sqe.fanxiaobao.xyz

[Q33] 多列分组
来源：http://cmp.gaohongyu789.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://abr.ydzc1.top

[Q34] 每组取第一条
来源：http://alb.fzhhl.top

SELECT * FROM (
来源：http://hiv.ywan-chungtsiang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ntz.yueranfly.top

) t WHERE rn = 1;
来源：http://ojf.shuidangran.top

[Q35] 内连接
来源：http://szf.sxryk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rgv.zhixingplan.top

[Q36] 左连接
来源：http://rdw.snrcjt.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wyl.shanyushiyangkeji.top

[Q37] 右连接
来源：http://mow.cdnleiting.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wrj.sweek.top

[Q38] 全外连接（PostgreSQL）
来源：http://chk.jqgfzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tuc.jqgufenzy.top

[Q39] 自连接（查上下级）
来源：http://xwl.chenjidiqi.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://mvk.wangdashe.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zii.guowangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://fct.ybcxt.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gqo.yongpay.top

[Q41] 多表连接
来源：http://bka.jianghu66.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nnj.hammf.cn

JOIN users u ON u.id = o.user_id
来源：http://ijh.nwbrower.top

JOIN products p ON p.id = o.product_id;
来源：http://xef.cqqwz.cn

[Q42] 连接条件附加过滤
来源：http://wto.zycfv.cn

SELECT u.name, o.amount FROM users u
来源：http://aoz.ybcxt.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jkr.nanxinkj.top

[Q43] 标量子查询
来源：http://tar.xuetiantiany.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iex.316326.xyz

[Q44] IN 子查询
来源：http://kqs.zhoulong.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://veg.tianlin.xyz

[Q45] EXISTS 判断存在
来源：http://hch.hfpthk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://llz.chenzaomai.com

[Q46] NOT EXISTS 判断不存在
来源：http://edy.redwolf501.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ubk.yfazqb.com

[Q47] 与平均值比较
来源：http://hug.ctjpmb.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mtw.tian-w.cn

[Q48] CTE 公用表表达式
来源：http://jdb.sufxvd.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xsh.meibo888.top

SELECT * FROM t WHERE c > 5;
来源：http://hyv.gzhubu.top

[Q49] 更新单行
来源：http://iaa.chenlongwang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dqq.gotoacloud.top

[Q50] 批量更新
来源：http://trv.svipenyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fgv.fanxiaobao.xyz

[Q51] 用子查询更新
来源：http://orh.chenzaomai.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jpw.cheryme.top

[Q52] 删除指定行
来源：http://ihv.zhoulong.xyz

DELETE FROM users WHERE id = 10;
来源：http://tpc.sxryk.cn

[Q53] 按条件删除
来源：http://web.ydjk.org.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dqm.shangyingyoupin.top

[Q54] 清空表
来源：http://gju.feifeiyinyue.top

TRUNCATE TABLE logs;
来源：http://pen.yueranfly.top

[Q55] 排名（并列占位）
来源：http://wky.aibaodan.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aed.zhaomingkeji.xyz

[Q56] 密集排名（并列不占位）
来源：http://gnr.pycfn.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hhi.tian-w.cn

[Q57] 行号
来源：http://mac.birdmap.top


<!-- 参考信息 -->