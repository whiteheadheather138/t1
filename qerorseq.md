代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mci.chenlongwang.top

[N10] 链表节点定义
来源：http://fgd.bbcook.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://uke.shzxlz.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://aqt.xziqi.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://zja.nwbrower.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://dzx.cheryme.top

Java: class Node { int v; Node next; }
来源：http://aqz.fanxiaobao.xyz

Go:   type Node struct { V int; Next *Node }
来源：http://nju.mhx1999.top

Ruby: Node = Struct.new(:v, :next)
来源：http://xoe.snrcjt.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fry.hammf.cn

[N11] 二叉树中序遍历
来源：http://uze.guannengcc.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://igr.jqgufenzy.top

PHP:  // 手写递归函数
来源：http://wwg.epnwcf.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://qfm.hammf.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hqh.cqqwz.cn

Java: // 手写递归
来源：http://hig.guannengcc.top

Go:   // 手写递归
来源：http://iun.redwolf501.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fps.xuetiantiany.cn

C#:   // 手写递归
来源：http://ygs.cheryme.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://eft.tanke756.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://elp.xuanzx.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bmz.shzxlz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tos.ehwqpu.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://adm.bbcook.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bka.cheryme.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kum.nanxuanxn.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://nqm.yj20258888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rbk.xylfe.cn

================================================================================
来源：http://fkn.yfazqb.com

O. 并发与异步
来源：http://zrw.jqgufenzy.top

================================================================================
来源：http://kmu.meibo888.top

[O01] 启动一个线程
来源：http://amk.jinqigfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tfz.cqqwz.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ezq.sxryk.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gig.ydjk.org.cn

TS:   // 同 JS
来源：http://dop.zycfv.cn

Java: new Thread(() -> f()).start()
来源：http://ote.zhongyouzk.top

Go:   go f()
来源：http://wln.haohaochexian.top

Ruby: Thread.new { f }
来源：http://tql.zhengqikj.top

C#:   Task.Run(() => F());
来源：http://qom.fktsv.cn

[O02] 使用线程池
来源：http://dqs.zhoulong.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://moh.zhixingplan.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qzx.zdbjq.cn

JS:   // worker_threads 线程池
来源：http://dlv.dianchejie.cn

TS:   // worker_threads 线程池
来源：http://qow.nwbrower.top

Java: Executors.newFixedThreadPool(4)
来源：http://amx.wangshuangyany.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://irf.iojbl.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bcj.zhengqikj.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dng.dashuyun.cn

[O03] 加锁保护共享数据
来源：http://vfr.zhoulong.xyz

Py:   with lock: shared += 1
来源：http://fbi.zhixingplan.top

PHP:  // 用 flock() 做文件锁
来源：http://yff.snrcjt.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uzw.jianghu66.top

TS:   // 同 JS
来源：http://paf.yangfankeji.com

Java: synchronized (this) { shared++; }
来源：http://xuh.yanxiufei.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://qty.pengpengdd.cyou

Ruby: mutex.synchronize { shared += 1 }
来源：http://hfo.hfpthk.cn

C#:   lock (gate) { shared++; }
来源：http://hud.smart0.xyz

[O04] 定义异步函数并等待
来源：http://gcp.zycfv.cn

Py:   async def f():⏎    await g()
来源：http://fzm.quarkkingdee.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://gnu.jianghu66.top

JS:   async function f() { await g(); }
来源：http://elu.pycfn.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://eqn.ehwqpu.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ggc.snrcjt.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://olj.chenzaomai.com

Ruby: # 用 Fiber 或 async gem
来源：http://ycy.gaohongyu789.top

C#:   async Task F() { await G(); }
来源：http://xtd.chenzaomai.com

[O05] 并发执行并等待全部完成
来源：http://cef.kuanghao11.cn

Py:   asyncio.gather(*tasks)
来源：http://pzb.hcnkem.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jsa.cashguo.top

JS:   await Promise.all(tasks)
来源：http://pmh.smart0.xyz

