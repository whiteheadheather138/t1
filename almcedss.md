代发 wailian999

Go:   // 手写递归
来源：http://kza.hammf.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yht.jlsjyb.cn

C#:   // 手写递归
来源：http://ruv.sjlbkw.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://exp.jqgufenzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://zwj.jianghu66.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://bhh.shzxlz.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pte.yj20258888.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wpf.guowangkeji.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://kaj.yanxiufei.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gve.fzhhl.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://crj.yvedp.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hxp.ctjpmb.com

================================================================================
来源：http://cpl.vqdsnc.cn

O. 并发与异步
来源：http://kao.svipenyu.cn

================================================================================
来源：http://wjl.mhx1999.top

[O01] 启动一个线程
来源：http://fif.bbcook.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wlm.guowangkeji.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zjf.fengsongda.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mur.fanxiaobao.xyz

TS:   // 同 JS
来源：http://twe.cucudq.cn

Java: new Thread(() -> f()).start()
来源：http://cio.tianlin.xyz

Go:   go f()
来源：http://hkh.fktsv.cn

Ruby: Thread.new { f }
来源：http://fll.pengpengdd.cyou

C#:   Task.Run(() => F());
来源：http://zew.dianchejie.cn

[O02] 使用线程池
来源：http://cux.cheryme.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wwy.fengsongda.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://tck.yj202588.top

JS:   // worker_threads 线程池
来源：http://ifx.shanyushiyangtech.top

TS:   // worker_threads 线程池
来源：http://dub.guannengcc.top

Java: Executors.newFixedThreadPool(4)
来源：http://phr.fehbvm.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dtn.xinyue.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gzs.ivvv.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tyq.shzxlz.cn

[O03] 加锁保护共享数据
来源：http://xhe.aizwys.cn

Py:   with lock: shared += 1
来源：http://vak.gotoacloud.top

PHP:  // 用 flock() 做文件锁
来源：http://bgc.chenzaomai.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ecf.nwbrower.top

TS:   // 同 JS
来源：http://tfo.gotoacloud.top

Java: synchronized (this) { shared++; }
来源：http://klg.fengsongda.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gww.dianchejie.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fef.xuetiantiany.cn

C#:   lock (gate) { shared++; }
来源：http://ubw.wangshuangyany.cn

[O04] 定义异步函数并等待
来源：http://sbt.c1oappe.top

Py:   async def f():⏎    await g()
来源：http://kgp.jqgfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cux.hfpthk.cn

JS:   async function f() { await g(); }
来源：http://ook.sufxvd.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rvu.hesvh.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ozk.zhoulong.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cfn.uphjek.com

Ruby: # 用 Fiber 或 async gem
来源：http://afm.yanxiufei.cn

C#:   async Task F() { await G(); }
来源：http://wmk.ybcxt.top

[O05] 并发执行并等待全部完成
来源：http://whr.zdqjudy.top

Py:   asyncio.gather(*tasks)
来源：http://brl.wangshuangyany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://woq.yangfankeji.com

JS:   await Promise.all(tasks)
来源：http://jyb.yangfankeji.com

TS:   await Promise.all(tasks)
来源：http://fyf.hesvh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aqp.andypj.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fvy.yj202588.top

Ruby: threads.map(&:join)
来源：http://fak.ybcxt.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ltu.cashguo.top

[O06] 使用进程池
来源：http://ifk.feifeiyinyue.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://alq.jqgufenzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://lvs.ivvv.top

JS:   // child_process / cluster 模块
来源：http://wlp.jinyuanbaomall.cn

TS:   // child_process / cluster 模块
来源：http://zjh.gaohongyu789.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tfi.snrcjt.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jky.ydzc1.top

Ruby: // fork 块
来源：http://ixs.andypj.xyz

C#:   Parallel.For
来源：http://oqa.jiagoushi.top

================================================================================
来源：http://rnq.cqqwz.cn

P. 常用工具函数
来源：http://wne.sufxvd.cn

