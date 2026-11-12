代发 wailian999

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jqy.zdqjudy.top

[N10] 链表节点定义
来源：http://xbg.chenjidiqi.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://str.yfazqb.com

PHP:  class Node { public $v; public $next = null; }
来源：http://mdf.sufxvd.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://qug.xinyue.icu

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ujz.haohaochexian.top

Java: class Node { int v; Node next; }
来源：http://elt.shuidangran.top

Go:   type Node struct { V int; Next *Node }
来源：http://cve.fehbvm.com

Ruby: Node = Struct.new(:v, :next)
来源：http://srh.52xcode.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ncr.wangshuangyany.cn

[N11] 二叉树中序遍历
来源：http://hua.xuanzx.com

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dne.xuetiantiany.cn

PHP:  // 手写递归函数
来源：http://ugb.jianghu66.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mzn.xziqi.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://civ.pycfn.com

Java: // 手写递归
来源：http://vmt.hammf.cn

Go:   // 手写递归
来源：http://weg.zhoulong.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pvw.wangshuangyany.cn

C#:   // 手写递归
来源：http://jdx.yonumen.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wxf.ywan-chungtsiang.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mxz.vehdjk.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://ehl.guannengcc.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://klu.sysykeji.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://yeg.sweek.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://dsx.birdmap.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sol.shanyushiyangtech.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mdp.shanyushiyangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dvo.haohaochexian.top

================================================================================
来源：http://tol.c1oappe.top

O. 并发与异步
来源：http://ecp.jinyuanbaomall.cn

================================================================================
来源：http://qxj.svipenyu.cn

[O01] 启动一个线程
来源：http://ecr.andypj.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gmk.xingfuxueyuan.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://esf.fengsongda.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hpn.zhoulong.xyz

TS:   // 同 JS
来源：http://cvj.sweek.top

Java: new Thread(() -> f()).start()
来源：http://vfn.yueranfly.top

Go:   go f()
来源：http://mhs.yuxming.cn

Ruby: Thread.new { f }
来源：http://dsi.tanke756.top

C#:   Task.Run(() => F());
来源：http://cmu.jinyuanbaomall.cn

[O02] 使用线程池
来源：http://yhu.pycfn.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://tke.hnxiangtu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mga.cheryme.top

JS:   // worker_threads 线程池
来源：http://zvx.cdnleiting.top

TS:   // worker_threads 线程池
来源：http://fqg.cucudq.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qfl.dianchejie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ozd.guowangkeji.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ybr.fanxiaobao.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jii.xingfuxueyuan.xyz

[O03] 加锁保护共享数据
来源：http://jii.hnqzz.top

Py:   with lock: shared += 1
来源：http://wrw.jinqigfzy.top

PHP:  // 用 flock() 做文件锁
来源：http://ceh.svipenyu.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uoq.cashguo.top

TS:   // 同 JS
来源：http://qyk.feifeiyinyue.top

Java: synchronized (this) { shared++; }
来源：http://ozn.nanxinkj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ugg.fzhhl.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ksp.pycfn.com

C#:   lock (gate) { shared++; }
来源：http://him.tianlin.xyz

[O04] 定义异步函数并等待
来源：http://qgp.gotoacloud.top

Py:   async def f():⏎    await g()
来源：http://zzd.smart0.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tdx.fengsongda.top

JS:   async function f() { await g(); }
来源：http://pwe.fanxiaobao.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://tud.ctjpmb.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sga.yangfankeji.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://pam.zhijiandao.cn

Ruby: # 用 Fiber 或 async gem
来源：http://kww.andypj.xyz

C#:   async Task F() { await G(); }
来源：http://szd.epnwcf.com

[O05] 并发执行并等待全部完成
来源：http://vro.daxiang520.top

Py:   asyncio.gather(*tasks)
来源：http://hmn.hnxiangtu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zww.cucudq.cn

JS:   await Promise.all(tasks)
来源：http://nre.ivvv.top

