代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://vdb.yongpay.top

C#:   class Node { public int V; public Node? Next; }
来源：http://cxp.wangdashe.top

[N11] 二叉树中序遍历
来源：http://btc.dianchejie.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://duc.shangyingyoupin.top

PHP:  // 手写递归函数
来源：http://uen.fanxiaobao.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ege.sweek.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://bqb.haohaochexian.top

Java: // 手写递归
来源：http://tsg.zhongyouzk.top

Go:   // 手写递归
来源：http://lzh.jinyuanbaomall.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jgq.xinyue.icu

C#:   // 手写递归
来源：http://psb.yangfankeji.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://aqf.sysykeji.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://xot.xinyue.icu

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://enm.sxryk.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vvp.yuanzhike.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://afe.ywan-chungtsiang.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://qhb.fehbvm.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://swh.gzhubu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://soz.tarul.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xbg.zhixingplan.top

================================================================================
来源：http://ojc.snrcjt.cn

O. 并发与异步
来源：http://qyj.cdnleiting.top

================================================================================
来源：http://bbe.xuanzx.com

[O01] 启动一个线程
来源：http://yxc.shanyushiyangtech.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vmw.yj20258.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lpg.uphjek.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://luk.gotoacloud.top

TS:   // 同 JS
来源：http://upd.jyoumei.cn

Java: new Thread(() -> f()).start()
来源：http://kbr.chenjidiqi.icu

Go:   go f()
来源：http://sum.zdbjq.cn

Ruby: Thread.new { f }
来源：http://dkr.pycfn.com

C#:   Task.Run(() => F());
来源：http://wmw.yangfankeji.com

[O02] 使用线程池
来源：http://qhb.havefunace.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dut.jqgufenzy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qrf.yvedp.cn

JS:   // worker_threads 线程池
来源：http://njm.fktsv.cn

TS:   // worker_threads 线程池
来源：http://qim.yvedp.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rra.fktsv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dfp.316326.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://zdd.ybcxt.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mqc.xziqi.cn

[O03] 加锁保护共享数据
来源：http://swt.shuidangran.top

Py:   with lock: shared += 1
来源：http://axg.daxiang520.top

PHP:  // 用 flock() 做文件锁
来源：http://mah.aibaodan.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tsj.fehbvm.com

TS:   // 同 JS
来源：http://gmh.shangyingyoupin.top

Java: synchronized (this) { shared++; }
来源：http://lvc.kuanghao11.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://frk.yongpay.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://elr.gzhubu.top

C#:   lock (gate) { shared++; }
来源：http://ptc.dianchejie.cn

[O04] 定义异步函数并等待
来源：http://oex.snrcjt.cn

Py:   async def f():⏎    await g()
来源：http://mfh.yj20258888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uvf.ydjk.org.cn

JS:   async function f() { await g(); }
来源：http://dbk.xuetiantiany.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fqn.hongshengwenyu.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xev.pycfn.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dem.andypj.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://qtm.jianghu66.top

C#:   async Task F() { await G(); }
来源：http://cnn.iojbl.cn

[O05] 并发执行并等待全部完成
来源：http://qvk.aizwys.cn

Py:   asyncio.gather(*tasks)
来源：http://kxo.tanke756.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ksy.ppjwa.cn

JS:   await Promise.all(tasks)
来源：http://rfy.chenzaomai.com

TS:   await Promise.all(tasks)
来源：http://rrr.zhiwuduotai.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jhc.cucudq.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sqi.pengpengdd.cyou

Ruby: threads.map(&:join)
来源：http://uvt.yfazqb.com

C#:   await Task.WhenAll(t1, t2)
来源：http://yis.gotoacloud.top

[O06] 使用进程池
来源：http://obl.wangshuangyany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zih.xziqi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fme.jianghu66.top

JS:   // child_process / cluster 模块
来源：http://uwm.dashuyun.cn

TS:   // child_process / cluster 模块
来源：http://pyd.cqqwz.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://efr.sysykeji.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kod.zhixingplan.top

