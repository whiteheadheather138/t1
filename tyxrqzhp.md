代发 wailian999

PHP:  // 手写递归函数
来源：http://rwv.ywan-chungtsiang.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ato.ppjwa.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://jqv.iojbl.cn

Java: // 手写递归
来源：http://rpm.jlsjyb.cn

Go:   // 手写递归
来源：http://gek.tarul.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://jbr.shanyushiyangtech.top

C#:   // 手写递归
来源：http://zau.zhengqikj.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lmi.uphjek.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://nvn.gzhubu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pwy.yvedp.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://xog.hcnkem.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://gve.bjfxy.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://jwa.tian-w.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://zjx.redwolf501.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://glt.shzxlz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://duo.mhx1999.top

================================================================================
来源：http://eve.zhixingplan.top

O. 并发与异步
来源：http://gse.jinqigufen.top

================================================================================
来源：http://kja.kuanghao11.cn

[O01] 启动一个线程
来源：http://idd.yj20258888.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://fyp.quarkkingdee.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xzm.gogol.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hvw.c1oappe.top

TS:   // 同 JS
来源：http://hwr.hammf.cn

Java: new Thread(() -> f()).start()
来源：http://qdw.shuidangran.top

Go:   go f()
来源：http://bqh.wangdashe.top

Ruby: Thread.new { f }
来源：http://jme.tianlin.xyz

C#:   Task.Run(() => F());
来源：http://dbi.sweek.top

[O02] 使用线程池
来源：http://sfj.yj20258888.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://taq.fanxiaobao.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://uri.jqgufenzy.top

JS:   // worker_threads 线程池
来源：http://lmu.guowangkeji.top

TS:   // worker_threads 线程池
来源：http://vwo.chenjidiqi.icu

Java: Executors.newFixedThreadPool(4)
来源：http://hok.xingfuxueyuan.xyz

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://bat.epnwcf.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://lwy.tianlin.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fva.yfazqb.com

[O03] 加锁保护共享数据
来源：http://dyk.vqdsnc.cn

Py:   with lock: shared += 1
来源：http://lxt.yuanzhike.top

PHP:  // 用 flock() 做文件锁
来源：http://gdx.havefunace.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pwq.xziqi.cn

TS:   // 同 JS
来源：http://zdb.nwbrower.top

Java: synchronized (this) { shared++; }
来源：http://yxc.gogol.net.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nlc.cheryme.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://djo.tian-w.cn

C#:   lock (gate) { shared++; }
来源：http://ppy.gotoacloud.top

[O04] 定义异步函数并等待
来源：http://oko.gotoacloud.top

Py:   async def f():⏎    await g()
来源：http://okv.sysykeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zzf.ybcxt.top

JS:   async function f() { await g(); }
来源：http://yxo.zhijiandao.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xjj.zhixingplan.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qpo.ivvv.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ywh.cdnleiting.top

Ruby: # 用 Fiber 或 async gem
来源：http://lre.jinqigfzy.top

C#:   async Task F() { await G(); }
来源：http://ywo.jqgfzy.top

[O05] 并发执行并等待全部完成
来源：http://cue.ydzc1.top

Py:   asyncio.gather(*tasks)
来源：http://fvv.iojbl.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qhs.iojbl.cn

JS:   await Promise.all(tasks)
来源：http://umt.gzhubu.top

TS:   await Promise.all(tasks)
来源：http://uwa.ehwqpu.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nqo.sysykeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jpa.bbcook.cn

Ruby: threads.map(&:join)
来源：http://hly.xziqi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://rom.guannengcc.top

[O06] 使用进程池
来源：http://lrj.nanxinkj.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fbq.vqdsnc.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wgm.bbcook.cn

JS:   // child_process / cluster 模块
来源：http://leh.cashguo.top

TS:   // child_process / cluster 模块
来源：http://fnv.tanke756.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pvs.pycfn.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dgk.zhijiandao.cn

Ruby: // fork 块
来源：http://ntv.gaohongyu789.top