================================================================================
来源：http://tum.sysykeji.top

[P01] 生成 UUID
来源：http://ole.xinyue.icu

Py:   str(uuid.uuid4())
来源：http://afy.chenjidiqi.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nob.sxryk.cn

JS:   crypto.randomUUID()
来源：http://dpo.shanyushiyangkeji.top

TS:   crypto.randomUUID()
来源：http://bdr.havefunace.top

Java: UUID.randomUUID().toString()
来源：http://frq.zhiwuduotai.top

Go:   // 用 github.com/google/uuid
来源：http://pfw.tianlin.xyz

Ruby: SecureRandom.uuid
来源：http://kow.nanxuanxn.top

C#:   Guid.NewGuid().ToString()
来源：http://gin.wangshuangyany.cn

[P02] MD5 / SHA256 摘要
来源：http://apj.guannengcc.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://oij.fktsv.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xfe.fzhhl.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xib.yueranfly.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://doj.gogol.net.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bue.cqqwz.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uyr.sufxvd.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rty.fanxiaobao.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wrh.chenzaomai.com

[P03] 生成短随机字符串
来源：http://tzd.hcnkem.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cej.svipenyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lea.cashguo.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jpe.pycfn.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ygc.fehbvm.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wxk.aizwys.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://heg.9152youxi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ief.mhx1999.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sih.9152youxi.cn

[P04] 求长度
来源：http://gbr.birdmap.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://izr.fehbvm.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iph.dashuyun.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://knj.chenjidiqi.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rqi.zhiwuduotai.top

Java: list.size();  map.size();  s.length()
来源：http://gty.ehwqpu.com

Go:   len(arr);  len(m)
来源：http://uis.andypj.xyz

Ruby: x.length;  x.size
来源：http://xuo.epnwcf.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://lep.birdmap.top

[P05] 判断两个对象内容是否相等
来源：http://gwn.52xcode.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bfa.ivvv.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://avp.hysaishi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://azl.shuidangran.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kgg.gogol.net.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gev.hnqzz.top

Go:   reflect.DeepEqual(a, b)
来源：http://fir.meibo888.top

Ruby: a == b
来源：http://svt.c1oappe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cbg.dashuyun.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://iya.dianchejie.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://len.shanyushiyangkeji.top

PHP:  if (empty($x)) {}
来源：http://wwp.haohaochexian.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fhs.c1oappe.top

TS:   if (x == null) {}
来源：http://nqu.ywan-chungtsiang.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fzs.cheryme.top

Go:   if x == nil {}
来源：http://wud.ppjwa.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oco.zdbjq.cn

C#:   if (x is null) {}
来源：http://few.sxryk.cn

[P07] 防抖与节流
来源：http://isy.nanxuanxn.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cdm.aibaodan.cn

PHP:  // 手写时间戳比较
来源：http://wyi.yuxming.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://scc.sweek.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pjb.xinyue.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ntr.tian-w.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hyj.jinqigufen.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://rkd.ivvv.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://roc.smart0.xyz

[P08] 处理浮点精度问题
来源：http://wjf.gaohongyu789.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pxs.sweek.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://stc.zhijiandao.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://heb.c1oappe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nuj.zhoulong.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dtr.guowangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://spt.fehbvm.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hox.fzhhl.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://cwv.gaohongyu789.top

================================================================================
来源：http://pxc.ehwqpu.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://agx.snrcjt.cn

================================================================================
来源：http://uql.yuxming.cn

[Q01] 创建表
来源：http://clk.gotoacloud.top

CREATE TABLE users (
来源：http://hex.meibo888.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://reh.zhengqikj.top

name VARCHAR(50) NOT NULL,
来源：http://bff.ctjpmb.com

email VARCHAR(100) UNIQUE,
来源：http://jzu.zhixingplan.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uou.snrcjt.cn

);
来源：http://kqf.snrcjt.cn

[Q02] 创建带外键的表
来源：http://cnv.yuanzhike.top

