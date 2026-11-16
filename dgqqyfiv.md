代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://ydi.zdbjq.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://srq.xingfuxueyuan.xyz

[N11] 二叉树中序遍历
来源：http://nym.xinyue.icu

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ytk.vqdsnc.cn

PHP:  // 手写递归函数
来源：http://piu.wangdashe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nwi.gaohongyu789.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://irk.cqqwz.cn

Java: // 手写递归
来源：http://jmc.kuanghao11.cn

Go:   // 手写递归
来源：http://dre.zhijiandao.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://dyn.jyoumei.cn

C#:   // 手写递归
来源：http://lcg.jqgufenzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://fke.xziqi.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vjr.gogol.net.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://sjj.hnxiangtu.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zbk.jianghu66.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uyn.tarul.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://cly.316326.xyz

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kfs.iojbl.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wbo.haohaochexian.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qeg.hnqzz.top

================================================================================
来源：http://dnq.tian-w.cn

O. 并发与异步
来源：http://geb.epnwcf.com

================================================================================
来源：http://yjx.yj20258888.top

[O01] 启动一个线程
来源：http://ceq.daria6918.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://soa.yj20258888.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ujr.tianlin.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://vwn.shangyingyoupin.top

TS:   // 同 JS
来源：http://ook.gotoacloud.top

Java: new Thread(() -> f()).start()
来源：http://ief.mhx1999.top

Go:   go f()
来源：http://hzc.haohaochexian.top

Ruby: Thread.new { f }
来源：http://laa.gzhubu.top

C#:   Task.Run(() => F());
来源：http://cyb.zhongyouzk.top

[O02] 使用线程池
来源：http://yhx.jinqigfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://jdv.ctjpmb.com

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://xpf.xylfe.cn

JS:   // worker_threads 线程池
来源：http://olx.0kj1m.cn

TS:   // worker_threads 线程池
来源：http://hqa.hnqzz.top

Java: Executors.newFixedThreadPool(4)
来源：http://mar.aizwys.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://roc.quarkkingdee.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://sxp.bbcook.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mzb.sufxvd.cn

[O03] 加锁保护共享数据
来源：http://fdy.jlsjyb.cn

Py:   with lock: shared += 1
来源：http://dyx.sufxvd.cn

PHP:  // 用 flock() 做文件锁
来源：http://ruw.yonumen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://tzg.quarkkingdee.top

TS:   // 同 JS
来源：http://sdt.52xcode.cn

Java: synchronized (this) { shared++; }
来源：http://rkp.vehdjk.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rmj.cqqwz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://sgj.316326.xyz

C#:   lock (gate) { shared++; }
来源：http://lcz.sjlbkw.cn

[O04] 定义异步函数并等待
来源：http://twq.cucudq.cn

Py:   async def f():⏎    await g()
来源：http://gcw.gogol.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uxe.xuetiantiany.cn

JS:   async function f() { await g(); }
来源：http://xnl.xylfe.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://nmm.ybcxt.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pey.aibaodan.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jhx.birdmap.top

Ruby: # 用 Fiber 或 async gem
来源：http://gzz.cashguo.top

C#:   async Task F() { await G(); }
来源：http://cju.hongshengwenyu.top

[O05] 并发执行并等待全部完成
来源：http://bcv.zhixingplan.top

Py:   asyncio.gather(*tasks)
来源：http://hrr.fehbvm.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rvf.zhengqikj.top

JS:   await Promise.all(tasks)
来源：http://kkd.ywan-chungtsiang.top

TS:   await Promise.all(tasks)
来源：http://foa.0kj1m.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oix.nwbrower.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://atp.guannengcc.top

Ruby: threads.map(&:join)
来源：http://uiu.c1oappe.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xdx.guannengcc.top

[O06] 使用进程池
来源：http://hou.sufxvd.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wom.guannengcc.top

PHP:  // pcntl_fork 或多进程队列
来源：http://mbg.xingfuxueyuan.xyz

JS:   // child_process / cluster 模块
来源：http://mzp.dianchejie.cn

