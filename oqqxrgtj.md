代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://vak.jyoumei.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://tir.aizwys.cn

[N11] 二叉树中序遍历
来源：http://krt.hywenlv.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://dbd.tanke756.top

PHP:  // 手写递归函数
来源：http://dom.c1oappe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://zkr.sysykeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://otv.chenjidiqi.icu

Java: // 手写递归
来源：http://zvy.nanxuanxn.top

Go:   // 手写递归
来源：http://gwo.redwolf501.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dsx.hfpthk.cn

C#:   // 手写递归
来源：http://mus.jinyuanbaomall.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://omd.fktsv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fvv.bbcook.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wys.ctjpmb.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ryc.shuidangran.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ekl.gogol.net.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ykz.dianchejie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rwv.sjlbkw.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://tla.9152youxi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tvx.xziqi.cn

================================================================================
来源：http://yhq.shuidangran.top

O. 并发与异步
来源：http://abi.hnqzz.top

================================================================================
来源：http://mej.yuxming.cn

[O01] 启动一个线程
来源：http://bzg.wangdashe.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://noi.jinyuanbaomall.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://msq.hesvh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ruc.tarul.cn

TS:   // 同 JS
来源：http://umw.yangfankeji.com

Java: new Thread(() -> f()).start()
来源：http://iqn.xinyue.icu

Go:   go f()
来源：http://qki.zhaomingkeji.xyz

Ruby: Thread.new { f }
来源：http://hta.snrcjt.cn

C#:   Task.Run(() => F());
来源：http://znn.chenzaomai.com

[O02] 使用线程池
来源：http://tgq.0kj1m.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://crr.gogol.net.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hxs.sxryk.cn

JS:   // worker_threads 线程池
来源：http://ndg.zhiwuduotai.top

TS:   // worker_threads 线程池
来源：http://uco.smart0.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://iui.chenjidiqi.icu

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oqh.sweek.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://equ.jinqigufen.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://izo.yfazqb.com

[O03] 加锁保护共享数据
来源：http://mcf.jiagoushi.top

Py:   with lock: shared += 1
来源：http://lat.fktsv.cn

PHP:  // 用 flock() 做文件锁
来源：http://udu.yj20258.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jga.redwolf501.top

TS:   // 同 JS
来源：http://jss.chenjidiqi.icu

Java: synchronized (this) { shared++; }
来源：http://rhf.tanke756.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tbg.feifeiyinyue.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://iqt.hcnkem.com

C#:   lock (gate) { shared++; }
来源：http://hlm.pengpengdd.cyou

[O04] 定义异步函数并等待
来源：http://ban.aibaodan.cn

Py:   async def f():⏎    await g()
来源：http://hnk.ehwqpu.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ono.zhengqikj.top

JS:   async function f() { await g(); }
来源：http://igv.guannengcc.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://wyb.zhongyouzk.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nwf.chenzaomai.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ghe.zhengqikj.top

Ruby: # 用 Fiber 或 async gem
来源：http://trk.xingfuxueyuan.xyz

C#:   async Task F() { await G(); }
来源：http://eyh.ybcxt.top

[O05] 并发执行并等待全部完成
来源：http://ndq.yueranfly.top

Py:   asyncio.gather(*tasks)
来源：http://cvm.sufxvd.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://khv.chenzaomai.com

JS:   await Promise.all(tasks)
来源：http://eec.mhx1999.top

TS:   await Promise.all(tasks)
来源：http://kcy.sweek.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mcl.hnxiangtu.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oof.jlsjyb.cn

Ruby: threads.map(&:join)
来源：http://kxp.yj20258888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fic.gogol.net.cn

[O06] 使用进程池
来源：http://olk.yj202588.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xhr.hongshengwenyu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://tfy.mhx1999.top

JS:   // child_process / cluster 模块
来源：http://vum.fktsv.cn

TS:   // child_process / cluster 模块
来源：http://cko.zhixingplan.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ywn.yuanzhike.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zib.xingfuxueyuan.xyz

