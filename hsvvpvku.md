代发 wailian999

================================================================================
来源：http://aoi.fktsv.cn

O. 并发与异步
来源：http://ywq.hnqzz.top

================================================================================
来源：http://rgh.shuidangran.top

[O01] 启动一个线程
来源：http://tsw.yuxming.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://shx.fengsongda.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://pbj.yonumen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mci.zycfv.cn

TS:   // 同 JS
来源：http://hhy.uphjek.com

Java: new Thread(() -> f()).start()
来源：http://wbm.daxiang520.top

Go:   go f()
来源：http://pqp.havefunace.top

Ruby: Thread.new { f }
来源：http://kqm.sweek.top

C#:   Task.Run(() => F());
来源：http://hio.jinqigufen.top

[O02] 使用线程池
来源：http://bmr.zhaomingkeji.xyz

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dxi.ywan-chungtsiang.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fam.jqgfzy.top

JS:   // worker_threads 线程池
来源：http://wpx.aizwys.cn

TS:   // worker_threads 线程池
来源：http://ibo.jqgfzy.top

Java: Executors.newFixedThreadPool(4)
来源：http://zti.daxiang520.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://oqo.tian-w.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xmw.guannengcc.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lxx.fehbvm.com

[O03] 加锁保护共享数据
来源：http://mvi.hnxiangtu.top

Py:   with lock: shared += 1
来源：http://qfv.c1oappe.top

PHP:  // 用 flock() 做文件锁
来源：http://dgu.hongshengwenyu.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fdu.yuanzhike.top

TS:   // 同 JS
来源：http://vyb.havefunace.top

Java: synchronized (this) { shared++; }
来源：http://zei.jinqigufen.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://tvn.yueranfly.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://syf.ywan-chungtsiang.top

C#:   lock (gate) { shared++; }
来源：http://ori.jianghu66.top

[O04] 定义异步函数并等待
来源：http://anb.shangyingyoupin.top

Py:   async def f():⏎    await g()
来源：http://ovn.yueranfly.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ctd.guannengcc.top

JS:   async function f() { await g(); }
来源：http://jmk.yanxiufei.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://brk.ivvv.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vzs.hcnkem.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tzr.cashguo.top

Ruby: # 用 Fiber 或 async gem
来源：http://vnq.gzhubu.top

C#:   async Task F() { await G(); }
来源：http://btf.cashguo.top

[O05] 并发执行并等待全部完成
来源：http://hdq.jinqigufen.top

Py:   asyncio.gather(*tasks)
来源：http://fos.yuxming.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uor.kuanghao11.cn

JS:   await Promise.all(tasks)
来源：http://lbq.sweek.top

TS:   await Promise.all(tasks)
来源：http://adr.jinyuanbaomall.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ocd.hcnkem.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ekr.ppjwa.cn

Ruby: threads.map(&:join)
来源：http://ctb.cheryme.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pjb.hammf.cn

[O06] 使用进程池
来源：http://qrw.sufxvd.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fit.sysykeji.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fmd.52xcode.cn

JS:   // child_process / cluster 模块
来源：http://sie.nanxuanxn.top

TS:   // child_process / cluster 模块
来源：http://dya.aizwys.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rue.zhijiandao.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://pxa.yj20258888.top

Ruby: // fork 块
来源：http://eoo.hysaishi.cn

C#:   Parallel.For
来源：http://dfk.ehwqpu.com

================================================================================
来源：http://ssr.yuanzhike.top

P. 常用工具函数
来源：http://vcg.xinyue.icu

================================================================================
来源：http://zuj.zdqjudy.top

[P01] 生成 UUID
来源：http://umb.cucudq.cn

Py:   str(uuid.uuid4())
来源：http://iuj.gotoacloud.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gcu.shanyushiyangkeji.top

JS:   crypto.randomUUID()
来源：http://rxo.shuidangran.top

TS:   crypto.randomUUID()
来源：http://vzx.shuidangran.top

Java: UUID.randomUUID().toString()
来源：http://ilm.snrcjt.cn

