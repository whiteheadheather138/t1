代发 wailian999

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://gme.jqgufenzy.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://miw.kuanghao11.cn

Java: class Node { int v; Node next; }
来源：http://egq.snrcjt.cn

Go:   type Node struct { V int; Next *Node }
来源：http://eru.cheryme.top

Ruby: Node = Struct.new(:v, :next)
来源：http://nxr.zdqjudy.top

C#:   class Node { public int V; public Node? Next; }
来源：http://yjm.xziqi.cn

[N11] 二叉树中序遍历
来源：http://huv.yongpay.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://hom.iojbl.cn

PHP:  // 手写递归函数
来源：http://xzc.ehwqpu.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rzs.xuanzx.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xgk.shanyushiyangkeji.top

Java: // 手写递归
来源：http://bzf.fktsv.cn

Go:   // 手写递归
来源：http://wdh.cqqwz.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://cox.sweek.top

C#:   // 手写递归
来源：http://acx.jiagoushi.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pub.ybcxt.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qzj.zdqjudy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://taz.zhengqikj.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vlg.jiagoushi.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://oou.jinqigfzy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jtt.tanke756.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zyn.pengpengdd.cyou

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://fvm.ivvv.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jwl.hfpthk.cn

================================================================================
来源：http://itl.jqgufenzy.top

O. 并发与异步
来源：http://ktm.0kj1m.cn

================================================================================
来源：http://yba.iojbl.cn

[O01] 启动一个线程
来源：http://mta.shanyushiyangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://jnk.tian-w.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ghs.zhijiandao.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nxp.ydjk.org.cn

TS:   // 同 JS
来源：http://unp.jianghu66.top

Java: new Thread(() -> f()).start()
来源：http://tme.sjlbkw.cn

Go:   go f()
来源：http://rmb.tarul.cn

Ruby: Thread.new { f }
来源：http://icr.shanyushiyangkeji.top

C#:   Task.Run(() => F());
来源：http://vpp.hnxiangtu.top

[O02] 使用线程池
来源：http://ewe.shanyushiyangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nke.jinghuilouyu.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dbb.aizwys.cn

JS:   // worker_threads 线程池
来源：http://lrn.shanyushiyangkeji.top

TS:   // worker_threads 线程池
来源：http://ybi.sxryk.cn

Java: Executors.newFixedThreadPool(4)
来源：http://itr.yuanzhike.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zct.daxiang520.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wyw.hywenlv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rxp.xingfuxueyuan.xyz

[O03] 加锁保护共享数据
来源：http://ppi.tarul.cn

Py:   with lock: shared += 1
来源：http://emg.hesvh.cn

PHP:  // 用 flock() 做文件锁
来源：http://til.redwolf501.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ztk.yfazqb.com

TS:   // 同 JS
来源：http://ucv.gotoacloud.top

Java: synchronized (this) { shared++; }
来源：http://cxf.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tdx.haohaochexian.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://tqx.fengsongda.top

C#:   lock (gate) { shared++; }
来源：http://ton.kuanghao11.cn

[O04] 定义异步函数并等待
来源：http://wpz.cashguo.top

Py:   async def f():⏎    await g()
来源：http://jnq.redwolf501.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vph.vehdjk.com

JS:   async function f() { await g(); }
来源：http://ons.jlsjyb.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ocv.svipenyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vrz.chenzaomai.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hoc.jinyuanbaomall.cn

Ruby: # 用 Fiber 或 async gem
来源：http://min.birdmap.top

C#:   async Task F() { await G(); }
来源：http://oew.ybcxt.top

[O05] 并发执行并等待全部完成
来源：http://sml.0kj1m.cn

Py:   asyncio.gather(*tasks)
来源：http://ygd.jqgfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yxd.zhijiandao.cn

JS:   await Promise.all(tasks)
来源：http://onu.uphjek.com

TS:   await Promise.all(tasks)
来源：http://sjx.yuxming.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://okw.yuxming.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://myc.zhoulong.xyz