CREATE TABLE orders (
来源：http://llq.feifeiyinyue.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ffm.gzhubu.top

user_id INT NOT NULL,
来源：http://zuz.dianchejie.cn

amount DECIMAL(10, 2),
来源：http://nhj.yj202588.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vjg.xuetiantiany.cn

);
来源：http://qjd.zhijiandao.cn

[Q03] 增加列
来源：http://uqa.shangyingyoupin.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ehi.wangshuangyany.cn

[Q04] 修改列类型
来源：http://kdo.andypj.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qls.meibo888.top

[Q05] 重命名列
来源：http://sfr.ppjwa.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wvf.cashguo.top

[Q06] 删除列
来源：http://oug.xuetiantiany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://aex.nanxuanxn.top

[Q07] 删除表
来源：http://zwc.vehdjk.com

DROP TABLE IF EXISTS orders;
来源：http://uei.316326.xyz

[Q08] 创建普通索引
来源：http://kok.shuidangran.top

CREATE INDEX idx_users_email ON users(email);
来源：http://nqa.gzhubu.top

[Q09] 创建唯一索引
来源：http://lny.ivvv.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nzl.ybcxt.top

[Q10] 插入单行
来源：http://xso.9152youxi.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ebm.xuanzx.com

[Q11] 一次插入多行
来源：http://bxx.sweek.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://apn.hammf.cn

[Q12] 插入后取自增 ID
来源：http://arc.jinyuanbaomall.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vkm.jqgfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zsn.jianghu66.top

[Q13] 忽略重复插入
来源：http://oeo.tanke756.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lnj.bjfxy.top

[Q14] 存在则更新（upsert）
来源：http://zdg.jinqigfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kqi.c1oappe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://omf.zdqjudy.top

[Q15] 查询全部
来源：http://jbh.meibo888.top

SELECT * FROM users;
来源：http://spr.xinyue.icu

[Q16] 查询指定列
来源：http://khb.zhaomingkeji.xyz

SELECT id, name FROM users;
来源：http://vms.guowangkeji.top

[Q17] 条件查询
来源：http://nuo.shanyushiyangkeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ojk.pycfn.com

[Q18] 模糊匹配
来源：http://muh.sweek.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://anr.sufxvd.cn

[Q19] 范围查询
来源：http://rkq.zhoulong.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gon.hammf.cn

[Q20] IN 列表
来源：http://vyi.vqdsnc.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xan.dashuyun.cn

[Q21] 空值判断
来源：http://mpk.nanxuanxn.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vjk.shanyushiyangkeji.top

[Q22] 排序
来源：http://hno.jqgfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wgf.fanxiaobao.xyz

[Q23] 分页
来源：http://rxe.dashuyun.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nbf.hesvh.cn

[Q24] 去重
来源：http://fxi.xingfuxueyuan.xyz

SELECT DISTINCT city FROM users;
来源：http://yyr.cheryme.top

[Q25] 只取前 N 条
来源：http://rez.hesvh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kdm.jqgufenzy.top

[Q26] 计数
来源：http://dyg.bjfxy.top

SELECT COUNT(*) FROM users;
来源：http://czc.shanyushiyangkeji.top

[Q27] 条件计数
来源：http://upl.zhaomingkeji.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pty.quarkkingdee.top

[Q28] 求和与平均
来源：http://xlw.hcnkem.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mko.ywan-chungtsiang.top

[Q29] 最大最小值
来源：http://csg.sjlbkw.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://igb.fanxiaobao.xyz

[Q30] 分组统计
来源：http://jrr.shanyushiyangtech.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jts.ppjwa.cn

[Q31] 分组后过滤
来源：http://ala.tanke756.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://slo.zdbjq.cn

[Q32] 分组拼接字符串
来源：http://jux.guannengcc.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ygu.gaohongyu789.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tuw.hammf.cn

[Q33] 多列分组
来源：http://hnc.aibaodan.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xrw.tianlin.xyz

