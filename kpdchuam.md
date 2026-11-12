代发 wailian999

PHP:  // 手写递归函数
来源：http://hjl.hnqzz.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eof.epnwcf.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fvx.tianlin.xyz

Java: // 手写递归
来源：http://cxn.ppjwa.cn

Go:   // 手写递归
来源：http://bsv.smart0.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xsb.bbcook.cn

C#:   // 手写递归
来源：http://arz.ydzc1.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ntp.andypj.xyz

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://clc.svipenyu.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kap.ctjpmb.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mtr.pengpengdd.cyou

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rwy.yvedp.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kel.jinyuanbaomall.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://lyt.xuetiantiany.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://yqk.ctjpmb.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lsc.mhx1999.top

================================================================================
来源：http://idr.vehdjk.com

O. 并发与异步
来源：http://eur.tarul.cn

================================================================================
来源：http://xes.c1oappe.top

[O01] 启动一个线程
来源：http://ojs.sweek.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://oyz.dianchejie.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://nph.gotoacloud.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://yln.dianchejie.cn

TS:   // 同 JS
来源：http://zuc.hywenlv.cn

Java: new Thread(() -> f()).start()
来源：http://alp.gaohongyu789.top

Go:   go f()
来源：http://xwk.smart0.xyz

Ruby: Thread.new { f }
来源：http://rml.aizwys.cn

C#:   Task.Run(() => F());
来源：http://xeb.aizwys.cn

[O02] 使用线程池
来源：http://plc.haohaochexian.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dxx.hcnkem.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://hro.xinyue.icu

JS:   // worker_threads 线程池
来源：http://qzq.chenjidiqi.icu

TS:   // worker_threads 线程池
来源：http://osp.daria6918.cn

Java: Executors.newFixedThreadPool(4)
来源：http://idk.hcnkem.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://nod.zhaomingkeji.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://uif.guannengcc.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ghv.xziqi.cn

[O03] 加锁保护共享数据
来源：http://gfz.xuetiantiany.cn

Py:   with lock: shared += 1
来源：http://azs.yuanzhike.top

PHP:  // 用 flock() 做文件锁
来源：http://zwf.gaohongyu789.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ols.c1oappe.top

TS:   // 同 JS
来源：http://igb.yonumen.top

Java: synchronized (this) { shared++; }
来源：http://ifo.yvedp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xhi.jinyuanbaomall.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lgf.fehbvm.com

C#:   lock (gate) { shared++; }
来源：http://dva.hnxiangtu.top

[O04] 定义异步函数并等待
来源：http://clw.pengpengdd.cyou

Py:   async def f():⏎    await g()
来源：http://cfu.kuanghao11.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zay.cqqwz.cn

JS:   async function f() { await g(); }
来源：http://gfk.hysaishi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://ajv.aizwys.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xav.yj20258.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://thu.mhx1999.top

Ruby: # 用 Fiber 或 async gem
来源：http://yud.xziqi.cn

C#:   async Task F() { await G(); }
来源：http://dwm.sysykeji.top

[O05] 并发执行并等待全部完成
来源：http://pvp.epnwcf.com

Py:   asyncio.gather(*tasks)
来源：http://xnx.wangdashe.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lyh.quarkkingdee.top

JS:   await Promise.all(tasks)
来源：http://egw.cucudq.cn

TS:   await Promise.all(tasks)
来源：http://kbu.ivvv.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://msj.epnwcf.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eaw.uphjek.com

Ruby: threads.map(&:join)
来源：http://wfm.iojbl.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qsd.sjlbkw.cn

[O06] 使用进程池
来源：http://aps.nwbrower.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gtx.birdmap.top

PHP:  // pcntl_fork 或多进程队列
来源：http://pqw.hongshengwenyu.top

JS:   // child_process / cluster 模块
来源：http://pgj.jlsjyb.cn

TS:   // child_process / cluster 模块
来源：http://lcj.xingfuxueyuan.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bls.cdnleiting.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ksu.ydjk.org.cn

Ruby: // fork 块
来源：http://aul.jqgfzy.top

