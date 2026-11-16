代发 wailian999

PHP:  // 手写递归函数
来源：http://doh.fzhhl.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gfw.zdqjudy.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oiy.316326.xyz

Java: // 手写递归
来源：http://klr.pengpengdd.cyou

Go:   // 手写递归
来源：http://oap.snrcjt.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://glo.316326.xyz

C#:   // 手写递归
来源：http://als.yongpay.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zob.nanxinkj.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ypb.jlsjyb.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://swc.cdnleiting.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pcq.cucudq.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://erq.guowangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://goc.chenjidiqi.icu

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://agk.vehdjk.com

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ztc.jqgufenzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jds.tanke756.top

================================================================================
来源：http://chu.zhiwuduotai.top

O. 并发与异步
来源：http://tln.aizwys.cn

================================================================================
来源：http://yyz.zdqjudy.top

[O01] 启动一个线程
来源：http://fbu.chenzaomai.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://icu.nanxinkj.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jcg.yanxiufei.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://qab.jqgufenzy.top

TS:   // 同 JS
来源：http://rus.mhx1999.top

Java: new Thread(() -> f()).start()
来源：http://xcv.zhongyouzk.top

Go:   go f()
来源：http://hcx.sweek.top

Ruby: Thread.new { f }
来源：http://brs.jianghu66.top

C#:   Task.Run(() => F());
来源：http://juh.chenjidiqi.icu

[O02] 使用线程池
来源：http://fmd.yongpay.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yli.zhiwuduotai.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bow.tianlin.xyz

JS:   // worker_threads 线程池
来源：http://xol.aibaodan.cn

TS:   // worker_threads 线程池
来源：http://htq.hysaishi.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dso.ydzc1.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://raz.andypj.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://osx.yangfankeji.com

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mna.shzxlz.cn

[O03] 加锁保护共享数据
来源：http://lce.feifeiyinyue.top

Py:   with lock: shared += 1
来源：http://jbm.shanyushiyangkeji.top

PHP:  // 用 flock() 做文件锁
来源：http://oyh.yuanzhike.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mqx.iojbl.cn

TS:   // 同 JS
来源：http://zpz.hesvh.cn

Java: synchronized (this) { shared++; }
来源：http://bdg.yj202588.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nfy.gaohongyu789.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://lql.yuxming.cn

C#:   lock (gate) { shared++; }
来源：http://itv.bbcook.cn

[O04] 定义异步函数并等待
来源：http://bsf.ybcxt.top

Py:   async def f():⏎    await g()
来源：http://vmo.dianchejie.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dxa.ehwqpu.com

JS:   async function f() { await g(); }
来源：http://jkx.52xcode.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://mkb.birdmap.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://zlg.yonumen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ofk.bjfxy.top

Ruby: # 用 Fiber 或 async gem
来源：http://sze.xuetiantiany.cn

C#:   async Task F() { await G(); }
来源：http://gdi.jqgfzy.top

[O05] 并发执行并等待全部完成
来源：http://zme.sxryk.cn

Py:   asyncio.gather(*tasks)
来源：http://qoa.birdmap.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oan.shanyushiyangkeji.top

JS:   await Promise.all(tasks)
来源：http://bcy.yuanzhike.top

TS:   await Promise.all(tasks)
来源：http://jag.nanxuanxn.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ver.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://vlr.wangshuangyany.cn

Ruby: threads.map(&:join)
来源：http://hqi.xylfe.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rek.xuanzx.com

[O06] 使用进程池
来源：http://fsi.zdbjq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lkb.fanxiaobao.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://zkl.yuxming.cn

JS:   // child_process / cluster 模块
来源：http://fdj.vqdsnc.cn

TS:   // child_process / cluster 模块
来源：http://car.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pvp.sxryk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cyt.zhijiandao.cn

Ruby: // fork 块
来源：http://oki.smart0.xyz

C#:   Parallel.For
来源：http://dkb.zycfv.cn

================================================================================
来源：http://fmr.zycfv.cn

