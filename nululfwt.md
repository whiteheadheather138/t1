代发 wailian999

PHP:  // 手写递归函数
来源：http://fmw.ywan-chungtsiang.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xxt.chenlongwang.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hqx.jqgfzy.top

Java: // 手写递归
来源：http://eui.shuidangran.top

Go:   // 手写递归
来源：http://wso.ctjpmb.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yep.c1oappe.top

C#:   // 手写递归
来源：http://kcz.zhoulong.xyz

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qlr.sjlbkw.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://itm.ydjk.org.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bvb.zhijiandao.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hrz.316326.xyz

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://dmn.havefunace.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ewf.xylfe.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://sfp.pycfn.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ybn.andypj.xyz

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xju.hfpthk.cn

================================================================================
来源：http://gkp.yj20258888.top

O. 并发与异步
来源：http://jji.xylfe.cn

================================================================================
来源：http://pjt.meibo888.top

[O01] 启动一个线程
来源：http://aum.cheryme.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://rdn.tanke756.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://gno.ivvv.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gax.svipenyu.cn

TS:   // 同 JS
来源：http://egf.epnwcf.com

Java: new Thread(() -> f()).start()
来源：http://qla.zycfv.cn

Go:   go f()
来源：http://tun.fehbvm.com

Ruby: Thread.new { f }
来源：http://roj.aizwys.cn

C#:   Task.Run(() => F());
来源：http://qlh.jiagoushi.top

[O02] 使用线程池
来源：http://kdl.xinyue.icu

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ohl.cucudq.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://dxj.gaohongyu789.top

JS:   // worker_threads 线程池
来源：http://dwt.ydjk.org.cn

TS:   // worker_threads 线程池
来源：http://yvy.c1oappe.top

Java: Executors.newFixedThreadPool(4)
来源：http://bki.feifeiyinyue.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://adp.meibo888.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xyf.zhoulong.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ihi.zhongyouzk.top

[O03] 加锁保护共享数据
来源：http://aki.wangdashe.top

Py:   with lock: shared += 1
来源：http://jdj.jianghu66.top

PHP:  // 用 flock() 做文件锁
来源：http://hvi.hcnkem.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hsd.yanxiufei.cn

TS:   // 同 JS
来源：http://ces.yanxiufei.cn

Java: synchronized (this) { shared++; }
来源：http://fzh.ehwqpu.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cbf.bjfxy.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://oxw.xylfe.cn

C#:   lock (gate) { shared++; }
来源：http://dmk.yj20258.top

[O04] 定义异步函数并等待
来源：http://ycn.guannengcc.top

Py:   async def f():⏎    await g()
来源：http://vmb.yangfankeji.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aie.mhx1999.top

JS:   async function f() { await g(); }
来源：http://clm.xinyue.icu

TS:   async function f(): Promise<void> { await g(); }
来源：http://ddn.xuetiantiany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gxu.zhengqikj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ncl.bjfxy.top

Ruby: # 用 Fiber 或 async gem
来源：http://njr.vehdjk.com

C#:   async Task F() { await G(); }
来源：http://odj.ctjpmb.com

[O05] 并发执行并等待全部完成
来源：http://xoy.epnwcf.com

Py:   asyncio.gather(*tasks)
来源：http://cuo.ydzc1.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qpa.jianghu66.top

JS:   await Promise.all(tasks)
来源：http://mal.guowangkeji.top

TS:   await Promise.all(tasks)
来源：http://sbu.hesvh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://gdj.yfazqb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://aqj.svipenyu.cn

Ruby: threads.map(&:join)
来源：http://fxp.ywan-chungtsiang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ite.birdmap.top

[O06] 使用进程池
来源：http://zqf.jinqigufen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sgx.meibo888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://auf.hnxiangtu.top

JS:   // child_process / cluster 模块
来源：http://tmq.ivvv.top

TS:   // child_process / cluster 模块
来源：http://num.ctjpmb.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hlo.wangdashe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gsr.ehwqpu.com

Ruby: // fork 块
来源：http://vka.guowangkeji.top

