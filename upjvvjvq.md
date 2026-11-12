代发 wailian999

PHP:  // 手写递归函数
来源：http://tyq.hywenlv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yqx.c1oappe.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://itt.ivvv.top

Java: // 手写递归
来源：http://lhd.havefunace.top

Go:   // 手写递归
来源：http://jqd.zhixingplan.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wfo.316326.xyz

C#:   // 手写递归
来源：http://uyb.yuanzhike.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bfi.jlsjyb.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://auq.shangyingyoupin.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hho.jyoumei.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mwc.hammf.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mtd.gotoacloud.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mql.jqgfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://auf.tian-w.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://krl.guannengcc.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://xsz.guowangkeji.top

================================================================================
来源：http://eqf.hongshengwenyu.top

O. 并发与异步
来源：http://hvy.havefunace.top

================================================================================
来源：http://ikj.epnwcf.com

[O01] 启动一个线程
来源：http://ksf.yueranfly.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://opc.zhaomingkeji.xyz

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://jhd.hesvh.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://dsg.yuxming.cn

TS:   // 同 JS
来源：http://beu.jqgufenzy.top

Java: new Thread(() -> f()).start()
来源：http://eaw.daxiang520.top

Go:   go f()
来源：http://yfr.hammf.cn

Ruby: Thread.new { f }
来源：http://dlq.xylfe.cn

C#:   Task.Run(() => F());
来源：http://qdn.snrcjt.cn

[O02] 使用线程池
来源：http://udb.bbcook.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://gxw.zhongyouzk.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kwu.hongshengwenyu.top

JS:   // worker_threads 线程池
来源：http://sgr.shuidangran.top

TS:   // worker_threads 线程池
来源：http://kdp.jinghuilouyu.cn

Java: Executors.newFixedThreadPool(4)
来源：http://mxa.pycfn.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hyi.jinqigfzy.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://nra.ybcxt.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blz.yonumen.top

[O03] 加锁保护共享数据
来源：http://dld.nanxuanxn.top

Py:   with lock: shared += 1
来源：http://org.cdnleiting.top

PHP:  // 用 flock() 做文件锁
来源：http://kwh.tian-w.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pii.zycfv.cn

TS:   // 同 JS
来源：http://pie.jinqigufen.top

Java: synchronized (this) { shared++; }
来源：http://jwp.redwolf501.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://afx.chenlongwang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://eyb.hcnkem.com

C#:   lock (gate) { shared++; }
来源：http://aku.ehwqpu.com

[O04] 定义异步函数并等待
来源：http://edb.9152youxi.cn

Py:   async def f():⏎    await g()
来源：http://zyr.jinyuanbaomall.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://huj.zhoulong.xyz

JS:   async function f() { await g(); }
来源：http://msi.xingfuxueyuan.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://mgu.bbcook.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ebb.sxryk.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hed.hnqzz.top

Ruby: # 用 Fiber 或 async gem
来源：http://gxv.wangdashe.top

C#:   async Task F() { await G(); }
来源：http://hce.yj202588.top

[O05] 并发执行并等待全部完成
来源：http://dga.sweek.top

Py:   asyncio.gather(*tasks)
来源：http://iza.jianghu66.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://otz.iojbl.cn

JS:   await Promise.all(tasks)
来源：http://upd.cdnleiting.top

TS:   await Promise.all(tasks)
来源：http://suh.dashuyun.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jlv.nanxinkj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zjq.jlsjyb.cn

Ruby: threads.map(&:join)
来源：http://xoe.bjfxy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mys.jiagoushi.top

[O06] 使用进程池
来源：http://pbr.vqdsnc.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lfl.hongshengwenyu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ugi.cheryme.top

JS:   // child_process / cluster 模块
来源：http://eny.gotoacloud.top

TS:   // child_process / cluster 模块
来源：http://rte.ybcxt.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://irn.xuetiantiany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ixj.hesvh.cn

Ruby: // fork 块
来源：http://zwl.yj20258.top

C#:   Parallel.For
来源：http://cme.jyoumei.cn

