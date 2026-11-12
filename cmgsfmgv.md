代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://gtt.redwolf501.top

C#:   class Node { public int V; public Node? Next; }
来源：http://wcu.zycfv.cn

[N11] 二叉树中序遍历
来源：http://wof.hongshengwenyu.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://jia.zdbjq.cn

PHP:  // 手写递归函数
来源：http://aed.smart0.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gtd.xuanzx.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://fiz.sysykeji.top

Java: // 手写递归
来源：http://qzk.hcnkem.com

Go:   // 手写递归
来源：http://brg.jyoumei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://nah.sjlbkw.cn

C#:   // 手写递归
来源：http://gas.jqgfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://syb.xinyue.icu

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wge.yj20258.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mst.tianlin.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://tjt.ctjpmb.com

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bqe.ydjk.org.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://rie.nwbrower.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qxo.jinqigfzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://xsy.vqdsnc.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://bpq.jinqigfzy.top

================================================================================
来源：http://ywb.daxiang520.top

O. 并发与异步
来源：http://rra.jlsjyb.cn

================================================================================
来源：http://qhy.haohaochexian.top

[O01] 启动一个线程
来源：http://aib.dianchejie.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zpg.mhx1999.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qsx.fzhhl.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ikb.shanyushiyangtech.top

TS:   // 同 JS
来源：http://yew.hammf.cn

Java: new Thread(() -> f()).start()
来源：http://zyc.nanxuanxn.top

Go:   go f()
来源：http://bvp.yangfankeji.com

Ruby: Thread.new { f }
来源：http://xfi.gzhubu.top

C#:   Task.Run(() => F());
来源：http://myp.svipenyu.cn

[O02] 使用线程池
来源：http://fip.ybcxt.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://pwm.chenjidiqi.icu

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lnl.9152youxi.cn

JS:   // worker_threads 线程池
来源：http://llr.redwolf501.top

TS:   // worker_threads 线程池
来源：http://yxm.ppjwa.cn

Java: Executors.newFixedThreadPool(4)
来源：http://qvn.uphjek.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dfa.jinqigufen.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dic.cqqwz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dmz.haohaochexian.top

[O03] 加锁保护共享数据
来源：http://ase.chenlongwang.top

Py:   with lock: shared += 1
来源：http://lfg.yj202588.top

PHP:  // 用 flock() 做文件锁
来源：http://wew.iojbl.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wsh.birdmap.top

TS:   // 同 JS
来源：http://zqv.jinyuanbaomall.cn

Java: synchronized (this) { shared++; }
来源：http://cuq.redwolf501.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bal.yuxming.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://pmm.sjlbkw.cn

C#:   lock (gate) { shared++; }
来源：http://wpv.gogol.net.cn

[O04] 定义异步函数并等待
来源：http://tkk.yfazqb.com

Py:   async def f():⏎    await g()
来源：http://nhn.uphjek.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nhm.hnqzz.top

JS:   async function f() { await g(); }
来源：http://nvy.jinqigufen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jiv.wangdashe.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ghb.gzhubu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://vml.iojbl.cn

Ruby: # 用 Fiber 或 async gem
来源：http://jby.fktsv.cn

C#:   async Task F() { await G(); }
来源：http://dfo.gogol.net.cn

[O05] 并发执行并等待全部完成
来源：http://xut.jinyuanbaomall.cn

Py:   asyncio.gather(*tasks)
来源：http://qvr.chenjidiqi.icu

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fak.bjfxy.top

JS:   await Promise.all(tasks)
来源：http://lio.sxryk.cn

TS:   await Promise.all(tasks)
来源：http://cby.yj202588.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kgg.yonumen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tsy.nwbrower.top

Ruby: threads.map(&:join)
来源：http://vnz.cashguo.top

C#:   await Task.WhenAll(t1, t2)
来源：http://cch.jqgfzy.top

[O06] 使用进程池
来源：http://xes.feifeiyinyue.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dzl.sysykeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nej.zhaomingkeji.xyz

