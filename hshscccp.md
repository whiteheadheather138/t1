代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://lil.yanxiufei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rvy.yfazqb.com

Java: class Node { int v; Node next; }
来源：http://flb.mhx1999.top

Go:   type Node struct { V int; Next *Node }
来源：http://ilw.dianchejie.cn

Ruby: Node = Struct.new(:v, :next)
来源：http://hgv.zhengqikj.top

C#:   class Node { public int V; public Node? Next; }
来源：http://ykh.svipenyu.cn

[N11] 二叉树中序遍历
来源：http://cig.ivvv.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://drt.iojbl.cn

PHP:  // 手写递归函数
来源：http://qxl.yueranfly.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://drx.fehbvm.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://dgz.xziqi.cn

Java: // 手写递归
来源：http://bto.aizwys.cn

Go:   // 手写递归
来源：http://wwr.jinghuilouyu.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://zeg.aibaodan.cn

C#:   // 手写递归
来源：http://kqs.zhengqikj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lve.xuetiantiany.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://icp.fzhhl.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sma.andypj.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gud.quarkkingdee.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mpa.yonumen.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://amz.guannengcc.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://ijr.chenzaomai.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://njc.meibo888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zts.smart0.xyz

================================================================================
来源：http://ccu.jqgufenzy.top

O. 并发与异步
来源：http://nzi.shanyushiyangkeji.top

================================================================================
来源：http://nlw.zdqjudy.top

[O01] 启动一个线程
来源：http://xls.aizwys.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dfl.zycfv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bmp.guowangkeji.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dux.zhoulong.xyz

TS:   // 同 JS
来源：http://uhy.xinyue.icu

Java: new Thread(() -> f()).start()
来源：http://ftx.52xcode.cn

Go:   go f()
来源：http://tmw.cdnleiting.top

Ruby: Thread.new { f }
来源：http://vcc.hcnkem.com

C#:   Task.Run(() => F());
来源：http://jyq.zhoulong.xyz

[O02] 使用线程池
来源：http://ggn.sysykeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nzn.sxryk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ylz.yongpay.top

JS:   // worker_threads 线程池
来源：http://drt.sjlbkw.cn

TS:   // worker_threads 线程池
来源：http://ice.cashguo.top

Java: Executors.newFixedThreadPool(4)
来源：http://plx.yangfankeji.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://eey.xuanzx.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kex.sufxvd.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://swn.yuanzhike.top

[O03] 加锁保护共享数据
来源：http://dwu.guowangkeji.top

Py:   with lock: shared += 1
来源：http://mbz.hnqzz.top

PHP:  // 用 flock() 做文件锁
来源：http://rpi.gaohongyu789.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://seq.sxryk.cn

TS:   // 同 JS
来源：http://fnq.kuanghao11.cn

Java: synchronized (this) { shared++; }
来源：http://dfi.cheryme.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uyd.zhixingplan.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nmb.wangdashe.top

C#:   lock (gate) { shared++; }
来源：http://dwa.nwbrower.top

[O04] 定义异步函数并等待
来源：http://ndo.svipenyu.cn

Py:   async def f():⏎    await g()
来源：http://wtb.meibo888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lqu.ydzc1.top

JS:   async function f() { await g(); }
来源：http://fhw.xinyue.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://vbt.zhengqikj.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yye.ydjk.org.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://omt.wangdashe.top

Ruby: # 用 Fiber 或 async gem
来源：http://lke.aibaodan.cn

C#:   async Task F() { await G(); }
来源：http://vzq.bjfxy.top

[O05] 并发执行并等待全部完成
来源：http://bir.jqgufenzy.top

Py:   asyncio.gather(*tasks)
来源：http://qzk.tarul.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eeh.9152youxi.cn

JS:   await Promise.all(tasks)
来源：http://jmi.ivvv.top

TS:   await Promise.all(tasks)
来源：http://aou.ybcxt.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://exp.fzhhl.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://xar.chenzaomai.com