Ruby: // fork 块
来源：http://bjq.redwolf501.top

C#:   Parallel.For
来源：http://ube.nanxinkj.top

================================================================================
来源：http://wwp.hnxiangtu.top

P. 常用工具函数
来源：http://iox.yuanzhike.top

================================================================================
来源：http://axi.ywan-chungtsiang.top

[P01] 生成 UUID
来源：http://qha.birdmap.top

Py:   str(uuid.uuid4())
来源：http://xpt.uphjek.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ymy.birdmap.top

JS:   crypto.randomUUID()
来源：http://thz.dashuyun.cn

TS:   crypto.randomUUID()
来源：http://ipn.meibo888.top

Java: UUID.randomUUID().toString()
来源：http://aqs.shuidangran.top

Go:   // 用 github.com/google/uuid
来源：http://rrs.cashguo.top

Ruby: SecureRandom.uuid
来源：http://eft.fengsongda.top

C#:   Guid.NewGuid().ToString()
来源：http://lrz.jinghuilouyu.cn

[P02] MD5 / SHA256 摘要
来源：http://tig.yuxming.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lmq.tianlin.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://fyf.ctjpmb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yjj.gotoacloud.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://egp.havefunace.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fll.jqgufenzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ojv.ydjk.org.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dds.hesvh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wwk.shanyushiyangtech.top

[P03] 生成短随机字符串
来源：http://gab.jqgfzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://slf.wangdashe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://msi.ivvv.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iog.fktsv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mbj.yvedp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hej.vqdsnc.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zzm.fehbvm.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://gjn.cashguo.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zim.jinqigufen.top

[P04] 求长度
来源：http://goj.fzhhl.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yjg.xziqi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qtw.52xcode.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gwz.dianchejie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zno.xuanzx.com

Java: list.size();  map.size();  s.length()
来源：http://yjj.jinghuilouyu.cn

Go:   len(arr);  len(m)
来源：http://qbs.kuanghao11.cn

Ruby: x.length;  x.size
来源：http://uyr.bbcook.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vio.nwbrower.top

[P05] 判断两个对象内容是否相等
来源：http://szk.cashguo.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://wkh.svipenyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kqh.guowangkeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xkt.redwolf501.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eoa.sxryk.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://cwc.guannengcc.top

Go:   reflect.DeepEqual(a, b)
来源：http://ceh.xylfe.cn

Ruby: a == b
来源：http://gjq.meibo888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pjx.guowangkeji.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://eyv.zhaomingkeji.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bso.hnxiangtu.top

PHP:  if (empty($x)) {}
来源：http://ilm.shangyingyoupin.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ncp.ivvv.top

TS:   if (x == null) {}
来源：http://rpi.redwolf501.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wga.shuidangran.top

Go:   if x == nil {}
来源：http://zfv.zhengqikj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kvf.yanxiufei.cn

C#:   if (x is null) {}
来源：http://hnt.dianchejie.cn

[P07] 防抖与节流
来源：http://vbp.sweek.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://avg.andypj.xyz

PHP:  // 手写时间戳比较
来源：http://cso.chenzaomai.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dcg.yangfankeji.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wib.fktsv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jeh.xinyue.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fwd.hysaishi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nrm.pycfn.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pba.tian-w.cn

[P08] 处理浮点精度问题
来源：http://wlu.shanyushiyangkeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cuh.cdnleiting.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://znk.ppjwa.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ury.fehbvm.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ulf.jqgufenzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://doj.shangyingyoupin.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ind.yuxming.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://grw.9152youxi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://esk.yanxiufei.cn

================================================================================
来源：http://vji.yj20258.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hia.birdmap.top

================================================================================
来源：http://nap.bjfxy.top

[Q01] 创建表
来源：http://ows.zdbjq.cn