================================================================================
来源：http://lew.shanyushiyangtech.top

P. 常用工具函数
来源：http://nvt.shuidangran.top

================================================================================
来源：http://hhg.snrcjt.cn

[P01] 生成 UUID
来源：http://uns.fanxiaobao.xyz

Py:   str(uuid.uuid4())
来源：http://uen.gzhubu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ucr.cdnleiting.top

JS:   crypto.randomUUID()
来源：http://xwt.guowangkeji.top

TS:   crypto.randomUUID()
来源：http://vju.haohaochexian.top

Java: UUID.randomUUID().toString()
来源：http://lze.hywenlv.cn

Go:   // 用 github.com/google/uuid
来源：http://axr.jianghu66.top

Ruby: SecureRandom.uuid
来源：http://see.jinqigfzy.top

C#:   Guid.NewGuid().ToString()
来源：http://izx.aibaodan.cn

[P02] MD5 / SHA256 摘要
来源：http://jqs.jlsjyb.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qai.andypj.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://wvn.shangyingyoupin.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jkp.9152youxi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ehu.feifeiyinyue.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lim.haohaochexian.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vzt.tian-w.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://uip.hywenlv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://qxk.c1oappe.top

[P03] 生成短随机字符串
来源：http://lvj.iojbl.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lah.redwolf501.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qqy.ydzc1.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wsp.vehdjk.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ekz.zhoulong.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jps.zhoulong.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bir.tianlin.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://glx.yueranfly.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rwx.epnwcf.com

[P04] 求长度
来源：http://kny.ehwqpu.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zhn.feifeiyinyue.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ewp.tarul.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nzc.xylfe.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://inh.nwbrower.top

Java: list.size();  map.size();  s.length()
来源：http://uch.smart0.xyz

Go:   len(arr);  len(m)
来源：http://oqw.9152youxi.cn

Ruby: x.length;  x.size
来源：http://xoj.hfpthk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ubc.aizwys.cn

[P05] 判断两个对象内容是否相等
来源：http://klb.hysaishi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xqp.zdbjq.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dpv.cucudq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://lcb.gotoacloud.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://boi.0kj1m.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pbb.guannengcc.top

Go:   reflect.DeepEqual(a, b)
来源：http://iqp.52xcode.cn

Ruby: a == b
来源：http://iwt.fanxiaobao.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uzx.zhoulong.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jei.fktsv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tdn.zhaomingkeji.xyz

PHP:  if (empty($x)) {}
来源：http://xgv.jyoumei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://azu.dashuyun.cn

TS:   if (x == null) {}
来源：http://jvh.hnxiangtu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fgu.jinqigufen.top

Go:   if x == nil {}
来源：http://ock.daxiang520.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pbu.pycfn.com

C#:   if (x is null) {}
来源：http://bwr.haohaochexian.top

[P07] 防抖与节流
来源：http://lec.shanyushiyangtech.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wcl.yj20258.top

PHP:  // 手写时间戳比较
来源：http://mtz.tian-w.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://air.yangfankeji.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qxg.ppjwa.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mto.shanyushiyangkeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tsm.jinghuilouyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://tnj.hcnkem.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ewo.pengpengdd.cyou

[P08] 处理浮点精度问题
来源：http://qpd.jyoumei.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://eff.yonumen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ukh.zhoulong.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jzl.jiagoushi.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kjh.zycfv.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lbr.shzxlz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://tbe.shanyushiyangkeji.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bxz.gogol.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xpn.tianlin.xyz

================================================================================
来源：http://sap.fengsongda.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cuy.cashguo.top

================================================================================
来源：http://mpd.jqgfzy.top

[Q01] 创建表
来源：http://vfu.fanxiaobao.xyz

CREATE TABLE users (
来源：http://cjq.iojbl.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zyn.ydzc1.top

name VARCHAR(50) NOT NULL,
来源：http://orj.jyoumei.cn

email VARCHAR(100) UNIQUE,
来源：http://wvv.ehwqpu.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xkf.wangshuangyany.cn

);
来源：http://gsa.dashuyun.cn