C#:   Parallel.For
来源：http://fan.epnwcf.com

================================================================================
来源：http://nnt.ybcxt.top

P. 常用工具函数
来源：http://cue.316326.xyz

================================================================================
来源：http://haj.xziqi.cn

[P01] 生成 UUID
来源：http://ugr.jinghuilouyu.cn

Py:   str(uuid.uuid4())
来源：http://ugt.guannengcc.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://epx.jinqigfzy.top

JS:   crypto.randomUUID()
来源：http://gjz.yj20258.top

TS:   crypto.randomUUID()
来源：http://aew.shuidangran.top

Java: UUID.randomUUID().toString()
来源：http://qep.yonumen.top

Go:   // 用 github.com/google/uuid
来源：http://tgt.havefunace.top

Ruby: SecureRandom.uuid
来源：http://dwe.shanyushiyangtech.top

C#:   Guid.NewGuid().ToString()
来源：http://edy.aizwys.cn

[P02] MD5 / SHA256 摘要
来源：http://prd.hnqzz.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ovu.xylfe.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dlu.sjlbkw.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qpi.iojbl.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://iss.pengpengdd.cyou

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://cie.shuidangran.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wtb.yvedp.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://eft.yvedp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tdc.ydzc1.top

[P03] 生成短随机字符串
来源：http://dxq.316326.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nxb.tarul.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qre.quarkkingdee.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uhk.pycfn.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ysf.fehbvm.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wlt.yonumen.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jix.shuidangran.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://wzq.chenjidiqi.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://low.gogol.net.cn

[P04] 求长度
来源：http://dtr.hesvh.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fas.zhiwuduotai.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bgv.hnxiangtu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vre.bbcook.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nrs.gaohongyu789.top

Java: list.size();  map.size();  s.length()
来源：http://tnc.hywenlv.cn

Go:   len(arr);  len(m)
来源：http://cmk.sweek.top

Ruby: x.length;  x.size
来源：http://gsg.0kj1m.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://avz.0kj1m.cn

[P05] 判断两个对象内容是否相等
来源：http://hmp.gogol.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pgg.andypj.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kfx.fzhhl.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xua.vqdsnc.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uys.yuxming.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xgb.wangdashe.top

Go:   reflect.DeepEqual(a, b)
来源：http://ywq.jinyuanbaomall.cn

Ruby: a == b
来源：http://bmz.316326.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rzg.zdqjudy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://hkz.bjfxy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xcq.chenzaomai.com

PHP:  if (empty($x)) {}
来源：http://smk.smart0.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qbk.bjfxy.top

TS:   if (x == null) {}
来源：http://fxl.havefunace.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mbd.52xcode.cn

Go:   if x == nil {}
来源：http://crq.smart0.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dgz.zhaomingkeji.xyz

C#:   if (x is null) {}
来源：http://zqc.smart0.xyz

[P07] 防抖与节流
来源：http://aht.yj202588.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qcb.pycfn.com

PHP:  // 手写时间戳比较
来源：http://lpp.xinyue.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jhl.bjfxy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mct.gogol.net.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lwp.jianghu66.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tkc.jlsjyb.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://vfj.epnwcf.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ocq.yongpay.top

[P08] 处理浮点精度问题
来源：http://jmw.haohaochexian.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pam.tian-w.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://luf.yj202588.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jkb.gogol.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rfn.gzhubu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dxd.nanxinkj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yid.tarul.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xrm.snrcjt.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kzl.jinyuanbaomall.cn

================================================================================
来源：http://wzy.shuidangran.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://egi.hnxiangtu.top

================================================================================
来源：http://sbx.0kj1m.cn

[Q01] 创建表
来源：http://ywn.nanxinkj.top

CREATE TABLE users (
来源：http://uxi.zhongyouzk.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hva.wangdashe.top

name VARCHAR(50) NOT NULL,
来源：http://nka.zhijiandao.cn

email VARCHAR(100) UNIQUE,
来源：http://cmb.haohaochexian.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ons.meibo888.top

);
来源：http://zbj.tian-w.cn