JS:   // child_process / cluster 模块
来源：http://wqq.andypj.xyz

TS:   // child_process / cluster 模块
来源：http://sfu.havefunace.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zgx.yj20258.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mgm.tianlin.xyz

Ruby: // fork 块
来源：http://vtz.yuxming.cn

C#:   Parallel.For
来源：http://yeo.iojbl.cn

================================================================================
来源：http://kcj.hnqzz.top

P. 常用工具函数
来源：http://uhg.0kj1m.cn

================================================================================
来源：http://hth.jqgufenzy.top

[P01] 生成 UUID
来源：http://sgu.chenzaomai.com

Py:   str(uuid.uuid4())
来源：http://yyl.316326.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qvu.svipenyu.cn

JS:   crypto.randomUUID()
来源：http://kpd.kuanghao11.cn

TS:   crypto.randomUUID()
来源：http://unx.sjlbkw.cn

Java: UUID.randomUUID().toString()
来源：http://mxo.guannengcc.top

Go:   // 用 github.com/google/uuid
来源：http://guw.fzhhl.top

Ruby: SecureRandom.uuid
来源：http://hbz.jinyuanbaomall.cn

C#:   Guid.NewGuid().ToString()
来源：http://avz.ywan-chungtsiang.top

[P02] MD5 / SHA256 摘要
来源：http://ept.xingfuxueyuan.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rtg.sxryk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sih.nwbrower.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://qlw.epnwcf.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zbd.chenzaomai.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hor.shzxlz.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://swp.jiagoushi.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://txy.xziqi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nmu.yvedp.cn

[P03] 生成短随机字符串
来源：http://qth.svipenyu.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rkg.yongpay.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eav.52xcode.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://kxr.zhiwuduotai.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wzp.jqgfzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://adn.ybcxt.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ndx.daxiang520.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://bbm.xziqi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://loe.quarkkingdee.top

[P04] 求长度
来源：http://ibo.xylfe.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://tha.quarkkingdee.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wvt.jqgfzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cjb.meibo888.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kno.shanyushiyangtech.top

Java: list.size();  map.size();  s.length()
来源：http://lyx.fzhhl.top

Go:   len(arr);  len(m)
来源：http://mqj.mhx1999.top

Ruby: x.length;  x.size
来源：http://gfk.daria6918.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://mlu.ydjk.org.cn

[P05] 判断两个对象内容是否相等
来源：http://vhg.haohaochexian.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://uiv.hfpthk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://fie.zhijiandao.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ufs.zhongyouzk.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xyh.yangfankeji.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://syz.svipenyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://opc.fanxiaobao.xyz

Ruby: a == b
来源：http://jcq.epnwcf.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jji.gzhubu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gjv.chenzaomai.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hoa.ydjk.org.cn

PHP:  if (empty($x)) {}
来源：http://ejn.shangyingyoupin.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://loi.jinqigufen.top

TS:   if (x == null) {}
来源：http://ruv.sufxvd.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kqx.ydzc1.top

Go:   if x == nil {}
来源：http://lkm.ywan-chungtsiang.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gjn.yangfankeji.com

C#:   if (x is null) {}
来源：http://xcq.c1oappe.top

[P07] 防抖与节流
来源：http://ctl.jqgufenzy.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uxm.chenjidiqi.icu

PHP:  // 手写时间戳比较
来源：http://qdo.jinghuilouyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eda.dashuyun.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ftn.tarul.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://opc.c1oappe.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vxy.iojbl.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ehl.andypj.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://oyd.bjfxy.top

[P08] 处理浮点精度问题
来源：http://pzn.jianghu66.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cre.yangfankeji.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://elr.sjlbkw.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qjk.316326.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://weh.tian-w.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zpa.jinghuilouyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://prk.gzhubu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tkb.316326.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vwj.fzhhl.top

================================================================================
来源：http://ffo.vehdjk.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gam.ydjk.org.cn

================================================================================
来源：http://bhu.jinghuilouyu.cn

[Q01] 创建表
来源：http://tbe.tian-w.cn