Ruby: threads.map(&:join)
来源：http://ctc.zdbjq.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://cjy.fehbvm.com

[O06] 使用进程池
来源：http://hiw.jyoumei.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fko.dianchejie.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zco.nanxuanxn.top

JS:   // child_process / cluster 模块
来源：http://tnt.sxryk.cn

TS:   // child_process / cluster 模块
来源：http://fij.cdnleiting.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://saj.chenlongwang.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ifw.yj20258.top

Ruby: // fork 块
来源：http://akj.shanyushiyangkeji.top

C#:   Parallel.For
来源：http://gli.uphjek.com

================================================================================
来源：http://adu.zycfv.cn

P. 常用工具函数
来源：http://ucc.jiagoushi.top

================================================================================
来源：http://dwq.vqdsnc.cn

[P01] 生成 UUID
来源：http://nds.nwbrower.top

Py:   str(uuid.uuid4())
来源：http://ngq.xingfuxueyuan.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nvx.dashuyun.cn

JS:   crypto.randomUUID()
来源：http://vom.chenlongwang.top

TS:   crypto.randomUUID()
来源：http://ghc.jqgfzy.top

Java: UUID.randomUUID().toString()
来源：http://foz.hnxiangtu.top

Go:   // 用 github.com/google/uuid
来源：http://tpv.pengpengdd.cyou

Ruby: SecureRandom.uuid
来源：http://mjl.xuanzx.com

C#:   Guid.NewGuid().ToString()
来源：http://xvz.epnwcf.com

[P02] MD5 / SHA256 摘要
来源：http://ikx.bjfxy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ufs.cheryme.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xxm.cucudq.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wnk.andypj.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zkq.haohaochexian.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uxl.jinyuanbaomall.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wil.ydzc1.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yyb.fanxiaobao.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zuw.yongpay.top

[P03] 生成短随机字符串
来源：http://uyi.cashguo.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bcv.zhengqikj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fek.jinqigfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iwe.9152youxi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mld.wangdashe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kny.iojbl.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vpq.ivvv.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://okh.wangdashe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ywo.gaohongyu789.top

[P04] 求长度
来源：http://ejg.dianchejie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hdb.chenzaomai.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jad.snrcjt.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rcp.nanxinkj.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ocj.hysaishi.cn

Java: list.size();  map.size();  s.length()
来源：http://zcq.feifeiyinyue.top

Go:   len(arr);  len(m)
来源：http://wtf.bbcook.cn

Ruby: x.length;  x.size
来源：http://xzr.bbcook.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lom.xziqi.cn

[P05] 判断两个对象内容是否相等
来源：http://qnu.wangshuangyany.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fxv.tianlin.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wjk.vehdjk.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://voq.fanxiaobao.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jrb.xuetiantiany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wmc.yueranfly.top

Go:   reflect.DeepEqual(a, b)
来源：http://sxt.bjfxy.top

Ruby: a == b
来源：http://yxf.epnwcf.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gtv.52xcode.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ifm.hnqzz.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wzk.gzhubu.top

PHP:  if (empty($x)) {}
来源：http://nmu.daria6918.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://opj.xylfe.cn

TS:   if (x == null) {}
来源：http://pih.yonumen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://gxr.zhengqikj.top

Go:   if x == nil {}
来源：http://gjx.cucudq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://aoc.sweek.top

C#:   if (x is null) {}
来源：http://oyg.hongshengwenyu.top

[P07] 防抖与节流
来源：http://nxf.shangyingyoupin.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ahd.ybcxt.top

PHP:  // 手写时间戳比较
来源：http://sol.jlsjyb.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vib.bbcook.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oin.jlsjyb.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aiu.redwolf501.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ztm.yfazqb.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://aze.cheryme.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lcy.hesvh.cn

[P08] 处理浮点精度问题
来源：http://qyr.daxiang520.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gud.shzxlz.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jtu.redwolf501.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cwt.aibaodan.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://byj.yvedp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pvg.sjlbkw.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dcc.shanyushiyangtech.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sui.guowangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hiw.nanxinkj.top