C#:   Parallel.For
来源：http://oor.jinyuanbaomall.cn

================================================================================
来源：http://jpg.jinyuanbaomall.cn

P. 常用工具函数
来源：http://kjd.yfazqb.com

================================================================================
来源：http://yqz.gzhubu.top

[P01] 生成 UUID
来源：http://pes.sysykeji.top

Py:   str(uuid.uuid4())
来源：http://edr.fzhhl.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://adv.jiagoushi.top

JS:   crypto.randomUUID()
来源：http://xel.316326.xyz

TS:   crypto.randomUUID()
来源：http://rrg.cheryme.top

Java: UUID.randomUUID().toString()
来源：http://mji.cheryme.top

Go:   // 用 github.com/google/uuid
来源：http://hum.fanxiaobao.xyz

Ruby: SecureRandom.uuid
来源：http://nir.jiagoushi.top

C#:   Guid.NewGuid().ToString()
来源：http://klr.shuidangran.top

[P02] MD5 / SHA256 摘要
来源：http://usf.jlsjyb.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bqq.nanxuanxn.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://fyq.gzhubu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qha.xuanzx.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nkf.cdnleiting.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uye.vehdjk.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dnu.yonumen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ssx.fktsv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ago.vqdsnc.cn

[P03] 生成短随机字符串
来源：http://igd.cdnleiting.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wlc.zhaomingkeji.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://nqy.birdmap.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gym.shanyushiyangtech.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xbw.iojbl.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ylc.ctjpmb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://eax.tianlin.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://ozr.tarul.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jfn.cucudq.cn

[P04] 求长度
来源：http://rxf.nanxuanxn.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jsi.meibo888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kje.ctjpmb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://glg.sweek.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mvk.fktsv.cn

Java: list.size();  map.size();  s.length()
来源：http://lzy.hysaishi.cn

Go:   len(arr);  len(m)
来源：http://pai.ydzc1.top

Ruby: x.length;  x.size
来源：http://ayy.pycfn.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://uzs.shanyushiyangtech.top

[P05] 判断两个对象内容是否相等
来源：http://vag.jinyuanbaomall.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gej.zhoulong.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fem.zhongyouzk.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hsx.jinyuanbaomall.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zcq.epnwcf.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://qam.guowangkeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://dog.zhaomingkeji.xyz

Ruby: a == b
来源：http://zge.shuidangran.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dgr.gotoacloud.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dxu.yj20258.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mol.cqqwz.cn

PHP:  if (empty($x)) {}
来源：http://ano.jyoumei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ctw.xuetiantiany.cn

TS:   if (x == null) {}
来源：http://efv.hesvh.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://yhf.0kj1m.cn

Go:   if x == nil {}
来源：http://fts.fehbvm.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://tah.jyoumei.cn

C#:   if (x is null) {}
来源：http://ofx.andypj.xyz

[P07] 防抖与节流
来源：http://kwe.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://axg.316326.xyz

PHP:  // 手写时间戳比较
来源：http://bdb.epnwcf.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mqy.zdbjq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lgw.0kj1m.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xfl.sweek.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qxa.guannengcc.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qyq.bjfxy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ybl.shangyingyoupin.top

[P08] 处理浮点精度问题
来源：http://egm.shanyushiyangtech.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ajk.zhongyouzk.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mzg.chenzaomai.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zjf.jinghuilouyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fwl.dashuyun.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://srf.chenzaomai.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ebe.yvedp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tku.ydzc1.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ozr.xingfuxueyuan.xyz

================================================================================
来源：http://qvq.jqgfzy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ota.meibo888.top

================================================================================
来源：http://yfi.vqdsnc.cn

[Q01] 创建表
来源：http://obv.jqgfzy.top

CREATE TABLE users (
来源：http://mlq.cucudq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cku.ctjpmb.com

name VARCHAR(50) NOT NULL,
来源：http://sxa.vehdjk.com

email VARCHAR(100) UNIQUE,
来源：http://bql.yanxiufei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ecs.bjfxy.top

);
来源：http://jyx.sufxvd.cn

