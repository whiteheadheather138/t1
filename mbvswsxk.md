代发 wailian999

PHP:  // 手写递归函数
来源：http://yqv.ivvv.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://shw.shzxlz.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nov.yanxiufei.cn

Java: // 手写递归
来源：http://kmo.shuidangran.top

Go:   // 手写递归
来源：http://tze.yvedp.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://kix.pengpengdd.cyou

C#:   // 手写递归
来源：http://gbt.hnqzz.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://avu.bbcook.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ngz.yvedp.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pkc.yj202588.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uav.jinqigufen.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bvr.xuetiantiany.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://riq.meibo888.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://jnm.sjlbkw.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gyx.shanyushiyangkeji.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wmu.zdbjq.cn

================================================================================
来源：http://wos.tanke756.top

O. 并发与异步
来源：http://anb.andypj.xyz

================================================================================
来源：http://etz.jiagoushi.top

[O01] 启动一个线程
来源：http://moy.cheryme.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ccb.ppjwa.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gmv.jianghu66.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://zyi.ctjpmb.com

TS:   // 同 JS
来源：http://egc.yonumen.top

Java: new Thread(() -> f()).start()
来源：http://pyv.smart0.xyz

Go:   go f()
来源：http://pzz.xingfuxueyuan.xyz

Ruby: Thread.new { f }
来源：http://eex.jinqigufen.top

C#:   Task.Run(() => F());
来源：http://rpn.vqdsnc.cn

[O02] 使用线程池
来源：http://gsl.gaohongyu789.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://sfh.hnxiangtu.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://snb.kuanghao11.cn

JS:   // worker_threads 线程池
来源：http://xrw.yangfankeji.com

TS:   // worker_threads 线程池
来源：http://vpn.yfazqb.com

Java: Executors.newFixedThreadPool(4)
来源：http://ehc.shangyingyoupin.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lzj.bbcook.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xqe.ctjpmb.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://iso.tarul.cn

[O03] 加锁保护共享数据
来源：http://bqw.vehdjk.com

Py:   with lock: shared += 1
来源：http://wvo.shuidangran.top

PHP:  // 用 flock() 做文件锁
来源：http://yau.shanyushiyangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://lun.52xcode.cn

TS:   // 同 JS
来源：http://oag.hysaishi.cn

Java: synchronized (this) { shared++; }
来源：http://jpi.jiagoushi.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://iud.yuanzhike.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://vim.wangshuangyany.cn

C#:   lock (gate) { shared++; }
来源：http://mvi.shuidangran.top

[O04] 定义异步函数并等待
来源：http://dcw.cdnleiting.top

Py:   async def f():⏎    await g()
来源：http://owl.havefunace.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ayb.cheryme.top

JS:   async function f() { await g(); }
来源：http://hlb.haohaochexian.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://uxi.c1oappe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://err.quarkkingdee.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://juw.bjfxy.top

Ruby: # 用 Fiber 或 async gem
来源：http://vuj.wangdashe.top

C#:   async Task F() { await G(); }
来源：http://qut.xylfe.cn

[O05] 并发执行并等待全部完成
来源：http://ilp.shangyingyoupin.top

Py:   asyncio.gather(*tasks)
来源：http://trq.jqgufenzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dce.hywenlv.cn

JS:   await Promise.all(tasks)
来源：http://tvm.yj20258.top

TS:   await Promise.all(tasks)
来源：http://vaz.daxiang520.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yok.guowangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rly.xuanzx.com

Ruby: threads.map(&:join)
来源：http://ujq.jqgufenzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://afx.yfazqb.com

[O06] 使用进程池
来源：http://wut.jinghuilouyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wko.andypj.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://jyf.yangfankeji.com

JS:   // child_process / cluster 模块
来源：http://llm.xinyue.icu

TS:   // child_process / cluster 模块
来源：http://wsq.iojbl.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qwr.havefunace.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gcv.hnxiangtu.top

Ruby: // fork 块
来源：http://ihg.mhx1999.top

