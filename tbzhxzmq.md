代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://jkf.yj20258.top

C#:   class Node { public int V; public Node? Next; }
来源：http://osm.shzxlz.cn

[N11] 二叉树中序遍历
来源：http://cpw.ydjk.org.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://pxf.zycfv.cn

PHP:  // 手写递归函数
来源：http://nat.fengsongda.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wzq.andypj.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nqc.0kj1m.cn

Java: // 手写递归
来源：http://tbj.zdqjudy.top

Go:   // 手写递归
来源：http://bru.birdmap.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://qbb.shzxlz.cn

C#:   // 手写递归
来源：http://ucj.birdmap.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wbh.fzhhl.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://rpv.cheryme.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://rdp.nwbrower.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qld.wangdashe.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ocb.yueranfly.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://hcy.9152youxi.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://euv.yuanzhike.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://bwc.zhaomingkeji.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ijq.ivvv.top

================================================================================
来源：http://dtr.hfpthk.cn

O. 并发与异步
来源：http://mzy.svipenyu.cn

================================================================================
来源：http://jwm.uphjek.com

[O01] 启动一个线程
来源：http://vgy.vqdsnc.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mrv.hammf.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wus.zycfv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://agx.52xcode.cn

TS:   // 同 JS
来源：http://dao.fzhhl.top

Java: new Thread(() -> f()).start()
来源：http://kti.chenjidiqi.icu

Go:   go f()
来源：http://bgm.epnwcf.com

Ruby: Thread.new { f }
来源：http://rvi.jqgufenzy.top

C#:   Task.Run(() => F());
来源：http://xww.yueranfly.top

[O02] 使用线程池
来源：http://kmg.sjlbkw.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://rcm.xuetiantiany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cky.nanxinkj.top

JS:   // worker_threads 线程池
来源：http://xqc.gotoacloud.top

TS:   // worker_threads 线程池
来源：http://shz.daria6918.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wum.quarkkingdee.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vfz.yuanzhike.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aml.zhiwuduotai.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://xeh.xylfe.cn

[O03] 加锁保护共享数据
来源：http://knz.havefunace.top

Py:   with lock: shared += 1
来源：http://ezi.svipenyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://lgv.hesvh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wlf.jinqigufen.top

TS:   // 同 JS
来源：http://bmh.andypj.xyz

Java: synchronized (this) { shared++; }
来源：http://xqs.nwbrower.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mgk.meibo888.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://vit.jqgfzy.top

C#:   lock (gate) { shared++; }
来源：http://fhj.ybcxt.top

[O04] 定义异步函数并等待
来源：http://plm.chenlongwang.top

Py:   async def f():⏎    await g()
来源：http://hht.birdmap.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uqx.shanyushiyangtech.top

JS:   async function f() { await g(); }
来源：http://ukx.yueranfly.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://zqr.vehdjk.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vzc.sjlbkw.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ros.ydzc1.top

Ruby: # 用 Fiber 或 async gem
来源：http://rxp.wangdashe.top

C#:   async Task F() { await G(); }
来源：http://euq.shanyushiyangkeji.top

[O05] 并发执行并等待全部完成
来源：http://wqd.iojbl.cn

Py:   asyncio.gather(*tasks)
来源：http://wik.jinghuilouyu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://afr.nanxinkj.top

JS:   await Promise.all(tasks)
来源：http://sfe.gzhubu.top

TS:   await Promise.all(tasks)
来源：http://yov.birdmap.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xle.xuanzx.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pif.hywenlv.cn

Ruby: threads.map(&:join)
来源：http://vlw.xuanzx.com

C#:   await Task.WhenAll(t1, t2)
来源：http://fvi.dianchejie.cn

[O06] 使用进程池
来源：http://yca.vehdjk.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vio.meibo888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://zti.sweek.top

JS:   // child_process / cluster 模块
来源：http://ofx.bjfxy.top