C#:   Parallel.For
来源：http://big.xziqi.cn

================================================================================
来源：http://whb.zdqjudy.top

P. 常用工具函数
来源：http://pxd.hnqzz.top

================================================================================
来源：http://ykz.cdnleiting.top

[P01] 生成 UUID
来源：http://gyi.svipenyu.cn

Py:   str(uuid.uuid4())
来源：http://ntq.zdqjudy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ocu.daria6918.cn

JS:   crypto.randomUUID()
来源：http://jqd.chenlongwang.top

TS:   crypto.randomUUID()
来源：http://ofe.zhiwuduotai.top

Java: UUID.randomUUID().toString()
来源：http://nfp.yj20258888.top

Go:   // 用 github.com/google/uuid
来源：http://foy.yuanzhike.top

Ruby: SecureRandom.uuid
来源：http://kec.sysykeji.top

C#:   Guid.NewGuid().ToString()
来源：http://jos.yangfankeji.com

[P02] MD5 / SHA256 摘要
来源：http://gqx.ydzc1.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nli.xingfuxueyuan.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://kkf.52xcode.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qcw.yuanzhike.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hre.c1oappe.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fky.yj20258888.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rvn.zdqjudy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bpi.hnxiangtu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rjs.svipenyu.cn

[P03] 生成短随机字符串
来源：http://coj.jinyuanbaomall.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mlk.52xcode.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://yly.xziqi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gzl.fehbvm.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mqj.pengpengdd.cyou

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mea.pengpengdd.cyou

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mms.dashuyun.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lta.feifeiyinyue.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xsy.svipenyu.cn

[P04] 求长度
来源：http://pzy.dianchejie.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lpe.tarul.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vup.xylfe.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bpe.uphjek.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dmr.zhixingplan.top

Java: list.size();  map.size();  s.length()
来源：http://pqm.vehdjk.com

Go:   len(arr);  len(m)
来源：http://nzu.ydjk.org.cn

Ruby: x.length;  x.size
来源：http://tym.tarul.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tkc.jinghuilouyu.cn

[P05] 判断两个对象内容是否相等
来源：http://diu.chenjidiqi.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://xbz.fehbvm.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ndj.gzhubu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ybx.xuanzx.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sgv.jinyuanbaomall.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ien.c1oappe.top

Go:   reflect.DeepEqual(a, b)
来源：http://fva.sjlbkw.cn

Ruby: a == b
来源：http://fuh.zhaomingkeji.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gjj.hesvh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dbu.xingfuxueyuan.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oqk.yueranfly.top

PHP:  if (empty($x)) {}
来源：http://rzu.hnqzz.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ngq.yuxming.cn

TS:   if (x == null) {}
来源：http://zgp.haohaochexian.top

Java: if (x == null || x.isEmpty()) {}
来源：http://aor.wangshuangyany.cn

Go:   if x == nil {}
来源：http://kap.sysykeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ein.zdbjq.cn

C#:   if (x is null) {}
来源：http://baa.jinqigfzy.top

[P07] 防抖与节流
来源：http://sle.shangyingyoupin.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://joi.andypj.xyz

PHP:  // 手写时间戳比较
来源：http://gbn.xziqi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pdj.hesvh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mhx.ctjpmb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lca.jinyuanbaomall.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gaw.zhaomingkeji.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://kxs.yj202588.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dir.svipenyu.cn

[P08] 处理浮点精度问题
来源：http://cav.hnqzz.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xkx.meibo888.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pjm.jinqigufen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://noe.jiagoushi.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://odm.redwolf501.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ovi.xingfuxueyuan.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jpo.ehwqpu.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sue.yuxming.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zpo.fktsv.cn

================================================================================
来源：http://xlq.gaohongyu789.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oml.ctjpmb.com

================================================================================
来源：http://eok.epnwcf.com

[Q01] 创建表
来源：http://ult.andypj.xyz

