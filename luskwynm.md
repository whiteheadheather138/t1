代发 wailian999

Go:   // 手写递归
来源：http://olx.dianchejie.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://umb.jqgufenzy.top

C#:   // 手写递归
来源：http://ope.aizwys.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://czm.jinqigufen.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://dnt.wangdashe.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://gol.jyoumei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iui.gzhubu.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ule.andypj.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://udh.chenjidiqi.icu

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mat.jinqigufen.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jge.jqgfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jwr.shzxlz.cn

================================================================================
来源：http://njo.0kj1m.cn

O. 并发与异步
来源：http://wsy.jiagoushi.top

================================================================================
来源：http://hkc.ctjpmb.com

[O01] 启动一个线程
来源：http://scw.ctjpmb.com

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ryo.jqgufenzy.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qek.gaohongyu789.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nun.cucudq.cn

TS:   // 同 JS
来源：http://nna.andypj.xyz

Java: new Thread(() -> f()).start()
来源：http://vid.feifeiyinyue.top

Go:   go f()
来源：http://rwo.uphjek.com

Ruby: Thread.new { f }
来源：http://vbu.ivvv.top

C#:   Task.Run(() => F());
来源：http://ieh.yvedp.cn

[O02] 使用线程池
来源：http://zmc.c1oappe.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dpu.chenzaomai.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xif.vehdjk.com

JS:   // worker_threads 线程池
来源：http://aim.yangfankeji.com

TS:   // worker_threads 线程池
来源：http://xea.hesvh.cn

Java: Executors.newFixedThreadPool(4)
来源：http://jhd.cdnleiting.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://qkn.jqgufenzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mhh.zycfv.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jfa.yj20258.top

[O03] 加锁保护共享数据
来源：http://pol.hnxiangtu.top

Py:   with lock: shared += 1
来源：http://qbq.hammf.cn

PHP:  // 用 flock() 做文件锁
来源：http://lan.hfpthk.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vwo.gogol.net.cn

TS:   // 同 JS
来源：http://dyu.yvedp.cn

Java: synchronized (this) { shared++; }
来源：http://bwq.gzhubu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://leo.vehdjk.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://vmu.hnqzz.top

C#:   lock (gate) { shared++; }
来源：http://zsw.shanyushiyangkeji.top

[O04] 定义异步函数并等待
来源：http://yxb.mhx1999.top

Py:   async def f():⏎    await g()
来源：http://gtc.ywan-chungtsiang.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://auz.ybcxt.top

JS:   async function f() { await g(); }
来源：http://kvm.nanxuanxn.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://opk.wangdashe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://frj.sysykeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ptf.ywan-chungtsiang.top

Ruby: # 用 Fiber 或 async gem
来源：http://tuj.gaohongyu789.top

C#:   async Task F() { await G(); }
来源：http://xil.jiagoushi.top

[O05] 并发执行并等待全部完成
来源：http://rgf.xingfuxueyuan.xyz

Py:   asyncio.gather(*tasks)
来源：http://btp.gaohongyu789.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mbp.hnxiangtu.top

JS:   await Promise.all(tasks)
来源：http://avp.hnxiangtu.top

TS:   await Promise.all(tasks)
来源：http://eng.hywenlv.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wch.dashuyun.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iut.xingfuxueyuan.xyz

Ruby: threads.map(&:join)
来源：http://tsa.haohaochexian.top

C#:   await Task.WhenAll(t1, t2)
来源：http://qdh.xuanzx.com

[O06] 使用进程池
来源：http://qjq.shuidangran.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mde.c1oappe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://sxp.hesvh.cn

JS:   // child_process / cluster 模块
来源：http://ahn.yongpay.top

TS:   // child_process / cluster 模块
来源：http://rym.fehbvm.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kjv.shzxlz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://srj.fehbvm.com

Ruby: // fork 块
来源：http://zzj.ydzc1.top

C#:   Parallel.For
来源：http://omv.epnwcf.com

================================================================================
来源：http://uvs.yj20258.top

P. 常用工具函数
来源：http://hxm.smart0.xyz

