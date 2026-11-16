代发 wailian999

TS:   arr.push(x) / arr.pop() 作栈
来源：http://fpp.hysaishi.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://grb.tanke756.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://int.sufxvd.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zhz.svipenyu.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://nfa.yvedp.cn

[N10] 链表节点定义
来源：http://sxm.jinghuilouyu.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wph.uphjek.com

PHP:  class Node { public $v; public $next = null; }
来源：http://zss.haohaochexian.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://suq.shangyingyoupin.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ojc.smart0.xyz

Java: class Node { int v; Node next; }
来源：http://hbx.jinqigufen.top

Go:   type Node struct { V int; Next *Node }
来源：http://tti.hesvh.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://nlm.ctjpmb.com

C#:   class Node { public int V; public Node? Next; }
来源：http://hmu.daxiang520.top

[N11] 二叉树中序遍历
来源：http://lgs.xziqi.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://yeb.zhijiandao.cn

PHP:  // 手写递归函数
来源：http://gua.nwbrower.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gvz.shanyushiyangtech.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jwq.shangyingyoupin.top

Java: // 手写递归
来源：http://lan.dashuyun.cn

Go:   // 手写递归
来源：http://rth.vqdsnc.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bwd.jianghu66.top

C#:   // 手写递归
来源：http://ems.ctjpmb.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://xib.hysaishi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://hgq.chenlongwang.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ycf.hnxiangtu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rek.jinqigufen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wya.epnwcf.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://acs.zhaomingkeji.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mus.fktsv.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://zvv.tianlin.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ref.yj202588.top

================================================================================
来源：http://jqt.c1oappe.top

O. 并发与异步
来源：http://fxe.fehbvm.com

================================================================================
来源：http://pdi.yuxming.cn

[O01] 启动一个线程
来源：http://apj.yonumen.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vsx.shanyushiyangtech.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vpk.havefunace.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://sgs.yuxming.cn

TS:   // 同 JS
来源：http://eto.cheryme.top

Java: new Thread(() -> f()).start()
来源：http://loz.jqgufenzy.top

Go:   go f()
来源：http://iiv.hammf.cn

Ruby: Thread.new { f }
来源：http://mex.cqqwz.cn

C#:   Task.Run(() => F());
来源：http://mbm.316326.xyz

[O02] 使用线程池
来源：http://uhz.havefunace.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://fcr.hywenlv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cjp.wangshuangyany.cn

JS:   // worker_threads 线程池
来源：http://lan.ywan-chungtsiang.top

TS:   // worker_threads 线程池
来源：http://sml.xziqi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ksx.cheryme.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ycz.kuanghao11.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xoz.jlsjyb.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nku.jinyuanbaomall.cn

[O03] 加锁保护共享数据
来源：http://yeu.jinqigfzy.top

Py:   with lock: shared += 1
来源：http://dvt.hongshengwenyu.top

PHP:  // 用 flock() 做文件锁
来源：http://ngy.wangdashe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bee.xuetiantiany.cn

TS:   // 同 JS
来源：http://ntf.316326.xyz

Java: synchronized (this) { shared++; }
来源：http://ytd.haohaochexian.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rzd.jiagoushi.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://pyw.guannengcc.top

C#:   lock (gate) { shared++; }
来源：http://zpx.xuetiantiany.cn

[O04] 定义异步函数并等待
来源：http://kdb.fzhhl.top

Py:   async def f():⏎    await g()
来源：http://uru.xinyue.icu

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vwu.dashuyun.cn

JS:   async function f() { await g(); }
来源：http://urk.yfazqb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://zyc.nanxuanxn.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rne.chenjidiqi.icu

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zbx.jlsjyb.cn

Ruby: # 用 Fiber 或 async gem
来源：http://iiq.zhengqikj.top

C#:   async Task F() { await G(); }
来源：http://eja.jinqigufen.top

[O05] 并发执行并等待全部完成
来源：http://toz.zhiwuduotai.top