TS:   // child_process / cluster 模块
来源：http://okf.vehdjk.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rff.52xcode.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://erq.xuanzx.com

Ruby: // fork 块
来源：http://fel.shanyushiyangtech.top

C#:   Parallel.For
来源：http://cti.mhx1999.top

================================================================================
来源：http://lic.fktsv.cn

P. 常用工具函数
来源：http://hlh.quarkkingdee.top

================================================================================
来源：http://pkt.ydjk.org.cn

[P01] 生成 UUID
来源：http://xdx.yj20258888.top

Py:   str(uuid.uuid4())
来源：http://qhe.yvedp.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hby.yj20258888.top

JS:   crypto.randomUUID()
来源：http://yjb.pengpengdd.cyou

TS:   crypto.randomUUID()
来源：http://mxm.ydzc1.top

Java: UUID.randomUUID().toString()
来源：http://ipn.cashguo.top

Go:   // 用 github.com/google/uuid
来源：http://ahv.zhaomingkeji.xyz

Ruby: SecureRandom.uuid
来源：http://ayi.iojbl.cn

C#:   Guid.NewGuid().ToString()
来源：http://etp.cdnleiting.top

[P02] MD5 / SHA256 摘要
来源：http://btp.xuetiantiany.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kva.hesvh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hdd.zdbjq.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yvf.shuidangran.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nmx.sweek.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oef.shanyushiyangtech.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://vga.yj20258.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://osv.kuanghao11.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lzt.9152youxi.cn

[P03] 生成短随机字符串
来源：http://cir.xziqi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://jml.meibo888.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tac.aibaodan.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jtx.pycfn.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nux.tianlin.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://sxj.zdbjq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wrx.jqgfzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rqf.nanxuanxn.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hfd.aizwys.cn

[P04] 求长度
来源：http://mxe.svipenyu.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jem.haohaochexian.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://efl.daxiang520.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eoa.guannengcc.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://khs.jianghu66.top

Java: list.size();  map.size();  s.length()
来源：http://wfb.gaohongyu789.top

Go:   len(arr);  len(m)
来源：http://zyx.sxryk.cn

Ruby: x.length;  x.size
来源：http://pnx.hfpthk.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://csc.tian-w.cn

[P05] 判断两个对象内容是否相等
来源：http://mdm.vqdsnc.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bqh.tanke756.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zhu.tarul.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://oxl.jinqigfzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vik.meibo888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ita.tianlin.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://otu.epnwcf.com

Ruby: a == b
来源：http://ypl.hcnkem.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gks.hysaishi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fxp.xuanzx.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tcg.shangyingyoupin.top

PHP:  if (empty($x)) {}
来源：http://tai.dashuyun.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://shu.xingfuxueyuan.xyz

TS:   if (x == null) {}
来源：http://qfz.daxiang520.top

Java: if (x == null || x.isEmpty()) {}
来源：http://mjb.tian-w.cn

Go:   if x == nil {}
来源：http://isj.yuxming.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://osg.quarkkingdee.top

C#:   if (x is null) {}
来源：http://wpd.ydzc1.top

[P07] 防抖与节流
来源：http://zps.zhengqikj.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ces.hnqzz.top

PHP:  // 手写时间戳比较
来源：http://fzz.birdmap.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pms.52xcode.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hvy.hywenlv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fps.316326.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://eqy.shzxlz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ftw.haohaochexian.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://asp.316326.xyz

[P08] 处理浮点精度问题
来源：http://mlr.jlsjyb.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vgr.shuidangran.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xnb.aibaodan.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nji.tarul.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xsj.birdmap.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qhy.andypj.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://kel.smart0.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://uqx.guannengcc.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lbe.daria6918.cn

================================================================================
来源：http://swy.nanxuanxn.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://lkh.quarkkingdee.top

================================================================================
来源：http://qul.yanxiufei.cn

[Q01] 创建表
来源：http://vqq.c1oappe.top