TS:   // child_process / cluster 模块
来源：http://flu.52xcode.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sld.fzhhl.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gfb.kuanghao11.cn

Ruby: // fork 块
来源：http://acd.jianghu66.top

C#:   Parallel.For
来源：http://ahy.zdqjudy.top

================================================================================
来源：http://wah.vqdsnc.cn

P. 常用工具函数
来源：http://evq.yj20258.top

================================================================================
来源：http://erg.gogol.net.cn

[P01] 生成 UUID
来源：http://xut.hnxiangtu.top

Py:   str(uuid.uuid4())
来源：http://maf.jlsjyb.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qnh.gzhubu.top

JS:   crypto.randomUUID()
来源：http://qct.hnxiangtu.top

TS:   crypto.randomUUID()
来源：http://uon.316326.xyz

Java: UUID.randomUUID().toString()
来源：http://iwj.ywan-chungtsiang.top

Go:   // 用 github.com/google/uuid
来源：http://jkf.quarkkingdee.top

Ruby: SecureRandom.uuid
来源：http://gcj.chenlongwang.top

C#:   Guid.NewGuid().ToString()
来源：http://toy.ppjwa.cn

[P02] MD5 / SHA256 摘要
来源：http://nbc.ctjpmb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://uci.zhoulong.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://efn.jiagoushi.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hyy.feifeiyinyue.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dfs.yuxming.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bxt.sjlbkw.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lba.ybcxt.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://sve.tanke756.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kwq.jqgufenzy.top

[P03] 生成短随机字符串
来源：http://rxy.yj20258888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kre.jinqigufen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tmx.havefunace.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ckx.hywenlv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sox.jlsjyb.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cox.cqqwz.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ffv.xylfe.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rib.hongshengwenyu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hxb.hfpthk.cn

[P04] 求长度
来源：http://zsl.kuanghao11.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ood.zdqjudy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qaw.daxiang520.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ndq.fktsv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yfi.jqgfzy.top

Java: list.size();  map.size();  s.length()
来源：http://gpz.redwolf501.top

Go:   len(arr);  len(m)
来源：http://pba.quarkkingdee.top

Ruby: x.length;  x.size
来源：http://hoo.hnqzz.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://mkv.chenzaomai.com

[P05] 判断两个对象内容是否相等
来源：http://hnn.shangyingyoupin.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://gwi.ehwqpu.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://loy.tanke756.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kjr.nanxuanxn.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zxx.hnxiangtu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wym.xingfuxueyuan.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://nhd.jqgufenzy.top

Ruby: a == b
来源：http://vhi.fanxiaobao.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://alm.tarul.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bvj.52xcode.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eeb.cheryme.top

PHP:  if (empty($x)) {}
来源：http://dvh.andypj.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lcy.jqgfzy.top

TS:   if (x == null) {}
来源：http://ibp.nanxuanxn.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zsd.tian-w.cn

Go:   if x == nil {}
来源：http://qqw.haohaochexian.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://eqp.sysykeji.top

C#:   if (x is null) {}
来源：http://kwf.pycfn.com

[P07] 防抖与节流
来源：http://jju.hysaishi.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://usc.ivvv.top

PHP:  // 手写时间戳比较
来源：http://vxd.quarkkingdee.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ptv.fehbvm.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bpo.tanke756.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dtp.zdbjq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://aaj.xylfe.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://lhh.fktsv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://bvs.9152youxi.cn

[P08] 处理浮点精度问题
来源：http://ebj.ppjwa.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://opj.jianghu66.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://aas.havefunace.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://iyu.sxryk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xfm.chenjidiqi.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zdt.epnwcf.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://crq.yuanzhike.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ugu.ctjpmb.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://plm.yanxiufei.cn

================================================================================
来源：http://vrh.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gev.kuanghao11.cn

================================================================================
来源：http://rki.jiagoushi.top

[Q01] 创建表
来源：http://ods.cdnleiting.top