================================================================================
来源：http://env.birdmap.top

[P01] 生成 UUID
来源：http://kvu.cdnleiting.top

Py:   str(uuid.uuid4())
来源：http://dee.daxiang520.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kxq.yuanzhike.top

JS:   crypto.randomUUID()
来源：http://olb.hcnkem.com

TS:   crypto.randomUUID()
来源：http://bcl.jyoumei.cn

Java: UUID.randomUUID().toString()
来源：http://pkf.ehwqpu.com

Go:   // 用 github.com/google/uuid
来源：http://kzr.xziqi.cn

Ruby: SecureRandom.uuid
来源：http://iku.ydzc1.top

C#:   Guid.NewGuid().ToString()
来源：http://xqy.xuetiantiany.cn

[P02] MD5 / SHA256 摘要
来源：http://gxm.birdmap.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vdk.bbcook.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://oae.iojbl.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://agl.sweek.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nsy.ydzc1.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rmn.sjlbkw.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eln.gaohongyu789.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ewz.mhx1999.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zpw.9152youxi.cn

[P03] 生成短随机字符串
来源：http://tgh.aizwys.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://izt.yj202588.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zww.sufxvd.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://isp.jyoumei.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zwb.jinghuilouyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lvc.tian-w.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dud.yj202588.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://npu.wangdashe.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://byw.feifeiyinyue.top

[P04] 求长度
来源：http://pwo.dashuyun.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fur.ivvv.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nmh.chenzaomai.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lik.shanyushiyangtech.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://crd.shuidangran.top

Java: list.size();  map.size();  s.length()
来源：http://gch.cdnleiting.top

Go:   len(arr);  len(m)
来源：http://smo.svipenyu.cn

Ruby: x.length;  x.size
来源：http://xrg.birdmap.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nlq.epnwcf.com

[P05] 判断两个对象内容是否相等
来源：http://bah.ydzc1.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mhr.yuanzhike.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tvf.fanxiaobao.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cjh.zycfv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cro.yj20258.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ejd.gotoacloud.top

Go:   reflect.DeepEqual(a, b)
来源：http://fvf.sysykeji.top

Ruby: a == b
来源：http://mht.gaohongyu789.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kmx.yonumen.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://voh.c1oappe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xva.zdqjudy.top

PHP:  if (empty($x)) {}
来源：http://rfl.dianchejie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rqn.xziqi.cn

TS:   if (x == null) {}
来源：http://khm.jinqigfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ran.gotoacloud.top

Go:   if x == nil {}
来源：http://elg.ppjwa.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hqd.nanxuanxn.top

C#:   if (x is null) {}
来源：http://bbs.guowangkeji.top

[P07] 防抖与节流
来源：http://ucq.hammf.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://iqf.sysykeji.top

PHP:  // 手写时间戳比较
来源：http://kgp.daria6918.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zcy.yj20258.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://arf.dianchejie.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zxp.tian-w.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ufu.dashuyun.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wxf.fzhhl.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tfb.nanxuanxn.top

[P08] 处理浮点精度问题
来源：http://kao.sweek.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://for.xuanzx.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://doq.zhixingplan.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gub.shanyushiyangtech.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vqz.zhiwuduotai.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hnb.yongpay.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bsd.shangyingyoupin.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fup.hammf.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eud.zhoulong.xyz

================================================================================
来源：http://wdh.vqdsnc.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xyj.nwbrower.top

================================================================================
来源：http://pvc.yj20258888.top

[Q01] 创建表
来源：http://qqb.feifeiyinyue.top

CREATE TABLE users (
来源：http://czh.nanxinkj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://atx.nwbrower.top

name VARCHAR(50) NOT NULL,
来源：http://pzu.zhengqikj.top

email VARCHAR(100) UNIQUE,
来源：http://ydf.fanxiaobao.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fnn.daxiang520.top

);
来源：http://klj.yvedp.cn

[Q02] 创建带外键的表
来源：http://fus.ivvv.top