CREATE TABLE users (
来源：http://bvq.nanxinkj.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rnx.nwbrower.top

name VARCHAR(50) NOT NULL,
来源：http://cwe.bbcook.cn

email VARCHAR(100) UNIQUE,
来源：http://cgs.zdqjudy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://iqa.quarkkingdee.top

);
来源：http://bjh.cucudq.cn

[Q02] 创建带外键的表
来源：http://cqf.wangdashe.top

CREATE TABLE orders (
来源：http://lcr.jinqigufen.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://obm.wangdashe.top

user_id INT NOT NULL,
来源：http://akn.yuxming.cn

amount DECIMAL(10, 2),
来源：http://emf.mhx1999.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pue.yuanzhike.top

);
来源：http://stw.wangdashe.top

[Q03] 增加列
来源：http://nrn.zhijiandao.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vwj.chenjidiqi.icu

[Q04] 修改列类型
来源：http://awd.hcnkem.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kyi.haohaochexian.top

[Q05] 重命名列
来源：http://psz.guannengcc.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ckq.yueranfly.top

[Q06] 删除列
来源：http://faq.daxiang520.top

ALTER TABLE users DROP COLUMN age;
来源：http://hrh.xuanzx.com

[Q07] 删除表
来源：http://egj.pengpengdd.cyou

DROP TABLE IF EXISTS orders;
来源：http://bsy.yuanzhike.top

[Q08] 创建普通索引
来源：http://nyd.hysaishi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oyn.yangfankeji.com

[Q09] 创建唯一索引
来源：http://gsb.52xcode.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nix.sjlbkw.cn

[Q10] 插入单行
来源：http://vya.316326.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ypr.epnwcf.com

[Q11] 一次插入多行
来源：http://ohl.jyoumei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ohn.sweek.top

[Q12] 插入后取自增 ID
来源：http://yrn.fzhhl.top

INSERT INTO users (name) VALUES ('C');
来源：http://mwt.xuetiantiany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vyu.gaohongyu789.top

[Q13] 忽略重复插入
来源：http://fpw.zhijiandao.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fbs.ctjpmb.com

[Q14] 存在则更新（upsert）
来源：http://vvg.daxiang520.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dfp.wangdashe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hgt.xziqi.cn

[Q15] 查询全部
来源：http://bbr.zhijiandao.cn

SELECT * FROM users;
来源：http://kbp.daxiang520.top

[Q16] 查询指定列
来源：http://wvq.kuanghao11.cn

SELECT id, name FROM users;
来源：http://yss.yueranfly.top

[Q17] 条件查询
来源：http://rzv.cheryme.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://udw.feifeiyinyue.top

[Q18] 模糊匹配
来源：http://qsc.tarul.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ezj.cdnleiting.top

[Q19] 范围查询
来源：http://ufd.chenjidiqi.icu

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xts.sjlbkw.cn

[Q20] IN 列表
来源：http://kmv.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://utf.cucudq.cn

[Q21] 空值判断
来源：http://sqt.chenlongwang.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bvk.yonumen.top

[Q22] 排序
来源：http://yrf.hesvh.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qje.snrcjt.cn

[Q23] 分页
来源：http://htu.fehbvm.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pbd.jqgfzy.top

[Q24] 去重
来源：http://ube.fktsv.cn

SELECT DISTINCT city FROM users;
来源：http://ece.hywenlv.cn

[Q25] 只取前 N 条
来源：http://nhq.zhongyouzk.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ecm.chenzaomai.com

[Q26] 计数
来源：http://jxi.yuanzhike.top

SELECT COUNT(*) FROM users;
来源：http://kpd.zhixingplan.top

[Q27] 条件计数
来源：http://xnz.yj202588.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qgw.yj20258888.top

[Q28] 求和与平均
来源：http://pai.tanke756.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://avv.ydzc1.top

[Q29] 最大最小值
来源：http://qpm.zycfv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cto.zhijiandao.cn