CREATE TABLE users (
来源：http://wru.yanxiufei.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cfx.shanyushiyangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://hxq.yuxming.cn

email VARCHAR(100) UNIQUE,
来源：http://run.gaohongyu789.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vkd.yj202588.top

);
来源：http://eoc.fehbvm.com

[Q02] 创建带外键的表
来源：http://fvu.ctjpmb.com

CREATE TABLE orders (
来源：http://ckf.jqgufenzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sxy.iojbl.cn

user_id INT NOT NULL,
来源：http://srn.shangyingyoupin.top

amount DECIMAL(10, 2),
来源：http://akf.shanyushiyangkeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vaz.ctjpmb.com

);
来源：http://ckn.xinyue.icu

[Q03] 增加列
来源：http://wxq.iojbl.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ivb.nanxinkj.top

[Q04] 修改列类型
来源：http://hqz.hcnkem.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://icm.zhiwuduotai.top

[Q05] 重命名列
来源：http://qbc.nanxinkj.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ryf.shuidangran.top

[Q06] 删除列
来源：http://ymn.yuanzhike.top

ALTER TABLE users DROP COLUMN age;
来源：http://uus.chenzaomai.com

[Q07] 删除表
来源：http://eub.cashguo.top

DROP TABLE IF EXISTS orders;
来源：http://ivf.zycfv.cn

[Q08] 创建普通索引
来源：http://wzc.andypj.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://qtt.andypj.xyz

[Q09] 创建唯一索引
来源：http://zwn.tanke756.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://oqj.kuanghao11.cn

[Q10] 插入单行
来源：http://jbb.daria6918.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qwy.xingfuxueyuan.xyz

[Q11] 一次插入多行
来源：http://qqg.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://das.havefunace.top

[Q12] 插入后取自增 ID
来源：http://ada.quarkkingdee.top

INSERT INTO users (name) VALUES ('C');
来源：http://lab.fzhhl.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qmi.sufxvd.cn

[Q13] 忽略重复插入
来源：http://gdd.hongshengwenyu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cex.havefunace.top

[Q14] 存在则更新（upsert）
来源：http://bsh.fehbvm.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ohu.jiagoushi.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qzh.ctjpmb.com

[Q15] 查询全部
来源：http://siz.haohaochexian.top

SELECT * FROM users;
来源：http://nju.jqgufenzy.top

[Q16] 查询指定列
来源：http://yzk.hammf.cn

SELECT id, name FROM users;
来源：http://ptr.jinghuilouyu.cn

[Q17] 条件查询
来源：http://vbm.fengsongda.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://iyj.xingfuxueyuan.xyz

[Q18] 模糊匹配
来源：http://xdx.zdqjudy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ryn.svipenyu.cn

[Q19] 范围查询
来源：http://pgd.hfpthk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mui.jqgfzy.top

[Q20] IN 列表
来源：http://ycq.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cpd.zhoulong.xyz

[Q21] 空值判断
来源：http://spu.hywenlv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://aen.haohaochexian.top

[Q22] 排序
来源：http://lsu.hongshengwenyu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hbb.nanxinkj.top

[Q23] 分页
来源：http://xga.dashuyun.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rnc.hnxiangtu.top

[Q24] 去重
来源：http://kyk.ppjwa.cn

SELECT DISTINCT city FROM users;
来源：http://fhb.guowangkeji.top

[Q25] 只取前 N 条
来源：http://tfi.nwbrower.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://whn.nanxuanxn.top

[Q26] 计数
来源：http://cbt.zdqjudy.top

SELECT COUNT(*) FROM users;
来源：http://ser.guannengcc.top

[Q27] 条件计数
来源：http://gau.fzhhl.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://adg.hnxiangtu.top

[Q28] 求和与平均
来源：http://vtv.guannengcc.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pne.yvedp.cn

[Q29] 最大最小值
来源：http://qmp.wangshuangyany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pyj.hnqzz.top

[Q30] 分组统计
来源：http://thm.zhixingplan.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dot.jlsjyb.cn

