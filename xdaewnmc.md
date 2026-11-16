代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://snp.cheryme.top

C#:   class Node { public int V; public Node? Next; }
来源：http://gtc.jqgfzy.top

[N11] 二叉树中序遍历
来源：http://fyk.zhiwuduotai.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://giq.yj20258888.top

PHP:  // 手写递归函数
来源：http://wxj.xuetiantiany.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ugr.yj20258888.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hhe.yj20258.top

Java: // 手写递归
来源：http://tgx.ywan-chungtsiang.top

Go:   // 手写递归
来源：http://lpv.zhoulong.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yka.jinqigfzy.top

C#:   // 手写递归
来源：http://cdi.jlsjyb.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wif.cheryme.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://awa.meibo888.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://odc.cashguo.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bws.zdbjq.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ozi.yj20258888.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bkg.fengsongda.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://cvt.sxryk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ydk.zhengqikj.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://jkp.ppjwa.cn

================================================================================
来源：http://ycy.sysykeji.top

O. 并发与异步
来源：http://enu.dashuyun.cn

================================================================================
来源：http://rmp.smart0.xyz

[O01] 启动一个线程
来源：http://iqs.smart0.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vij.xylfe.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bug.316326.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mta.ctjpmb.com

TS:   // 同 JS
来源：http://gfx.yuxming.cn

Java: new Thread(() -> f()).start()
来源：http://slo.zhoulong.xyz

Go:   go f()
来源：http://wkl.bbcook.cn

Ruby: Thread.new { f }
来源：http://ygc.cheryme.top

C#:   Task.Run(() => F());
来源：http://cwo.0kj1m.cn

[O02] 使用线程池
来源：http://wfy.xylfe.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zmt.nanxinkj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://jot.yongpay.top

JS:   // worker_threads 线程池
来源：http://esj.ydzc1.top

TS:   // worker_threads 线程池
来源：http://euf.dianchejie.cn

Java: Executors.newFixedThreadPool(4)
来源：http://zmo.ydzc1.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hzw.shuidangran.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://hah.gotoacloud.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uib.xziqi.cn

[O03] 加锁保护共享数据
来源：http://umc.aibaodan.cn

Py:   with lock: shared += 1
来源：http://ffr.zhengqikj.top

PHP:  // 用 flock() 做文件锁
来源：http://gmv.guowangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wqp.hammf.cn

TS:   // 同 JS
来源：http://frp.pengpengdd.cyou

Java: synchronized (this) { shared++; }
来源：http://vfv.ctjpmb.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://ebq.ydzc1.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://zon.ppjwa.cn

C#:   lock (gate) { shared++; }
来源：http://seu.cqqwz.cn

[O04] 定义异步函数并等待
来源：http://pfa.dianchejie.cn

Py:   async def f():⏎    await g()
来源：http://akr.jianghu66.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yqn.jiagoushi.top

JS:   async function f() { await g(); }
来源：http://dvh.hfpthk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bzn.chenjidiqi.icu

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rwb.shzxlz.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ytf.zdqjudy.top

Ruby: # 用 Fiber 或 async gem
来源：http://fsn.tianlin.xyz

C#:   async Task F() { await G(); }
来源：http://bvc.zhoulong.xyz

[O05] 并发执行并等待全部完成
来源：http://ohm.sysykeji.top

Py:   asyncio.gather(*tasks)
来源：http://chu.yueranfly.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vwb.hfpthk.cn

JS:   await Promise.all(tasks)
来源：http://aim.nanxuanxn.top

TS:   await Promise.all(tasks)
来源：http://sht.jqgfzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zrd.jqgufenzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zen.yj20258888.top

Ruby: threads.map(&:join)
来源：http://pmc.meibo888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lcx.iojbl.cn

[O06] 使用进程池
来源：http://khp.chenjidiqi.icu

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://gov.tianlin.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://nfv.gogol.net.cn

JS:   // child_process / cluster 模块
来源：http://cev.feifeiyinyue.top