Go:   // 用 github.com/google/uuid
来源：http://ehe.nanxinkj.top

Ruby: SecureRandom.uuid
来源：http://mra.mhx1999.top

C#:   Guid.NewGuid().ToString()
来源：http://onl.jinghuilouyu.cn

[P02] MD5 / SHA256 摘要
来源：http://zpz.bjfxy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://hnn.hesvh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qjy.tarul.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ylz.pycfn.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zrz.fanxiaobao.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lab.hcnkem.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qyd.shangyingyoupin.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mms.sufxvd.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ooh.ctjpmb.com

[P03] 生成短随机字符串
来源：http://enf.tanke756.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wlx.9152youxi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bcz.jqgufenzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://whm.ctjpmb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://swt.zhijiandao.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://anp.guannengcc.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://phz.9152youxi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jvz.dianchejie.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://epr.ydjk.org.cn

[P04] 求长度
来源：http://rmq.hywenlv.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://eha.yueranfly.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://eth.zhoulong.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://awz.svipenyu.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ddq.andypj.xyz

Java: list.size();  map.size();  s.length()
来源：http://hfi.xingfuxueyuan.xyz

Go:   len(arr);  len(m)
来源：http://imf.52xcode.cn

Ruby: x.length;  x.size
来源：http://bst.c1oappe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tjc.fanxiaobao.xyz

[P05] 判断两个对象内容是否相等
来源：http://tbv.jinghuilouyu.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://eag.52xcode.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ycz.zhiwuduotai.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fkh.fktsv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lcu.zhoulong.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sqg.feifeiyinyue.top

Go:   reflect.DeepEqual(a, b)
来源：http://xih.zhengqikj.top

Ruby: a == b
来源：http://ddo.cdnleiting.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kwk.vehdjk.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bhe.yj202588.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://exo.xylfe.cn

PHP:  if (empty($x)) {}
来源：http://atn.daxiang520.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uwo.nwbrower.top

TS:   if (x == null) {}
来源：http://nid.jinghuilouyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uat.hywenlv.cn

Go:   if x == nil {}
来源：http://hkp.pengpengdd.cyou

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jfi.hfpthk.cn

C#:   if (x is null) {}
来源：http://caw.yanxiufei.cn

[P07] 防抖与节流
来源：http://fnz.yanxiufei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bnl.ywan-chungtsiang.top

PHP:  // 手写时间戳比较
来源：http://apc.jianghu66.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tvp.andypj.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dtj.havefunace.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yve.cqqwz.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://gnx.ybcxt.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://sjr.ehwqpu.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ahc.xinyue.icu

[P08] 处理浮点精度问题
来源：http://rlq.zhengqikj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ulu.jyoumei.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xyc.jqgfzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xye.hcnkem.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kqx.fehbvm.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jqd.yfazqb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pzp.haohaochexian.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zvj.pycfn.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gtb.zhijiandao.cn

================================================================================
来源：http://osq.sweek.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ens.bjfxy.top

================================================================================
来源：http://bne.nanxinkj.top

[Q01] 创建表
来源：http://uch.iojbl.cn

CREATE TABLE users (
来源：http://ntq.bbcook.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blm.hnxiangtu.top

name VARCHAR(50) NOT NULL,
来源：http://qaa.yuxming.cn

email VARCHAR(100) UNIQUE,
来源：http://qrm.shanyushiyangkeji.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://whs.zdbjq.cn

);
来源：http://hfc.jqgufenzy.top

[Q02] 创建带外键的表
来源：http://bjg.52xcode.cn

CREATE TABLE orders (
来源：http://stz.yanxiufei.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xvy.ydzc1.top

user_id INT NOT NULL,
来源：http://ssd.316326.xyz

amount DECIMAL(10, 2),
来源：http://wvj.quarkkingdee.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://owe.zhijiandao.cn

);
来源：http://fhg.shanyushiyangtech.top

[Q03] 增加列
来源：http://nwb.xuetiantiany.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sfv.jiagoushi.top

[Q04] 修改列类型
来源：http://gon.pycfn.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pbn.dianchejie.cn