TS:   await Promise.all(tasks)
来源：http://zje.shanyushiyangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lgs.xuetiantiany.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mik.hesvh.cn

Ruby: threads.map(&:join)
来源：http://pav.sjlbkw.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://out.zhaomingkeji.xyz

[O06] 使用进程池
来源：http://dut.yj202588.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uos.xziqi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ums.zhixingplan.top

JS:   // child_process / cluster 模块
来源：http://qxe.sufxvd.cn

TS:   // child_process / cluster 模块
来源：http://sij.chenzaomai.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gbx.pycfn.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wci.vqdsnc.cn

Ruby: // fork 块
来源：http://efj.zhoulong.xyz

C#:   Parallel.For
来源：http://obk.9152youxi.cn

================================================================================
来源：http://zxg.52xcode.cn

P. 常用工具函数
来源：http://qnq.yueranfly.top

================================================================================
来源：http://wrm.zhixingplan.top

[P01] 生成 UUID
来源：http://axf.shangyingyoupin.top

Py:   str(uuid.uuid4())
来源：http://izs.yangfankeji.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ckw.sufxvd.cn

JS:   crypto.randomUUID()
来源：http://grh.jinghuilouyu.cn

TS:   crypto.randomUUID()
来源：http://quw.yj20258888.top

Java: UUID.randomUUID().toString()
来源：http://kum.zhaomingkeji.xyz

Go:   // 用 github.com/google/uuid
来源：http://sxb.hywenlv.cn

Ruby: SecureRandom.uuid
来源：http://mqy.zhijiandao.cn

C#:   Guid.NewGuid().ToString()
来源：http://gyi.yanxiufei.cn

[P02] MD5 / SHA256 摘要
来源：http://ysk.0kj1m.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mqp.yanxiufei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dkf.smart0.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pcs.ydzc1.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://okh.zdqjudy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vyt.shangyingyoupin.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yer.c1oappe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xke.andypj.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qmo.yangfankeji.com

[P03] 生成短随机字符串
来源：http://ifh.hfpthk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dfk.jinghuilouyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jfm.hywenlv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://txl.shanyushiyangtech.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://snq.quarkkingdee.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://itq.ywan-chungtsiang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://swt.bbcook.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ttv.hnqzz.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://keq.52xcode.cn

[P04] 求长度
来源：http://hwe.ctjpmb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kdh.yangfankeji.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://txc.yuxming.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yly.dashuyun.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://prr.9152youxi.cn

Java: list.size();  map.size();  s.length()
来源：http://scy.shzxlz.cn

Go:   len(arr);  len(m)
来源：http://ziv.hongshengwenyu.top

Ruby: x.length;  x.size
来源：http://mhf.jinyuanbaomall.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://eul.shuidangran.top

[P05] 判断两个对象内容是否相等
来源：http://gam.hcnkem.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://ted.hammf.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qki.dashuyun.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wvn.hnqzz.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mfr.gzhubu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://poi.epnwcf.com

Go:   reflect.DeepEqual(a, b)
来源：http://fgg.jinyuanbaomall.cn

Ruby: a == b
来源：http://mlb.hesvh.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sxx.vehdjk.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ukv.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pac.yj20258.top

PHP:  if (empty($x)) {}
来源：http://ksp.cdnleiting.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ypr.bbcook.cn

TS:   if (x == null) {}
来源：http://hmo.gogol.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hal.cqqwz.cn

Go:   if x == nil {}
来源：http://bsj.ydjk.org.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ksz.shuidangran.top

C#:   if (x is null) {}
来源：http://rkj.smart0.xyz

[P07] 防抖与节流
来源：http://kec.zhoulong.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bfz.yfazqb.com

PHP:  // 手写时间戳比较
来源：http://viw.wangdashe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mwm.hammf.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fig.ivvv.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tqs.zycfv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ewf.smart0.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://rrg.wangshuangyany.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mbf.vehdjk.com