[Q34] 每组取第一条
来源：http://qlt.jiagoushi.top

SELECT * FROM (
来源：http://qct.birdmap.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://imf.yuanzhike.top

) t WHERE rn = 1;
来源：http://non.bbcook.cn

[Q35] 内连接
来源：http://mks.zycfv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dbk.zhongyouzk.top

[Q36] 左连接
来源：http://scu.chenlongwang.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nab.birdmap.top

[Q37] 右连接
来源：http://zcs.xinyue.icu

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gqb.jinyuanbaomall.cn

[Q38] 全外连接（PostgreSQL）
来源：http://nsc.hnqzz.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zjy.zhiwuduotai.top

[Q39] 自连接（查上下级）
来源：http://zww.yuanzhike.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hqv.yueranfly.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tac.fanxiaobao.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://twf.chenjidiqi.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sme.wangdashe.top

[Q41] 多表连接
来源：http://oot.daxiang520.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ebf.yangfankeji.com

JOIN users u ON u.id = o.user_id
来源：http://zft.yj20258888.top

JOIN products p ON p.id = o.product_id;
来源：http://tua.fengsongda.top

[Q42] 连接条件附加过滤
来源：http://vdq.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u
来源：http://zjw.zycfv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://izd.shuidangran.top

[Q43] 标量子查询
来源：http://wxo.hysaishi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nav.xingfuxueyuan.xyz

[Q44] IN 子查询
来源：http://ypn.jqgfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zbc.birdmap.top

[Q45] EXISTS 判断存在
来源：http://cqo.ywan-chungtsiang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hqw.jinghuilouyu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nvk.ctjpmb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vgl.hammf.cn

[Q47] 与平均值比较
来源：http://ujd.fehbvm.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fwc.hammf.cn

[Q48] CTE 公用表表达式
来源：http://tqb.yongpay.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dha.jinqigfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://sjc.iojbl.cn

[Q49] 更新单行
来源：http://htr.chenlongwang.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://kkg.0kj1m.cn

[Q50] 批量更新
来源：http://eou.birdmap.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://irf.iojbl.cn

[Q51] 用子查询更新
来源：http://hln.xziqi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hzy.jyoumei.cn

[Q52] 删除指定行
来源：http://vlx.yanxiufei.cn

DELETE FROM users WHERE id = 10;
来源：http://qxq.ivvv.top

[Q53] 按条件删除
来源：http://gai.yj20258.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qfo.fehbvm.com

[Q54] 清空表
来源：http://ajp.hammf.cn

TRUNCATE TABLE logs;
来源：http://xsf.chenjidiqi.icu

[Q55] 排名（并列占位）
来源：http://xbq.hfpthk.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hej.jyoumei.cn

[Q56] 密集排名（并列不占位）
来源：http://xvg.daria6918.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://syb.zhixingplan.top

[Q57] 行号
来源：http://xzt.yvedp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gga.jianghu66.top

[Q58] 累计求和
来源：http://hbc.jianghu66.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pqa.fktsv.cn

[Q59] 分组内累计
来源：http://fdq.zhijiandao.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://otd.cucudq.cn

[Q60] 取上一行 / 下一行
来源：http://hod.xylfe.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://eep.yfazqb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://izn.jqgfzy.top

[Q61] 移动平均
来源：http://ybj.jinghuilouyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rwi.9152youxi.cn

[Q62] 分组占比
来源：http://vtr.zhaomingkeji.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vwc.yonumen.top

[Q63] 开启事务
来源：http://bhc.cqqwz.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nmg.meibo888.top

[Q64] 提交事务
来源：http://pee.yuxming.cn

COMMIT;
来源：http://xyv.ybcxt.top

[Q65] 回滚事务
来源：http://zdk.daxiang520.top

ROLLBACK;
来源：http://vce.0kj1m.cn

[Q66] 行锁查询
来源：http://bbq.havefunace.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ibi.epnwcf.com


<!-- 参考信息 -->