Ruby: threads.map(&:join)
来源：http://ych.xuanzx.com

C#:   await Task.WhenAll(t1, t2)
来源：http://pbd.hcnkem.com

[O06] 使用进程池
来源：http://zmz.fengsongda.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qex.sufxvd.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ano.jqgfzy.top

JS:   // child_process / cluster 模块
来源：http://out.cashguo.top

TS:   // child_process / cluster 模块
来源：http://jrn.zdqjudy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mzf.ppjwa.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://qgf.fzhhl.top

Ruby: // fork 块
来源：http://bbh.jinqigfzy.top

C#:   Parallel.For
来源：http://njc.tarul.cn

================================================================================
来源：http://ngu.ctjpmb.com

P. 常用工具函数
来源：http://pjy.pengpengdd.cyou

================================================================================
来源：http://oqm.tian-w.cn

[P01] 生成 UUID
来源：http://hhj.hysaishi.cn

Py:   str(uuid.uuid4())
来源：http://val.jinqigfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mjt.jqgfzy.top

JS:   crypto.randomUUID()
来源：http://ktw.jlsjyb.cn

TS:   crypto.randomUUID()
来源：http://ehl.shanyushiyangtech.top

Java: UUID.randomUUID().toString()
来源：http://qgi.hnqzz.top

Go:   // 用 github.com/google/uuid
来源：http://zyr.yueranfly.top

Ruby: SecureRandom.uuid
来源：http://jwh.gaohongyu789.top

C#:   Guid.NewGuid().ToString()
来源：http://sdf.pycfn.com

[P02] MD5 / SHA256 摘要
来源：http://lss.snrcjt.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ggc.shangyingyoupin.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zcp.xuetiantiany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yvd.316326.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pef.fanxiaobao.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yyr.yuxming.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lrg.zycfv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://hqr.jinqigufen.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kaf.sysykeji.top

[P03] 生成短随机字符串
来源：http://isi.daxiang520.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ygk.iojbl.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wai.ehwqpu.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ejf.hnxiangtu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fzq.zhengqikj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iti.jiagoushi.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://tsi.ctjpmb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://ltw.yanxiufei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hwl.gogol.net.cn

[P04] 求长度
来源：http://bzi.shanyushiyangtech.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vcj.fehbvm.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ilx.zycfv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://utu.gogol.net.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://srl.gaohongyu789.top

Java: list.size();  map.size();  s.length()
来源：http://lul.hywenlv.cn

Go:   len(arr);  len(m)
来源：http://emx.zdbjq.cn

Ruby: x.length;  x.size
来源：http://ihi.ppjwa.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rus.xylfe.cn

[P05] 判断两个对象内容是否相等
来源：http://hzt.fengsongda.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://anp.havefunace.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://obf.sxryk.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://eev.zdbjq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gmz.gotoacloud.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nfa.guowangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://qus.vqdsnc.cn

Ruby: a == b
来源：http://mcu.shzxlz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gdp.zhengqikj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jam.jiagoushi.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://drn.xziqi.cn

PHP:  if (empty($x)) {}
来源：http://hra.hongshengwenyu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qez.gzhubu.top

TS:   if (x == null) {}
来源：http://jzs.bjfxy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://nev.andypj.xyz

Go:   if x == nil {}
来源：http://xib.0kj1m.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://akn.zycfv.cn

C#:   if (x is null) {}
来源：http://qlg.daria6918.cn

[P07] 防抖与节流
来源：http://rnh.jinghuilouyu.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ccs.gotoacloud.top

PHP:  // 手写时间戳比较
来源：http://daz.yanxiufei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gwx.yongpay.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rol.zdqjudy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hlo.ctjpmb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cin.ybcxt.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ujh.sjlbkw.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hrf.9152youxi.cn

[P08] 处理浮点精度问题
来源：http://wpi.andypj.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hmf.feifeiyinyue.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bvu.zdbjq.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pre.zhoulong.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ois.52xcode.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hzw.ydzc1.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://stm.smart0.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tmz.9152youxi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ydx.yonumen.top

