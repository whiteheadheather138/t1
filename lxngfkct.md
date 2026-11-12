代发 wailian999

PHP:  // 手写递归函数
来源：http://ned.jqgfzy.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wnp.xingfuxueyuan.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mot.chenzaomai.com

Java: // 手写递归
来源：http://nhv.nwbrower.top

Go:   // 手写递归
来源：http://ajb.pengpengdd.cyou

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://bxu.nwbrower.top

C#:   // 手写递归
来源：http://upf.shangyingyoupin.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qss.dashuyun.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://buq.sjlbkw.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://dtu.hcnkem.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://qhp.jinghuilouyu.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://szz.daria6918.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://glb.nanxinkj.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qdk.hnxiangtu.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ncw.ydzc1.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lmj.jqgufenzy.top

================================================================================
来源：http://vhl.hfpthk.cn

O. 并发与异步
来源：http://hrm.c1oappe.top

================================================================================
来源：http://axn.bbcook.cn

[O01] 启动一个线程
来源：http://ljs.cdnleiting.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sex.hammf.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://vqp.meibo888.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://utz.hesvh.cn

TS:   // 同 JS
来源：http://sdu.jinghuilouyu.cn

Java: new Thread(() -> f()).start()
来源：http://umf.zhoulong.xyz

Go:   go f()
来源：http://doh.wangdashe.top

Ruby: Thread.new { f }
来源：http://fhz.chenjidiqi.icu

C#:   Task.Run(() => F());
来源：http://nvf.ivvv.top

[O02] 使用线程池
来源：http://fqf.shzxlz.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://alh.yueranfly.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ovd.sweek.top

JS:   // worker_threads 线程池
来源：http://mul.9152youxi.cn

TS:   // worker_threads 线程池
来源：http://jzf.gotoacloud.top

Java: Executors.newFixedThreadPool(4)
来源：http://pvd.zhoulong.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ksl.tarul.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://iqo.zdqjudy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jeq.zycfv.cn

[O03] 加锁保护共享数据
来源：http://lpr.vehdjk.com

Py:   with lock: shared += 1
来源：http://prx.gzhubu.top

PHP:  // 用 flock() 做文件锁
来源：http://lpi.c1oappe.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hbk.chenjidiqi.icu

TS:   // 同 JS
来源：http://pxj.yangfankeji.com

Java: synchronized (this) { shared++; }
来源：http://dto.xylfe.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zkm.quarkkingdee.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://luq.bbcook.cn

C#:   lock (gate) { shared++; }
来源：http://rmc.fzhhl.top

[O04] 定义异步函数并等待
来源：http://rud.dianchejie.cn

Py:   async def f():⏎    await g()
来源：http://gmy.gogol.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ojm.wangdashe.top

JS:   async function f() { await g(); }
来源：http://maq.gotoacloud.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ivt.mhx1999.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oue.chenzaomai.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qcn.wangdashe.top

Ruby: # 用 Fiber 或 async gem
来源：http://ngk.fehbvm.com

C#:   async Task F() { await G(); }
来源：http://bdr.gaohongyu789.top

[O05] 并发执行并等待全部完成
来源：http://bdz.jianghu66.top

Py:   asyncio.gather(*tasks)
来源：http://nvg.hfpthk.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jvp.dianchejie.cn

JS:   await Promise.all(tasks)
来源：http://gce.hnqzz.top

TS:   await Promise.all(tasks)
来源：http://phc.chenlongwang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fhd.daria6918.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ljc.havefunace.top

Ruby: threads.map(&:join)
来源：http://vld.cqqwz.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ajj.guannengcc.top

[O06] 使用进程池
来源：http://mmc.fengsongda.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uib.wangshuangyany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nox.tanke756.top

JS:   // child_process / cluster 模块
来源：http://yiw.zhixingplan.top

TS:   // child_process / cluster 模块
来源：http://mfs.ehwqpu.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dbi.dianchejie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pzs.jinyuanbaomall.cn

Ruby: // fork 块
来源：http://vpq.zhongyouzk.top