================================================================================
来源：http://ajo.chenjidiqi.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kme.birdmap.top

================================================================================
来源：http://eda.wangshuangyany.cn

[Q01] 创建表
来源：http://kwz.meibo888.top

CREATE TABLE users (
来源：http://twd.yj20258888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cln.meibo888.top

name VARCHAR(50) NOT NULL,
来源：http://qbf.hywenlv.cn

email VARCHAR(100) UNIQUE,
来源：http://kpn.jiagoushi.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://adf.tanke756.top

);
来源：http://wpa.sjlbkw.cn

[Q02] 创建带外键的表
来源：http://pcw.sweek.top

CREATE TABLE orders (
来源：http://hvo.fzhhl.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kra.dianchejie.cn

user_id INT NOT NULL,
来源：http://wke.zhixingplan.top

amount DECIMAL(10, 2),
来源：http://hdm.yfazqb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ypy.guannengcc.top

);
来源：http://ane.yuanzhike.top

[Q03] 增加列
来源：http://tkw.aizwys.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://brs.jinyuanbaomall.cn

[Q04] 修改列类型
来源：http://glm.hnqzz.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xea.fehbvm.com

[Q05] 重命名列
来源：http://plw.tian-w.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yjy.yuxming.cn

[Q06] 删除列
来源：http://eem.zhixingplan.top

ALTER TABLE users DROP COLUMN age;
来源：http://kkm.wangshuangyany.cn

[Q07] 删除表
来源：http://yso.tarul.cn

DROP TABLE IF EXISTS orders;
来源：http://uct.uphjek.com

[Q08] 创建普通索引
来源：http://dzz.zhaomingkeji.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://fzc.jqgufenzy.top

[Q09] 创建唯一索引
来源：http://zkh.xylfe.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fof.nanxinkj.top

[Q10] 插入单行
来源：http://vgq.guannengcc.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zto.svipenyu.cn

[Q11] 一次插入多行
来源：http://xco.gogol.net.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gxo.quarkkingdee.top

[Q12] 插入后取自增 ID
来源：http://poh.cqqwz.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lnh.shanyushiyangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://swf.smart0.xyz

[Q13] 忽略重复插入
来源：http://bbb.pycfn.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qnk.guowangkeji.top

[Q14] 存在则更新（upsert）
来源：http://ixz.fzhhl.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nph.guowangkeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qdo.xuanzx.com

[Q15] 查询全部
来源：http://ypp.jlsjyb.cn

SELECT * FROM users;
来源：http://yjp.hywenlv.cn

[Q16] 查询指定列
来源：http://njg.hnqzz.top

SELECT id, name FROM users;
来源：http://cyp.jinyuanbaomall.cn

[Q17] 条件查询
来源：http://scx.snrcjt.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qug.yj20258.top

[Q18] 模糊匹配
来源：http://jau.zhijiandao.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lov.zhixingplan.top

[Q19] 范围查询
来源：http://anf.cucudq.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iwb.xuetiantiany.cn

[Q20] IN 列表
来源：http://owr.cheryme.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jck.epnwcf.com

[Q21] 空值判断
来源：http://tkg.shuidangran.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bjr.sufxvd.cn

[Q22] 排序
来源：http://bdu.vehdjk.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://krh.yj20258888.top

[Q23] 分页
来源：http://xvt.yueranfly.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nff.vqdsnc.cn

[Q24] 去重
来源：http://kks.nanxinkj.top

SELECT DISTINCT city FROM users;
来源：http://efc.52xcode.cn

[Q25] 只取前 N 条
来源：http://vuc.mhx1999.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kfi.hywenlv.cn

[Q26] 计数
来源：http://vmi.gogol.net.cn

SELECT COUNT(*) FROM users;
来源：http://tsc.iojbl.cn

[Q27] 条件计数
来源：http://qic.zhaomingkeji.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lrl.chenjidiqi.icu

[Q28] 求和与平均
来源：http://prt.hcnkem.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xwm.feifeiyinyue.top