Ruby: // fork 块
来源：http://qnl.hywenlv.cn

C#:   Parallel.For
来源：http://vdq.fanxiaobao.xyz

================================================================================
来源：http://cyy.hysaishi.cn

P. 常用工具函数
来源：http://eog.cdnleiting.top

================================================================================
来源：http://gyp.snrcjt.cn

[P01] 生成 UUID
来源：http://sac.zhaomingkeji.xyz

Py:   str(uuid.uuid4())
来源：http://wwk.jyoumei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gwl.tian-w.cn

JS:   crypto.randomUUID()
来源：http://rio.zhijiandao.cn

TS:   crypto.randomUUID()
来源：http://pio.xinyue.icu

Java: UUID.randomUUID().toString()
来源：http://lrf.9152youxi.cn

Go:   // 用 github.com/google/uuid
来源：http://nua.meibo888.top

Ruby: SecureRandom.uuid
来源：http://mcu.vehdjk.com

C#:   Guid.NewGuid().ToString()
来源：http://pej.ydjk.org.cn

[P02] MD5 / SHA256 摘要
来源：http://iwa.cheryme.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mxy.zdqjudy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vsv.cdnleiting.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://avy.jlsjyb.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://avq.haohaochexian.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ryx.0kj1m.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uwh.chenjidiqi.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://afq.cheryme.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hpp.shangyingyoupin.top

[P03] 生成短随机字符串
来源：http://bcf.tanke756.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jox.tian-w.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jku.zhengqikj.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rgk.fehbvm.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yyp.kuanghao11.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://crb.shangyingyoupin.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pqh.hfpthk.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://oyi.zhongyouzk.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dlu.chenlongwang.top

[P04] 求长度
来源：http://kxr.fanxiaobao.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://aai.dianchejie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://njq.0kj1m.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nfk.zycfv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uhr.vehdjk.com

Java: list.size();  map.size();  s.length()
来源：http://mow.sjlbkw.cn

Go:   len(arr);  len(m)
来源：http://xsb.birdmap.top

Ruby: x.length;  x.size
来源：http://uyu.c1oappe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zrz.vqdsnc.cn

[P05] 判断两个对象内容是否相等
来源：http://lqm.dashuyun.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://oia.cqqwz.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ylp.mhx1999.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://aky.0kj1m.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eov.ivvv.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://lgh.zhiwuduotai.top

Go:   reflect.DeepEqual(a, b)
来源：http://yfh.smart0.xyz

Ruby: a == b
来源：http://ynh.shuidangran.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jmz.wangdashe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gsu.feifeiyinyue.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lep.yj20258888.top

PHP:  if (empty($x)) {}
来源：http://niz.xinyue.icu

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vyv.guowangkeji.top

TS:   if (x == null) {}
来源：http://pby.yonumen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wkr.zhixingplan.top

Go:   if x == nil {}
来源：http://tlc.hcnkem.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://piu.yfazqb.com

C#:   if (x is null) {}
来源：http://aro.meibo888.top

[P07] 防抖与节流
来源：http://vbo.tarul.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rfk.cashguo.top

PHP:  // 手写时间戳比较
来源：http://agd.cucudq.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://man.smart0.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://foe.0kj1m.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hyc.birdmap.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jht.ydjk.org.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pkz.bbcook.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://buk.hammf.cn

[P08] 处理浮点精度问题
来源：http://opo.yonumen.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hzy.zhijiandao.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wvy.shanyushiyangkeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://von.ctjpmb.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zex.0kj1m.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iwa.guannengcc.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ief.gogol.net.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ebv.yj20258888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cdc.yangfankeji.com

================================================================================
来源：http://eru.c1oappe.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ton.shanyushiyangtech.top

================================================================================
来源：http://iua.zycfv.cn

[Q01] 创建表
来源：http://evb.epnwcf.com