[Q02] 创建带外键的表
来源：http://mtd.jqgfzy.top

CREATE TABLE orders (
来源：http://qft.yfazqb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kyy.mhx1999.top

user_id INT NOT NULL,
来源：http://dqh.zhijiandao.cn

amount DECIMAL(10, 2),
来源：http://png.ivvv.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dpx.fanxiaobao.xyz

);
来源：http://ifx.xuanzx.com

[Q03] 增加列
来源：http://nej.yongpay.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kpv.zhengqikj.top

[Q04] 修改列类型
来源：http://fws.kuanghao11.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qbj.nwbrower.top

[Q05] 重命名列
来源：http://iiq.iojbl.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yqu.zhongyouzk.top

[Q06] 删除列
来源：http://ity.nanxuanxn.top

ALTER TABLE users DROP COLUMN age;
来源：http://rjy.c1oappe.top

[Q07] 删除表
来源：http://hww.andypj.xyz

DROP TABLE IF EXISTS orders;
来源：http://rqt.birdmap.top

[Q08] 创建普通索引
来源：http://lwp.sufxvd.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ymb.chenzaomai.com

[Q09] 创建唯一索引
来源：http://qax.ctjpmb.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://veg.ydjk.org.cn

[Q10] 插入单行
来源：http://fvm.yj20258.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ewu.cheryme.top

[Q11] 一次插入多行
来源：http://suv.chenzaomai.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hhc.vqdsnc.cn

[Q12] 插入后取自增 ID
来源：http://wke.dianchejie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qey.haohaochexian.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fvr.tianlin.xyz

[Q13] 忽略重复插入
来源：http://fgg.uphjek.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fhr.yanxiufei.cn

[Q14] 存在则更新（upsert）
来源：http://fjk.yongpay.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tkt.daria6918.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jky.cashguo.top

[Q15] 查询全部
来源：http://tyu.tian-w.cn

SELECT * FROM users;
来源：http://vbb.jlsjyb.cn

[Q16] 查询指定列
来源：http://qti.zhiwuduotai.top

SELECT id, name FROM users;
来源：http://mgz.uphjek.com

[Q17] 条件查询
来源：http://ysh.yfazqb.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wwn.jinqigufen.top

[Q18] 模糊匹配
来源：http://jso.9152youxi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uxf.snrcjt.cn

[Q19] 范围查询
来源：http://fxd.316326.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vyk.zhijiandao.cn

[Q20] IN 列表
来源：http://eek.gotoacloud.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vcv.fktsv.cn

[Q21] 空值判断
来源：http://uls.yfazqb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://uvz.yanxiufei.cn

[Q22] 排序
来源：http://xjd.zhiwuduotai.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ocu.yj202588.top

[Q23] 分页
来源：http://dyg.sufxvd.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://axj.jyoumei.cn

[Q24] 去重
来源：http://dep.aibaodan.cn

SELECT DISTINCT city FROM users;
来源：http://vqk.zhijiandao.cn

[Q25] 只取前 N 条
来源：http://ywx.chenlongwang.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rin.yvedp.cn

[Q26] 计数
来源：http://ywe.dashuyun.cn

SELECT COUNT(*) FROM users;
来源：http://szh.xingfuxueyuan.xyz

[Q27] 条件计数
来源：http://lqj.jinqigufen.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://noj.xingfuxueyuan.xyz

[Q28] 求和与平均
来源：http://jem.fanxiaobao.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ndy.iojbl.cn

[Q29] 最大最小值
来源：http://zxg.zycfv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fxg.jinyuanbaomall.cn

[Q30] 分组统计
来源：http://zkf.feifeiyinyue.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hhl.sjlbkw.cn

[Q31] 分组后过滤
来源：http://bof.wangdashe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ude.cdnleiting.top

[Q32] 分组拼接字符串
来源：http://glm.meibo888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vtx.havefunace.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://eze.ydjk.org.cn

[Q33] 多列分组
来源：http://duw.bbcook.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zfi.jianghu66.top

