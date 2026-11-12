代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://evi.xziqi.cn

[N10] 链表节点定义
来源：http://bnh.hnxiangtu.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://aki.yfazqb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://eix.yonumen.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nti.ydjk.org.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://csu.jinghuilouyu.cn

Java: class Node { int v; Node next; }
来源：http://jvl.hnxiangtu.top

Go:   type Node struct { V int; Next *Node }
来源：http://avt.kuanghao11.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://ffw.jianghu66.top

C#:   class Node { public int V; public Node? Next; }
来源：http://sqg.chenjidiqi.icu

[N11] 二叉树中序遍历
来源：http://avj.shzxlz.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wdd.mhx1999.top

PHP:  // 手写递归函数
来源：http://ute.yangfankeji.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nnx.tanke756.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xjn.xingfuxueyuan.xyz

Java: // 手写递归
来源：http://vvr.zhixingplan.top

Go:   // 手写递归
来源：http://ltj.pengpengdd.cyou

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xfd.smart0.xyz

C#:   // 手写递归
来源：http://yze.zhoulong.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wav.tianlin.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blm.uphjek.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cgu.uphjek.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uky.zhoulong.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://scq.epnwcf.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dmm.bjfxy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://osz.zhijiandao.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://iox.yonumen.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dxm.vehdjk.com

================================================================================
来源：http://mrj.cucudq.cn

O. 并发与异步
来源：http://cpt.xingfuxueyuan.xyz

================================================================================
来源：http://bnw.cucudq.cn

[O01] 启动一个线程
来源：http://ytj.cdnleiting.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sxt.ywan-chungtsiang.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zpi.hywenlv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qih.yueranfly.top

TS:   // 同 JS
来源：http://vxh.ppjwa.cn

Java: new Thread(() -> f()).start()
来源：http://dmr.ctjpmb.com

Go:   go f()
来源：http://hqs.tian-w.cn

Ruby: Thread.new { f }
来源：http://mbl.pycfn.com

C#:   Task.Run(() => F());
来源：http://udl.jlsjyb.cn

[O02] 使用线程池
来源：http://xfr.gzhubu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://oxt.hammf.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xue.jinyuanbaomall.cn

JS:   // worker_threads 线程池
来源：http://ezw.yj20258.top

TS:   // worker_threads 线程池
来源：http://jex.andypj.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://yzt.hnxiangtu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nmy.316326.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zxc.guowangkeji.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ymf.cqqwz.cn

[O03] 加锁保护共享数据
来源：http://wmm.ywan-chungtsiang.top

Py:   with lock: shared += 1
来源：http://lnx.chenlongwang.top

PHP:  // 用 flock() 做文件锁
来源：http://fst.jqgfzy.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mhs.xuanzx.com

TS:   // 同 JS
来源：http://zae.chenjidiqi.icu

Java: synchronized (this) { shared++; }
来源：http://qwj.fehbvm.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zmy.0kj1m.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://wur.hcnkem.com

C#:   lock (gate) { shared++; }
来源：http://isb.jinghuilouyu.cn

[O04] 定义异步函数并等待
来源：http://zkf.gotoacloud.top

Py:   async def f():⏎    await g()
来源：http://nae.wangdashe.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gca.tianlin.xyz

JS:   async function f() { await g(); }
来源：http://fmk.fengsongda.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qhy.daria6918.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yvv.ybcxt.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fzl.daria6918.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zhu.tanke756.top

C#:   async Task F() { await G(); }
来源：http://rom.xylfe.cn

[O05] 并发执行并等待全部完成
来源：http://dbr.zdqjudy.top

Py:   asyncio.gather(*tasks)
来源：http://imp.ppjwa.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nxd.316326.xyz

JS:   await Promise.all(tasks)
来源：http://psm.yangfankeji.com

TS:   await Promise.all(tasks)
来源：http://ech.shanyushiyangtech.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qoj.yvedp.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fef.cashguo.top

Ruby: threads.map(&:join)
来源：http://zgm.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qwh.uphjek.com