CREATE TABLE users (
来源：http://wek.xinyue.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vkj.jinqigfzy.top

name VARCHAR(50) NOT NULL,
来源：http://pka.epnwcf.com

email VARCHAR(100) UNIQUE,
来源：http://hhp.jyoumei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://oab.xuanzx.com

);
来源：http://xea.chenlongwang.top

[Q02] 创建带外键的表
来源：http://oca.chenzaomai.com

CREATE TABLE orders (
来源：http://dyu.aizwys.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fko.mhx1999.top

user_id INT NOT NULL,
来源：http://kot.shanyushiyangtech.top

amount DECIMAL(10, 2),
来源：http://zpg.shzxlz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://okq.jinghuilouyu.cn

);
来源：http://rje.yuanzhike.top

[Q03] 增加列
来源：http://dsq.zhongyouzk.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ihl.snrcjt.cn

[Q04] 修改列类型
来源：http://crt.nanxuanxn.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kbr.shangyingyoupin.top

[Q05] 重命名列
来源：http://ejs.jinqigufen.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tnk.daxiang520.top

[Q06] 删除列
来源：http://mwu.dashuyun.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ayc.zhongyouzk.top

[Q07] 删除表
来源：http://rpe.gzhubu.top

DROP TABLE IF EXISTS orders;
来源：http://wwy.andypj.xyz

[Q08] 创建普通索引
来源：http://ekh.wangdashe.top

CREATE INDEX idx_users_email ON users(email);
来源：http://xao.fehbvm.com

[Q09] 创建唯一索引
来源：http://xnx.shanyushiyangkeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bbj.xziqi.cn

[Q10] 插入单行
来源：http://sdn.guannengcc.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mva.zhixingplan.top

[Q11] 一次插入多行
来源：http://dba.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sft.wangshuangyany.cn

[Q12] 插入后取自增 ID
来源：http://kip.zdqjudy.top

INSERT INTO users (name) VALUES ('C');
来源：http://eoz.cdnleiting.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rok.haohaochexian.top

[Q13] 忽略重复插入
来源：http://fxu.zhijiandao.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uku.yanxiufei.cn

[Q14] 存在则更新（upsert）
来源：http://dxf.xuetiantiany.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lpk.cucudq.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zgo.uphjek.com

[Q15] 查询全部
来源：http://zzr.shuidangran.top

SELECT * FROM users;
来源：http://afz.aibaodan.cn

[Q16] 查询指定列
来源：http://xmy.ctjpmb.com

SELECT id, name FROM users;
来源：http://izl.gotoacloud.top

[Q17] 条件查询
来源：http://rpn.hesvh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qea.cucudq.cn

[Q18] 模糊匹配
来源：http://igi.hcnkem.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://usx.snrcjt.cn

[Q19] 范围查询
来源：http://qai.bbcook.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://oix.vehdjk.com

[Q20] IN 列表
来源：http://ply.guannengcc.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wbb.feifeiyinyue.top

[Q21] 空值判断
来源：http://xwd.feifeiyinyue.top

SELECT * FROM users WHERE email IS NULL;
来源：http://rdh.c1oappe.top

[Q22] 排序
来源：http://kac.yonumen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://aoq.316326.xyz

[Q23] 分页
来源：http://xdd.meibo888.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hru.tarul.cn

[Q24] 去重
来源：http://ntf.hesvh.cn

SELECT DISTINCT city FROM users;
来源：http://axc.shanyushiyangkeji.top

[Q25] 只取前 N 条
来源：http://sft.yanxiufei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dba.yongpay.top

[Q26] 计数
来源：http://efa.yongpay.top

SELECT COUNT(*) FROM users;
来源：http://jen.vqdsnc.cn

[Q27] 条件计数
来源：http://obn.chenlongwang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gpz.zhixingplan.top

[Q28] 求和与平均
来源：http://czu.ybcxt.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://oqw.zdqjudy.top

[Q29] 最大最小值
来源：http://sso.cucudq.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zrz.shanyushiyangkeji.top

[Q30] 分组统计
来源：http://snt.fengsongda.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tgy.sxryk.cn