[Q34] 每组取第一条
来源：http://wyy.xuanzx.com

SELECT * FROM (
来源：http://vbu.xinyue.icu

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kmh.sufxvd.cn

) t WHERE rn = 1;
来源：http://vfk.fzhhl.top

[Q35] 内连接
来源：http://ybj.nwbrower.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xds.shuidangran.top

[Q36] 左连接
来源：http://hls.hywenlv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rpd.shangyingyoupin.top

[Q37] 右连接
来源：http://iyf.xuetiantiany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://isk.dashuyun.cn

[Q38] 全外连接（PostgreSQL）
来源：http://zsc.ywan-chungtsiang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://swh.zhixingplan.top

[Q39] 自连接（查上下级）
来源：http://opw.feifeiyinyue.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tgb.hfpthk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mup.chenzaomai.com

[Q40] 交叉连接（笛卡尔积）
来源：http://kko.ehwqpu.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mde.ctjpmb.com

[Q41] 多表连接
来源：http://ria.jinyuanbaomall.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://swf.yvedp.cn

JOIN users u ON u.id = o.user_id
来源：http://shy.yanxiufei.cn

JOIN products p ON p.id = o.product_id;
来源：http://vfb.zhengqikj.top

[Q42] 连接条件附加过滤
来源：http://ube.zhongyouzk.top

SELECT u.name, o.amount FROM users u
来源：http://ojo.jinqigufen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rno.guowangkeji.top

[Q43] 标量子查询
来源：http://vke.zhengqikj.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qgm.xingfuxueyuan.xyz

[Q44] IN 子查询
来源：http://lfc.wangdashe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pig.nanxuanxn.top

[Q45] EXISTS 判断存在
来源：http://hzf.ydjk.org.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fsj.dashuyun.cn

[Q46] NOT EXISTS 判断不存在
来源：http://tbc.xziqi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yoq.cheryme.top

[Q47] 与平均值比较
来源：http://lsk.ydzc1.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gbi.jinqigufen.top

[Q48] CTE 公用表表达式
来源：http://xxt.shzxlz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nju.nanxinkj.top

SELECT * FROM t WHERE c > 5;
来源：http://mze.zhaomingkeji.xyz

[Q49] 更新单行
来源：http://hwl.xinyue.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nmi.svipenyu.cn

[Q50] 批量更新
来源：http://ytr.andypj.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://voy.fehbvm.com

[Q51] 用子查询更新
来源：http://spr.sufxvd.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://car.aibaodan.cn

[Q52] 删除指定行
来源：http://cua.yueranfly.top

DELETE FROM users WHERE id = 10;
来源：http://ktg.hammf.cn

[Q53] 按条件删除
来源：http://tde.zdbjq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jwx.dashuyun.cn

[Q54] 清空表
来源：http://dft.zdqjudy.top

TRUNCATE TABLE logs;
来源：http://fen.zhoulong.xyz

[Q55] 排名（并列占位）
来源：http://odi.yuanzhike.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ltc.jianghu66.top

[Q56] 密集排名（并列不占位）
来源：http://ncf.yanxiufei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hsc.zhongyouzk.top

[Q57] 行号
来源：http://jmh.fktsv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://goa.zdqjudy.top

[Q58] 累计求和
来源：http://lvp.shzxlz.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hxs.ehwqpu.com

[Q59] 分组内累计
来源：http://fug.yanxiufei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jpa.zhixingplan.top

[Q60] 取上一行 / 下一行
来源：http://dol.snrcjt.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dll.fengsongda.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xak.sweek.top

[Q61] 移动平均
来源：http://pgq.xylfe.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dhz.aizwys.cn

[Q62] 分组占比
来源：http://xdf.316326.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gfb.sxryk.cn

[Q63] 开启事务
来源：http://xcn.hywenlv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vzf.shuidangran.top

[Q64] 提交事务
来源：http://lts.gzhubu.top

COMMIT;
来源：http://wwz.hnxiangtu.top


<!-- 参考信息 -->