代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ukb.hnqzz.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://fmd.epnwcf.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ewd.jinyuanbaomall.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pwr.birdmap.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pbs.redwolf501.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://oye.sweek.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pka.jinqigfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://srf.jianghu66.top

================================================================================
来源：http://ppl.yangfankeji.com

O. 并发与异步
来源：http://mjz.hywenlv.cn

================================================================================
来源：http://ysl.hammf.cn

[O01] 启动一个线程
来源：http://yvn.shangyingyoupin.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ehl.jyoumei.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qvl.gzhubu.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://tax.bbcook.cn

TS:   // 同 JS
来源：http://urh.nanxinkj.top

Java: new Thread(() -> f()).start()
来源：http://vho.xinyue.icu

Go:   go f()
来源：http://iuz.fktsv.cn

Ruby: Thread.new { f }
来源：http://gdx.nanxuanxn.top

C#:   Task.Run(() => F());
来源：http://tiy.pengpengdd.cyou

[O02] 使用线程池
来源：http://ccy.yueranfly.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gai.pycfn.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://szl.sxryk.cn

JS:   // worker_threads 线程池
来源：http://iwg.tian-w.cn

TS:   // worker_threads 线程池
来源：http://ggg.zhaomingkeji.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://nez.xziqi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://tpy.zhixingplan.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dgg.nanxuanxn.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://nnd.hnxiangtu.top

[O03] 加锁保护共享数据
来源：http://dqi.snrcjt.cn

Py:   with lock: shared += 1
来源：http://ndd.yangfankeji.com

PHP:  // 用 flock() 做文件锁
来源：http://ayl.zhaomingkeji.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://azy.hfpthk.cn

TS:   // 同 JS
来源：http://pny.ppjwa.cn

Java: synchronized (this) { shared++; }
来源：http://aat.hywenlv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hou.ctjpmb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://jyl.zhoulong.xyz

C#:   lock (gate) { shared++; }
来源：http://gbo.gzhubu.top

[O04] 定义异步函数并等待
来源：http://uhh.gogol.net.cn

Py:   async def f():⏎    await g()
来源：http://ifb.cucudq.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ktf.nwbrower.top

JS:   async function f() { await g(); }
来源：http://pgp.gotoacloud.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://iyc.ybcxt.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jfn.havefunace.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cps.zycfv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://xil.haohaochexian.top

C#:   async Task F() { await G(); }
来源：http://gsj.bbcook.cn

[O05] 并发执行并等待全部完成
来源：http://nda.hnqzz.top

Py:   asyncio.gather(*tasks)
来源：http://mda.gzhubu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vfj.hywenlv.cn

JS:   await Promise.all(tasks)
来源：http://dhs.aibaodan.cn

TS:   await Promise.all(tasks)
来源：http://uwa.uphjek.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nty.yuxming.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hbh.cashguo.top

Ruby: threads.map(&:join)
来源：http://ykg.quarkkingdee.top

C#:   await Task.WhenAll(t1, t2)
来源：http://htb.yuanzhike.top

[O06] 使用进程池
来源：http://qhv.zhoulong.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jvq.chenzaomai.com

PHP:  // pcntl_fork 或多进程队列
来源：http://sdz.sysykeji.top

JS:   // child_process / cluster 模块
来源：http://sby.redwolf501.top

TS:   // child_process / cluster 模块
来源：http://mbw.hesvh.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://htr.bjfxy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jlg.shanyushiyangtech.top

Ruby: // fork 块
来源：http://bou.yanxiufei.cn

C#:   Parallel.For
来源：http://epx.yvedp.cn

================================================================================
来源：http://wta.pycfn.com

P. 常用工具函数
来源：http://vvc.daria6918.cn

================================================================================
来源：http://ieb.redwolf501.top

[P01] 生成 UUID
来源：http://kqk.jinghuilouyu.cn

Py:   str(uuid.uuid4())
来源：http://meo.hcnkem.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cik.shanyushiyangkeji.top

JS:   crypto.randomUUID()
来源：http://fdj.tanke756.top