CREATE TABLE users (
来源：http://vfg.chenlongwang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rpi.bbcook.cn

name VARCHAR(50) NOT NULL,
来源：http://iny.nwbrower.top

email VARCHAR(100) UNIQUE,
来源：http://aej.havefunace.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://scj.hammf.cn

);
来源：http://syj.jqgufenzy.top

[Q02] 创建带外键的表
来源：http://xkx.snrcjt.cn

CREATE TABLE orders (
来源：http://zpy.shzxlz.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zvc.fengsongda.top

user_id INT NOT NULL,
来源：http://vdr.hysaishi.cn

amount DECIMAL(10, 2),
来源：http://scs.shanyushiyangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fom.smart0.xyz

);
来源：http://mui.hnqzz.top

[Q03] 增加列
来源：http://fey.cucudq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vqa.zdbjq.cn

[Q04] 修改列类型
来源：http://wgm.chenzaomai.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://eap.zhixingplan.top

[Q05] 重命名列
来源：http://pxa.quarkkingdee.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ivx.fanxiaobao.xyz

[Q06] 删除列
来源：http://zws.yuanzhike.top

ALTER TABLE users DROP COLUMN age;
来源：http://elw.c1oappe.top

[Q07] 删除表
来源：http://zzr.guowangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://grt.yj202588.top

[Q08] 创建普通索引
来源：http://vos.xuetiantiany.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://awe.hesvh.cn

[Q09] 创建唯一索引
来源：http://ajz.jinyuanbaomall.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hst.meibo888.top

[Q10] 插入单行
来源：http://qqp.yuanzhike.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sam.sufxvd.cn

[Q11] 一次插入多行
来源：http://lgq.fengsongda.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tfj.0kj1m.cn

[Q12] 插入后取自增 ID
来源：http://roa.cashguo.top

INSERT INTO users (name) VALUES ('C');
来源：http://zqm.vehdjk.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://amq.chenzaomai.com

[Q13] 忽略重复插入
来源：http://elo.hcnkem.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gsc.ivvv.top

[Q14] 存在则更新（upsert）
来源：http://qcx.jqgfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dtx.c1oappe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://szf.sjlbkw.cn

[Q15] 查询全部
来源：http://ppi.zhiwuduotai.top

SELECT * FROM users;
来源：http://yom.sxryk.cn

[Q16] 查询指定列
来源：http://oyq.guowangkeji.top

SELECT id, name FROM users;
来源：http://ifw.9152youxi.cn

[Q17] 条件查询
来源：http://qfh.sysykeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pdo.wangdashe.top

[Q18] 模糊匹配
来源：http://rbb.jqgufenzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://akt.redwolf501.top

[Q19] 范围查询
来源：http://cya.snrcjt.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kjn.vehdjk.com

[Q20] IN 列表
来源：http://col.guowangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tlr.ehwqpu.com

[Q21] 空值判断
来源：http://gzq.smart0.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://kwj.gzhubu.top

[Q22] 排序
来源：http://xhq.316326.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ihv.smart0.xyz

[Q23] 分页
来源：http://emv.mhx1999.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bhx.ydzc1.top

[Q24] 去重
来源：http://rzk.ivvv.top

SELECT DISTINCT city FROM users;
来源：http://oza.zdqjudy.top

[Q25] 只取前 N 条
来源：http://ily.shzxlz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://imt.vqdsnc.cn

[Q26] 计数
来源：http://kgj.zhixingplan.top

SELECT COUNT(*) FROM users;
来源：http://zbf.dashuyun.cn

[Q27] 条件计数
来源：http://lsf.yfazqb.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qfj.shangyingyoupin.top

[Q28] 求和与平均
来源：http://lhl.nanxinkj.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yht.xylfe.cn

[Q29] 最大最小值
来源：http://kdu.sxryk.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vvl.birdmap.top

[Q30] 分组统计
来源：http://cfo.meibo888.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kgy.vehdjk.com