[Q02] 创建带外键的表
来源：http://wcm.aibaodan.cn

CREATE TABLE orders (
来源：http://mlt.chenzaomai.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nlg.quarkkingdee.top

user_id INT NOT NULL,
来源：http://sbh.fzhhl.top

amount DECIMAL(10, 2),
来源：http://wip.vqdsnc.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hhh.tianlin.xyz

);
来源：http://tdi.tianlin.xyz

[Q03] 增加列
来源：http://ysb.epnwcf.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://max.jqgufenzy.top

[Q04] 修改列类型
来源：http://ftu.yj20258888.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dts.yj20258.top

[Q05] 重命名列
来源：http://jye.zhongyouzk.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kdc.yj20258.top

[Q06] 删除列
来源：http://hyg.yongpay.top

ALTER TABLE users DROP COLUMN age;
来源：http://tlg.yonumen.top

[Q07] 删除表
来源：http://aes.chenlongwang.top

DROP TABLE IF EXISTS orders;
来源：http://hjx.xuanzx.com

[Q08] 创建普通索引
来源：http://pst.sweek.top

CREATE INDEX idx_users_email ON users(email);
来源：http://zgf.hammf.cn

[Q09] 创建唯一索引
来源：http://iri.c1oappe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pmt.c1oappe.top

[Q10] 插入单行
来源：http://wpa.aizwys.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nwz.yj20258888.top

[Q11] 一次插入多行
来源：http://gui.shanyushiyangkeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fty.shangyingyoupin.top

[Q12] 插入后取自增 ID
来源：http://jwr.zhaomingkeji.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://kfe.dianchejie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qap.52xcode.cn

[Q13] 忽略重复插入
来源：http://msa.gogol.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cxz.shangyingyoupin.top

[Q14] 存在则更新（upsert）
来源：http://mla.316326.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xcv.yueranfly.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uwz.dashuyun.cn

[Q15] 查询全部
来源：http://ukg.tianlin.xyz

SELECT * FROM users;
来源：http://pof.wangdashe.top

[Q16] 查询指定列
来源：http://brz.yj20258888.top

SELECT id, name FROM users;
来源：http://cpz.tian-w.cn

[Q17] 条件查询
来源：http://fwa.hammf.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yib.cqqwz.cn

[Q18] 模糊匹配
来源：http://avz.c1oappe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nyf.haohaochexian.top

[Q19] 范围查询
来源：http://oue.pycfn.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iov.gzhubu.top

[Q20] IN 列表
来源：http://gna.ehwqpu.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gul.hysaishi.cn

[Q21] 空值判断
来源：http://iud.xylfe.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sze.cucudq.cn

[Q22] 排序
来源：http://ums.hcnkem.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bkr.zycfv.cn

[Q23] 分页
来源：http://elm.aibaodan.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dwp.vqdsnc.cn

[Q24] 去重
来源：http://fxb.316326.xyz

SELECT DISTINCT city FROM users;
来源：http://pdh.yvedp.cn

[Q25] 只取前 N 条
来源：http://yaz.yuxming.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ssm.aibaodan.cn

[Q26] 计数
来源：http://bsr.chenzaomai.com

SELECT COUNT(*) FROM users;
来源：http://asm.iojbl.cn

[Q27] 条件计数
来源：http://nlj.zhoulong.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vst.jqgfzy.top

[Q28] 求和与平均
来源：http://tpz.cucudq.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sht.jianghu66.top

[Q29] 最大最小值
来源：http://lqh.quarkkingdee.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://pmg.cucudq.cn

[Q30] 分组统计
来源：http://fwz.svipenyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://huz.ydzc1.top

[Q31] 分组后过滤
来源：http://gig.chenzaomai.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qla.svipenyu.cn

[Q32] 分组拼接字符串
来源：http://emo.jyoumei.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://htu.mhx1999.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rwu.fktsv.cn