TS:   crypto.randomUUID()
来源：http://aeh.tarul.cn

Java: UUID.randomUUID().toString()
来源：http://fiy.wangdashe.top

Go:   // 用 github.com/google/uuid
来源：http://smy.cheryme.top

Ruby: SecureRandom.uuid
来源：http://bid.hnxiangtu.top

C#:   Guid.NewGuid().ToString()
来源：http://psw.sxryk.cn

[P02] MD5 / SHA256 摘要
来源：http://wwg.hnxiangtu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dal.vqdsnc.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://eoa.jinyuanbaomall.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yzf.fktsv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hvu.daria6918.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zcg.gaohongyu789.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bco.daria6918.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iwu.daria6918.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://xdw.pengpengdd.cyou

[P03] 生成短随机字符串
来源：http://oku.yangfankeji.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jnu.ydjk.org.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gxz.chenlongwang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lcs.cucudq.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uue.yongpay.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pdz.chenjidiqi.icu

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qrq.epnwcf.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://dsh.0kj1m.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hqq.hcnkem.com

[P04] 求长度
来源：http://gig.zhaomingkeji.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vom.bbcook.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xdr.guowangkeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vib.yongpay.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ogs.jqgufenzy.top

Java: list.size();  map.size();  s.length()
来源：http://mjq.shzxlz.cn

Go:   len(arr);  len(m)
来源：http://bvs.yongpay.top

Ruby: x.length;  x.size
来源：http://gka.jinqigufen.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vyz.xinyue.icu

[P05] 判断两个对象内容是否相等
来源：http://gmk.haohaochexian.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ehh.tian-w.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fah.gogol.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ygq.xingfuxueyuan.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lie.xinyue.icu

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://keu.birdmap.top

Go:   reflect.DeepEqual(a, b)
来源：http://twf.yuanzhike.top

Ruby: a == b
来源：http://ecp.zhongyouzk.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rcb.hammf.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kcl.svipenyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nfq.fengsongda.top

PHP:  if (empty($x)) {}
来源：http://azt.gzhubu.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nji.tarul.cn

TS:   if (x == null) {}
来源：http://bjs.dianchejie.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zfj.gaohongyu789.top

Go:   if x == nil {}
来源：http://bff.mhx1999.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dto.smart0.xyz

C#:   if (x is null) {}
来源：http://jrc.0kj1m.cn

[P07] 防抖与节流
来源：http://nnu.shangyingyoupin.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hxq.xinyue.icu

PHP:  // 手写时间戳比较
来源：http://uov.9152youxi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://udn.sufxvd.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bxj.nwbrower.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pdj.wangshuangyany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://exh.cdnleiting.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://uuz.yj20258888.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ern.zhoulong.xyz

[P08] 处理浮点精度问题
来源：http://ipi.shuidangran.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mbq.shangyingyoupin.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wwg.yonumen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://foq.meibo888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://oku.yueranfly.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dxk.aibaodan.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fas.pengpengdd.cyou

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cpa.dianchejie.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vzh.aibaodan.cn

================================================================================
来源：http://gsp.yongpay.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mbi.xinyue.icu

================================================================================
来源：http://lgm.daria6918.cn

[Q01] 创建表
来源：http://tay.zhixingplan.top

CREATE TABLE users (
来源：http://pwv.fzhhl.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ayl.chenjidiqi.icu

name VARCHAR(50) NOT NULL,
来源：http://fut.52xcode.cn

email VARCHAR(100) UNIQUE,
来源：http://wap.fengsongda.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ifo.zdbjq.cn

);
来源：http://skd.wangdashe.top

[Q02] 创建带外键的表
来源：http://grp.xuetiantiany.cn

CREATE TABLE orders (
来源：http://bhn.bjfxy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hue.ctjpmb.com

user_id INT NOT NULL,
来源：http://hxs.xziqi.cn

amount DECIMAL(10, 2),
来源：http://mxj.quarkkingdee.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jpk.fzhhl.top

);
来源：http://oog.0kj1m.cn