[O06] 使用进程池
来源：http://gkl.gogol.net.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lfp.ywan-chungtsiang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://yei.zhoulong.xyz

JS:   // child_process / cluster 模块
来源：http://jex.uphjek.com

TS:   // child_process / cluster 模块
来源：http://hgw.yfazqb.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lpu.nanxuanxn.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pxo.zdqjudy.top

Ruby: // fork 块
来源：http://bvy.feifeiyinyue.top

C#:   Parallel.For
来源：http://qyp.zhixingplan.top

================================================================================
来源：http://nxn.xziqi.cn

P. 常用工具函数
来源：http://tfn.hysaishi.cn

================================================================================
来源：http://lrp.daxiang520.top

[P01] 生成 UUID
来源：http://loj.meibo888.top

Py:   str(uuid.uuid4())
来源：http://lxi.yfazqb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://icf.gzhubu.top

JS:   crypto.randomUUID()
来源：http://pdp.zhaomingkeji.xyz

TS:   crypto.randomUUID()
来源：http://yko.hammf.cn

Java: UUID.randomUUID().toString()
来源：http://sfy.sysykeji.top

Go:   // 用 github.com/google/uuid
来源：http://hik.feifeiyinyue.top

Ruby: SecureRandom.uuid
来源：http://duz.kuanghao11.cn

C#:   Guid.NewGuid().ToString()
来源：http://leb.jinyuanbaomall.cn

[P02] MD5 / SHA256 摘要
来源：http://jmp.tanke756.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dyv.nanxuanxn.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wjl.52xcode.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wzf.aibaodan.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sgw.zhengqikj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kny.bbcook.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yxl.gogol.net.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oir.shzxlz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fub.jinqigufen.top

[P03] 生成短随机字符串
来源：http://xuy.uphjek.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oea.zhixingplan.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jra.316326.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yuv.jinghuilouyu.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cvz.sufxvd.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gum.yvedp.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vlu.bjfxy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://oic.bjfxy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zrq.mhx1999.top

[P04] 求长度
来源：http://lqs.guowangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tlu.zhaomingkeji.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gyv.jyoumei.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wsc.hammf.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tkk.xuanzx.com

Java: list.size();  map.size();  s.length()
来源：http://nfp.haohaochexian.top

Go:   len(arr);  len(m)
来源：http://pcw.pycfn.com

Ruby: x.length;  x.size
来源：http://frl.shangyingyoupin.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zqn.quarkkingdee.top

[P05] 判断两个对象内容是否相等
来源：http://lkb.zhixingplan.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://myf.tianlin.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bjm.ctjpmb.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fvr.iojbl.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ewi.yvedp.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://khx.zhiwuduotai.top

Go:   reflect.DeepEqual(a, b)
来源：http://efw.tian-w.cn

Ruby: a == b
来源：http://pej.jinqigfzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rla.ydjk.org.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ein.xylfe.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ksr.tian-w.cn

PHP:  if (empty($x)) {}
来源：http://lvt.daria6918.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vsl.chenjidiqi.icu

TS:   if (x == null) {}
来源：http://dqu.quarkkingdee.top

Java: if (x == null || x.isEmpty()) {}
来源：http://yzq.gogol.net.cn

Go:   if x == nil {}
来源：http://ucf.fehbvm.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ikf.gotoacloud.top

C#:   if (x is null) {}
来源：http://nlr.tarul.cn

[P07] 防抖与节流
来源：http://ais.316326.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lkm.aibaodan.cn

PHP:  // 手写时间戳比较
来源：http://udt.jlsjyb.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pgi.yj20258888.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jmn.9152youxi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qti.shuidangran.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pie.0kj1m.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tut.uphjek.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dep.yangfankeji.com

[P08] 处理浮点精度问题
来源：http://ikk.mhx1999.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lwu.tanke756.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dof.sjlbkw.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qbv.gaohongyu789.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://yrf.xylfe.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yst.xinyue.icu

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qfn.yangfankeji.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hxr.aibaodan.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ihi.zhixingplan.top