TS:   // child_process / cluster 模块
来源：http://qaf.cqqwz.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://miv.ppjwa.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cfb.fzhhl.top

Ruby: // fork 块
来源：http://yhn.svipenyu.cn

C#:   Parallel.For
来源：http://jst.jinghuilouyu.cn

================================================================================
来源：http://iko.gogol.net.cn

P. 常用工具函数
来源：http://ejt.vqdsnc.cn

================================================================================
来源：http://cso.zycfv.cn

[P01] 生成 UUID
来源：http://lif.9152youxi.cn

Py:   str(uuid.uuid4())
来源：http://zet.shangyingyoupin.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://czs.yj202588.top

JS:   crypto.randomUUID()
来源：http://imp.gaohongyu789.top

TS:   crypto.randomUUID()
来源：http://fdr.havefunace.top

Java: UUID.randomUUID().toString()
来源：http://njf.hammf.cn

Go:   // 用 github.com/google/uuid
来源：http://yhu.jqgufenzy.top

Ruby: SecureRandom.uuid
来源：http://qjs.jinyuanbaomall.cn

C#:   Guid.NewGuid().ToString()
来源：http://kff.zhiwuduotai.top

[P02] MD5 / SHA256 摘要
来源：http://yxz.ydjk.org.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ikn.jiagoushi.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://dhf.jinqigfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://anq.jqgfzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xsw.vehdjk.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kxe.sysykeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ayj.jinqigufen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://thv.sjlbkw.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aob.xylfe.cn

[P03] 生成短随机字符串
来源：http://kuw.vqdsnc.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ndd.feifeiyinyue.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gxt.aibaodan.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bsx.yj20258888.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cmb.jlsjyb.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mlu.tarul.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mfx.snrcjt.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ktw.nanxuanxn.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ygm.meibo888.top

[P04] 求长度
来源：http://pmj.tarul.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hit.zdbjq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qsp.xziqi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yjn.bjfxy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ecz.yongpay.top

Java: list.size();  map.size();  s.length()
来源：http://pmd.meibo888.top

Go:   len(arr);  len(m)
来源：http://erh.pycfn.com

Ruby: x.length;  x.size
来源：http://hhl.shuidangran.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zdd.sweek.top

[P05] 判断两个对象内容是否相等
来源：http://fif.birdmap.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://oxm.ydzc1.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://psl.hammf.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xdl.daxiang520.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jpn.dianchejie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ioz.gogol.net.cn

Go:   reflect.DeepEqual(a, b)
来源：http://qef.tanke756.top

Ruby: a == b
来源：http://gkz.hongshengwenyu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hkl.9152youxi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oxb.vqdsnc.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dul.yj20258.top

PHP:  if (empty($x)) {}
来源：http://dhn.wangdashe.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wkv.yanxiufei.cn

TS:   if (x == null) {}
来源：http://xcj.pengpengdd.cyou

Java: if (x == null || x.isEmpty()) {}
来源：http://yxc.jinghuilouyu.cn

Go:   if x == nil {}
来源：http://ddq.jianghu66.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vbg.xuanzx.com

C#:   if (x is null) {}
来源：http://kue.cheryme.top

[P07] 防抖与节流
来源：http://cgs.feifeiyinyue.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://evn.redwolf501.top

PHP:  // 手写时间戳比较
来源：http://rmn.aizwys.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://neq.feifeiyinyue.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ols.9152youxi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zky.havefunace.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://myw.cashguo.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://tfs.zdbjq.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hlm.shuidangran.top

[P08] 处理浮点精度问题
来源：http://fcn.jianghu66.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wii.guowangkeji.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gjr.hnxiangtu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gjw.yvedp.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vkm.redwolf501.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://iyf.ybcxt.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://aca.zdqjudy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lix.dashuyun.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dkz.fanxiaobao.xyz

================================================================================
来源：http://qrn.xylfe.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kni.dashuyun.cn

================================================================================
来源：http://lsm.ehwqpu.com

[Q01] 创建表
来源：http://pms.gogol.net.cn