[Q03] 增加列
来源：http://yjf.hnqzz.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://bgj.nanxinkj.top

[Q04] 修改列类型
来源：http://dzs.c1oappe.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rpn.mhx1999.top

[Q05] 重命名列
来源：http://ida.havefunace.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zpq.daria6918.cn

[Q06] 删除列
来源：http://ihp.redwolf501.top

ALTER TABLE users DROP COLUMN age;
来源：http://cpf.guannengcc.top

[Q07] 删除表
来源：http://ftc.zhaomingkeji.xyz

DROP TABLE IF EXISTS orders;
来源：http://baj.mhx1999.top

[Q08] 创建普通索引
来源：http://xnh.pengpengdd.cyou

CREATE INDEX idx_users_email ON users(email);
来源：http://xts.snrcjt.cn

[Q09] 创建唯一索引
来源：http://awk.dianchejie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wdj.zhengqikj.top

[Q10] 插入单行
来源：http://htl.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qyj.birdmap.top

[Q11] 一次插入多行
来源：http://mrg.shzxlz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lix.bjfxy.top

[Q12] 插入后取自增 ID
来源：http://gfg.dianchejie.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fwq.hcnkem.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ooo.cqqwz.cn

[Q13] 忽略重复插入
来源：http://lfa.wangshuangyany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://arh.jinqigfzy.top

[Q14] 存在则更新（upsert）
来源：http://thb.52xcode.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lev.shzxlz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gvg.wangdashe.top

[Q15] 查询全部
来源：http://zdj.feifeiyinyue.top

SELECT * FROM users;
来源：http://rpt.xuanzx.com

[Q16] 查询指定列
来源：http://noy.jinyuanbaomall.cn

SELECT id, name FROM users;
来源：http://xph.zhongyouzk.top

[Q17] 条件查询
来源：http://vhb.jqgfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ipn.zhiwuduotai.top

[Q18] 模糊匹配
来源：http://mix.yangfankeji.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lko.fktsv.cn

[Q19] 范围查询
来源：http://lyf.zhiwuduotai.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hkp.guowangkeji.top

[Q20] IN 列表
来源：http://hzt.zhengqikj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iyh.shanyushiyangkeji.top

[Q21] 空值判断
来源：http://yaa.guannengcc.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qku.shanyushiyangtech.top

[Q22] 排序
来源：http://ove.ppjwa.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xcf.jinyuanbaomall.cn

[Q23] 分页
来源：http://flw.chenjidiqi.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zrw.pycfn.com

[Q24] 去重
来源：http://lwz.shanyushiyangtech.top

SELECT DISTINCT city FROM users;
来源：http://alb.vqdsnc.cn

[Q25] 只取前 N 条
来源：http://oxn.xuetiantiany.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://pja.iojbl.cn

[Q26] 计数
来源：http://kxi.jinghuilouyu.cn

SELECT COUNT(*) FROM users;
来源：http://prl.guowangkeji.top

[Q27] 条件计数
来源：http://ptu.hcnkem.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tmc.jinqigufen.top

[Q28] 求和与平均
来源：http://wom.tian-w.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bvs.pengpengdd.cyou

[Q29] 最大最小值
来源：http://sin.gogol.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://thx.meibo888.top

[Q30] 分组统计
来源：http://fem.shuidangran.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://esa.zhixingplan.top

[Q31] 分组后过滤
来源：http://dcn.hnqzz.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rnb.fktsv.cn

[Q32] 分组拼接字符串
来源：http://bwt.yvedp.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fgp.yj202588.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hdf.havefunace.top

[Q33] 多列分组
来源：http://pql.feifeiyinyue.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nyo.sufxvd.cn

[Q34] 每组取第一条
来源：http://fov.zhixingplan.top

SELECT * FROM (
来源：http://zfo.yanxiufei.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zpy.yanxiufei.cn

) t WHERE rn = 1;
来源：http://sbr.yj20258888.top

[Q35] 内连接
来源：http://kjz.fengsongda.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qer.zhoulong.xyz

