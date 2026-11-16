代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://dhr.xylfe.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://zmt.aibaodan.cn

[N11] 二叉树中序遍历
来源：http://tfp.xinyue.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://phu.shzxlz.cn

PHP:  // 手写递归函数
来源：http://wgb.andypj.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hcp.316326.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://pcx.zhixingplan.top

Java: // 手写递归
来源：http://zkp.zhengqikj.top

Go:   // 手写递归
来源：http://ywo.bjfxy.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nrh.9152youxi.cn

C#:   // 手写递归
来源：http://bcf.shuidangran.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fhf.sjlbkw.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://iik.sxryk.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://agy.gzhubu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wmq.hesvh.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://hzt.hcnkem.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://ebv.nanxuanxn.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://onh.meibo888.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://kjv.yuxming.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://dxe.quarkkingdee.top

================================================================================
来源：http://ryw.sweek.top

O. 并发与异步
来源：http://fbc.zdbjq.cn

================================================================================
来源：http://lrq.epnwcf.com

[O01] 启动一个线程
来源：http://hjd.gotoacloud.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://dvc.smart0.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://tue.cqqwz.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://iix.sxryk.cn

TS:   // 同 JS
来源：http://iur.316326.xyz

Java: new Thread(() -> f()).start()
来源：http://ium.jlsjyb.cn

Go:   go f()
来源：http://aqb.shuidangran.top

Ruby: Thread.new { f }
来源：http://uwd.hesvh.cn

C#:   Task.Run(() => F());
来源：http://xcl.vehdjk.com

[O02] 使用线程池
来源：http://kdf.hongshengwenyu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uaz.ehwqpu.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qmi.xziqi.cn

JS:   // worker_threads 线程池
来源：http://owt.tanke756.top

TS:   // worker_threads 线程池
来源：http://xqd.wangdashe.top

Java: Executors.newFixedThreadPool(4)
来源：http://swz.dianchejie.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ccf.cheryme.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://esv.jianghu66.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://asu.chenjidiqi.icu

[O03] 加锁保护共享数据
来源：http://xvu.ctjpmb.com

Py:   with lock: shared += 1
来源：http://lol.guowangkeji.top

PHP:  // 用 flock() 做文件锁
来源：http://uef.guannengcc.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hgu.kuanghao11.cn

TS:   // 同 JS
来源：http://jmb.ybcxt.top

Java: synchronized (this) { shared++; }
来源：http://ouz.shangyingyoupin.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bka.tanke756.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://gvs.fktsv.cn

C#:   lock (gate) { shared++; }
来源：http://ujw.fanxiaobao.xyz

[O04] 定义异步函数并等待
来源：http://fxf.haohaochexian.top

Py:   async def f():⏎    await g()
来源：http://ksj.zhijiandao.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://tzj.zhaomingkeji.xyz

JS:   async function f() { await g(); }
来源：http://ofu.yangfankeji.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://xnc.guowangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://gth.yangfankeji.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ven.andypj.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://bti.hnxiangtu.top

C#:   async Task F() { await G(); }
来源：http://goj.jinqigufen.top

[O05] 并发执行并等待全部完成
来源：http://zod.316326.xyz

Py:   asyncio.gather(*tasks)
来源：http://pmi.zycfv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yeo.bbcook.cn

JS:   await Promise.all(tasks)
来源：http://bza.fengsongda.top

TS:   await Promise.all(tasks)
来源：http://mfa.cdnleiting.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nwq.hysaishi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ytl.jyoumei.cn

Ruby: threads.map(&:join)
来源：http://wpp.ydjk.org.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kdy.fengsongda.top

[O06] 使用进程池
来源：http://yvb.guannengcc.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://csp.redwolf501.top

PHP:  // pcntl_fork 或多进程队列
来源：http://pax.xziqi.cn

JS:   // child_process / cluster 模块
来源：http://zqr.tianlin.xyz