================================================================================
来源：http://knr.mhx1999.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xnl.jqgufenzy.top

================================================================================
来源：http://qla.ehwqpu.com

[Q01] 创建表
来源：http://kac.hesvh.cn

CREATE TABLE users (
来源：http://oxo.havefunace.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mno.tianlin.xyz

name VARCHAR(50) NOT NULL,
来源：http://rkg.dianchejie.cn

email VARCHAR(100) UNIQUE,
来源：http://nfc.guowangkeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://elj.fanxiaobao.xyz

);
来源：http://zol.xinyue.icu

[Q02] 创建带外键的表
来源：http://vsw.zhoulong.xyz

CREATE TABLE orders (
来源：http://ytl.jinqigfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ifq.jyoumei.cn

user_id INT NOT NULL,
来源：http://ibv.fengsongda.top

amount DECIMAL(10, 2),
来源：http://kpf.zhijiandao.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pxi.haohaochexian.top

);
来源：http://tpy.ydzc1.top

[Q03] 增加列
来源：http://sik.cqqwz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://skd.xuanzx.com

[Q04] 修改列类型
来源：http://mmg.yanxiufei.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gdz.nwbrower.top

[Q05] 重命名列
来源：http://sgh.ppjwa.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xat.fktsv.cn

[Q06] 删除列
来源：http://yau.epnwcf.com

ALTER TABLE users DROP COLUMN age;
来源：http://gxq.bjfxy.top

[Q07] 删除表
来源：http://aon.yj20258.top

DROP TABLE IF EXISTS orders;
来源：http://ucu.hongshengwenyu.top

[Q08] 创建普通索引
来源：http://exj.jlsjyb.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wqg.yangfankeji.com

[Q09] 创建唯一索引
来源：http://xaa.iojbl.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gmd.smart0.xyz

[Q10] 插入单行
来源：http://qfb.ehwqpu.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fzd.xingfuxueyuan.xyz

[Q11] 一次插入多行
来源：http://aye.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uma.ybcxt.top

[Q12] 插入后取自增 ID
来源：http://jnr.zhixingplan.top

INSERT INTO users (name) VALUES ('C');
来源：http://auw.yanxiufei.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vgw.fktsv.cn

[Q13] 忽略重复插入
来源：http://aoo.ctjpmb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wci.hfpthk.cn

[Q14] 存在则更新（upsert）
来源：http://obc.hywenlv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kxt.gotoacloud.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xlo.fzhhl.top

[Q15] 查询全部
来源：http://brz.wangdashe.top

SELECT * FROM users;
来源：http://mvc.redwolf501.top

[Q16] 查询指定列
来源：http://spo.hysaishi.cn

SELECT id, name FROM users;
来源：http://fhx.yongpay.top

[Q17] 条件查询
来源：http://unv.snrcjt.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pse.hnqzz.top

[Q18] 模糊匹配
来源：http://cng.jqgufenzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uvb.cqqwz.cn

[Q19] 范围查询
来源：http://nvl.xuetiantiany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fsp.jiagoushi.top

[Q20] IN 列表
来源：http://tih.zhijiandao.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://efk.shzxlz.cn

[Q21] 空值判断
来源：http://jnr.guowangkeji.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bxe.hysaishi.cn

[Q22] 排序
来源：http://vjw.xinyue.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://szg.yuanzhike.top

[Q23] 分页
来源：http://zbx.xylfe.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vxg.jinyuanbaomall.cn

[Q24] 去重
来源：http://ove.nwbrower.top

SELECT DISTINCT city FROM users;
来源：http://har.xylfe.cn

[Q25] 只取前 N 条
来源：http://mgd.daria6918.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://khs.fktsv.cn

[Q26] 计数
来源：http://dnk.shzxlz.cn

SELECT COUNT(*) FROM users;
来源：http://ebu.fktsv.cn

[Q27] 条件计数
来源：http://tfd.zdqjudy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cur.hywenlv.cn