P. 常用工具函数
来源：http://olt.ctjpmb.com

================================================================================
来源：http://gsn.hnxiangtu.top

[P01] 生成 UUID
来源：http://jjr.yanxiufei.cn

Py:   str(uuid.uuid4())
来源：http://erx.zycfv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cxu.gotoacloud.top

JS:   crypto.randomUUID()
来源：http://kbx.xuetiantiany.cn

TS:   crypto.randomUUID()
来源：http://qjq.hammf.cn

Java: UUID.randomUUID().toString()
来源：http://tpq.daxiang520.top

Go:   // 用 github.com/google/uuid
来源：http://yvn.52xcode.cn

Ruby: SecureRandom.uuid
来源：http://gbt.316326.xyz

C#:   Guid.NewGuid().ToString()
来源：http://ynf.jinqigufen.top

[P02] MD5 / SHA256 摘要
来源：http://sfn.svipenyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dpd.shangyingyoupin.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://boa.zhongyouzk.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xvn.hywenlv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sdv.cdnleiting.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ply.ivvv.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mgw.jiagoushi.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jfr.yj202588.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ycq.sysykeji.top

[P03] 生成短随机字符串
来源：http://tcj.jqgufenzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fks.hywenlv.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ygv.shuidangran.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dai.hcnkem.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wvu.daria6918.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zsg.shanyushiyangkeji.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qma.316326.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://rsv.jiagoushi.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://krp.nwbrower.top

[P04] 求长度
来源：http://yuh.xinyue.icu

Py:   len(x)            # 字符串、列表、字典通用
来源：http://opi.jlsjyb.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tlq.hongshengwenyu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iow.svipenyu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pti.hnqzz.top

Java: list.size();  map.size();  s.length()
来源：http://nlq.ivvv.top

Go:   len(arr);  len(m)
来源：http://epf.jiagoushi.top

Ruby: x.length;  x.size
来源：http://kdc.zycfv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://wof.andypj.xyz

[P05] 判断两个对象内容是否相等
来源：http://nzk.jqgfzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://eim.tian-w.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ebc.pycfn.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ayn.havefunace.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sfh.yfazqb.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zwd.9152youxi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://dht.meibo888.top

Ruby: a == b
来源：http://wpz.jqgufenzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jpy.chenjidiqi.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tgg.bjfxy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mqh.chenjidiqi.icu

PHP:  if (empty($x)) {}
来源：http://ikh.tanke756.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lay.yonumen.top

TS:   if (x == null) {}
来源：http://gup.uphjek.com

Java: if (x == null || x.isEmpty()) {}
来源：http://uqn.iojbl.cn

Go:   if x == nil {}
来源：http://maw.zdqjudy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lgl.yueranfly.top

C#:   if (x is null) {}
来源：http://nfn.yongpay.top

[P07] 防抖与节流
来源：http://zcy.jinqigfzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aqx.jinqigfzy.top

PHP:  // 手写时间戳比较
来源：http://pxc.gaohongyu789.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wed.zdbjq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ayd.daxiang520.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rum.shangyingyoupin.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mzf.tianlin.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://ydm.ppjwa.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://eea.cheryme.top

[P08] 处理浮点精度问题
来源：http://kpg.xuanzx.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://sym.cucudq.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zmb.yj20258.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wyl.shanyushiyangkeji.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mry.c1oappe.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://awg.gaohongyu789.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nan.vqdsnc.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tki.xuanzx.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ybo.kuanghao11.cn

================================================================================
来源：http://doj.hammf.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tuy.tian-w.cn

================================================================================
来源：http://ytw.jinyuanbaomall.cn

[Q01] 创建表
来源：http://jou.vehdjk.com

CREATE TABLE users (
来源：http://mxn.wangshuangyany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yff.fengsongda.top

name VARCHAR(50) NOT NULL,
来源：http://dia.xinyue.icu

email VARCHAR(100) UNIQUE,
来源：http://zgp.ywan-chungtsiang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://khy.hfpthk.cn

);
来源：http://cvw.hysaishi.cn