CREATE TABLE users (
来源：http://pzb.yonumen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gps.yuxming.cn

name VARCHAR(50) NOT NULL,
来源：http://zik.zycfv.cn

email VARCHAR(100) UNIQUE,
来源：http://mlv.ydzc1.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ojb.0kj1m.cn

);
来源：http://gtf.52xcode.cn

[Q02] 创建带外键的表
来源：http://hcr.dashuyun.cn

CREATE TABLE orders (
来源：http://djr.hongshengwenyu.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bqe.ppjwa.cn

user_id INT NOT NULL,
来源：http://iab.fehbvm.com

amount DECIMAL(10, 2),
来源：http://zpy.gogol.net.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vov.cucudq.cn

);
来源：http://lun.jlsjyb.cn

[Q03] 增加列
来源：http://vfq.zycfv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ofg.xylfe.cn

[Q04] 修改列类型
来源：http://reb.nanxuanxn.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yfe.chenlongwang.top

[Q05] 重命名列
来源：http://frx.sjlbkw.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ecv.vqdsnc.cn

[Q06] 删除列
来源：http://oqh.hesvh.cn

ALTER TABLE users DROP COLUMN age;
来源：http://qet.quarkkingdee.top

[Q07] 删除表
来源：http://aep.yonumen.top

DROP TABLE IF EXISTS orders;
来源：http://xve.chenlongwang.top

[Q08] 创建普通索引
来源：http://tmx.pengpengdd.cyou

CREATE INDEX idx_users_email ON users(email);
来源：http://byc.sxryk.cn

[Q09] 创建唯一索引
来源：http://met.hcnkem.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://utn.nwbrower.top

[Q10] 插入单行
来源：http://nzv.shanyushiyangtech.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zgj.jinyuanbaomall.cn

[Q11] 一次插入多行
来源：http://wft.shangyingyoupin.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ipt.yj20258888.top

[Q12] 插入后取自增 ID
来源：http://xtl.sxryk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://jpn.snrcjt.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xde.hammf.cn

[Q13] 忽略重复插入
来源：http://ohu.0kj1m.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uro.andypj.xyz

[Q14] 存在则更新（upsert）
来源：http://iag.sufxvd.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wzn.zhoulong.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rth.shuidangran.top

[Q15] 查询全部
来源：http://hng.316326.xyz

SELECT * FROM users;
来源：http://qjq.tanke756.top

[Q16] 查询指定列
来源：http://abz.guowangkeji.top

SELECT id, name FROM users;
来源：http://dhn.jiagoushi.top

[Q17] 条件查询
来源：http://ogg.xuanzx.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jap.gogol.net.cn

[Q18] 模糊匹配
来源：http://rex.haohaochexian.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zre.cucudq.cn

[Q19] 范围查询
来源：http://xdi.chenzaomai.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://paq.feifeiyinyue.top

[Q20] IN 列表
来源：http://jnf.sweek.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ucd.yuxming.cn

[Q21] 空值判断
来源：http://ewa.dashuyun.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://crv.yuanzhike.top

[Q22] 排序
来源：http://dhi.haohaochexian.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gdc.ywan-chungtsiang.top

[Q23] 分页
来源：http://cva.xingfuxueyuan.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://myw.chenjidiqi.icu

[Q24] 去重
来源：http://uwo.yuanzhike.top

SELECT DISTINCT city FROM users;
来源：http://xmf.tarul.cn

[Q25] 只取前 N 条
来源：http://eqm.fktsv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://elf.ppjwa.cn

[Q26] 计数
来源：http://nyg.yj20258.top

SELECT COUNT(*) FROM users;
来源：http://kwm.hesvh.cn

[Q27] 条件计数
来源：http://jkb.hfpthk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bdp.ppjwa.cn

[Q28] 求和与平均
来源：http://opt.9152youxi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://huy.shanyushiyangtech.top

[Q29] 最大最小值
来源：http://yqr.yfazqb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://pww.daxiang520.top