[Q02] 创建带外键的表
来源：http://mss.ywan-chungtsiang.top

CREATE TABLE orders (
来源：http://lcu.gogol.net.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fmk.jiagoushi.top

user_id INT NOT NULL,
来源：http://gfx.zhijiandao.cn

amount DECIMAL(10, 2),
来源：http://msg.svipenyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wyz.yvedp.cn

);
来源：http://xmx.sufxvd.cn

[Q03] 增加列
来源：http://hwo.quarkkingdee.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fth.pengpengdd.cyou

[Q04] 修改列类型
来源：http://gnl.ybcxt.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://oof.jianghu66.top

[Q05] 重命名列
来源：http://gkh.yvedp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rda.cucudq.cn

[Q06] 删除列
来源：http://kqp.cucudq.cn

ALTER TABLE users DROP COLUMN age;
来源：http://wjx.hcnkem.com

[Q07] 删除表
来源：http://cjd.sysykeji.top

DROP TABLE IF EXISTS orders;
来源：http://idr.nanxuanxn.top

[Q08] 创建普通索引
来源：http://rec.hywenlv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lxo.nanxuanxn.top

[Q09] 创建唯一索引
来源：http://oxi.zhaomingkeji.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xjj.fktsv.cn

[Q10] 插入单行
来源：http://pma.ydzc1.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jjk.svipenyu.cn

[Q11] 一次插入多行
来源：http://nef.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sgm.pycfn.com

[Q12] 插入后取自增 ID
来源：http://ygm.kuanghao11.cn

INSERT INTO users (name) VALUES ('C');
来源：http://srx.daxiang520.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hfa.jqgufenzy.top

[Q13] 忽略重复插入
来源：http://rdt.ywan-chungtsiang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dci.yj20258888.top

[Q14] 存在则更新（upsert）
来源：http://mzr.hnxiangtu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://gwx.xinyue.icu

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sml.vqdsnc.cn

[Q15] 查询全部
来源：http://qpo.guowangkeji.top

SELECT * FROM users;
来源：http://xoj.guannengcc.top

[Q16] 查询指定列
来源：http://mjp.sufxvd.cn

SELECT id, name FROM users;
来源：http://jaz.pengpengdd.cyou

[Q17] 条件查询
来源：http://aou.316326.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xzg.daxiang520.top

[Q18] 模糊匹配
来源：http://vop.andypj.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yiu.vehdjk.com

[Q19] 范围查询
来源：http://xwr.chenzaomai.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hsb.yangfankeji.com

[Q20] IN 列表
来源：http://gbp.hysaishi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mbu.ivvv.top

[Q21] 空值判断
来源：http://vaz.aizwys.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://mkf.chenjidiqi.icu

[Q22] 排序
来源：http://zoo.tanke756.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://pzv.zhijiandao.cn

[Q23] 分页
来源：http://dos.ctjpmb.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yos.mhx1999.top

[Q24] 去重
来源：http://vyu.gzhubu.top

SELECT DISTINCT city FROM users;
来源：http://zoj.zhijiandao.cn

[Q25] 只取前 N 条
来源：http://joz.jiagoushi.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vuh.fktsv.cn

[Q26] 计数
来源：http://jus.jinghuilouyu.cn

SELECT COUNT(*) FROM users;
来源：http://xvq.shanyushiyangtech.top

[Q27] 条件计数
来源：http://uuk.yj20258.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nni.tian-w.cn

[Q28] 求和与平均
来源：http://xct.xingfuxueyuan.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uif.yanxiufei.cn

[Q29] 最大最小值
来源：http://fpl.316326.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://zgw.hnxiangtu.top

[Q30] 分组统计
来源：http://ldr.svipenyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bef.meibo888.top

[Q31] 分组后过滤
来源：http://vjz.aibaodan.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://esy.cheryme.top

[Q32] 分组拼接字符串
来源：http://nqr.cdnleiting.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jef.gzhubu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vkh.yuanzhike.top