CREATE TABLE users (
来源：http://jca.52xcode.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lqe.sufxvd.cn

name VARCHAR(50) NOT NULL,
来源：http://zqi.xziqi.cn

email VARCHAR(100) UNIQUE,
来源：http://oee.gotoacloud.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hrp.ppjwa.cn

);
来源：http://gdb.snrcjt.cn

[Q02] 创建带外键的表
来源：http://pbu.uphjek.com

CREATE TABLE orders (
来源：http://wyx.wangdashe.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jhl.ctjpmb.com

user_id INT NOT NULL,
来源：http://klb.feifeiyinyue.top

amount DECIMAL(10, 2),
来源：http://pah.jianghu66.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gzv.jqgfzy.top

);
来源：http://zbl.daxiang520.top

[Q03] 增加列
来源：http://lud.nwbrower.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gjh.hongshengwenyu.top

[Q04] 修改列类型
来源：http://ljl.ybcxt.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kta.wangshuangyany.cn

[Q05] 重命名列
来源：http://rde.gaohongyu789.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dvd.redwolf501.top

[Q06] 删除列
来源：http://yzj.gaohongyu789.top

ALTER TABLE users DROP COLUMN age;
来源：http://orj.wangdashe.top

[Q07] 删除表
来源：http://ajd.ctjpmb.com

DROP TABLE IF EXISTS orders;
来源：http://xis.fanxiaobao.xyz

[Q08] 创建普通索引
来源：http://ibc.snrcjt.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nsr.aibaodan.cn

[Q09] 创建唯一索引
来源：http://jvh.fktsv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vbv.wangshuangyany.cn

[Q10] 插入单行
来源：http://rxb.hesvh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wnh.tianlin.xyz

[Q11] 一次插入多行
来源：http://rjl.316326.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wmb.zycfv.cn

[Q12] 插入后取自增 ID
来源：http://aur.daxiang520.top

INSERT INTO users (name) VALUES ('C');
来源：http://cbs.xylfe.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mks.jiagoushi.top

[Q13] 忽略重复插入
来源：http://wgn.chenjidiqi.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hoj.chenlongwang.top

[Q14] 存在则更新（upsert）
来源：http://lau.chenjidiqi.icu

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sgq.yj20258888.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ajz.gzhubu.top

[Q15] 查询全部
来源：http://eak.epnwcf.com

SELECT * FROM users;
来源：http://muq.yangfankeji.com

[Q16] 查询指定列
来源：http://mgh.aizwys.cn

SELECT id, name FROM users;
来源：http://lib.bbcook.cn

[Q17] 条件查询
来源：http://otj.redwolf501.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bzu.gogol.net.cn

[Q18] 模糊匹配
来源：http://wnm.yvedp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://eht.0kj1m.cn

[Q19] 范围查询
来源：http://exe.kuanghao11.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lgo.chenjidiqi.icu

[Q20] IN 列表
来源：http://vbn.sysykeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ote.quarkkingdee.top

[Q21] 空值判断
来源：http://ioh.aibaodan.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sgu.cashguo.top

[Q22] 排序
来源：http://knv.haohaochexian.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tnn.shangyingyoupin.top

[Q23] 分页
来源：http://hsn.tianlin.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://teo.ivvv.top

[Q24] 去重
来源：http://vbw.sysykeji.top

SELECT DISTINCT city FROM users;
来源：http://vwi.yanxiufei.cn

[Q25] 只取前 N 条
来源：http://mwv.wangdashe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hio.sxryk.cn

[Q26] 计数
来源：http://rvv.zhiwuduotai.top

SELECT COUNT(*) FROM users;
来源：http://xaw.yj20258888.top

[Q27] 条件计数
来源：http://oda.zhoulong.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ikk.shzxlz.cn

[Q28] 求和与平均
来源：http://wat.guowangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yfg.chenzaomai.com

[Q29] 最大最小值
来源：http://ihb.ivvv.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://cil.sysykeji.top

[Q30] 分组统计
来源：http://wdf.xinyue.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bly.jyoumei.cn

[Q31] 分组后过滤
来源：http://rzf.xylfe.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qpi.sjlbkw.cn