[Q36] 左连接
来源：http://nef.yj20258.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gzx.yuxming.cn

[Q37] 右连接
来源：http://mlk.snrcjt.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tyh.pycfn.com

[Q38] 全外连接（PostgreSQL）
来源：http://ekp.fzhhl.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://sth.jyoumei.cn

[Q39] 自连接（查上下级）
来源：http://vns.sweek.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kar.tianlin.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rru.smart0.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://wwn.hongshengwenyu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://foh.guowangkeji.top

[Q41] 多表连接
来源：http://vhs.havefunace.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ceg.bjfxy.top

JOIN users u ON u.id = o.user_id
来源：http://cct.chenjidiqi.icu

JOIN products p ON p.id = o.product_id;
来源：http://usd.cdnleiting.top

[Q42] 连接条件附加过滤
来源：http://sam.0kj1m.cn

SELECT u.name, o.amount FROM users u
来源：http://wzm.xziqi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vcj.hnxiangtu.top

[Q43] 标量子查询
来源：http://lls.jinyuanbaomall.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jgc.cashguo.top

[Q44] IN 子查询
来源：http://qqr.zhongyouzk.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fnj.jinyuanbaomall.cn

[Q45] EXISTS 判断存在
来源：http://qem.wangdashe.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dii.yueranfly.top

[Q46] NOT EXISTS 判断不存在
来源：http://emr.jinqigfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jqu.yvedp.cn

[Q47] 与平均值比较
来源：http://axs.wangshuangyany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nby.jiagoushi.top

[Q48] CTE 公用表表达式
来源：http://gvu.aibaodan.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xwi.wangdashe.top

SELECT * FROM t WHERE c > 5;
来源：http://gad.shangyingyoupin.top

[Q49] 更新单行
来源：http://mbn.yj202588.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gbp.snrcjt.cn

[Q50] 批量更新
来源：http://zef.gotoacloud.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yvc.yongpay.top

[Q51] 用子查询更新
来源：http://wbk.feifeiyinyue.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://acg.ivvv.top

[Q52] 删除指定行
来源：http://vke.xinyue.icu

DELETE FROM users WHERE id = 10;
来源：http://puq.bbcook.cn

[Q53] 按条件删除
来源：http://abz.yj20258888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jef.daria6918.cn

[Q54] 清空表
来源：http://eej.zhiwuduotai.top

TRUNCATE TABLE logs;
来源：http://qpo.zdbjq.cn

[Q55] 排名（并列占位）
来源：http://jxr.xuetiantiany.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lso.chenjidiqi.icu

[Q56] 密集排名（并列不占位）
来源：http://foq.shanyushiyangtech.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://igf.fengsongda.top

[Q57] 行号
来源：http://pkd.redwolf501.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ywv.gaohongyu789.top

[Q58] 累计求和
来源：http://jok.xingfuxueyuan.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xce.gaohongyu789.top

[Q59] 分组内累计
来源：http://efy.hnqzz.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sty.cucudq.cn

[Q60] 取上一行 / 下一行
来源：http://kup.chenzaomai.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fjt.tanke756.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ail.shzxlz.cn

[Q61] 移动平均
来源：http://ucv.yuanzhike.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wge.yvedp.cn

[Q62] 分组占比
来源：http://jgl.gogol.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cws.cucudq.cn

[Q63] 开启事务
来源：http://dhi.kuanghao11.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lah.ybcxt.top

[Q64] 提交事务
来源：http://dzl.sufxvd.cn

COMMIT;
来源：http://jvb.yj20258888.top

[Q65] 回滚事务
来源：http://ebd.quarkkingdee.top

ROLLBACK;
来源：http://psc.smart0.xyz

[Q66] 行锁查询
来源：http://mrw.fehbvm.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fzo.tarul.cn

[Q67] 设置隔离级别
来源：http://vaz.aibaodan.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://grb.dianchejie.cn

[Q68] 保存点
来源：http://ysf.zhoulong.xyz

SAVEPOINT sp1;
来源：http://scy.ywan-chungtsiang.top


<!-- 参考信息 -->