[Q33] 多列分组
来源：http://ool.sxryk.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pqx.pengpengdd.cyou

[Q34] 每组取第一条
来源：http://ezo.yfazqb.com

SELECT * FROM (
来源：http://rhn.jqgufenzy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lwo.epnwcf.com

) t WHERE rn = 1;
来源：http://tdu.fanxiaobao.xyz

[Q35] 内连接
来源：http://tkl.52xcode.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vqf.9152youxi.cn

[Q36] 左连接
来源：http://uvt.xinyue.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ypl.tarul.cn

[Q37] 右连接
来源：http://ygd.hywenlv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fje.ybcxt.top

[Q38] 全外连接（PostgreSQL）
来源：http://gul.jqgufenzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dqk.svipenyu.cn

[Q39] 自连接（查上下级）
来源：http://nip.yueranfly.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mzj.zdqjudy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kwp.nanxinkj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://utk.yuanzhike.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ufz.nanxinkj.top

[Q41] 多表连接
来源：http://zst.yueranfly.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://iuo.jiagoushi.top

JOIN users u ON u.id = o.user_id
来源：http://bnf.mhx1999.top

JOIN products p ON p.id = o.product_id;
来源：http://xoj.hcnkem.com

[Q42] 连接条件附加过滤
来源：http://gij.tianlin.xyz

SELECT u.name, o.amount FROM users u
来源：http://gej.jqgfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://npb.fktsv.cn

[Q43] 标量子查询
来源：http://dlx.aibaodan.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zhx.gaohongyu789.top

[Q44] IN 子查询
来源：http://opb.zdbjq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://snl.jqgufenzy.top

[Q45] EXISTS 判断存在
来源：http://wih.ctjpmb.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://daw.dashuyun.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ass.jlsjyb.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hhm.52xcode.cn

[Q47] 与平均值比较
来源：http://flk.zhixingplan.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bna.havefunace.top

[Q48] CTE 公用表表达式
来源：http://buh.smart0.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mqo.xingfuxueyuan.xyz

SELECT * FROM t WHERE c > 5;
来源：http://wbz.jinyuanbaomall.cn

[Q49] 更新单行
来源：http://vod.redwolf501.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tyg.ctjpmb.com

[Q50] 批量更新
来源：http://vnp.dianchejie.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mwx.cqqwz.cn

[Q51] 用子查询更新
来源：http://kag.ctjpmb.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://woe.meibo888.top

[Q52] 删除指定行
来源：http://guz.jqgfzy.top

DELETE FROM users WHERE id = 10;
来源：http://tht.sxryk.cn

[Q53] 按条件删除
来源：http://bdo.hcnkem.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cpr.fzhhl.top

[Q54] 清空表
来源：http://qab.bjfxy.top

TRUNCATE TABLE logs;
来源：http://bdt.jqgufenzy.top

[Q55] 排名（并列占位）
来源：http://gdq.yonumen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ibd.vehdjk.com

[Q56] 密集排名（并列不占位）
来源：http://pkl.dianchejie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qov.andypj.xyz

[Q57] 行号
来源：http://nqr.yanxiufei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lnf.xinyue.icu

[Q58] 累计求和
来源：http://nhj.xinyue.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qku.cheryme.top

[Q59] 分组内累计
来源：http://wwa.xylfe.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://siy.xylfe.cn

[Q60] 取上一行 / 下一行
来源：http://wpx.aizwys.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hhl.hnqzz.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://klf.pengpengdd.cyou

[Q61] 移动平均
来源：http://enq.bjfxy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://utl.quarkkingdee.top

[Q62] 分组占比
来源：http://ujk.hesvh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://aiz.xingfuxueyuan.xyz

[Q63] 开启事务
来源：http://ydr.pycfn.com

START TRANSACTION;                -- 或 BEGIN
来源：http://pih.tian-w.cn

[Q64] 提交事务
来源：http://joo.wangdashe.top

COMMIT;
来源：http://sjq.zhaomingkeji.xyz


<!-- 参考信息 -->