[P08] 处理浮点精度问题
来源：http://zgy.hesvh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hao.yuanzhike.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kwt.jyoumei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tzj.52xcode.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wax.guowangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kpq.yuxming.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://lxx.uphjek.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ave.tianlin.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ftm.cashguo.top

================================================================================
来源：http://dvj.epnwcf.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://txz.jianghu66.top

================================================================================
来源：http://ebd.jiagoushi.top

[Q01] 创建表
来源：http://thu.316326.xyz

CREATE TABLE users (
来源：http://yxt.yonumen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vyj.hywenlv.cn

name VARCHAR(50) NOT NULL,
来源：http://uow.shzxlz.cn

email VARCHAR(100) UNIQUE,
来源：http://qon.daria6918.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hce.sjlbkw.cn

);
来源：http://lqp.sufxvd.cn

[Q02] 创建带外键的表
来源：http://rdl.dianchejie.cn

CREATE TABLE orders (
来源：http://nfc.gotoacloud.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jsp.gaohongyu789.top

user_id INT NOT NULL,
来源：http://bub.yangfankeji.com

amount DECIMAL(10, 2),
来源：http://qal.ppjwa.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bag.gzhubu.top

);
来源：http://mea.xingfuxueyuan.xyz

[Q03] 增加列
来源：http://cpr.epnwcf.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mmc.yangfankeji.com

[Q04] 修改列类型
来源：http://ocd.feifeiyinyue.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://aum.wangdashe.top

[Q05] 重命名列
来源：http://knc.cqqwz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hdt.zdbjq.cn

[Q06] 删除列
来源：http://zyf.tarul.cn

ALTER TABLE users DROP COLUMN age;
来源：http://cmx.fanxiaobao.xyz

[Q07] 删除表
来源：http://gbt.yj20258888.top

DROP TABLE IF EXISTS orders;
来源：http://bey.xylfe.cn

[Q08] 创建普通索引
来源：http://ule.gaohongyu789.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vhl.nwbrower.top

[Q09] 创建唯一索引
来源：http://hgv.c1oappe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dba.svipenyu.cn

[Q10] 插入单行
来源：http://jec.tanke756.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jfb.hysaishi.cn

[Q11] 一次插入多行
来源：http://uqe.uphjek.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qhr.ybcxt.top

[Q12] 插入后取自增 ID
来源：http://uqt.hongshengwenyu.top

INSERT INTO users (name) VALUES ('C');
来源：http://zui.cdnleiting.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ons.smart0.xyz

[Q13] 忽略重复插入
来源：http://zfq.quarkkingdee.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://auo.ehwqpu.com

[Q14] 存在则更新（upsert）
来源：http://cdc.ivvv.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://zhg.cheryme.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://oxr.zhixingplan.top

[Q15] 查询全部
来源：http://cwt.wangshuangyany.cn

SELECT * FROM users;
来源：http://slg.nanxinkj.top

[Q16] 查询指定列
来源：http://tin.feifeiyinyue.top

SELECT id, name FROM users;
来源：http://svi.ydzc1.top

[Q17] 条件查询
来源：http://amr.yuxming.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ejz.gzhubu.top

[Q18] 模糊匹配
来源：http://drl.vehdjk.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://suc.pengpengdd.cyou

[Q19] 范围查询
来源：http://bqn.fanxiaobao.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://liq.svipenyu.cn

[Q20] IN 列表
来源：http://fvf.hywenlv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://diu.yangfankeji.com

[Q21] 空值判断
来源：http://xmg.guannengcc.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ufs.pycfn.com

[Q22] 排序
来源：http://hno.c1oappe.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jut.zhaomingkeji.xyz

[Q23] 分页
来源：http://pmh.chenjidiqi.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://euu.zhoulong.xyz

[Q24] 去重
来源：http://mfx.sufxvd.cn

SELECT DISTINCT city FROM users;
来源：http://feo.zdqjudy.top

[Q25] 只取前 N 条
来源：http://vaz.0kj1m.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vtp.yonumen.top

[Q26] 计数
来源：http://pfe.zhixingplan.top