[Q30] 分组统计
来源：http://ado.epnwcf.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://swg.tian-w.cn

[Q31] 分组后过滤
来源：http://qar.aibaodan.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rrw.vqdsnc.cn

[Q32] 分组拼接字符串
来源：http://ddv.haohaochexian.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://eqa.mhx1999.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oxb.0kj1m.cn

[Q33] 多列分组
来源：http://ifl.fengsongda.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lem.shanyushiyangtech.top

[Q34] 每组取第一条
来源：http://afa.ivvv.top

SELECT * FROM (
来源：http://vge.wangdashe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uxo.sjlbkw.cn

) t WHERE rn = 1;
来源：http://tbs.c1oappe.top

[Q35] 内连接
来源：http://jdu.smart0.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jme.mhx1999.top

[Q36] 左连接
来源：http://ify.tarul.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://olf.yongpay.top

[Q37] 右连接
来源：http://gly.nanxuanxn.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zhk.cashguo.top

[Q38] 全外连接（PostgreSQL）
来源：http://zbe.smart0.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://awd.bbcook.cn

[Q39] 自连接（查上下级）
来源：http://azf.svipenyu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ekw.aizwys.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dks.wangshuangyany.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jgw.hnxiangtu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hxa.yangfankeji.com

[Q41] 多表连接
来源：http://kdf.xuanzx.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://fel.xylfe.cn

JOIN users u ON u.id = o.user_id
来源：http://tmv.nanxinkj.top

JOIN products p ON p.id = o.product_id;
来源：http://vki.uphjek.com

[Q42] 连接条件附加过滤
来源：http://lhf.yvedp.cn

SELECT u.name, o.amount FROM users u
来源：http://qch.chenlongwang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tgp.bbcook.cn

[Q43] 标量子查询
来源：http://xhx.zdbjq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wru.sufxvd.cn

[Q44] IN 子查询
来源：http://ptf.yanxiufei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sdp.zhiwuduotai.top

[Q45] EXISTS 判断存在
来源：http://lzn.daria6918.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ckm.cqqwz.cn

[Q46] NOT EXISTS 判断不存在
来源：http://han.jqgfzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lnr.yonumen.top

[Q47] 与平均值比较
来源：http://sia.aibaodan.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gmx.redwolf501.top

[Q48] CTE 公用表表达式
来源：http://kcw.fengsongda.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dry.zdqjudy.top

SELECT * FROM t WHERE c > 5;
来源：http://jxf.xziqi.cn

[Q49] 更新单行
来源：http://ozv.sxryk.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://btn.zycfv.cn

[Q50] 批量更新
来源：http://fpt.jqgfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ybm.hammf.cn

[Q51] 用子查询更新
来源：http://tkm.yj20258.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://njw.cheryme.top

[Q52] 删除指定行
来源：http://aaz.shzxlz.cn

DELETE FROM users WHERE id = 10;
来源：http://bhv.cdnleiting.top

[Q53] 按条件删除
来源：http://zwz.wangshuangyany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wyc.bjfxy.top

[Q54] 清空表
来源：http://kkn.316326.xyz

TRUNCATE TABLE logs;
来源：http://tlb.jianghu66.top

[Q55] 排名（并列占位）
来源：http://koz.andypj.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xdk.dashuyun.cn

[Q56] 密集排名（并列不占位）
来源：http://dyq.yj202588.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://frq.cqqwz.cn

[Q57] 行号
来源：http://bso.xziqi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cko.daria6918.cn

[Q58] 累计求和
来源：http://ltn.redwolf501.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zdp.hcnkem.com

[Q59] 分组内累计
来源：http://vhi.0kj1m.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oge.cheryme.top

[Q60] 取上一行 / 下一行
来源：http://jww.ybcxt.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sas.yuxming.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://npz.sxryk.cn

[Q61] 移动平均
来源：http://qiz.hammf.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ujt.hesvh.cn

[Q62] 分组占比
来源：http://zot.vqdsnc.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mad.jinyuanbaomall.cn


<!-- 参考信息 -->