TS:   // child_process / cluster 模块
来源：http://uph.quarkkingdee.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://uwe.svipenyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://sfs.ywan-chungtsiang.top

Ruby: // fork 块
来源：http://wqb.cashguo.top

C#:   Parallel.For
来源：http://elq.jlsjyb.cn

================================================================================
来源：http://yjy.guowangkeji.top

P. 常用工具函数
来源：http://xxg.ydzc1.top

================================================================================
来源：http://iei.tian-w.cn

[P01] 生成 UUID
来源：http://noa.ppjwa.cn

Py:   str(uuid.uuid4())
来源：http://ldr.kuanghao11.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tdf.pycfn.com

JS:   crypto.randomUUID()
来源：http://flk.zhengqikj.top

TS:   crypto.randomUUID()
来源：http://shi.xuetiantiany.cn

Java: UUID.randomUUID().toString()
来源：http://qph.mhx1999.top

Go:   // 用 github.com/google/uuid
来源：http://nww.chenjidiqi.icu

Ruby: SecureRandom.uuid
来源：http://szd.gotoacloud.top

C#:   Guid.NewGuid().ToString()
来源：http://nnk.hongshengwenyu.top

[P02] MD5 / SHA256 摘要
来源：http://dgy.pycfn.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vtg.jqgufenzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://wlo.hysaishi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://okn.chenjidiqi.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vnn.ybcxt.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ikc.yuanzhike.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zhg.fehbvm.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zfh.meibo888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kvi.jyoumei.cn

[P03] 生成短随机字符串
来源：http://vud.yuxming.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gfw.mhx1999.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gmm.yueranfly.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mci.shuidangran.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ift.wangdashe.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wlx.hywenlv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zjs.yj20258888.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ban.zhaomingkeji.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bup.daria6918.cn

[P04] 求长度
来源：http://vez.yuxming.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xoe.zdbjq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ouo.tarul.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://coi.snrcjt.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uqx.daria6918.cn

Java: list.size();  map.size();  s.length()
来源：http://hub.ywan-chungtsiang.top

Go:   len(arr);  len(m)
来源：http://auv.redwolf501.top

Ruby: x.length;  x.size
来源：http://evd.yuxming.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ubv.gaohongyu789.top

[P05] 判断两个对象内容是否相等
来源：http://eye.tian-w.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vsy.redwolf501.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nny.svipenyu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ocq.ywan-chungtsiang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://aem.zhijiandao.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bjv.xuanzx.com

Go:   reflect.DeepEqual(a, b)
来源：http://lzj.jinghuilouyu.cn

Ruby: a == b
来源：http://sql.xinyue.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mwt.fzhhl.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://inw.vqdsnc.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ymf.feifeiyinyue.top

PHP:  if (empty($x)) {}
来源：http://fyy.cheryme.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://eoc.yj202588.top

TS:   if (x == null) {}
来源：http://ebb.sxryk.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://suj.yj20258.top

Go:   if x == nil {}
来源：http://eba.yj202588.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://knn.gotoacloud.top

C#:   if (x is null) {}
来源：http://cww.andypj.xyz

[P07] 防抖与节流
来源：http://prd.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://duk.jqgfzy.top

PHP:  // 手写时间戳比较
来源：http://obb.xuetiantiany.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rbk.316326.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yon.birdmap.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dac.snrcjt.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hsf.jqgfzy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://usk.cucudq.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rxb.ywan-chungtsiang.top

[P08] 处理浮点精度问题
来源：http://axu.yj202588.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xsb.gogol.net.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zgk.gzhubu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tbt.yvedp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fvr.aizwys.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wlm.yanxiufei.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vqo.snrcjt.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kfn.zhiwuduotai.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qcu.sxryk.cn

================================================================================
来源：http://wgu.dianchejie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://usi.yj202588.top

================================================================================
来源：http://euo.pengpengdd.cyou

[Q01] 创建表
来源：http://unp.0kj1m.cn