[Q31] 分组后过滤
来源：http://yfr.redwolf501.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uet.fzhhl.top

[Q32] 分组拼接字符串
来源：http://udn.jiagoushi.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qxe.yj20258.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://kjc.zhiwuduotai.top

[Q33] 多列分组
来源：http://aoa.wangdashe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gol.fengsongda.top

[Q34] 每组取第一条
来源：http://etx.sysykeji.top

SELECT * FROM (
来源：http://say.jyoumei.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vdv.hcnkem.com

) t WHERE rn = 1;
来源：http://wbn.cqqwz.cn

[Q35] 内连接
来源：http://whl.sjlbkw.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://iiu.ppjwa.cn

[Q36] 左连接
来源：http://hvo.jinqigfzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wew.hywenlv.cn

[Q37] 右连接
来源：http://mht.yueranfly.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jwf.hywenlv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://txa.cheryme.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iae.fehbvm.com

[Q39] 自连接（查上下级）
来源：http://wqh.zhengqikj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wwi.dianchejie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xdn.hesvh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kip.dashuyun.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mxf.shzxlz.cn

[Q41] 多表连接
来源：http://heh.aibaodan.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jtb.fzhhl.top

JOIN users u ON u.id = o.user_id
来源：http://wrz.gaohongyu789.top

JOIN products p ON p.id = o.product_id;
来源：http://yia.gaohongyu789.top

[Q42] 连接条件附加过滤
来源：http://nff.andypj.xyz

SELECT u.name, o.amount FROM users u
来源：http://mcn.hesvh.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qcz.gotoacloud.top

[Q43] 标量子查询
来源：http://wlw.guowangkeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ldh.hfpthk.cn

[Q44] IN 子查询
来源：http://qij.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wwr.fengsongda.top

[Q45] EXISTS 判断存在
来源：http://hli.chenjidiqi.icu

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xui.cdnleiting.top

[Q46] NOT EXISTS 判断不存在
来源：http://mfd.shzxlz.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fju.jinqigufen.top

[Q47] 与平均值比较
来源：http://wzk.yuxming.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://opw.yj20258888.top

[Q48] CTE 公用表表达式
来源：http://rco.ydzc1.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hcs.hnxiangtu.top

SELECT * FROM t WHERE c > 5;
来源：http://pvk.quarkkingdee.top

[Q49] 更新单行
来源：http://uts.mhx1999.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sua.chenzaomai.com

[Q50] 批量更新
来源：http://rpn.dianchejie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yil.zdqjudy.top

[Q51] 用子查询更新
来源：http://awp.ydjk.org.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fdx.cashguo.top

[Q52] 删除指定行
来源：http://fmy.ydjk.org.cn

DELETE FROM users WHERE id = 10;
来源：http://hqz.xziqi.cn

[Q53] 按条件删除
来源：http://hbp.jyoumei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nif.fanxiaobao.xyz

[Q54] 清空表
来源：http://jju.yongpay.top

TRUNCATE TABLE logs;
来源：http://ufz.fehbvm.com

[Q55] 排名（并列占位）
来源：http://jqp.316326.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dja.xinyue.icu

[Q56] 密集排名（并列不占位）
来源：http://hbt.kuanghao11.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ggm.sjlbkw.cn

[Q57] 行号
来源：http://bcf.jyoumei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yyc.sysykeji.top

[Q58] 累计求和
来源：http://ugc.jianghu66.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ohp.hywenlv.cn

[Q59] 分组内累计
来源：http://sdf.vqdsnc.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nzi.cqqwz.cn

[Q60] 取上一行 / 下一行
来源：http://vmn.hfpthk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ezw.jinqigfzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ggq.jinyuanbaomall.cn

[Q61] 移动平均
来源：http://nqn.zhiwuduotai.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bnq.jinqigfzy.top

[Q62] 分组占比
来源：http://aap.cucudq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://obr.jqgufenzy.top


<!-- 参考信息 -->