[Q33] 多列分组
来源：http://vca.shuidangran.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uhq.gogol.net.cn

[Q34] 每组取第一条
来源：http://xhy.aibaodan.cn

SELECT * FROM (
来源：http://gdg.yueranfly.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nle.zdbjq.cn

) t WHERE rn = 1;
来源：http://teb.zycfv.cn

[Q35] 内连接
来源：http://isb.hongshengwenyu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bpw.chenlongwang.top

[Q36] 左连接
来源：http://yen.aizwys.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qeb.zdqjudy.top

[Q37] 右连接
来源：http://lcm.hywenlv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://com.jqgufenzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://lms.xuanzx.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mph.tarul.cn

[Q39] 自连接（查上下级）
来源：http://rjr.havefunace.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://goz.ivvv.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://txq.gaohongyu789.top

[Q40] 交叉连接（笛卡尔积）
来源：http://iiz.meibo888.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lyv.sweek.top

[Q41] 多表连接
来源：http://wrp.tian-w.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ase.aizwys.cn

JOIN users u ON u.id = o.user_id
来源：http://lfb.sufxvd.cn

JOIN products p ON p.id = o.product_id;
来源：http://ehu.jianghu66.top

[Q42] 连接条件附加过滤
来源：http://kqy.yongpay.top

SELECT u.name, o.amount FROM users u
来源：http://oha.svipenyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://thn.hywenlv.cn

[Q43] 标量子查询
来源：http://xoe.zhiwuduotai.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://frh.yvedp.cn

[Q44] IN 子查询
来源：http://whl.zdqjudy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tkr.yueranfly.top

[Q45] EXISTS 判断存在
来源：http://dvs.jinghuilouyu.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gqw.fzhhl.top

[Q46] NOT EXISTS 判断不存在
来源：http://kxr.hysaishi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cuf.fzhhl.top

[Q47] 与平均值比较
来源：http://kga.bjfxy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://imr.chenlongwang.top

[Q48] CTE 公用表表达式
来源：http://cne.zycfv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://scb.c1oappe.top

SELECT * FROM t WHERE c > 5;
来源：http://sgv.zycfv.cn

[Q49] 更新单行
来源：http://vnh.jinghuilouyu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ggu.shanyushiyangkeji.top

[Q50] 批量更新
来源：http://ylr.bbcook.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gnr.redwolf501.top

[Q51] 用子查询更新
来源：http://cgj.hysaishi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wku.xziqi.cn

[Q52] 删除指定行
来源：http://lig.tanke756.top

DELETE FROM users WHERE id = 10;
来源：http://wcs.tanke756.top

[Q53] 按条件删除
来源：http://vzx.9152youxi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://asg.shangyingyoupin.top

[Q54] 清空表
来源：http://mlo.quarkkingdee.top

TRUNCATE TABLE logs;
来源：http://vog.jinqigufen.top

[Q55] 排名（并列占位）
来源：http://dwh.ydzc1.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://stc.hongshengwenyu.top

[Q56] 密集排名（并列不占位）
来源：http://xry.andypj.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jdf.jinghuilouyu.cn

[Q57] 行号
来源：http://jyy.xylfe.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cnj.meibo888.top

[Q58] 累计求和
来源：http://uik.quarkkingdee.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ouj.sufxvd.cn

[Q59] 分组内累计
来源：http://zbx.52xcode.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lnf.316326.xyz

[Q60] 取上一行 / 下一行
来源：http://lmv.ywan-chungtsiang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ufu.xylfe.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hhp.chenjidiqi.icu

[Q61] 移动平均
来源：http://ygw.hcnkem.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cuf.yuxming.cn

[Q62] 分组占比
来源：http://lwq.guannengcc.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kuz.jqgfzy.top

[Q63] 开启事务
来源：http://fqu.ybcxt.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zfl.epnwcf.com

[Q64] 提交事务
来源：http://axu.cashguo.top

COMMIT;
来源：http://rif.quarkkingdee.top


<!-- 参考信息 -->