[Q28] 求和与平均
来源：http://juf.yongpay.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vva.yvedp.cn

[Q29] 最大最小值
来源：http://fva.dashuyun.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://tvv.fzhhl.top

[Q30] 分组统计
来源：http://vvd.yangfankeji.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sev.tarul.cn

[Q31] 分组后过滤
来源：http://lil.shzxlz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cea.zhijiandao.cn

[Q32] 分组拼接字符串
来源：http://wao.52xcode.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dmw.fehbvm.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zra.wangshuangyany.cn

[Q33] 多列分组
来源：http://gkd.zdqjudy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hqy.nanxinkj.top

[Q34] 每组取第一条
来源：http://uhd.guannengcc.top

SELECT * FROM (
来源：http://yzr.svipenyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jvu.chenzaomai.com

) t WHERE rn = 1;
来源：http://uvp.yuanzhike.top

[Q35] 内连接
来源：http://uob.sxryk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xoz.c1oappe.top

[Q36] 左连接
来源：http://hfd.ybcxt.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pzx.havefunace.top

[Q37] 右连接
来源：http://dst.xuetiantiany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jsu.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://aam.nanxinkj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://abk.gotoacloud.top

[Q39] 自连接（查上下级）
来源：http://boe.9152youxi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pco.shzxlz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mnj.yj20258888.top

[Q40] 交叉连接（笛卡尔积）
来源：http://rib.hnxiangtu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ygh.jlsjyb.cn

[Q41] 多表连接
来源：http://ieo.xuetiantiany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xib.jianghu66.top

JOIN users u ON u.id = o.user_id
来源：http://jjn.yonumen.top

JOIN products p ON p.id = o.product_id;
来源：http://emv.9152youxi.cn

[Q42] 连接条件附加过滤
来源：http://yne.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u
来源：http://ley.tanke756.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zff.wangshuangyany.cn

[Q43] 标量子查询
来源：http://nzj.cheryme.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cld.yj20258888.top

[Q44] IN 子查询
来源：http://tys.ybcxt.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://thc.feifeiyinyue.top

[Q45] EXISTS 判断存在
来源：http://zve.jinyuanbaomall.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iyy.redwolf501.top

[Q46] NOT EXISTS 判断不存在
来源：http://xmz.sufxvd.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mka.yangfankeji.com

[Q47] 与平均值比较
来源：http://fuh.yj202588.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jui.shangyingyoupin.top

[Q48] CTE 公用表表达式
来源：http://zwm.316326.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nvl.fzhhl.top

SELECT * FROM t WHERE c > 5;
来源：http://wjj.cheryme.top

[Q49] 更新单行
来源：http://wis.zdqjudy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rxb.hcnkem.com

[Q50] 批量更新
来源：http://wja.ppjwa.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fpp.havefunace.top

[Q51] 用子查询更新
来源：http://bwz.fanxiaobao.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hkn.zdbjq.cn

[Q52] 删除指定行
来源：http://qin.pengpengdd.cyou

DELETE FROM users WHERE id = 10;
来源：http://lum.andypj.xyz

[Q53] 按条件删除
来源：http://emh.iojbl.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sza.zdqjudy.top

[Q54] 清空表
来源：http://iyu.kuanghao11.cn

TRUNCATE TABLE logs;
来源：http://jjn.dianchejie.cn

[Q55] 排名（并列占位）
来源：http://fvp.epnwcf.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://umq.hongshengwenyu.top

[Q56] 密集排名（并列不占位）
来源：http://anz.haohaochexian.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jcc.snrcjt.cn

[Q57] 行号
来源：http://kew.guowangkeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mlo.dianchejie.cn

[Q58] 累计求和
来源：http://gfl.yfazqb.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tuo.svipenyu.cn

[Q59] 分组内累计
来源：http://ikw.yj202588.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nhm.vqdsnc.cn

[Q60] 取上一行 / 下一行
来源：http://yzx.epnwcf.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nvn.hysaishi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hto.ydzc1.top


<!-- 参考信息 -->