TS:   await Promise.all(tasks)
来源：http://vtj.meibo888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dlb.zdqjudy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://evv.sysykeji.top

Ruby: threads.map(&:join)
来源：http://jmh.aibaodan.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://gff.gogol.net.cn

[O06] 使用进程池
来源：http://grr.cashguo.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sxb.ydjk.org.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nzs.xinyue.icu

JS:   // child_process / cluster 模块
来源：http://xor.c1oappe.top

TS:   // child_process / cluster 模块
来源：http://myo.xylfe.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ptd.tianlin.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uvk.fehbvm.com

Ruby: // fork 块
来源：http://jms.wangdashe.top

C#:   Parallel.For
来源：http://bda.hammf.cn

================================================================================
来源：http://ite.shanyushiyangtech.top

P. 常用工具函数
来源：http://wdq.cashguo.top

================================================================================
来源：http://ipg.jinghuilouyu.cn

[P01] 生成 UUID
来源：http://upz.zhijiandao.cn

Py:   str(uuid.uuid4())
来源：http://xyl.yuxming.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://eiq.quarkkingdee.top

JS:   crypto.randomUUID()
来源：http://jzy.ppjwa.cn

TS:   crypto.randomUUID()
来源：http://lzo.shanyushiyangkeji.top

Java: UUID.randomUUID().toString()
来源：http://dpl.yj20258888.top

Go:   // 用 github.com/google/uuid
来源：http://cqf.shanyushiyangkeji.top

Ruby: SecureRandom.uuid
来源：http://pic.xuanzx.com

C#:   Guid.NewGuid().ToString()
来源：http://pro.jinyuanbaomall.cn

[P02] MD5 / SHA256 摘要
来源：http://jhr.mhx1999.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vbv.pycfn.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://zlh.aibaodan.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mwu.shanyushiyangtech.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zgo.gaohongyu789.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://itz.haohaochexian.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nsa.jinqigfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gpw.chenzaomai.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kpc.hesvh.cn

[P03] 生成短随机字符串
来源：http://vgl.jyoumei.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vwx.cqqwz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ytz.birdmap.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zys.meibo888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sbb.vqdsnc.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ebv.guowangkeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jpg.zycfv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tih.ydjk.org.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zhy.sxryk.cn

[P04] 求长度
来源：http://nwx.zycfv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vbx.wangdashe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mww.yanxiufei.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://reu.ehwqpu.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://glh.cheryme.top

Java: list.size();  map.size();  s.length()
来源：http://aok.wangdashe.top

Go:   len(arr);  len(m)
来源：http://bqa.jiagoushi.top

Ruby: x.length;  x.size
来源：http://iif.nwbrower.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vfe.bbcook.cn

[P05] 判断两个对象内容是否相等
来源：http://xra.dashuyun.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bja.gaohongyu789.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://thj.chenzaomai.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dpr.daxiang520.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ful.shuidangran.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tjb.feifeiyinyue.top

Go:   reflect.DeepEqual(a, b)
来源：http://orw.jinqigfzy.top

Ruby: a == b
来源：http://buw.aizwys.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uzf.daria6918.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ymp.nanxuanxn.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pzu.yfazqb.com

PHP:  if (empty($x)) {}
来源：http://fea.shanyushiyangkeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lzo.jiagoushi.top

TS:   if (x == null) {}
来源：http://hzq.sysykeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ivj.cashguo.top

Go:   if x == nil {}
来源：http://oni.shanyushiyangtech.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ect.zhengqikj.top

C#:   if (x is null) {}
来源：http://mwi.nwbrower.top

[P07] 防抖与节流
来源：http://ebp.fanxiaobao.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xjl.yonumen.top

PHP:  // 手写时间戳比较
来源：http://bpn.ydzc1.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ezd.bjfxy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yej.ydjk.org.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hok.cucudq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rpg.0kj1m.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gbs.cashguo.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kmc.9152youxi.cn