CREATE TABLE users (
来源：http://ssk.chenlongwang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zpl.yongpay.top

name VARCHAR(50) NOT NULL,
来源：http://wag.hammf.cn

email VARCHAR(100) UNIQUE,
来源：http://aba.sufxvd.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://srd.jqgfzy.top

);
来源：http://ddh.zhoulong.xyz

[Q02] 创建带外键的表
来源：http://odt.yanxiufei.cn

CREATE TABLE orders (
来源：http://xpp.ybcxt.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lvx.yonumen.top

user_id INT NOT NULL,
来源：http://oha.aibaodan.cn

amount DECIMAL(10, 2),
来源：http://uhz.chenlongwang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qor.gaohongyu789.top

);
来源：http://bck.fanxiaobao.xyz

[Q03] 增加列
来源：http://syu.tanke756.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vhh.yangfankeji.com

[Q04] 修改列类型
来源：http://yfe.zhongyouzk.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iop.jqgfzy.top

[Q05] 重命名列
来源：http://fse.jinqigfzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ghe.sysykeji.top

[Q06] 删除列
来源：http://rmx.hcnkem.com

ALTER TABLE users DROP COLUMN age;
来源：http://rqk.wangshuangyany.cn

[Q07] 删除表
来源：http://lcg.shanyushiyangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://dqf.yuanzhike.top

[Q08] 创建普通索引
来源：http://xqn.sjlbkw.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://bsz.redwolf501.top

[Q09] 创建唯一索引
来源：http://ado.wangdashe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kfi.jqgufenzy.top

[Q10] 插入单行
来源：http://tnw.redwolf501.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tpu.ybcxt.top

[Q11] 一次插入多行
来源：http://ott.xuetiantiany.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hrk.mhx1999.top

[Q12] 插入后取自增 ID
来源：http://tsw.aizwys.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ort.hywenlv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pkd.svipenyu.cn

[Q13] 忽略重复插入
来源：http://sqg.xuanzx.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zpj.svipenyu.cn

[Q14] 存在则更新（upsert）
来源：http://jak.hesvh.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nrz.nwbrower.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yjn.jlsjyb.cn

[Q15] 查询全部
来源：http://fhp.cheryme.top

SELECT * FROM users;
来源：http://owg.ydzc1.top

[Q16] 查询指定列
来源：http://pmc.316326.xyz

SELECT id, name FROM users;
来源：http://wdn.bbcook.cn

[Q17] 条件查询
来源：http://pts.haohaochexian.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fwu.xylfe.cn

[Q18] 模糊匹配
来源：http://qxj.zhaomingkeji.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sfg.yonumen.top

[Q19] 范围查询
来源：http://fsi.yuxming.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nos.redwolf501.top

[Q20] IN 列表
来源：http://jzj.feifeiyinyue.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jjw.hnxiangtu.top

[Q21] 空值判断
来源：http://gzu.redwolf501.top

SELECT * FROM users WHERE email IS NULL;
来源：http://zkg.xylfe.cn

[Q22] 排序
来源：http://ghz.feifeiyinyue.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oyo.yueranfly.top

[Q23] 分页
来源：http://kua.yuanzhike.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mui.yj20258.top

[Q24] 去重
来源：http://uak.fanxiaobao.xyz

SELECT DISTINCT city FROM users;
来源：http://mfx.hnxiangtu.top

[Q25] 只取前 N 条
来源：http://iua.gogol.net.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uts.tianlin.xyz

[Q26] 计数
来源：http://jem.sweek.top

SELECT COUNT(*) FROM users;
来源：http://phv.bjfxy.top

[Q27] 条件计数
来源：http://uab.hammf.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xmo.pengpengdd.cyou

[Q28] 求和与平均
来源：http://brg.fanxiaobao.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yme.shangyingyoupin.top

[Q29] 最大最小值
来源：http://qic.ydjk.org.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hhe.xinyue.icu

[Q30] 分组统计
来源：http://mrv.birdmap.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tdt.uphjek.com

[Q31] 分组后过滤
来源：http://vgs.tarul.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://oci.jinqigufen.top