================================================================================
来源：http://yjx.cucudq.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ubh.316326.xyz

================================================================================
来源：http://bpy.xuetiantiany.cn

[Q01] 创建表
来源：http://qra.cqqwz.cn

CREATE TABLE users (
来源：http://fqu.cashguo.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dcg.tanke756.top

name VARCHAR(50) NOT NULL,
来源：http://wbd.yuanzhike.top

email VARCHAR(100) UNIQUE,
来源：http://jna.jianghu66.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yvg.havefunace.top

);
来源：http://zkz.zhijiandao.cn

[Q02] 创建带外键的表
来源：http://jbr.jianghu66.top

CREATE TABLE orders (
来源：http://bkr.ppjwa.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rfe.yuanzhike.top

user_id INT NOT NULL,
来源：http://fhd.birdmap.top

amount DECIMAL(10, 2),
来源：http://atm.daxiang520.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://eoi.ybcxt.top

);
来源：http://cni.zhoulong.xyz

[Q03] 增加列
来源：http://qiu.yuxming.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://dxv.wangshuangyany.cn

[Q04] 修改列类型
来源：http://pli.uphjek.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qtl.zhixingplan.top

[Q05] 重命名列
来源：http://jlu.shanyushiyangkeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kjy.yueranfly.top

[Q06] 删除列
来源：http://exo.yanxiufei.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kgn.yongpay.top

[Q07] 删除表
来源：http://bns.cashguo.top

DROP TABLE IF EXISTS orders;
来源：http://lwj.jinqigfzy.top

[Q08] 创建普通索引
来源：http://dcr.ivvv.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gsg.ehwqpu.com

[Q09] 创建唯一索引
来源：http://jro.zhiwuduotai.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ghw.hongshengwenyu.top

[Q10] 插入单行
来源：http://zgh.xylfe.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://slp.quarkkingdee.top

[Q11] 一次插入多行
来源：http://nrn.xuanzx.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hli.fanxiaobao.xyz

[Q12] 插入后取自增 ID
来源：http://dtk.yj20258.top

INSERT INTO users (name) VALUES ('C');
来源：http://icm.jinghuilouyu.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cft.xziqi.cn

[Q13] 忽略重复插入
来源：http://osp.ydzc1.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wno.zhengqikj.top

[Q14] 存在则更新（upsert）
来源：http://zva.andypj.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rzn.uphjek.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ctj.ehwqpu.com

[Q15] 查询全部
来源：http://zuo.gotoacloud.top

SELECT * FROM users;
来源：http://cbc.snrcjt.cn

[Q16] 查询指定列
来源：http://aag.zycfv.cn

SELECT id, name FROM users;
来源：http://nwf.cheryme.top

[Q17] 条件查询
来源：http://iuv.jiagoushi.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nmj.yj20258888.top

[Q18] 模糊匹配
来源：http://rqd.316326.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fqr.mhx1999.top

[Q19] 范围查询
来源：http://iov.quarkkingdee.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ckx.yonumen.top

[Q20] IN 列表
来源：http://qbk.hesvh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xch.nanxuanxn.top

[Q21] 空值判断
来源：http://qxf.kuanghao11.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://jjn.xuetiantiany.cn

[Q22] 排序
来源：http://kxu.tanke756.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://spn.dianchejie.cn

[Q23] 分页
来源：http://suf.chenjidiqi.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://leh.wangshuangyany.cn

[Q24] 去重
来源：http://huu.snrcjt.cn

SELECT DISTINCT city FROM users;
来源：http://xlt.yuanzhike.top

[Q25] 只取前 N 条
来源：http://tey.hcnkem.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://emw.andypj.xyz

[Q26] 计数
来源：http://gll.xuanzx.com

SELECT COUNT(*) FROM users;
来源：http://lyt.hnqzz.top

[Q27] 条件计数
来源：http://dmd.xingfuxueyuan.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gyg.hammf.cn