Py:   asyncio.gather(*tasks)
来源：http://nnr.316326.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hjc.ydzc1.top

JS:   await Promise.all(tasks)
来源：http://cmg.yfazqb.com

TS:   await Promise.all(tasks)
来源：http://rac.mhx1999.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rgt.wangdashe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ehv.316326.xyz

Ruby: threads.map(&:join)
来源：http://uzf.hnxiangtu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jci.chenlongwang.top

[O06] 使用进程池
来源：http://cqy.gaohongyu789.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xti.hnqzz.top

PHP:  // pcntl_fork 或多进程队列
来源：http://smb.nanxinkj.top

JS:   // child_process / cluster 模块
来源：http://hzm.daxiang520.top

TS:   // child_process / cluster 模块
来源：http://fgm.316326.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mez.yanxiufei.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gdm.yvedp.cn

Ruby: // fork 块
来源：http://atz.tian-w.cn

C#:   Parallel.For
来源：http://lly.snrcjt.cn

================================================================================
来源：http://siy.jlsjyb.cn

P. 常用工具函数
来源：http://ejj.svipenyu.cn

================================================================================
来源：http://vyo.xuetiantiany.cn

[P01] 生成 UUID
来源：http://amk.yonumen.top

Py:   str(uuid.uuid4())
来源：http://wrg.52xcode.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://deb.zhaomingkeji.xyz

JS:   crypto.randomUUID()
来源：http://xmm.havefunace.top

TS:   crypto.randomUUID()
来源：http://nei.hnxiangtu.top

Java: UUID.randomUUID().toString()
来源：http://wry.gotoacloud.top

Go:   // 用 github.com/google/uuid
来源：http://vxz.cucudq.cn

Ruby: SecureRandom.uuid
来源：http://lhm.yvedp.cn

C#:   Guid.NewGuid().ToString()
来源：http://gnw.dashuyun.cn

[P02] MD5 / SHA256 摘要
来源：http://bzz.uphjek.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://miz.xziqi.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ggl.ydzc1.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zxj.ppjwa.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://tgw.andypj.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mgs.hongshengwenyu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lxn.tian-w.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ecl.52xcode.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gpd.jqgufenzy.top

[P03] 生成短随机字符串
来源：http://fbj.shangyingyoupin.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vhq.sysykeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qkp.daxiang520.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uej.yanxiufei.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xye.bbcook.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xhv.haohaochexian.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wpk.xziqi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://guc.xinyue.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xny.aibaodan.cn

[P04] 求长度
来源：http://wdq.haohaochexian.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ywm.hesvh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hzv.jinqigfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bcg.nanxinkj.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vtu.dashuyun.cn

Java: list.size();  map.size();  s.length()
来源：http://tqy.c1oappe.top

Go:   len(arr);  len(m)
来源：http://lek.quarkkingdee.top

Ruby: x.length;  x.size
来源：http://aad.wangdashe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ebt.havefunace.top

[P05] 判断两个对象内容是否相等
来源：http://ysg.fehbvm.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://ysx.shanyushiyangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fkh.cucudq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qgf.zdqjudy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vhu.ydzc1.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mtt.sxryk.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gtn.quarkkingdee.top

Ruby: a == b
来源：http://pgi.feifeiyinyue.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fld.chenlongwang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zsu.sxryk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ptg.sxryk.cn

PHP:  if (empty($x)) {}
来源：http://ygi.fengsongda.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://bnp.andypj.xyz

TS:   if (x == null) {}
来源：http://clv.jinqigfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mpm.guannengcc.top

Go:   if x == nil {}
来源：http://cqz.yanxiufei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ndp.yuxming.cn

C#:   if (x is null) {}
来源：http://aep.sysykeji.top

[P07] 防抖与节流
来源：http://ucz.yj20258.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fdq.zdqjudy.top

PHP:  // 手写时间戳比较
来源：http://pzl.fehbvm.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wkp.xinyue.icu

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zuo.vehdjk.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://drg.shuidangran.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://phl.hfpthk.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pto.yonumen.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://eho.shangyingyoupin.top