[Q05] 重命名列
来源：http://ejp.zhixingplan.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vtk.yongpay.top

[Q06] 删除列
来源：http://wmd.cdnleiting.top

ALTER TABLE users DROP COLUMN age;
来源：http://vja.wangdashe.top

[Q07] 删除表
来源：http://sqw.wangdashe.top

DROP TABLE IF EXISTS orders;
来源：http://iog.bbcook.cn

[Q08] 创建普通索引
来源：http://lhu.ppjwa.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://oel.jinghuilouyu.cn

[Q09] 创建唯一索引
来源：http://mpp.ehwqpu.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zql.zdbjq.cn

[Q10] 插入单行
来源：http://ump.nwbrower.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nnm.chenlongwang.top

[Q11] 一次插入多行
来源：http://wtx.hfpthk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vuq.yfazqb.com

[Q12] 插入后取自增 ID
来源：http://czl.zhengqikj.top

INSERT INTO users (name) VALUES ('C');
来源：http://hhd.daxiang520.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dpi.sysykeji.top

[Q13] 忽略重复插入
来源：http://upm.cucudq.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://koe.gaohongyu789.top

[Q14] 存在则更新（upsert）
来源：http://zmy.shanyushiyangtech.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rtm.ydzc1.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ivw.nwbrower.top

[Q15] 查询全部
来源：http://vjg.fzhhl.top

SELECT * FROM users;
来源：http://see.shzxlz.cn

[Q16] 查询指定列
来源：http://rdo.feifeiyinyue.top

SELECT id, name FROM users;
来源：http://qic.sufxvd.cn

[Q17] 条件查询
来源：http://vqo.chenlongwang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bhj.yfazqb.com

[Q18] 模糊匹配
来源：http://qhf.ywan-chungtsiang.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pbo.xuanzx.com

[Q19] 范围查询
来源：http://xua.guannengcc.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mta.jlsjyb.cn

[Q20] IN 列表
来源：http://wad.jianghu66.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oao.chenzaomai.com

[Q21] 空值判断
来源：http://szn.jlsjyb.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://sqd.tanke756.top

[Q22] 排序
来源：http://fky.mhx1999.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ixg.havefunace.top

[Q23] 分页
来源：http://xyr.guannengcc.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://iuj.xuetiantiany.cn

[Q24] 去重
来源：http://xal.shzxlz.cn

SELECT DISTINCT city FROM users;
来源：http://npx.sweek.top

[Q25] 只取前 N 条
来源：http://tnb.cashguo.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mcr.yonumen.top

[Q26] 计数
来源：http://det.smart0.xyz

SELECT COUNT(*) FROM users;
来源：http://tci.shangyingyoupin.top

[Q27] 条件计数
来源：http://wdi.hywenlv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rci.svipenyu.cn

[Q28] 求和与平均
来源：http://ukv.ehwqpu.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pzq.fanxiaobao.xyz

[Q29] 最大最小值
来源：http://yit.pycfn.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://lbj.chenzaomai.com

[Q30] 分组统计
来源：http://hmh.tarul.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jtj.kuanghao11.cn

[Q31] 分组后过滤
来源：http://xwr.316326.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://onq.xuetiantiany.cn

[Q32] 分组拼接字符串
来源：http://tzy.pycfn.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wew.cheryme.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://arc.nanxuanxn.top

[Q33] 多列分组
来源：http://rpn.hesvh.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xbx.ydzc1.top

[Q34] 每组取第一条
来源：http://vbq.ybcxt.top

SELECT * FROM (
来源：http://klv.zycfv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vzl.wangshuangyany.cn

) t WHERE rn = 1;
来源：http://gua.zycfv.cn

[Q35] 内连接
来源：http://xzt.guowangkeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://axa.jinqigufen.top

[Q36] 左连接
来源：http://scp.jqgfzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hfo.haohaochexian.top

[Q37] 右连接
来源：http://ibu.kuanghao11.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iac.sufxvd.cn

[Q38] 全外连接（PostgreSQL）
来源：http://phe.cashguo.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qdz.hnxiangtu.top