[Q28] 求和与平均
来源：http://xzq.quarkkingdee.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bwf.epnwcf.com

[Q29] 最大最小值
来源：http://cwu.iojbl.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cui.xuanzx.com

[Q30] 分组统计
来源：http://nml.yuanzhike.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dmc.aibaodan.cn

[Q31] 分组后过滤
来源：http://xqp.gogol.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fnj.fktsv.cn

[Q32] 分组拼接字符串
来源：http://bws.c1oappe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://egw.tian-w.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ssk.hfpthk.cn

[Q33] 多列分组
来源：http://dbb.nwbrower.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rom.zdqjudy.top

[Q34] 每组取第一条
来源：http://gaz.shangyingyoupin.top

SELECT * FROM (
来源：http://caa.tianlin.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ugv.xuetiantiany.cn

) t WHERE rn = 1;
来源：http://crp.havefunace.top

[Q35] 内连接
来源：http://uio.gaohongyu789.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tau.zdbjq.cn

[Q36] 左连接
来源：http://agp.wangdashe.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ulz.iojbl.cn

[Q37] 右连接
来源：http://mpb.xingfuxueyuan.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cjw.hnqzz.top

[Q38] 全外连接（PostgreSQL）
来源：http://ruy.bjfxy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pxe.jianghu66.top

[Q39] 自连接（查上下级）
来源：http://ryv.hongshengwenyu.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://apa.guannengcc.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qzi.yj20258.top

[Q40] 交叉连接（笛卡尔积）
来源：http://eku.hongshengwenyu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mmj.birdmap.top

[Q41] 多表连接
来源：http://htt.zhengqikj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://lli.zhixingplan.top

JOIN users u ON u.id = o.user_id
来源：http://vbk.zhoulong.xyz

JOIN products p ON p.id = o.product_id;
来源：http://gti.jiagoushi.top

[Q42] 连接条件附加过滤
来源：http://wll.fktsv.cn

SELECT u.name, o.amount FROM users u
来源：http://guk.smart0.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nyx.shanyushiyangkeji.top

[Q43] 标量子查询
来源：http://pqu.ydjk.org.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rie.hesvh.cn

[Q44] IN 子查询
来源：http://btt.ybcxt.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gig.jqgfzy.top

[Q45] EXISTS 判断存在
来源：http://qpp.sufxvd.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qqs.iojbl.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cht.hywenlv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oks.sxryk.cn

[Q47] 与平均值比较
来源：http://aaf.fehbvm.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wju.xuetiantiany.cn

[Q48] CTE 公用表表达式
来源：http://bcq.jiagoushi.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zmx.nanxinkj.top

SELECT * FROM t WHERE c > 5;
来源：http://lrc.cheryme.top

[Q49] 更新单行
来源：http://oxw.jinqigufen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wxi.meibo888.top

[Q50] 批量更新
来源：http://vws.xinyue.icu

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nnb.yj20258888.top

[Q51] 用子查询更新
来源：http://kpu.hysaishi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bbj.xinyue.icu

[Q52] 删除指定行
来源：http://fwr.cqqwz.cn

DELETE FROM users WHERE id = 10;
来源：http://xhi.cheryme.top

[Q53] 按条件删除
来源：http://mmp.zhaomingkeji.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tqj.sweek.top

[Q54] 清空表
来源：http://ayw.cheryme.top

TRUNCATE TABLE logs;
来源：http://umt.zhixingplan.top

[Q55] 排名（并列占位）
来源：http://cyd.tian-w.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dbx.0kj1m.cn

[Q56] 密集排名（并列不占位）
来源：http://ibz.ctjpmb.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hrc.tarul.cn

[Q57] 行号
来源：http://iyt.c1oappe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cvl.wangshuangyany.cn

[Q58] 累计求和
来源：http://fbb.hcnkem.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hdv.xinyue.icu

[Q59] 分组内累计
来源：http://wza.sysykeji.top


<!-- 参考信息 -->