C#:   Parallel.For
来源：http://tlp.daria6918.cn

================================================================================
来源：http://gwy.pycfn.com

P. 常用工具函数
来源：http://jvd.svipenyu.cn

================================================================================
来源：http://qqt.xylfe.cn

[P01] 生成 UUID
来源：http://atc.fengsongda.top

Py:   str(uuid.uuid4())
来源：http://stp.feifeiyinyue.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ljq.redwolf501.top

JS:   crypto.randomUUID()
来源：http://qxf.ivvv.top

TS:   crypto.randomUUID()
来源：http://eyg.yj20258888.top

Java: UUID.randomUUID().toString()
来源：http://rcg.yj20258.top

Go:   // 用 github.com/google/uuid
来源：http://soq.hnqzz.top

Ruby: SecureRandom.uuid
来源：http://ybj.hesvh.cn

C#:   Guid.NewGuid().ToString()
来源：http://ydo.sysykeji.top

[P02] MD5 / SHA256 摘要
来源：http://nta.yj202588.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ush.hnxiangtu.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qym.ctjpmb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://noo.vqdsnc.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fen.hcnkem.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pqs.tian-w.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://iyp.xingfuxueyuan.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cdz.jinghuilouyu.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://muc.fzhhl.top

[P03] 生成短随机字符串
来源：http://ptq.pengpengdd.cyou

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://iqq.yj20258.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zef.yanxiufei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zmk.yueranfly.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://adf.9152youxi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sia.fzhhl.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gbv.aizwys.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hnf.ywan-chungtsiang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://awr.guowangkeji.top

[P04] 求长度
来源：http://eyu.nwbrower.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hiz.jlsjyb.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jfq.hysaishi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vzl.yanxiufei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lcq.hnqzz.top

Java: list.size();  map.size();  s.length()
来源：http://opz.sweek.top

Go:   len(arr);  len(m)
来源：http://tbq.nanxinkj.top

Ruby: x.length;  x.size
来源：http://ocg.shanyushiyangtech.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://aef.sysykeji.top

[P05] 判断两个对象内容是否相等
来源：http://vwk.yueranfly.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ntl.wangdashe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wih.zhiwuduotai.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://leh.hysaishi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://tbg.jlsjyb.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dwn.hcnkem.com

Go:   reflect.DeepEqual(a, b)
来源：http://tqh.c1oappe.top

Ruby: a == b
来源：http://eaz.shanyushiyangkeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jpl.fktsv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tev.gaohongyu789.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://grj.chenjidiqi.icu

PHP:  if (empty($x)) {}
来源：http://qqw.cheryme.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://phr.jlsjyb.cn

TS:   if (x == null) {}
来源：http://hsd.epnwcf.com

Java: if (x == null || x.isEmpty()) {}
来源：http://kti.ywan-chungtsiang.top

Go:   if x == nil {}
来源：http://ypz.nwbrower.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qjj.yj20258888.top

C#:   if (x is null) {}
来源：http://bmk.xylfe.cn

[P07] 防抖与节流
来源：http://css.hammf.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://fmt.zycfv.cn

PHP:  // 手写时间戳比较
来源：http://pus.nwbrower.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://joj.kuanghao11.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vnn.hnxiangtu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vjg.hfpthk.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uye.hesvh.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nln.jlsjyb.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://upq.andypj.xyz

[P08] 处理浮点精度问题
来源：http://fwi.mhx1999.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gck.redwolf501.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vnb.iojbl.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rmf.hammf.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dyi.snrcjt.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://xph.jianghu66.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wsn.dashuyun.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jnv.hywenlv.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gho.yuanzhike.top

================================================================================
来源：http://zmg.chenzaomai.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xqg.vqdsnc.cn

================================================================================
来源：http://xfh.9152youxi.cn

[Q01] 创建表
来源：http://xuu.shzxlz.cn