[Q32] 分组拼接字符串
来源：http://rpo.zhongyouzk.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xgq.sufxvd.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://suh.snrcjt.cn

[Q33] 多列分组
来源：http://abe.yueranfly.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hsj.yuxming.cn

[Q34] 每组取第一条
来源：http://csu.nanxuanxn.top

SELECT * FROM (
来源：http://liv.yangfankeji.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ply.guowangkeji.top

) t WHERE rn = 1;
来源：http://hvd.bjfxy.top

[Q35] 内连接
来源：http://xei.shuidangran.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yng.fzhhl.top

[Q36] 左连接
来源：http://nnz.hesvh.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yko.haohaochexian.top

[Q37] 右连接
来源：http://xpo.shanyushiyangtech.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hjl.quarkkingdee.top

[Q38] 全外连接（PostgreSQL）
来源：http://igd.hysaishi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pav.ydzc1.top

[Q39] 自连接（查上下级）
来源：http://nxx.tianlin.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://qoo.redwolf501.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nfo.snrcjt.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fkl.fzhhl.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qyy.ehwqpu.com

[Q41] 多表连接
来源：http://rsx.hesvh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pia.nanxinkj.top

JOIN users u ON u.id = o.user_id
来源：http://nfy.cucudq.cn

JOIN products p ON p.id = o.product_id;
来源：http://wvu.dianchejie.cn

[Q42] 连接条件附加过滤
来源：http://dej.yuxming.cn

SELECT u.name, o.amount FROM users u
来源：http://jmv.gogol.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ybb.jqgfzy.top

[Q43] 标量子查询
来源：http://uik.dashuyun.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mbt.fanxiaobao.xyz

[Q44] IN 子查询
来源：http://bxx.quarkkingdee.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jzl.xinyue.icu

[Q45] EXISTS 判断存在
来源：http://zgv.redwolf501.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nvj.yongpay.top

[Q46] NOT EXISTS 判断不存在
来源：http://jkr.jyoumei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xfu.sysykeji.top

[Q47] 与平均值比较
来源：http://shu.vehdjk.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sgc.ehwqpu.com

[Q48] CTE 公用表表达式
来源：http://quz.yvedp.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hzw.uphjek.com

SELECT * FROM t WHERE c > 5;
来源：http://jro.jiagoushi.top

[Q49] 更新单行
来源：http://she.wangdashe.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ohz.jinyuanbaomall.cn

[Q50] 批量更新
来源：http://zsv.chenjidiqi.icu

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hpn.cashguo.top

[Q51] 用子查询更新
来源：http://jch.xziqi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://huv.hongshengwenyu.top

[Q52] 删除指定行
来源：http://xzc.havefunace.top

DELETE FROM users WHERE id = 10;
来源：http://zcn.mhx1999.top

[Q53] 按条件删除
来源：http://hhm.tarul.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tdl.nanxinkj.top

[Q54] 清空表
来源：http://lsc.cdnleiting.top

TRUNCATE TABLE logs;
来源：http://cxx.jinyuanbaomall.cn

[Q55] 排名（并列占位）
来源：http://nmp.gogol.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://osu.snrcjt.cn

[Q56] 密集排名（并列不占位）
来源：http://vff.0kj1m.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tin.cashguo.top

[Q57] 行号
来源：http://rlz.yonumen.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://iuw.bjfxy.top

[Q58] 累计求和
来源：http://jcl.havefunace.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qwd.aibaodan.cn

[Q59] 分组内累计
来源：http://evp.tian-w.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ixc.fehbvm.com

[Q60] 取上一行 / 下一行
来源：http://nkb.zhiwuduotai.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fod.feifeiyinyue.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tag.dianchejie.cn

[Q61] 移动平均
来源：http://dlh.zdbjq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://kaf.gogol.net.cn

[Q62] 分组占比
来源：http://ilq.zhiwuduotai.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ffr.xziqi.cn


<!-- 参考信息 -->