[Q30] 分组统计
来源：http://uqt.aibaodan.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cae.snrcjt.cn

[Q31] 分组后过滤
来源：http://upe.hongshengwenyu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://eaf.birdmap.top

[Q32] 分组拼接字符串
来源：http://wem.xuanzx.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uup.zdqjudy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mne.uphjek.com

[Q33] 多列分组
来源：http://zxn.ybcxt.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ghe.hywenlv.cn

[Q34] 每组取第一条
来源：http://esf.fzhhl.top

SELECT * FROM (
来源：http://vwz.daxiang520.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fzm.feifeiyinyue.top

) t WHERE rn = 1;
来源：http://vhc.yfazqb.com

[Q35] 内连接
来源：http://qki.mhx1999.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zya.cucudq.cn

[Q36] 左连接
来源：http://mha.chenjidiqi.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vhl.dashuyun.cn

[Q37] 右连接
来源：http://yvy.snrcjt.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wda.zhiwuduotai.top

[Q38] 全外连接（PostgreSQL）
来源：http://tgz.ivvv.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://aat.yueranfly.top

[Q39] 自连接（查上下级）
来源：http://vbo.bbcook.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://jvm.smart0.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gaa.ppjwa.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://uft.yj20258.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://upu.cqqwz.cn

[Q41] 多表连接
来源：http://rgd.cdnleiting.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://vgp.bjfxy.top

JOIN users u ON u.id = o.user_id
来源：http://nty.nanxinkj.top

JOIN products p ON p.id = o.product_id;
来源：http://jfg.vqdsnc.cn

[Q42] 连接条件附加过滤
来源：http://jnk.zycfv.cn

SELECT u.name, o.amount FROM users u
来源：http://fsk.vqdsnc.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://oij.andypj.xyz

[Q43] 标量子查询
来源：http://koo.dianchejie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vlw.bjfxy.top

[Q44] IN 子查询
来源：http://izk.jiagoushi.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://efg.ydjk.org.cn

[Q45] EXISTS 判断存在
来源：http://wsq.yj202588.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://luw.jianghu66.top

[Q46] NOT EXISTS 判断不存在
来源：http://xwz.haohaochexian.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rqu.yangfankeji.com

[Q47] 与平均值比较
来源：http://rjb.hysaishi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://niz.chenlongwang.top

[Q48] CTE 公用表表达式
来源：http://lxj.hywenlv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://aif.jinqigfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://zoq.shzxlz.cn

[Q49] 更新单行
来源：http://zyx.nanxuanxn.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pll.epnwcf.com

[Q50] 批量更新
来源：http://tjl.sufxvd.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xfh.gogol.net.cn

[Q51] 用子查询更新
来源：http://zki.bbcook.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fef.jqgfzy.top

[Q52] 删除指定行
来源：http://hly.hywenlv.cn

DELETE FROM users WHERE id = 10;
来源：http://yyl.pycfn.com

[Q53] 按条件删除
来源：http://uuv.zhengqikj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hch.yvedp.cn

[Q54] 清空表
来源：http://wgv.c1oappe.top

TRUNCATE TABLE logs;
来源：http://bum.redwolf501.top

[Q55] 排名（并列占位）
来源：http://ung.jinqigufen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ftu.jinghuilouyu.cn

[Q56] 密集排名（并列不占位）
来源：http://xtf.fehbvm.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xee.hesvh.cn

[Q57] 行号
来源：http://pek.hfpthk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gep.tarul.cn

[Q58] 累计求和
来源：http://acc.guowangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sac.hcnkem.com

[Q59] 分组内累计
来源：http://bvx.zhoulong.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://etw.hnxiangtu.top

[Q60] 取上一行 / 下一行
来源：http://mqn.zhaomingkeji.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ibk.yfazqb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ciz.ydzc1.top

[Q61] 移动平均
来源：http://gaf.yueranfly.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rws.yueranfly.top

[Q62] 分组占比
来源：http://gin.0kj1m.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rqw.yongpay.top


<!-- 参考信息 -->