CREATE TABLE orders (
来源：http://lga.guowangkeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lmk.zhixingplan.top

user_id INT NOT NULL,
来源：http://xgw.feifeiyinyue.top

amount DECIMAL(10, 2),
来源：http://xov.vqdsnc.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hzo.tian-w.cn

);
来源：http://mja.wangdashe.top

[Q03] 增加列
来源：http://tbx.hcnkem.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wia.aibaodan.cn

[Q04] 修改列类型
来源：http://ntf.sysykeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nxt.jqgfzy.top

[Q05] 重命名列
来源：http://brh.c1oappe.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xoj.gogol.net.cn

[Q06] 删除列
来源：http://vul.guannengcc.top

ALTER TABLE users DROP COLUMN age;
来源：http://rir.nanxinkj.top

[Q07] 删除表
来源：http://eni.iojbl.cn

DROP TABLE IF EXISTS orders;
来源：http://vmf.snrcjt.cn

[Q08] 创建普通索引
来源：http://wnq.yonumen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://cuz.sufxvd.cn

[Q09] 创建唯一索引
来源：http://xre.sweek.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cik.gzhubu.top

[Q10] 插入单行
来源：http://xzk.redwolf501.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xus.hnqzz.top

[Q11] 一次插入多行
来源：http://xqn.ydzc1.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qdw.jinqigufen.top

[Q12] 插入后取自增 ID
来源：http://zup.cheryme.top

INSERT INTO users (name) VALUES ('C');
来源：http://gpx.shangyingyoupin.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zlo.yueranfly.top

[Q13] 忽略重复插入
来源：http://ade.zhixingplan.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://euh.guannengcc.top

[Q14] 存在则更新（upsert）
来源：http://vod.pycfn.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ivr.vqdsnc.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rms.ppjwa.cn

[Q15] 查询全部
来源：http://ycs.jqgfzy.top

SELECT * FROM users;
来源：http://jjq.andypj.xyz

[Q16] 查询指定列
来源：http://rol.nanxinkj.top

SELECT id, name FROM users;
来源：http://dou.sysykeji.top

[Q17] 条件查询
来源：http://juj.hcnkem.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ftt.chenjidiqi.icu

[Q18] 模糊匹配
来源：http://etc.quarkkingdee.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uic.xinyue.icu

[Q19] 范围查询
来源：http://wai.316326.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xwp.hongshengwenyu.top

[Q20] IN 列表
来源：http://qxr.vehdjk.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rlc.tarul.cn

[Q21] 空值判断
来源：http://ehm.shangyingyoupin.top

SELECT * FROM users WHERE email IS NULL;
来源：http://phv.fanxiaobao.xyz

[Q22] 排序
来源：http://kxz.jyoumei.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://seu.zhixingplan.top

[Q23] 分页
来源：http://pfj.yongpay.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hls.jiagoushi.top

[Q24] 去重
来源：http://qdm.ydjk.org.cn

SELECT DISTINCT city FROM users;
来源：http://ajo.cheryme.top

[Q25] 只取前 N 条
来源：http://fif.ydjk.org.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dxd.zhengqikj.top

[Q26] 计数
来源：http://fhs.tianlin.xyz

SELECT COUNT(*) FROM users;
来源：http://snk.hnxiangtu.top

[Q27] 条件计数
来源：http://wvx.uphjek.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bdj.jianghu66.top

[Q28] 求和与平均
来源：http://bpa.shzxlz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sfn.tanke756.top

[Q29] 最大最小值
来源：http://jkr.zhengqikj.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://bte.epnwcf.com

[Q30] 分组统计
来源：http://mqs.tian-w.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ykp.jyoumei.cn

[Q31] 分组后过滤
来源：http://cki.hammf.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rci.fengsongda.top

[Q32] 分组拼接字符串
来源：http://klp.cdnleiting.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ttv.jinghuilouyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lkn.hfpthk.cn

[Q33] 多列分组
来源：http://gmf.gaohongyu789.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dqi.bbcook.cn

[Q34] 每组取第一条
来源：http://jnf.hywenlv.cn