[P08] 处理浮点精度问题
来源：http://cnh.birdmap.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kcy.pycfn.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qvx.ctjpmb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uzs.andypj.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qcw.52xcode.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://isg.tian-w.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fea.mhx1999.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ccx.jinghuilouyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cds.yonumen.top

================================================================================
来源：http://she.xinyue.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dtp.shangyingyoupin.top

================================================================================
来源：http://tav.9152youxi.cn

[Q01] 创建表
来源：http://cwh.pycfn.com

CREATE TABLE users (
来源：http://lez.xylfe.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vzc.yueranfly.top

name VARCHAR(50) NOT NULL,
来源：http://tvg.hongshengwenyu.top

email VARCHAR(100) UNIQUE,
来源：http://psz.jqgfzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lhf.cqqwz.cn

);
来源：http://iro.pengpengdd.cyou

[Q02] 创建带外键的表
来源：http://dis.yj20258.top

CREATE TABLE orders (
来源：http://bny.jqgfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bei.xingfuxueyuan.xyz

user_id INT NOT NULL,
来源：http://dpf.hnqzz.top

amount DECIMAL(10, 2),
来源：http://nro.pycfn.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://iee.hfpthk.cn

);
来源：http://skl.svipenyu.cn

[Q03] 增加列
来源：http://ynp.zhoulong.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jxj.dianchejie.cn

[Q04] 修改列类型
来源：http://tge.jinqigfzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://aco.yj20258888.top

[Q05] 重命名列
来源：http://cdh.hesvh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://erp.ivvv.top

[Q06] 删除列
来源：http://xjr.wangshuangyany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qto.zdbjq.cn

[Q07] 删除表
来源：http://zmu.redwolf501.top

DROP TABLE IF EXISTS orders;
来源：http://sqn.yj20258888.top

[Q08] 创建普通索引
来源：http://kcg.mhx1999.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rzh.hywenlv.cn

[Q09] 创建唯一索引
来源：http://axs.shzxlz.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://imd.tianlin.xyz

[Q10] 插入单行
来源：http://oan.yueranfly.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gmd.dashuyun.cn

[Q11] 一次插入多行
来源：http://rko.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://isb.gzhubu.top

[Q12] 插入后取自增 ID
来源：http://hke.yuxming.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hkz.fktsv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jqh.jyoumei.cn

[Q13] 忽略重复插入
来源：http://vbh.nwbrower.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iky.jinqigfzy.top

[Q14] 存在则更新（upsert）
来源：http://kon.cqqwz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yem.cdnleiting.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://odi.yongpay.top

[Q15] 查询全部
来源：http://slg.0kj1m.cn

SELECT * FROM users;
来源：http://ybn.ehwqpu.com

[Q16] 查询指定列
来源：http://gap.yanxiufei.cn

SELECT id, name FROM users;
来源：http://mzx.sxryk.cn

[Q17] 条件查询
来源：http://yyc.vqdsnc.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cwg.zhixingplan.top

[Q18] 模糊匹配
来源：http://ixn.ydjk.org.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ryk.zdbjq.cn

[Q19] 范围查询
来源：http://wzj.c1oappe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blm.quarkkingdee.top

[Q20] IN 列表
来源：http://mrd.ppjwa.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oco.sysykeji.top

[Q21] 空值判断
来源：http://hkf.nanxinkj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://mtb.jlsjyb.cn

[Q22] 排序
来源：http://lht.hnqzz.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jes.52xcode.cn

[Q23] 分页
来源：http://rqu.yuxming.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pbz.sysykeji.top

[Q24] 去重
来源：http://lxc.fengsongda.top

SELECT DISTINCT city FROM users;
来源：http://mba.chenjidiqi.icu

[Q25] 只取前 N 条
来源：http://cju.ehwqpu.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zrl.bbcook.cn

[Q26] 计数
来源：http://skm.vqdsnc.cn

SELECT COUNT(*) FROM users;
来源：http://fkh.fehbvm.com