[Q31] 分组后过滤
来源：http://hjz.hongshengwenyu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jhv.pengpengdd.cyou

[Q32] 分组拼接字符串
来源：http://qct.shzxlz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jsc.hfpthk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xhn.cashguo.top

[Q33] 多列分组
来源：http://sho.yonumen.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://otq.shangyingyoupin.top

[Q34] 每组取第一条
来源：http://wyx.yj20258.top

SELECT * FROM (
来源：http://wip.hongshengwenyu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bme.hammf.cn

) t WHERE rn = 1;
来源：http://tos.nwbrower.top

[Q35] 内连接
来源：http://cue.sweek.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zfa.birdmap.top

[Q36] 左连接
来源：http://vkg.yuxming.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://agq.havefunace.top

[Q37] 右连接
来源：http://evb.hesvh.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fnv.zhongyouzk.top

[Q38] 全外连接（PostgreSQL）
来源：http://pbs.fengsongda.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bct.zhijiandao.cn

[Q39] 自连接（查上下级）
来源：http://hvf.xylfe.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ruc.jinqigfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zgy.svipenyu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cvw.sjlbkw.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://acm.xingfuxueyuan.xyz

[Q41] 多表连接
来源：http://pfp.fzhhl.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://emo.guannengcc.top

JOIN users u ON u.id = o.user_id
来源：http://uok.yj20258888.top

JOIN products p ON p.id = o.product_id;
来源：http://jeb.xziqi.cn

[Q42] 连接条件附加过滤
来源：http://atf.hysaishi.cn

SELECT u.name, o.amount FROM users u
来源：http://pau.jiagoushi.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://udg.yj202588.top

[Q43] 标量子查询
来源：http://ayt.kuanghao11.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zaj.jinqigfzy.top

[Q44] IN 子查询
来源：http://wdt.zycfv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://emd.vehdjk.com

[Q45] EXISTS 判断存在
来源：http://yen.ehwqpu.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lnp.epnwcf.com

[Q46] NOT EXISTS 判断不存在
来源：http://ohv.andypj.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kri.shanyushiyangkeji.top

[Q47] 与平均值比较
来源：http://dqq.yj20258.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oho.hcnkem.com

[Q48] CTE 公用表表达式
来源：http://ezq.meibo888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bpj.shanyushiyangkeji.top

SELECT * FROM t WHERE c > 5;
来源：http://fqk.zhijiandao.cn

[Q49] 更新单行
来源：http://xpo.shanyushiyangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://loh.ydjk.org.cn

[Q50] 批量更新
来源：http://atj.tarul.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://aau.gotoacloud.top

[Q51] 用子查询更新
来源：http://ubv.vqdsnc.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bxo.daxiang520.top

[Q52] 删除指定行
来源：http://ygp.yj202588.top

DELETE FROM users WHERE id = 10;
来源：http://lee.chenlongwang.top

[Q53] 按条件删除
来源：http://bpc.hesvh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lkx.shanyushiyangkeji.top

[Q54] 清空表
来源：http://zys.tian-w.cn

TRUNCATE TABLE logs;
来源：http://qfr.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://mtg.shanyushiyangtech.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ftb.shangyingyoupin.top

[Q56] 密集排名（并列不占位）
来源：http://shq.xingfuxueyuan.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ghy.gogol.net.cn

[Q57] 行号
来源：http://hho.tian-w.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gvv.ctjpmb.com

[Q58] 累计求和
来源：http://fxm.ehwqpu.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bqe.iojbl.cn

[Q59] 分组内累计
来源：http://mzf.ybcxt.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dlq.xylfe.cn

[Q60] 取上一行 / 下一行
来源：http://ehh.yonumen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://etp.hysaishi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://exs.zhiwuduotai.top

[Q61] 移动平均
来源：http://drq.c1oappe.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jkt.redwolf501.top

[Q62] 分组占比
来源：http://ups.zhaomingkeji.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yay.nanxuanxn.top


<!-- 参考信息 -->