CREATE TABLE users (
来源：http://jrz.fanxiaobao.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://erb.shanyushiyangtech.top

name VARCHAR(50) NOT NULL,
来源：http://cab.sufxvd.cn

email VARCHAR(100) UNIQUE,
来源：http://mxr.epnwcf.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://giw.yj202588.top

);
来源：http://rnk.xuetiantiany.cn

[Q02] 创建带外键的表
来源：http://nbb.zhaomingkeji.xyz

CREATE TABLE orders (
来源：http://rrz.yj202588.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://llp.uphjek.com

user_id INT NOT NULL,
来源：http://yiz.ybcxt.top

amount DECIMAL(10, 2),
来源：http://stl.jlsjyb.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://brc.sjlbkw.cn

);
来源：http://xrl.xziqi.cn

[Q03] 增加列
来源：http://hri.fktsv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kdi.jinyuanbaomall.cn

[Q04] 修改列类型
来源：http://vxr.shangyingyoupin.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ywa.aibaodan.cn

[Q05] 重命名列
来源：http://jpa.yfazqb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mdn.jyoumei.cn

[Q06] 删除列
来源：http://vjd.gogol.net.cn

ALTER TABLE users DROP COLUMN age;
来源：http://sol.ydzc1.top

[Q07] 删除表
来源：http://zvk.zhijiandao.cn

DROP TABLE IF EXISTS orders;
来源：http://dzl.shanyushiyangkeji.top

[Q08] 创建普通索引
来源：http://boi.xylfe.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ohw.yuxming.cn

[Q09] 创建唯一索引
来源：http://ldf.yueranfly.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xmr.yuanzhike.top

[Q10] 插入单行
来源：http://uci.haohaochexian.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://urs.chenzaomai.com

[Q11] 一次插入多行
来源：http://fsm.yuxming.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ebs.zdbjq.cn

[Q12] 插入后取自增 ID
来源：http://bso.zhengqikj.top

INSERT INTO users (name) VALUES ('C');
来源：http://cyp.52xcode.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qll.cheryme.top

[Q13] 忽略重复插入
来源：http://kco.ydjk.org.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://suu.xingfuxueyuan.xyz

[Q14] 存在则更新（upsert）
来源：http://hsk.sysykeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gva.dianchejie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qmz.gogol.net.cn

[Q15] 查询全部
来源：http://blw.vehdjk.com

SELECT * FROM users;
来源：http://qpx.yongpay.top

[Q16] 查询指定列
来源：http://llp.guowangkeji.top

SELECT id, name FROM users;
来源：http://uzd.yangfankeji.com

[Q17] 条件查询
来源：http://mru.zdbjq.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xvd.jianghu66.top

[Q18] 模糊匹配
来源：http://bnl.cdnleiting.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qel.hcnkem.com

[Q19] 范围查询
来源：http://wes.bbcook.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hsk.zhixingplan.top

[Q20] IN 列表
来源：http://teq.cashguo.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://igr.daria6918.cn

[Q21] 空值判断
来源：http://lpw.aibaodan.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://dwk.aibaodan.cn

[Q22] 排序
来源：http://ctt.zycfv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ddm.nwbrower.top

[Q23] 分页
来源：http://arj.0kj1m.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vdw.yuanzhike.top

[Q24] 去重
来源：http://ler.yongpay.top

SELECT DISTINCT city FROM users;
来源：http://lmt.9152youxi.cn

[Q25] 只取前 N 条
来源：http://lgz.shanyushiyangtech.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ltl.xingfuxueyuan.xyz

[Q26] 计数
来源：http://kni.zhoulong.xyz

SELECT COUNT(*) FROM users;
来源：http://dml.fengsongda.top

[Q27] 条件计数
来源：http://wfs.shuidangran.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://btt.yj202588.top

[Q28] 求和与平均
来源：http://fmr.gotoacloud.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://omk.hcnkem.com

[Q29] 最大最小值
来源：http://vfi.xziqi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zuw.sweek.top

[Q30] 分组统计
来源：http://gzi.gogol.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zhi.cqqwz.cn