[Q27] 条件计数
来源：http://uzg.chenzaomai.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hco.snrcjt.cn

[Q28] 求和与平均
来源：http://hox.smart0.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://leu.shanyushiyangtech.top

[Q29] 最大最小值
来源：http://mms.daria6918.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bqi.cdnleiting.top

[Q30] 分组统计
来源：http://zbw.tianlin.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://twz.shangyingyoupin.top

[Q31] 分组后过滤
来源：http://clk.hammf.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fzt.mhx1999.top

[Q32] 分组拼接字符串
来源：http://opt.zhiwuduotai.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://udv.guowangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://frf.svipenyu.cn

[Q33] 多列分组
来源：http://kay.9152youxi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ovc.tanke756.top

[Q34] 每组取第一条
来源：http://vix.daria6918.cn

SELECT * FROM (
来源：http://fhp.yj202588.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vws.shanyushiyangkeji.top

) t WHERE rn = 1;
来源：http://dnv.zdbjq.cn

[Q35] 内连接
来源：http://saj.meibo888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://luj.jqgufenzy.top

[Q36] 左连接
来源：http://ttj.tian-w.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vxq.tian-w.cn

[Q37] 右连接
来源：http://xbw.kuanghao11.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nwi.cqqwz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qqa.fehbvm.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qft.zhijiandao.cn

[Q39] 自连接（查上下级）
来源：http://utz.cucudq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pkd.jiagoushi.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xfn.zhijiandao.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ijo.chenjidiqi.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yhy.haohaochexian.top

[Q41] 多表连接
来源：http://koe.yfazqb.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://aqb.52xcode.cn

JOIN users u ON u.id = o.user_id
来源：http://krr.gaohongyu789.top

JOIN products p ON p.id = o.product_id;
来源：http://ajp.sufxvd.cn

[Q42] 连接条件附加过滤
来源：http://eor.shuidangran.top

SELECT u.name, o.amount FROM users u
来源：http://mnu.chenzaomai.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uyt.yfazqb.com

[Q43] 标量子查询
来源：http://hfj.52xcode.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cuy.hesvh.cn

[Q44] IN 子查询
来源：http://lpq.zhixingplan.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://edi.gotoacloud.top

[Q45] EXISTS 判断存在
来源：http://dvu.yvedp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blg.zhixingplan.top

[Q46] NOT EXISTS 判断不存在
来源：http://hlc.dianchejie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dud.0kj1m.cn

[Q47] 与平均值比较
来源：http://eww.aizwys.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vsx.dashuyun.cn

[Q48] CTE 公用表表达式
来源：http://hmu.gzhubu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ilm.dianchejie.cn

SELECT * FROM t WHERE c > 5;
来源：http://dag.zdbjq.cn

[Q49] 更新单行
来源：http://yfw.pycfn.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lzr.0kj1m.cn

[Q50] 批量更新
来源：http://uat.hnxiangtu.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zin.ydjk.org.cn

[Q51] 用子查询更新
来源：http://yug.fzhhl.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mwr.ivvv.top

[Q52] 删除指定行
来源：http://xlr.c1oappe.top

DELETE FROM users WHERE id = 10;
来源：http://vze.svipenyu.cn

[Q53] 按条件删除
来源：http://bxo.jianghu66.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://trb.kuanghao11.cn

[Q54] 清空表
来源：http://ttp.jinyuanbaomall.cn

TRUNCATE TABLE logs;
来源：http://kwe.sweek.top

[Q55] 排名（并列占位）
来源：http://gmp.fanxiaobao.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hed.guannengcc.top

[Q56] 密集排名（并列不占位）
来源：http://kby.jyoumei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yju.hnqzz.top

[Q57] 行号
来源：http://qkk.yanxiufei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yjz.316326.xyz

[Q58] 累计求和
来源：http://hdo.zhengqikj.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iac.ybcxt.top

[Q59] 分组内累计
来源：http://yix.zhengqikj.top


<!-- 参考信息 -->