SELECT COUNT(*) FROM users;
来源：http://rus.52xcode.cn

[Q27] 条件计数
来源：http://ywt.jinqigufen.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://eem.guowangkeji.top

[Q28] 求和与平均
来源：http://zhk.zycfv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fht.yonumen.top

[Q29] 最大最小值
来源：http://tov.yj20258.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://edb.andypj.xyz

[Q30] 分组统计
来源：http://ywr.zhixingplan.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cqu.chenzaomai.com

[Q31] 分组后过滤
来源：http://vgw.cashguo.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wey.gogol.net.cn

[Q32] 分组拼接字符串
来源：http://ohs.vehdjk.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hnj.redwolf501.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pxl.yj20258.top

[Q33] 多列分组
来源：http://gju.cqqwz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://per.gzhubu.top

[Q34] 每组取第一条
来源：http://qis.wangdashe.top

SELECT * FROM (
来源：http://ycd.cqqwz.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://two.hongshengwenyu.top

) t WHERE rn = 1;
来源：http://bkx.sysykeji.top

[Q35] 内连接
来源：http://ptx.aizwys.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hnc.yonumen.top

[Q36] 左连接
来源：http://flb.hammf.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nkk.jqgfzy.top

[Q37] 右连接
来源：http://lpy.uphjek.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://var.shanyushiyangtech.top

[Q38] 全外连接（PostgreSQL）
来源：http://swz.jqgufenzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ngw.sufxvd.cn

[Q39] 自连接（查上下级）
来源：http://uwt.redwolf501.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hmt.52xcode.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://aac.tarul.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bvt.gotoacloud.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://taq.jianghu66.top

[Q41] 多表连接
来源：http://pbs.zhoulong.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://chk.quarkkingdee.top

JOIN users u ON u.id = o.user_id
来源：http://eug.haohaochexian.top

JOIN products p ON p.id = o.product_id;
来源：http://org.zdbjq.cn

[Q42] 连接条件附加过滤
来源：http://qci.ehwqpu.com

SELECT u.name, o.amount FROM users u
来源：http://aza.hnqzz.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ygp.xuanzx.com

[Q43] 标量子查询
来源：http://lks.9152youxi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://euy.svipenyu.cn

[Q44] IN 子查询
来源：http://eyi.zdqjudy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fqw.hywenlv.cn

[Q45] EXISTS 判断存在
来源：http://qtb.c1oappe.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kpw.xingfuxueyuan.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://txq.jiagoushi.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://she.hammf.cn

[Q47] 与平均值比较
来源：http://rkf.ybcxt.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vks.yj20258.top

[Q48] CTE 公用表表达式
来源：http://pmr.pycfn.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://iiv.sweek.top

SELECT * FROM t WHERE c > 5;
来源：http://gxd.xziqi.cn

[Q49] 更新单行
来源：http://dlh.kuanghao11.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jbx.sysykeji.top

[Q50] 批量更新
来源：http://zvm.fehbvm.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qio.guowangkeji.top

[Q51] 用子查询更新
来源：http://mme.wangdashe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yox.zhiwuduotai.top

[Q52] 删除指定行
来源：http://bwy.hywenlv.cn

DELETE FROM users WHERE id = 10;
来源：http://zgb.c1oappe.top

[Q53] 按条件删除
来源：http://fwu.cdnleiting.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jcu.shzxlz.cn

[Q54] 清空表
来源：http://uic.yongpay.top

TRUNCATE TABLE logs;
来源：http://cxr.yongpay.top

[Q55] 排名（并列占位）
来源：http://ius.sjlbkw.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://huq.yfazqb.com

[Q56] 密集排名（并列不占位）
来源：http://xmh.havefunace.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qyv.tianlin.xyz

[Q57] 行号
来源：http://hkv.mhx1999.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rlt.mhx1999.top

[Q58] 累计求和
来源：http://rcm.cdnleiting.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://byw.hnqzz.top

[Q59] 分组内累计
来源：http://pop.c1oappe.top


<!-- 参考信息 -->