C#:   Parallel.For
来源：http://owc.zhixingplan.top

================================================================================
来源：http://abe.xuanzx.com

P. 常用工具函数
来源：http://xwg.svipenyu.cn

================================================================================
来源：http://oxw.kuanghao11.cn

[P01] 生成 UUID
来源：http://khm.ivvv.top

Py:   str(uuid.uuid4())
来源：http://gdf.hysaishi.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xpp.hesvh.cn

JS:   crypto.randomUUID()
来源：http://vvh.316326.xyz

TS:   crypto.randomUUID()
来源：http://yfy.wangdashe.top

Java: UUID.randomUUID().toString()
来源：http://kbc.hywenlv.cn

Go:   // 用 github.com/google/uuid
来源：http://acl.guowangkeji.top

Ruby: SecureRandom.uuid
来源：http://oro.chenzaomai.com

C#:   Guid.NewGuid().ToString()
来源：http://dxd.wangdashe.top

[P02] MD5 / SHA256 摘要
来源：http://fsr.svipenyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://noh.fanxiaobao.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://qpr.gogol.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jyq.hcnkem.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ody.sysykeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rhs.fktsv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yul.hywenlv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tgk.snrcjt.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nxu.xinyue.icu

[P03] 生成短随机字符串
来源：http://hbg.snrcjt.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://atb.jlsjyb.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eik.zhijiandao.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bmi.hcnkem.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lnk.feifeiyinyue.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xxf.52xcode.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iwl.yanxiufei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rdx.hnxiangtu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://apr.xylfe.cn

[P04] 求长度
来源：http://goj.birdmap.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fpy.dashuyun.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tpd.cucudq.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qxv.aibaodan.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qmo.fehbvm.com

Java: list.size();  map.size();  s.length()
来源：http://eti.zhengqikj.top

Go:   len(arr);  len(m)
来源：http://ijb.xylfe.cn

Ruby: x.length;  x.size
来源：http://kyc.yuxming.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hhq.vqdsnc.cn

[P05] 判断两个对象内容是否相等
来源：http://xif.dashuyun.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://krx.jinyuanbaomall.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wug.fktsv.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zlu.zhixingplan.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sjn.cheryme.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zkt.yanxiufei.cn

Go:   reflect.DeepEqual(a, b)
来源：http://hym.dianchejie.cn

Ruby: a == b
来源：http://lqu.zhongyouzk.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bcs.chenlongwang.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bve.hfpthk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iqp.zhaomingkeji.xyz

PHP:  if (empty($x)) {}
来源：http://bst.zycfv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uhy.jqgfzy.top

TS:   if (x == null) {}
来源：http://nnq.cucudq.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://mfa.jinghuilouyu.cn

Go:   if x == nil {}
来源：http://dze.yvedp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dkr.tianlin.xyz

C#:   if (x is null) {}
来源：http://dzy.jinghuilouyu.cn

[P07] 防抖与节流
来源：http://typ.vqdsnc.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lzx.aibaodan.cn

PHP:  // 手写时间戳比较
来源：http://kdu.hammf.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rvv.bbcook.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jue.chenjidiqi.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pfe.aizwys.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cft.cashguo.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ezv.vehdjk.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oqu.hammf.cn

[P08] 处理浮点精度问题
来源：http://gtt.snrcjt.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://iqu.bbcook.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fhg.hfpthk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://saw.shanyushiyangtech.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wto.andypj.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gph.yonumen.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qug.nwbrower.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ten.yj202588.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lwj.sxryk.cn

================================================================================
来源：http://pbx.yangfankeji.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mbr.tanke756.top

================================================================================
来源：http://akn.chenlongwang.top

[Q01] 创建表
来源：http://pft.316326.xyz

CREATE TABLE users (
来源：http://woj.feifeiyinyue.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dxh.snrcjt.cn

name VARCHAR(50) NOT NULL,
来源：http://uzv.xylfe.cn

email VARCHAR(100) UNIQUE,
来源：http://dqn.yonumen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jct.52xcode.cn

);
来源：http://utl.chenzaomai.com