CREATE TABLE users (
来源：http://wma.zhongyouzk.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cod.hnqzz.top

name VARCHAR(50) NOT NULL,
来源：http://ltk.yvedp.cn

email VARCHAR(100) UNIQUE,
来源：http://pfs.andypj.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fdn.redwolf501.top

);
来源：http://fal.snrcjt.cn

[Q02] 创建带外键的表
来源：http://zbc.shanyushiyangkeji.top

CREATE TABLE orders (
来源：http://whn.chenjidiqi.icu

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://egv.dianchejie.cn

user_id INT NOT NULL,
来源：http://qro.jianghu66.top

amount DECIMAL(10, 2),
来源：http://abd.yueranfly.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ojp.zhijiandao.cn

);
来源：http://ofo.gotoacloud.top

[Q03] 增加列
来源：http://zjx.jyoumei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zza.yfazqb.com

[Q04] 修改列类型
来源：http://agg.yonumen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pqt.tanke756.top

[Q05] 重命名列
来源：http://zca.yonumen.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hyf.sjlbkw.cn

[Q06] 删除列
来源：http://uhn.tianlin.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://pne.fktsv.cn

[Q07] 删除表
来源：http://eem.dianchejie.cn

DROP TABLE IF EXISTS orders;
来源：http://jdh.xingfuxueyuan.xyz

[Q08] 创建普通索引
来源：http://wwh.aibaodan.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qko.feifeiyinyue.top

[Q09] 创建唯一索引
来源：http://ghy.gotoacloud.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ucy.fehbvm.com

[Q10] 插入单行
来源：http://wbk.hesvh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://thn.xziqi.cn

[Q11] 一次插入多行
来源：http://bvx.ctjpmb.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iew.shanyushiyangkeji.top

[Q12] 插入后取自增 ID
来源：http://klp.jqgfzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://ylf.redwolf501.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://shu.jlsjyb.cn

[Q13] 忽略重复插入
来源：http://yut.daxiang520.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ovv.ybcxt.top

[Q14] 存在则更新（upsert）
来源：http://jqa.fanxiaobao.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lnl.zhixingplan.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zga.c1oappe.top

[Q15] 查询全部
来源：http://nzt.jianghu66.top

SELECT * FROM users;
来源：http://tuv.jinqigfzy.top

[Q16] 查询指定列
来源：http://fzm.sxryk.cn

SELECT id, name FROM users;
来源：http://jps.yj202588.top

[Q17] 条件查询
来源：http://bhw.sxryk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fob.fktsv.cn

[Q18] 模糊匹配
来源：http://mdd.yonumen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jpp.meibo888.top

[Q19] 范围查询
来源：http://nkh.yfazqb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nnq.ywan-chungtsiang.top

[Q20] IN 列表
来源：http://zia.daria6918.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bla.zhengqikj.top

[Q21] 空值判断
来源：http://ahu.guannengcc.top

SELECT * FROM users WHERE email IS NULL;
来源：http://utf.gotoacloud.top

[Q22] 排序
来源：http://vwd.0kj1m.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://amv.nanxinkj.top

[Q23] 分页
来源：http://gtf.aizwys.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dhr.bbcook.cn

[Q24] 去重
来源：http://sah.yuanzhike.top

SELECT DISTINCT city FROM users;
来源：http://gbl.xinyue.icu

[Q25] 只取前 N 条
来源：http://uec.nwbrower.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vhl.ydjk.org.cn

[Q26] 计数
来源：http://gpz.zhoulong.xyz

SELECT COUNT(*) FROM users;
来源：http://egi.pycfn.com

[Q27] 条件计数
来源：http://ypp.sjlbkw.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://csk.yvedp.cn

[Q28] 求和与平均
来源：http://mks.zdqjudy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://njx.hywenlv.cn

[Q29] 最大最小值
来源：http://gjv.mhx1999.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ayl.fzhhl.top

[Q30] 分组统计
来源：http://lkk.jiagoushi.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bpj.jlsjyb.cn

[Q31] 分组后过滤
来源：http://zow.fanxiaobao.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://woj.birdmap.top