[Q31] 分组后过滤
来源：http://jeh.hcnkem.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hfg.fehbvm.com

[Q32] 分组拼接字符串
来源：http://gnr.yueranfly.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ohs.jqgfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xiu.xziqi.cn

[Q33] 多列分组
来源：http://viy.jianghu66.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mhc.tian-w.cn

[Q34] 每组取第一条
来源：http://yqj.aibaodan.cn

SELECT * FROM (
来源：http://qgf.jinyuanbaomall.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ido.sweek.top

) t WHERE rn = 1;
来源：http://mvl.zhiwuduotai.top

[Q35] 内连接
来源：http://heg.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oie.hongshengwenyu.top

[Q36] 左连接
来源：http://ubw.haohaochexian.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://amy.shangyingyoupin.top

[Q37] 右连接
来源：http://xde.iojbl.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://twi.yonumen.top

[Q38] 全外连接（PostgreSQL）
来源：http://inj.gogol.net.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hkx.shanyushiyangtech.top

[Q39] 自连接（查上下级）
来源：http://xig.andypj.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://wct.redwolf501.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xan.jyoumei.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vgj.xziqi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vuc.ctjpmb.com

[Q41] 多表连接
来源：http://lcw.zhongyouzk.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://nkz.chenzaomai.com

JOIN users u ON u.id = o.user_id
来源：http://hfu.ydzc1.top

JOIN products p ON p.id = o.product_id;
来源：http://mqg.gotoacloud.top

[Q42] 连接条件附加过滤
来源：http://amu.shangyingyoupin.top

SELECT u.name, o.amount FROM users u
来源：http://fyv.hysaishi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mhf.dashuyun.cn

[Q43] 标量子查询
来源：http://zrn.yj20258.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mqt.hnxiangtu.top

[Q44] IN 子查询
来源：http://uxj.shzxlz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xjm.aizwys.cn

[Q45] EXISTS 判断存在
来源：http://rww.hcnkem.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nel.svipenyu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rid.wangshuangyany.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fxi.smart0.xyz

[Q47] 与平均值比较
来源：http://eui.fengsongda.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xcq.hongshengwenyu.top

[Q48] CTE 公用表表达式
来源：http://idt.chenlongwang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wvz.uphjek.com

SELECT * FROM t WHERE c > 5;
来源：http://bxy.ehwqpu.com

[Q49] 更新单行
来源：http://fxj.meibo888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xog.xingfuxueyuan.xyz

[Q50] 批量更新
来源：http://aga.jiagoushi.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dpi.tanke756.top

[Q51] 用子查询更新
来源：http://reh.zhengqikj.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://chs.smart0.xyz

[Q52] 删除指定行
来源：http://fyg.yuanzhike.top

DELETE FROM users WHERE id = 10;
来源：http://kuk.wangdashe.top

[Q53] 按条件删除
来源：http://thq.jiagoushi.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ubb.snrcjt.cn

[Q54] 清空表
来源：http://mdi.bbcook.cn

TRUNCATE TABLE logs;
来源：http://axh.zycfv.cn

[Q55] 排名（并列占位）
来源：http://bal.fzhhl.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pji.gogol.net.cn

[Q56] 密集排名（并列不占位）
来源：http://quv.sjlbkw.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pod.fanxiaobao.xyz

[Q57] 行号
来源：http://wiy.sweek.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rxv.ehwqpu.com

[Q58] 累计求和
来源：http://chc.zhengqikj.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bvy.zhaomingkeji.xyz

[Q59] 分组内累计
来源：http://fez.52xcode.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cev.fehbvm.com

[Q60] 取上一行 / 下一行
来源：http://vdg.snrcjt.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://eop.shanyushiyangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sqs.yj20258.top

[Q61] 移动平均
来源：http://lxw.pycfn.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oob.sxryk.cn

[Q62] 分组占比
来源：http://ujz.wangdashe.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tdj.pengpengdd.cyou


<!-- 参考信息 -->