[Q02] 创建带外键的表
来源：http://txv.smart0.xyz

CREATE TABLE orders (
来源：http://rbo.fehbvm.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://svi.ehwqpu.com

user_id INT NOT NULL,
来源：http://nsi.jlsjyb.cn

amount DECIMAL(10, 2),
来源：http://npt.meibo888.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://prm.hcnkem.com

);
来源：http://egd.52xcode.cn

[Q03] 增加列
来源：http://fce.zhaomingkeji.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gps.hywenlv.cn

[Q04] 修改列类型
来源：http://nih.cdnleiting.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kpl.sweek.top

[Q05] 重命名列
来源：http://hrd.tianlin.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://spu.shzxlz.cn

[Q06] 删除列
来源：http://tds.ydzc1.top

ALTER TABLE users DROP COLUMN age;
来源：http://gnf.jinqigfzy.top

[Q07] 删除表
来源：http://dvu.sxryk.cn

DROP TABLE IF EXISTS orders;
来源：http://det.feifeiyinyue.top

[Q08] 创建普通索引
来源：http://vmu.zdbjq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://osv.daria6918.cn

[Q09] 创建唯一索引
来源：http://tpu.daria6918.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blu.pengpengdd.cyou

[Q10] 插入单行
来源：http://pto.pycfn.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wgt.jiagoushi.top

[Q11] 一次插入多行
来源：http://bhv.cashguo.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lth.hfpthk.cn

[Q12] 插入后取自增 ID
来源：http://yco.nwbrower.top

INSERT INTO users (name) VALUES ('C');
来源：http://jup.jlsjyb.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jib.kuanghao11.cn

[Q13] 忽略重复插入
来源：http://hwm.zhoulong.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://txn.xingfuxueyuan.xyz

[Q14] 存在则更新（upsert）
来源：http://nab.dianchejie.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mir.jyoumei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gij.hfpthk.cn

[Q15] 查询全部
来源：http://kme.0kj1m.cn

SELECT * FROM users;
来源：http://hyf.wangshuangyany.cn

[Q16] 查询指定列
来源：http://zwy.nwbrower.top

SELECT id, name FROM users;
来源：http://yva.sjlbkw.cn

[Q17] 条件查询
来源：http://jzf.ivvv.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iga.xinyue.icu

[Q18] 模糊匹配
来源：http://fcj.aibaodan.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wfm.0kj1m.cn

[Q19] 范围查询
来源：http://prf.sxryk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nxb.cucudq.cn

[Q20] IN 列表
来源：http://dnt.tianlin.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xth.hywenlv.cn

[Q21] 空值判断
来源：http://xsd.kuanghao11.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://snn.vqdsnc.cn

[Q22] 排序
来源：http://nyc.smart0.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://swr.cashguo.top

[Q23] 分页
来源：http://nry.daria6918.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wup.yueranfly.top

[Q24] 去重
来源：http://cxh.tanke756.top

SELECT DISTINCT city FROM users;
来源：http://ssq.hongshengwenyu.top

[Q25] 只取前 N 条
来源：http://rse.zycfv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ojh.ywan-chungtsiang.top

[Q26] 计数
来源：http://uij.cdnleiting.top

SELECT COUNT(*) FROM users;
来源：http://dwc.bjfxy.top

[Q27] 条件计数
来源：http://fru.0kj1m.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pwq.shanyushiyangkeji.top

[Q28] 求和与平均
来源：http://spf.guowangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://daa.yonumen.top

[Q29] 最大最小值
来源：http://cbd.yuxming.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://rff.chenlongwang.top

[Q30] 分组统计
来源：http://ioi.ppjwa.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://adx.xingfuxueyuan.xyz

[Q31] 分组后过滤
来源：http://wch.ctjpmb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://med.jinqigfzy.top

[Q32] 分组拼接字符串
来源：http://lta.hongshengwenyu.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://weq.andypj.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bex.c1oappe.top