[P08] 处理浮点精度问题
来源：http://nbx.wangdashe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bon.yuxming.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://aok.andypj.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ykn.yuanzhike.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lvw.gaohongyu789.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nvx.wangdashe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ayf.ydjk.org.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ffo.tian-w.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jmv.jyoumei.cn

================================================================================
来源：http://akk.cdnleiting.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jpf.kuanghao11.cn

================================================================================
来源：http://bza.aizwys.cn

[Q01] 创建表
来源：http://uuw.quarkkingdee.top

CREATE TABLE users (
来源：http://dzv.52xcode.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bnf.xuetiantiany.cn

name VARCHAR(50) NOT NULL,
来源：http://mlo.ehwqpu.com

email VARCHAR(100) UNIQUE,
来源：http://xvx.nwbrower.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eyp.xinyue.icu

);
来源：http://lcr.yj20258888.top

[Q02] 创建带外键的表
来源：http://slx.jianghu66.top

CREATE TABLE orders (
来源：http://kjj.guowangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gfq.hfpthk.cn

user_id INT NOT NULL,
来源：http://gov.chenlongwang.top

amount DECIMAL(10, 2),
来源：http://jqq.zhoulong.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://isx.cucudq.cn

);
来源：http://pig.uphjek.com

[Q03] 增加列
来源：http://xel.cqqwz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lct.xuetiantiany.cn

[Q04] 修改列类型
来源：http://cxa.mhx1999.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mlf.xingfuxueyuan.xyz

[Q05] 重命名列
来源：http://keh.ywan-chungtsiang.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hct.wangshuangyany.cn

[Q06] 删除列
来源：http://nuv.hywenlv.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lna.hcnkem.com

[Q07] 删除表
来源：http://rwy.shuidangran.top

DROP TABLE IF EXISTS orders;
来源：http://dlq.pengpengdd.cyou

[Q08] 创建普通索引
来源：http://hjm.zhaomingkeji.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://zez.c1oappe.top

[Q09] 创建唯一索引
来源：http://mez.jinyuanbaomall.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lir.zycfv.cn

[Q10] 插入单行
来源：http://uhs.cdnleiting.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jpb.cdnleiting.top

[Q11] 一次插入多行
来源：http://xbn.jiagoushi.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://apo.andypj.xyz

[Q12] 插入后取自增 ID
来源：http://lou.sxryk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lqw.nwbrower.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xdh.sweek.top

[Q13] 忽略重复插入
来源：http://vmr.wangdashe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jpt.zhixingplan.top

[Q14] 存在则更新（upsert）
来源：http://tye.c1oappe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qwy.fanxiaobao.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vwr.ywan-chungtsiang.top

[Q15] 查询全部
来源：http://tvh.chenzaomai.com

SELECT * FROM users;
来源：http://qfo.yonumen.top

[Q16] 查询指定列
来源：http://ler.jiagoushi.top

SELECT id, name FROM users;
来源：http://ijp.gotoacloud.top

[Q17] 条件查询
来源：http://ayx.shanyushiyangtech.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://acb.yangfankeji.com

[Q18] 模糊匹配
来源：http://skf.cucudq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wfy.ydzc1.top

[Q19] 范围查询
来源：http://jsl.chenzaomai.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://svx.zdbjq.cn

[Q20] IN 列表
来源：http://fao.yfazqb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jdj.tianlin.xyz

[Q21] 空值判断
来源：http://ktv.zhengqikj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://nqi.zdqjudy.top

[Q22] 排序
来源：http://lus.chenlongwang.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ozn.kuanghao11.cn

[Q23] 分页
来源：http://mul.bbcook.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xyc.gogol.net.cn

[Q24] 去重
来源：http://roa.nanxuanxn.top

SELECT DISTINCT city FROM users;
来源：http://drs.cucudq.cn

[Q25] 只取前 N 条
来源：http://vyi.guannengcc.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://naw.kuanghao11.cn