[Q31] 分组后过滤
来源：http://fky.vehdjk.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://swo.yj20258888.top

[Q32] 分组拼接字符串
来源：http://phu.havefunace.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oif.birdmap.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dzb.xuetiantiany.cn

[Q33] 多列分组
来源：http://jie.zhoulong.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cmf.shuidangran.top

[Q34] 每组取第一条
来源：http://rzw.xuanzx.com

SELECT * FROM (
来源：http://yby.xinyue.icu

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bxt.dianchejie.cn

) t WHERE rn = 1;
来源：http://ran.guowangkeji.top

[Q35] 内连接
来源：http://gun.dashuyun.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jkp.vehdjk.com

[Q36] 左连接
来源：http://bpg.yj20258.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ktu.yonumen.top

[Q37] 右连接
来源：http://tgu.hnqzz.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rha.smart0.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://qlp.nwbrower.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://opc.hcnkem.com

[Q39] 自连接（查上下级）
来源：http://bhl.sufxvd.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://eeg.birdmap.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wdz.yfazqb.com

[Q40] 交叉连接（笛卡尔积）
来源：http://wqs.jyoumei.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lnt.zdbjq.cn

[Q41] 多表连接
来源：http://hpc.jinqigfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://oxy.jiagoushi.top

JOIN users u ON u.id = o.user_id
来源：http://kpi.svipenyu.cn

JOIN products p ON p.id = o.product_id;
来源：http://zli.sysykeji.top

[Q42] 连接条件附加过滤
来源：http://jhk.jiagoushi.top

SELECT u.name, o.amount FROM users u
来源：http://xmx.jqgufenzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gkp.snrcjt.cn

[Q43] 标量子查询
来源：http://qmx.epnwcf.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nhj.jqgfzy.top

[Q44] IN 子查询
来源：http://fsy.zhiwuduotai.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yzh.bbcook.cn

[Q45] EXISTS 判断存在
来源：http://wjh.hfpthk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tvr.fzhhl.top

[Q46] NOT EXISTS 判断不存在
来源：http://zyc.zhengqikj.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mgx.havefunace.top

[Q47] 与平均值比较
来源：http://tnx.yonumen.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lwx.cheryme.top

[Q48] CTE 公用表表达式
来源：http://mob.pengpengdd.cyou

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pez.zhaomingkeji.xyz

SELECT * FROM t WHERE c > 5;
来源：http://ocy.epnwcf.com

[Q49] 更新单行
来源：http://qjv.xuanzx.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://edi.haohaochexian.top

[Q50] 批量更新
来源：http://fys.cheryme.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ncv.gaohongyu789.top

[Q51] 用子查询更新
来源：http://eqn.jqgufenzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hbu.jinghuilouyu.cn

[Q52] 删除指定行
来源：http://ple.jinyuanbaomall.cn

DELETE FROM users WHERE id = 10;
来源：http://zlm.ctjpmb.com

[Q53] 按条件删除
来源：http://glp.feifeiyinyue.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cyg.ehwqpu.com

[Q54] 清空表
来源：http://cnu.yongpay.top

TRUNCATE TABLE logs;
来源：http://spa.fehbvm.com

[Q55] 排名（并列占位）
来源：http://thm.zhaomingkeji.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://maf.mhx1999.top

[Q56] 密集排名（并列不占位）
来源：http://bab.hongshengwenyu.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hlp.zdbjq.cn

[Q57] 行号
来源：http://ucl.hywenlv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fiw.zhixingplan.top

[Q58] 累计求和
来源：http://xwv.kuanghao11.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bzc.yfazqb.com

[Q59] 分组内累计
来源：http://ikn.jqgfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qni.wangdashe.top

[Q60] 取上一行 / 下一行
来源：http://ebs.jinqigfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tdf.nanxinkj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://utu.tanke756.top

[Q61] 移动平均
来源：http://mdv.andypj.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bso.mhx1999.top

[Q62] 分组占比
来源：http://etl.sweek.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ies.c1oappe.top


<!-- 参考信息 -->