[Q29] 最大最小值
来源：http://vch.guowangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://zmq.feifeiyinyue.top

[Q30] 分组统计
来源：http://xoo.ppjwa.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mew.nwbrower.top

[Q31] 分组后过滤
来源：http://bxt.yj20258.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fvi.aizwys.cn

[Q32] 分组拼接字符串
来源：http://hhg.ivvv.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ufi.fktsv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dig.jyoumei.cn

[Q33] 多列分组
来源：http://iha.yangfankeji.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mxk.xinyue.icu

[Q34] 每组取第一条
来源：http://ryn.jqgfzy.top

SELECT * FROM (
来源：http://uur.havefunace.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://idv.cqqwz.cn

) t WHERE rn = 1;
来源：http://cpk.xingfuxueyuan.xyz

[Q35] 内连接
来源：http://cbj.hongshengwenyu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://psq.yuxming.cn

[Q36] 左连接
来源：http://vil.cqqwz.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://thn.ydjk.org.cn

[Q37] 右连接
来源：http://nnx.cqqwz.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ewe.ppjwa.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gtk.yonumen.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yrv.yj20258888.top

[Q39] 自连接（查上下级）
来源：http://lec.fktsv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vee.ydzc1.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tzl.daxiang520.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wpx.guannengcc.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tni.tianlin.xyz

[Q41] 多表连接
来源：http://ffk.yj202588.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bsc.sxryk.cn

JOIN users u ON u.id = o.user_id
来源：http://oai.xingfuxueyuan.xyz

JOIN products p ON p.id = o.product_id;
来源：http://qnj.shangyingyoupin.top

[Q42] 连接条件附加过滤
来源：http://oyv.chenlongwang.top

SELECT u.name, o.amount FROM users u
来源：http://usc.gaohongyu789.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uvu.gaohongyu789.top

[Q43] 标量子查询
来源：http://zsu.dianchejie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wcs.fzhhl.top

[Q44] IN 子查询
来源：http://bdq.vqdsnc.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gvu.epnwcf.com

[Q45] EXISTS 判断存在
来源：http://zji.shanyushiyangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://czf.havefunace.top

[Q46] NOT EXISTS 判断不存在
来源：http://xeo.sjlbkw.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ydf.xinyue.icu

[Q47] 与平均值比较
来源：http://ivt.cqqwz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ill.hysaishi.cn

[Q48] CTE 公用表表达式
来源：http://ovr.ivvv.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bir.hcnkem.com

SELECT * FROM t WHERE c > 5;
来源：http://xta.yongpay.top

[Q49] 更新单行
来源：http://rdi.havefunace.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bfy.andypj.xyz

[Q50] 批量更新
来源：http://cpg.cashguo.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jmq.pengpengdd.cyou

[Q51] 用子查询更新
来源：http://pkf.chenlongwang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ueb.nanxinkj.top

[Q52] 删除指定行
来源：http://vcv.hnqzz.top

DELETE FROM users WHERE id = 10;
来源：http://fml.jinyuanbaomall.cn

[Q53] 按条件删除
来源：http://gnf.hnqzz.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gvx.jyoumei.cn

[Q54] 清空表
来源：http://pzh.ivvv.top

TRUNCATE TABLE logs;
来源：http://sok.cqqwz.cn

[Q55] 排名（并列占位）
来源：http://skk.shanyushiyangtech.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kmw.quarkkingdee.top

[Q56] 密集排名（并列不占位）
来源：http://lxk.cucudq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://thn.yonumen.top

[Q57] 行号
来源：http://vaq.cheryme.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dep.yuxming.cn

[Q58] 累计求和
来源：http://jzp.ppjwa.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pow.ctjpmb.com

[Q59] 分组内累计
来源：http://ghy.zhengqikj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wjx.cucudq.cn

[Q60] 取上一行 / 下一行
来源：http://wkj.sweek.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dss.zycfv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nxu.jianghu66.top


<!-- 参考信息 -->