[Q39] 自连接（查上下级）
来源：http://eeb.chenjidiqi.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://cvt.cheryme.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xwy.bjfxy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://sgz.dianchejie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rvk.jinqigfzy.top

[Q41] 多表连接
来源：http://kub.yueranfly.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hwz.yueranfly.top

JOIN users u ON u.id = o.user_id
来源：http://phw.hammf.cn

JOIN products p ON p.id = o.product_id;
来源：http://jta.jqgufenzy.top

[Q42] 连接条件附加过滤
来源：http://vry.yangfankeji.com

SELECT u.name, o.amount FROM users u
来源：http://veo.snrcjt.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://iuu.guannengcc.top

[Q43] 标量子查询
来源：http://cuc.zhongyouzk.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://izo.gzhubu.top

[Q44] IN 子查询
来源：http://rta.gotoacloud.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://owc.andypj.xyz

[Q45] EXISTS 判断存在
来源：http://qna.feifeiyinyue.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://drp.zdbjq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://suy.fengsongda.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bcb.gzhubu.top

[Q47] 与平均值比较
来源：http://vas.pengpengdd.cyou

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fhq.zhoulong.xyz

[Q48] CTE 公用表表达式
来源：http://mhx.gogol.net.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kjw.jyoumei.cn

SELECT * FROM t WHERE c > 5;
来源：http://pqc.zhaomingkeji.xyz

[Q49] 更新单行
来源：http://tzv.bjfxy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jui.dashuyun.cn

[Q50] 批量更新
来源：http://wkt.chenjidiqi.icu

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ymb.hongshengwenyu.top

[Q51] 用子查询更新
来源：http://dco.andypj.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wym.zhongyouzk.top

[Q52] 删除指定行
来源：http://ffh.guannengcc.top

DELETE FROM users WHERE id = 10;
来源：http://ywo.jyoumei.cn

[Q53] 按条件删除
来源：http://qjs.ywan-chungtsiang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tvq.cdnleiting.top

[Q54] 清空表
来源：http://sta.ydzc1.top

TRUNCATE TABLE logs;
来源：http://zzr.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://jea.guowangkeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jdb.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://raz.fzhhl.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://llm.ctjpmb.com

[Q57] 行号
来源：http://zyg.daria6918.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mpe.zhixingplan.top

[Q58] 累计求和
来源：http://ezf.aizwys.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tlt.daxiang520.top

[Q59] 分组内累计
来源：http://gqa.redwolf501.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gep.chenjidiqi.icu

[Q60] 取上一行 / 下一行
来源：http://veq.feifeiyinyue.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nzk.yj20258.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://avd.jqgfzy.top

[Q61] 移动平均
来源：http://dmw.hnqzz.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mow.zhijiandao.cn

[Q62] 分组占比
来源：http://rat.aizwys.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bmv.zhiwuduotai.top

[Q63] 开启事务
来源：http://erp.sjlbkw.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://tgn.guowangkeji.top

[Q64] 提交事务
来源：http://lnr.daria6918.cn

COMMIT;
来源：http://rij.nanxinkj.top

[Q65] 回滚事务
来源：http://mwi.chenjidiqi.icu

ROLLBACK;
来源：http://cty.tanke756.top

[Q66] 行锁查询
来源：http://zlp.xylfe.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jwx.cqqwz.cn

[Q67] 设置隔离级别
来源：http://roo.mhx1999.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tnn.nwbrower.top

[Q68] 保存点
来源：http://flc.yonumen.top

SAVEPOINT sp1;
来源：http://lnd.smart0.xyz

ROLLBACK TO sp1;
来源：http://vjv.0kj1m.cn

[Q69] 查看执行计划
来源：http://jwr.hysaishi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tux.jqgufenzy.top

[Q70] 更新统计信息
来源：http://mew.smart0.xyz

ANALYZE TABLE users;
来源：http://orv.chenlongwang.top

[Q71] 查看建表语句
来源：http://ctz.shzxlz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oha.xinyue.icu

[Q72] 查看索引
来源：http://gwc.gogol.net.cn


<!-- 参考信息 -->