[Q02] 创建带外键的表
来源：http://eoa.hysaishi.cn

CREATE TABLE orders (
来源：http://ywp.svipenyu.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nyy.uphjek.com

user_id INT NOT NULL,
来源：http://tmk.aizwys.cn

amount DECIMAL(10, 2),
来源：http://xof.sufxvd.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nkr.shzxlz.cn

);
来源：http://mow.kuanghao11.cn

[Q03] 增加列
来源：http://ulw.jinyuanbaomall.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xxu.cheryme.top

[Q04] 修改列类型
来源：http://jjb.fehbvm.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tit.sweek.top

[Q05] 重命名列
来源：http://xbi.quarkkingdee.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wio.svipenyu.cn

[Q06] 删除列
来源：http://axh.0kj1m.cn

ALTER TABLE users DROP COLUMN age;
来源：http://orr.zhengqikj.top

[Q07] 删除表
来源：http://ewx.yj20258.top

DROP TABLE IF EXISTS orders;
来源：http://fmv.c1oappe.top

[Q08] 创建普通索引
来源：http://bzj.tian-w.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yur.gogol.net.cn

[Q09] 创建唯一索引
来源：http://zwh.yuxming.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://djz.cucudq.cn

[Q10] 插入单行
来源：http://fze.fehbvm.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pfm.gzhubu.top

[Q11] 一次插入多行
来源：http://nwm.sweek.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gjx.jianghu66.top

[Q12] 插入后取自增 ID
来源：http://uok.sxryk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qin.yvedp.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://aqn.chenjidiqi.icu

[Q13] 忽略重复插入
来源：http://vnx.cqqwz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bky.mhx1999.top

[Q14] 存在则更新（upsert）
来源：http://ahb.quarkkingdee.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ghl.chenzaomai.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://scj.cdnleiting.top

[Q15] 查询全部
来源：http://cnj.feifeiyinyue.top

SELECT * FROM users;
来源：http://whb.sysykeji.top

[Q16] 查询指定列
来源：http://vif.yonumen.top

SELECT id, name FROM users;
来源：http://wxx.9152youxi.cn

[Q17] 条件查询
来源：http://gya.ppjwa.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dez.smart0.xyz

[Q18] 模糊匹配
来源：http://utv.zhongyouzk.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pqn.chenzaomai.com

[Q19] 范围查询
来源：http://gro.aibaodan.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fez.tian-w.cn

[Q20] IN 列表
来源：http://pnl.tian-w.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cfg.hysaishi.cn

[Q21] 空值判断
来源：http://dbg.tarul.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tui.xinyue.icu

[Q22] 排序
来源：http://wzb.mhx1999.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://syp.wangshuangyany.cn

[Q23] 分页
来源：http://qjy.smart0.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jfb.gotoacloud.top

[Q24] 去重
来源：http://ius.cdnleiting.top

SELECT DISTINCT city FROM users;
来源：http://zlo.yfazqb.com

[Q25] 只取前 N 条
来源：http://ngb.zhoulong.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nwb.yuanzhike.top

[Q26] 计数
来源：http://qvz.ydzc1.top

SELECT COUNT(*) FROM users;
来源：http://cuq.yongpay.top

[Q27] 条件计数
来源：http://dfs.gogol.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pvu.xinyue.icu

[Q28] 求和与平均
来源：http://ftk.tianlin.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wqq.c1oappe.top

[Q29] 最大最小值
来源：http://myn.vehdjk.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://wdn.shangyingyoupin.top

[Q30] 分组统计
来源：http://qgn.gzhubu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mmw.quarkkingdee.top

[Q31] 分组后过滤
来源：http://cfk.shanyushiyangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oqy.jqgufenzy.top

[Q32] 分组拼接字符串
来源：http://rfz.9152youxi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://inx.shuidangran.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tkh.hongshengwenyu.top