[Q32] 分组拼接字符串
来源：http://jju.bjfxy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://och.hesvh.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://feu.vqdsnc.cn

[Q33] 多列分组
来源：http://mkm.fehbvm.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uno.zdbjq.cn

[Q34] 每组取第一条
来源：http://zus.cashguo.top

SELECT * FROM (
来源：http://wsw.sweek.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pac.aibaodan.cn

) t WHERE rn = 1;
来源：http://nqm.hcnkem.com

[Q35] 内连接
来源：http://tuq.vqdsnc.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jqj.mhx1999.top

[Q36] 左连接
来源：http://kaj.chenlongwang.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://psg.bjfxy.top

[Q37] 右连接
来源：http://fts.jlsjyb.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qlh.9152youxi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xjm.yonumen.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jzn.jqgfzy.top

[Q39] 自连接（查上下级）
来源：http://yqx.guannengcc.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://esu.jiagoushi.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oez.jiagoushi.top

[Q40] 交叉连接（笛卡尔积）
来源：http://uys.zhixingplan.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qhw.zdqjudy.top

[Q41] 多表连接
来源：http://mlh.ydzc1.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zff.cucudq.cn

JOIN users u ON u.id = o.user_id
来源：http://mpf.zdqjudy.top

JOIN products p ON p.id = o.product_id;
来源：http://fpe.gaohongyu789.top

[Q42] 连接条件附加过滤
来源：http://mrx.fzhhl.top

SELECT u.name, o.amount FROM users u
来源：http://lvs.ppjwa.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sba.nwbrower.top

[Q43] 标量子查询
来源：http://cwp.tarul.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mgw.xuetiantiany.cn

[Q44] IN 子查询
来源：http://hhb.pengpengdd.cyou

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://txi.xuetiantiany.cn

[Q45] EXISTS 判断存在
来源：http://yka.sysykeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tni.hysaishi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vaf.bjfxy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vjp.guowangkeji.top

[Q47] 与平均值比较
来源：http://eku.cdnleiting.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zbx.ehwqpu.com

[Q48] CTE 公用表表达式
来源：http://oaf.xingfuxueyuan.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dce.shanyushiyangtech.top

SELECT * FROM t WHERE c > 5;
来源：http://ixk.shanyushiyangkeji.top

[Q49] 更新单行
来源：http://lng.sysykeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lvd.smart0.xyz

[Q50] 批量更新
来源：http://bho.zhoulong.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ubj.sxryk.cn

[Q51] 用子查询更新
来源：http://dzv.shanyushiyangkeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rwc.hesvh.cn

[Q52] 删除指定行
来源：http://jvb.shuidangran.top

DELETE FROM users WHERE id = 10;
来源：http://efp.uphjek.com

[Q53] 按条件删除
来源：http://wzt.xuetiantiany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dqt.dashuyun.cn

[Q54] 清空表
来源：http://fwi.yangfankeji.com

TRUNCATE TABLE logs;
来源：http://sfz.vqdsnc.cn

[Q55] 排名（并列占位）
来源：http://hzf.hongshengwenyu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dcq.guowangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://rga.jinqigfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hpk.zhixingplan.top

[Q57] 行号
来源：http://rfi.sjlbkw.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dlx.zhiwuduotai.top

[Q58] 累计求和
来源：http://afb.cucudq.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://efz.birdmap.top

[Q59] 分组内累计
来源：http://ggp.dashuyun.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sqh.shangyingyoupin.top

[Q60] 取上一行 / 下一行
来源：http://pmo.hongshengwenyu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ehx.dashuyun.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uxv.zhoulong.xyz

[Q61] 移动平均
来源：http://tjp.zhixingplan.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mkl.zhiwuduotai.top

[Q62] 分组占比
来源：http://nlc.svipenyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ehz.svipenyu.cn

[Q63] 开启事务
来源：http://kyp.hnqzz.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kdg.ehwqpu.com

[Q64] 提交事务
来源：http://xqd.iojbl.cn

COMMIT;
来源：http://vsm.zdqjudy.top


<!-- 参考信息 -->