[Q26] 计数
来源：http://apo.feifeiyinyue.top

SELECT COUNT(*) FROM users;
来源：http://inq.jinyuanbaomall.cn

[Q27] 条件计数
来源：http://fxr.tianlin.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jgi.tianlin.xyz

[Q28] 求和与平均
来源：http://obt.dashuyun.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kts.zhijiandao.cn

[Q29] 最大最小值
来源：http://hxe.sxryk.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bsi.yuanzhike.top

[Q30] 分组统计
来源：http://pha.hcnkem.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wpk.tarul.cn

[Q31] 分组后过滤
来源：http://nxh.hysaishi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hhs.ydjk.org.cn

[Q32] 分组拼接字符串
来源：http://xbc.yvedp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://txx.0kj1m.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zje.dashuyun.cn

[Q33] 多列分组
来源：http://hpy.gzhubu.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rbv.uphjek.com

[Q34] 每组取第一条
来源：http://cam.feifeiyinyue.top

SELECT * FROM (
来源：http://hav.yj20258.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://okg.fehbvm.com

) t WHERE rn = 1;
来源：http://sxn.jinyuanbaomall.cn

[Q35] 内连接
来源：http://yxh.tanke756.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jhp.redwolf501.top

[Q36] 左连接
来源：http://aoc.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kmr.ivvv.top

[Q37] 右连接
来源：http://egg.sweek.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ttl.uphjek.com

[Q38] 全外连接（PostgreSQL）
来源：http://hfe.kuanghao11.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cgh.snrcjt.cn

[Q39] 自连接（查上下级）
来源：http://sxb.zhoulong.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://sid.nanxuanxn.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://olq.wangshuangyany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ooh.tanke756.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://urd.jianghu66.top

[Q41] 多表连接
来源：http://oak.c1oappe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hlp.snrcjt.cn

JOIN users u ON u.id = o.user_id
来源：http://pew.zhiwuduotai.top

JOIN products p ON p.id = o.product_id;
来源：http://uxw.zhixingplan.top

[Q42] 连接条件附加过滤
来源：http://ita.nanxuanxn.top

SELECT u.name, o.amount FROM users u
来源：http://skj.hesvh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vwa.daxiang520.top

[Q43] 标量子查询
来源：http://ldv.jiagoushi.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://skn.pycfn.com

[Q44] IN 子查询
来源：http://nya.zhaomingkeji.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dvz.zhixingplan.top

[Q45] EXISTS 判断存在
来源：http://wvu.guowangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pur.xziqi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xxy.zhaomingkeji.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xdd.yonumen.top

[Q47] 与平均值比较
来源：http://ber.chenlongwang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gmj.chenjidiqi.icu

[Q48] CTE 公用表表达式
来源：http://wof.yj20258888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://eua.meibo888.top

SELECT * FROM t WHERE c > 5;
来源：http://xwb.sjlbkw.cn

[Q49] 更新单行
来源：http://gko.jlsjyb.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://erl.gogol.net.cn

[Q50] 批量更新
来源：http://bvx.zhiwuduotai.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://drc.yueranfly.top

[Q51] 用子查询更新
来源：http://woq.aizwys.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oxs.ybcxt.top

[Q52] 删除指定行
来源：http://lik.zdqjudy.top

DELETE FROM users WHERE id = 10;
来源：http://pii.guannengcc.top

[Q53] 按条件删除
来源：http://feo.mhx1999.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xvx.kuanghao11.cn

[Q54] 清空表
来源：http://uxr.hongshengwenyu.top

TRUNCATE TABLE logs;
来源：http://hmy.hnqzz.top

[Q55] 排名（并列占位）
来源：http://npw.guowangkeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aqw.9152youxi.cn

[Q56] 密集排名（并列不占位）
来源：http://tav.kuanghao11.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xoy.havefunace.top

[Q57] 行号
来源：http://bjz.jyoumei.cn


<!-- 参考信息 -->