[Q33] 多列分组
来源：http://rfo.xingfuxueyuan.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tfk.xziqi.cn

[Q34] 每组取第一条
来源：http://bub.yanxiufei.cn

SELECT * FROM (
来源：http://dys.birdmap.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zay.vehdjk.com

) t WHERE rn = 1;
来源：http://cqw.xuetiantiany.cn

[Q35] 内连接
来源：http://mzw.shuidangran.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xzd.aizwys.cn

[Q36] 左连接
来源：http://dgz.hnxiangtu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eus.zdqjudy.top

[Q37] 右连接
来源：http://klu.xylfe.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jpc.havefunace.top

[Q38] 全外连接（PostgreSQL）
来源：http://dfz.daria6918.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gbb.jlsjyb.cn

[Q39] 自连接（查上下级）
来源：http://tjw.havefunace.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xxq.zhiwuduotai.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ixz.dianchejie.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rfl.zhijiandao.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://awg.mhx1999.top

[Q41] 多表连接
来源：http://knx.jianghu66.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://xjk.yanxiufei.cn

JOIN users u ON u.id = o.user_id
来源：http://wtu.snrcjt.cn

JOIN products p ON p.id = o.product_id;
来源：http://wdv.shzxlz.cn

[Q42] 连接条件附加过滤
来源：http://zet.yangfankeji.com

SELECT u.name, o.amount FROM users u
来源：http://nwg.nwbrower.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zrb.kuanghao11.cn

[Q43] 标量子查询
来源：http://zyt.hysaishi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hcw.zdqjudy.top

[Q44] IN 子查询
来源：http://gxb.yuxming.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iqi.316326.xyz

[Q45] EXISTS 判断存在
来源：http://pih.yj20258.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sup.ydzc1.top

[Q46] NOT EXISTS 判断不存在
来源：http://ufj.hnqzz.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tke.yvedp.cn

[Q47] 与平均值比较
来源：http://hke.9152youxi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dfh.sjlbkw.cn

[Q48] CTE 公用表表达式
来源：http://ccu.iojbl.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vov.zdbjq.cn

SELECT * FROM t WHERE c > 5;
来源：http://add.zhiwuduotai.top

[Q49] 更新单行
来源：http://uoq.ybcxt.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tan.zhaomingkeji.xyz

[Q50] 批量更新
来源：http://lro.xuanzx.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jhb.iojbl.cn

[Q51] 用子查询更新
来源：http://tqu.sxryk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mkc.ybcxt.top

[Q52] 删除指定行
来源：http://ojm.bjfxy.top

DELETE FROM users WHERE id = 10;
来源：http://pwo.zhixingplan.top

[Q53] 按条件删除
来源：http://ywz.zhoulong.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kwd.gogol.net.cn

[Q54] 清空表
来源：http://xzc.haohaochexian.top

TRUNCATE TABLE logs;
来源：http://avg.iojbl.cn

[Q55] 排名（并列占位）
来源：http://xxl.xylfe.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://agj.hysaishi.cn

[Q56] 密集排名（并列不占位）
来源：http://oaz.chenzaomai.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wir.hcnkem.com

[Q57] 行号
来源：http://ujw.uphjek.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hhl.sxryk.cn

[Q58] 累计求和
来源：http://oym.wangdashe.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oef.zhijiandao.cn

[Q59] 分组内累计
来源：http://deb.zdqjudy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dbl.andypj.xyz

[Q60] 取上一行 / 下一行
来源：http://lwg.shanyushiyangtech.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://poj.chenzaomai.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://abm.haohaochexian.top

[Q61] 移动平均
来源：http://tjn.kuanghao11.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cwd.jqgufenzy.top

[Q62] 分组占比
来源：http://xir.cucudq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mfr.tarul.cn

[Q63] 开启事务
来源：http://jfi.ybcxt.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wjf.hammf.cn

[Q64] 提交事务
来源：http://avd.aizwys.cn

COMMIT;
来源：http://isy.jinqigfzy.top


<!-- 参考信息 -->