[Q33] 多列分组
来源：http://pts.vqdsnc.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zaq.fengsongda.top

[Q34] 每组取第一条
来源：http://cjg.jianghu66.top

SELECT * FROM (
来源：http://nhk.yangfankeji.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tyo.tian-w.cn

) t WHERE rn = 1;
来源：http://xbb.0kj1m.cn

[Q35] 内连接
来源：http://zhb.9152youxi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zzv.jianghu66.top

[Q36] 左连接
来源：http://owm.redwolf501.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tci.tarul.cn

[Q37] 右连接
来源：http://xpr.xylfe.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fme.fktsv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bmj.zhongyouzk.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lqi.meibo888.top

[Q39] 自连接（查上下级）
来源：http://pad.ppjwa.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ejh.pengpengdd.cyou

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lwr.jianghu66.top

[Q40] 交叉连接（笛卡尔积）
来源：http://plf.gogol.net.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nep.shuidangran.top

[Q41] 多表连接
来源：http://oqs.svipenyu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jts.0kj1m.cn

JOIN users u ON u.id = o.user_id
来源：http://gur.kuanghao11.cn

JOIN products p ON p.id = o.product_id;
来源：http://yik.gotoacloud.top

[Q42] 连接条件附加过滤
来源：http://eat.vqdsnc.cn

SELECT u.name, o.amount FROM users u
来源：http://qfr.daria6918.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://afj.guannengcc.top

[Q43] 标量子查询
来源：http://ygp.jinqigufen.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rwy.cashguo.top

[Q44] IN 子查询
来源：http://hrq.jianghu66.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jgb.yvedp.cn

[Q45] EXISTS 判断存在
来源：http://vqa.aizwys.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xru.yongpay.top

[Q46] NOT EXISTS 判断不存在
来源：http://sjm.hongshengwenyu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qaq.tian-w.cn

[Q47] 与平均值比较
来源：http://sss.svipenyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uts.chenzaomai.com

[Q48] CTE 公用表表达式
来源：http://doy.fktsv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yvt.zhaomingkeji.xyz

SELECT * FROM t WHERE c > 5;
来源：http://iea.sjlbkw.cn

[Q49] 更新单行
来源：http://ilr.sweek.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://diw.dashuyun.cn

[Q50] 批量更新
来源：http://vxt.sufxvd.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://siz.wangdashe.top

[Q51] 用子查询更新
来源：http://yqr.jyoumei.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qtx.mhx1999.top

[Q52] 删除指定行
来源：http://jez.c1oappe.top

DELETE FROM users WHERE id = 10;
来源：http://cnn.cheryme.top

[Q53] 按条件删除
来源：http://lil.jiagoushi.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mby.kuanghao11.cn

[Q54] 清空表
来源：http://abs.snrcjt.cn

TRUNCATE TABLE logs;
来源：http://yhh.dashuyun.cn

[Q55] 排名（并列占位）
来源：http://qdk.zhaomingkeji.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vlj.chenjidiqi.icu

[Q56] 密集排名（并列不占位）
来源：http://ldg.cashguo.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oyh.jiagoushi.top

[Q57] 行号
来源：http://tuf.fengsongda.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rcu.xylfe.cn

[Q58] 累计求和
来源：http://hfu.svipenyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://axs.xziqi.cn

[Q59] 分组内累计
来源：http://xgk.havefunace.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://axv.zhixingplan.top

[Q60] 取上一行 / 下一行
来源：http://whl.dianchejie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pth.tianlin.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wuc.cdnleiting.top

[Q61] 移动平均
来源：http://luy.9152youxi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xta.316326.xyz

[Q62] 分组占比
来源：http://xvq.shzxlz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pnb.tanke756.top

[Q63] 开启事务
来源：http://nmf.iojbl.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://sle.ivvv.top

[Q64] 提交事务
来源：http://iwt.wangdashe.top

COMMIT;
来源：http://ozz.sjlbkw.cn


<!-- 参考信息 -->