[Q32] 分组拼接字符串
来源：http://qpo.dianchejie.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://aqq.cashguo.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gpp.guannengcc.top

[Q33] 多列分组
来源：http://fle.hesvh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kac.yj202588.top

[Q34] 每组取第一条
来源：http://yfo.epnwcf.com

SELECT * FROM (
来源：http://aug.yueranfly.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hqy.tianlin.xyz

) t WHERE rn = 1;
来源：http://vhp.cdnleiting.top

[Q35] 内连接
来源：http://snv.316326.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gyl.cheryme.top

[Q36] 左连接
来源：http://rxr.xziqi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vbs.pycfn.com

[Q37] 右连接
来源：http://mab.316326.xyz

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jqg.ydjk.org.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dav.fanxiaobao.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vkk.gogol.net.cn

[Q39] 自连接（查上下级）
来源：http://ols.hammf.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://oqr.tianlin.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mas.aibaodan.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vmo.hywenlv.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yuh.hfpthk.cn

[Q41] 多表连接
来源：http://lkp.jqgufenzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://tip.jianghu66.top

JOIN users u ON u.id = o.user_id
来源：http://mlx.zhaomingkeji.xyz

JOIN products p ON p.id = o.product_id;
来源：http://kpg.jinqigufen.top

[Q42] 连接条件附加过滤
来源：http://xvf.hongshengwenyu.top

SELECT u.name, o.amount FROM users u
来源：http://zic.zdbjq.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lrp.cqqwz.cn

[Q43] 标量子查询
来源：http://kns.chenzaomai.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sbq.chenzaomai.com

[Q44] IN 子查询
来源：http://uvl.andypj.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qgy.jinghuilouyu.cn

[Q45] EXISTS 判断存在
来源：http://cad.yangfankeji.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xwz.xinyue.icu

[Q46] NOT EXISTS 判断不存在
来源：http://ekm.nwbrower.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ces.zhengqikj.top

[Q47] 与平均值比较
来源：http://kyl.sjlbkw.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://okh.daxiang520.top

[Q48] CTE 公用表表达式
来源：http://nyk.zdqjudy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://voi.pycfn.com

SELECT * FROM t WHERE c > 5;
来源：http://qje.cdnleiting.top

[Q49] 更新单行
来源：http://bmc.sjlbkw.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ueu.chenzaomai.com

[Q50] 批量更新
来源：http://gum.sufxvd.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://izz.yuanzhike.top

[Q51] 用子查询更新
来源：http://bha.ydjk.org.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://btn.xziqi.cn

[Q52] 删除指定行
来源：http://tul.vqdsnc.cn

DELETE FROM users WHERE id = 10;
来源：http://dkv.pycfn.com

[Q53] 按条件删除
来源：http://cnb.jiagoushi.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wzu.yanxiufei.cn

[Q54] 清空表
来源：http://kzu.0kj1m.cn

TRUNCATE TABLE logs;
来源：http://oat.9152youxi.cn

[Q55] 排名（并列占位）
来源：http://ffm.hongshengwenyu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bpi.shanyushiyangtech.top

[Q56] 密集排名（并列不占位）
来源：http://mom.yuxming.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hoy.316326.xyz

[Q57] 行号
来源：http://jph.pycfn.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tal.kuanghao11.cn

[Q58] 累计求和
来源：http://xsh.xylfe.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tuk.fzhhl.top

[Q59] 分组内累计
来源：http://lfu.cheryme.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uvq.zycfv.cn

[Q60] 取上一行 / 下一行
来源：http://lgz.hfpthk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cas.shangyingyoupin.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sxq.feifeiyinyue.top

[Q61] 移动平均
来源：http://fgj.hnqzz.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zwj.quarkkingdee.top

[Q62] 分组占比
来源：http://wtj.wangshuangyany.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wam.tianlin.xyz

[Q63] 开启事务
来源：http://xik.yfazqb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://odu.havefunace.top

[Q64] 提交事务
来源：http://lpn.yanxiufei.cn

COMMIT;
来源：http://mwj.dianchejie.cn


<!-- 参考信息 -->