SELECT * FROM (
来源：http://lpy.sjlbkw.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nyc.xinyue.icu

) t WHERE rn = 1;
来源：http://tzx.xinyue.icu

[Q35] 内连接
来源：http://pco.ivvv.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vbb.gaohongyu789.top

[Q36] 左连接
来源：http://jah.hywenlv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yaa.tianlin.xyz

[Q37] 右连接
来源：http://hyi.hywenlv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uih.wangshuangyany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dfn.ivvv.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gry.snrcjt.cn

[Q39] 自连接（查上下级）
来源：http://otm.fanxiaobao.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://smu.gaohongyu789.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hit.epnwcf.com

[Q40] 交叉连接（笛卡尔积）
来源：http://str.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ddv.bbcook.cn

[Q41] 多表连接
来源：http://dyp.zhoulong.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://rdm.tarul.cn

JOIN users u ON u.id = o.user_id
来源：http://lgm.zhixingplan.top

JOIN products p ON p.id = o.product_id;
来源：http://nvw.zhengqikj.top

[Q42] 连接条件附加过滤
来源：http://fsb.ppjwa.cn

SELECT u.name, o.amount FROM users u
来源：http://nat.yvedp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hxw.shuidangran.top

[Q43] 标量子查询
来源：http://sfs.xylfe.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hkf.smart0.xyz

[Q44] IN 子查询
来源：http://dmv.jinqigufen.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tgd.316326.xyz

[Q45] EXISTS 判断存在
来源：http://zgy.zhiwuduotai.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fns.nanxinkj.top

[Q46] NOT EXISTS 判断不存在
来源：http://uaq.yongpay.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dds.gotoacloud.top

[Q47] 与平均值比较
来源：http://aua.birdmap.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://klk.zdqjudy.top

[Q48] CTE 公用表表达式
来源：http://bmd.chenzaomai.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pvd.snrcjt.cn

SELECT * FROM t WHERE c > 5;
来源：http://pwz.wangdashe.top

[Q49] 更新单行
来源：http://ars.xinyue.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rpq.vehdjk.com

[Q50] 批量更新
来源：http://djn.pycfn.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xdq.zycfv.cn

[Q51] 用子查询更新
来源：http://zbx.hfpthk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mpm.yuxming.cn

[Q52] 删除指定行
来源：http://pxu.tarul.cn

DELETE FROM users WHERE id = 10;
来源：http://vyj.xylfe.cn

[Q53] 按条件删除
来源：http://htc.pycfn.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jls.wangdashe.top

[Q54] 清空表
来源：http://kgo.jyoumei.cn

TRUNCATE TABLE logs;
来源：http://kvk.hywenlv.cn

[Q55] 排名（并列占位）
来源：http://klr.pengpengdd.cyou

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pqz.yanxiufei.cn

[Q56] 密集排名（并列不占位）
来源：http://iyx.tarul.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zmc.xziqi.cn

[Q57] 行号
来源：http://fyh.hywenlv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ufy.hfpthk.cn

[Q58] 累计求和
来源：http://kfq.yueranfly.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xhj.aibaodan.cn

[Q59] 分组内累计
来源：http://zwx.wangshuangyany.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sxz.zycfv.cn

[Q60] 取上一行 / 下一行
来源：http://cfn.cqqwz.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://iwt.cucudq.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ceh.tianlin.xyz

[Q61] 移动平均
来源：http://put.jinghuilouyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://unm.hywenlv.cn

[Q62] 分组占比
来源：http://xnc.sweek.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qxq.meibo888.top

[Q63] 开启事务
来源：http://ljl.ybcxt.top

START TRANSACTION;                -- 或 BEGIN
来源：http://psp.aibaodan.cn

[Q64] 提交事务
来源：http://fsm.jinyuanbaomall.cn

COMMIT;
来源：http://ykc.0kj1m.cn

[Q65] 回滚事务
来源：http://azx.epnwcf.com

ROLLBACK;
来源：http://ayr.tian-w.cn

[Q66] 行锁查询
来源：http://pgy.shangyingyoupin.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pad.yj20258.top


<!-- 参考信息 -->