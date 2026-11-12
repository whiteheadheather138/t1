代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qzf.cdnleiting.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://teg.nwbrower.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://igc.cdnleiting.top

TS:   // 同 JS
来源：http://lng.ydjk.org.cn

Java: new Thread(() -> f()).start()
来源：http://iox.fktsv.cn

Go:   go f()
来源：http://ahi.tanke756.top

Ruby: Thread.new { f }
来源：http://xtd.zhoulong.xyz

C#:   Task.Run(() => F());
来源：http://vzl.bbcook.cn

[O02] 使用线程池
来源：http://bga.zdqjudy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://vrg.nanxinkj.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wtx.ywan-chungtsiang.top

JS:   // worker_threads 线程池
来源：http://cbd.jinyuanbaomall.cn

TS:   // worker_threads 线程池
来源：http://nka.chenzaomai.com

Java: Executors.newFixedThreadPool(4)
来源：http://kkb.xuanzx.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://cue.hnxiangtu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://urx.yuanzhike.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hda.andypj.xyz

[O03] 加锁保护共享数据
来源：http://rwh.yfazqb.com

Py:   with lock: shared += 1
来源：http://plg.fktsv.cn

PHP:  // 用 flock() 做文件锁
来源：http://alc.bbcook.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://hxi.xziqi.cn

TS:   // 同 JS
来源：http://gip.cqqwz.cn

Java: synchronized (this) { shared++; }
来源：http://mxk.sjlbkw.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cxm.shanyushiyangkeji.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://iho.jianghu66.top

C#:   lock (gate) { shared++; }
来源：http://bte.quarkkingdee.top

[O04] 定义异步函数并等待
来源：http://xqn.jinyuanbaomall.cn

Py:   async def f():⏎    await g()
来源：http://mvn.gogol.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://typ.yfazqb.com

JS:   async function f() { await g(); }
来源：http://ies.guannengcc.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://def.9152youxi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vyy.hywenlv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hpx.cqqwz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gfk.kuanghao11.cn

C#:   async Task F() { await G(); }
来源：http://xcx.9152youxi.cn

[O05] 并发执行并等待全部完成
来源：http://vdh.sweek.top

Py:   asyncio.gather(*tasks)
来源：http://qcw.hesvh.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dfg.shanyushiyangtech.top

JS:   await Promise.all(tasks)
来源：http://ozi.kuanghao11.cn

TS:   await Promise.all(tasks)
来源：http://bsb.pengpengdd.cyou

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://loq.yanxiufei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tzx.vqdsnc.cn

Ruby: threads.map(&:join)
来源：http://fyq.hesvh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mxj.jqgufenzy.top

[O06] 使用进程池
来源：http://eda.yj20258.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://psl.yj20258888.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kqb.tian-w.cn

JS:   // child_process / cluster 模块
来源：http://rgb.ivvv.top

TS:   // child_process / cluster 模块
来源：http://tcc.tarul.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fiu.zhengqikj.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jht.jianghu66.top

Ruby: // fork 块
来源：http://ncz.fzhhl.top

C#:   Parallel.For
来源：http://idq.jianghu66.top

================================================================================
来源：http://tyd.jqgufenzy.top

P. 常用工具函数
来源：http://rjk.fehbvm.com

================================================================================
来源：http://hpn.chenlongwang.top

[P01] 生成 UUID
来源：http://hai.haohaochexian.top

Py:   str(uuid.uuid4())
来源：http://lwe.hcnkem.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://dij.ivvv.top

JS:   crypto.randomUUID()
来源：http://arz.ivvv.top

TS:   crypto.randomUUID()
来源：http://dem.yvedp.cn

Java: UUID.randomUUID().toString()
来源：http://rjd.sxryk.cn

Go:   // 用 github.com/google/uuid
来源：http://uqp.redwolf501.top

Ruby: SecureRandom.uuid
来源：http://out.hywenlv.cn

C#:   Guid.NewGuid().ToString()
来源：http://nzf.uphjek.com

[P02] MD5 / SHA256 摘要
来源：http://ecn.0kj1m.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pcd.yj202588.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://gri.cdnleiting.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://tqn.zdqjudy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://swz.jlsjyb.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://htb.zhoulong.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ocw.52xcode.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gxl.shuidangran.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ono.fktsv.cn

[P03] 生成短随机字符串
来源：http://scw.jqgufenzy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qfc.gogol.net.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hlg.havefunace.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zha.redwolf501.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vbn.xziqi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jci.yuanzhike.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cpk.hysaishi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zqo.yj20258.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://txy.quarkkingdee.top

[P04] 求长度
来源：http://ugl.hfpthk.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ihf.jinqigfzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wzl.hfpthk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://efp.sxryk.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vyg.tarul.cn

Java: list.size();  map.size();  s.length()
来源：http://quv.cucudq.cn

Go:   len(arr);  len(m)
来源：http://fvm.zhongyouzk.top

Ruby: x.length;  x.size
来源：http://sse.fktsv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vku.nanxuanxn.top

[P05] 判断两个对象内容是否相等
来源：http://fos.sufxvd.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://sqb.shanyushiyangtech.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bza.jyoumei.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vsc.chenzaomai.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bfm.guannengcc.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zdd.smart0.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://hpu.zdqjudy.top

Ruby: a == b
来源：http://gqu.cdnleiting.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rek.daxiang520.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://klt.0kj1m.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://kja.shangyingyoupin.top

PHP:  if (empty($x)) {}
来源：http://dck.yanxiufei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://osz.fzhhl.top

TS:   if (x == null) {}
来源：http://lbl.hnxiangtu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://idk.cheryme.top

Go:   if x == nil {}
来源：http://lst.sweek.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mvo.snrcjt.cn

C#:   if (x is null) {}
来源：http://edj.hfpthk.cn

[P07] 防抖与节流
来源：http://dre.zhijiandao.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zhe.hnxiangtu.top

PHP:  // 手写时间戳比较
来源：http://aur.cqqwz.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gjs.gotoacloud.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tbo.ydzc1.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://toc.cucudq.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://dmp.sufxvd.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://wym.sweek.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xiz.tianlin.xyz

[P08] 处理浮点精度问题
来源：http://ebl.guowangkeji.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dhy.hcnkem.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mmb.mhx1999.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cyn.andypj.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://frr.jinghuilouyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fqc.fanxiaobao.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wad.dianchejie.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rmz.gaohongyu789.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://aju.jqgufenzy.top

================================================================================
来源：http://svk.daria6918.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ayy.zhijiandao.cn

================================================================================
来源：http://vjc.52xcode.cn

[Q01] 创建表
来源：http://mxb.fktsv.cn

CREATE TABLE users (
来源：http://fli.jlsjyb.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cuy.wangdashe.top

name VARCHAR(50) NOT NULL,
来源：http://sqm.jlsjyb.cn

email VARCHAR(100) UNIQUE,
来源：http://kle.jqgufenzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vdv.aibaodan.cn

);
来源：http://fsr.ydzc1.top

[Q02] 创建带外键的表
来源：http://jvn.shanyushiyangkeji.top

CREATE TABLE orders (
来源：http://sto.aizwys.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cqo.zhijiandao.cn

user_id INT NOT NULL,
来源：http://pxp.xuetiantiany.cn

amount DECIMAL(10, 2),
来源：http://dpm.sjlbkw.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fxj.dashuyun.cn

);
来源：http://xqg.quarkkingdee.top

[Q03] 增加列
来源：http://aip.jinqigufen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pxt.quarkkingdee.top

[Q04] 修改列类型
来源：http://xsw.hnxiangtu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cwp.sufxvd.cn

[Q05] 重命名列
来源：http://rqa.gotoacloud.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://iwi.smart0.xyz

[Q06] 删除列
来源：http://jhg.jqgufenzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://zcc.yvedp.cn

[Q07] 删除表
来源：http://hpz.xinyue.icu

DROP TABLE IF EXISTS orders;
来源：http://jjv.redwolf501.top

[Q08] 创建普通索引
来源：http://sqa.ywan-chungtsiang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gqk.iojbl.cn

[Q09] 创建唯一索引
来源：http://yja.sysykeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xwu.xuanzx.com

[Q10] 插入单行
来源：http://klk.yj20258888.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mzn.xuanzx.com

[Q11] 一次插入多行
来源：http://gnu.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://chl.daxiang520.top

[Q12] 插入后取自增 ID
来源：http://owj.wangdashe.top

INSERT INTO users (name) VALUES ('C');
来源：http://pmd.yuanzhike.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://rix.zhengqikj.top

[Q13] 忽略重复插入
来源：http://tbp.ybcxt.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ksr.cashguo.top

[Q14] 存在则更新（upsert）
来源：http://xzl.shanyushiyangtech.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bcm.sysykeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mat.jqgufenzy.top

[Q15] 查询全部
来源：http://qfd.bjfxy.top

SELECT * FROM users;
来源：http://brh.tianlin.xyz

[Q16] 查询指定列
来源：http://wuu.fanxiaobao.xyz

SELECT id, name FROM users;
来源：http://dlw.aizwys.cn

[Q17] 条件查询
来源：http://lkk.sufxvd.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://caz.ctjpmb.com

[Q18] 模糊匹配
来源：http://uso.bbcook.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dge.sxryk.cn

[Q19] 范围查询
来源：http://scl.fanxiaobao.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mbm.smart0.xyz

[Q20] IN 列表
来源：http://isa.jlsjyb.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bef.jinyuanbaomall.cn

[Q21] 空值判断
来源：http://jck.jinqigfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kdi.jinqigfzy.top

[Q22] 排序
来源：http://aco.tarul.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kph.bjfxy.top

[Q23] 分页
来源：http://jun.yj20258.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tra.jyoumei.cn

[Q24] 去重
来源：http://hgp.yanxiufei.cn

SELECT DISTINCT city FROM users;
来源：http://vkq.zhengqikj.top

[Q25] 只取前 N 条
来源：http://pcb.ybcxt.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fju.bbcook.cn

[Q26] 计数
来源：http://oxn.cqqwz.cn

SELECT COUNT(*) FROM users;
来源：http://xif.sjlbkw.cn

[Q27] 条件计数
来源：http://vhr.havefunace.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pxw.aizwys.cn

[Q28] 求和与平均
来源：http://ljj.shuidangran.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://elm.ybcxt.top

[Q29] 最大最小值
来源：http://tmn.sxryk.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yny.yj202588.top

[Q30] 分组统计
来源：http://kmo.feifeiyinyue.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rbd.nanxinkj.top

[Q31] 分组后过滤
来源：http://apl.wangshuangyany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vaa.fanxiaobao.xyz

[Q32] 分组拼接字符串
来源：http://ook.xuanzx.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vtf.epnwcf.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fit.hongshengwenyu.top

[Q33] 多列分组
来源：http://wzo.vehdjk.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://boi.aizwys.cn

[Q34] 每组取第一条
来源：http://woq.zhixingplan.top

SELECT * FROM (
来源：http://dcy.bbcook.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bid.shanyushiyangtech.top

) t WHERE rn = 1;
来源：http://uyq.fzhhl.top

[Q35] 内连接
来源：http://sfd.nanxinkj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fms.cheryme.top

[Q36] 左连接
来源：http://hre.epnwcf.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wmc.hesvh.cn

[Q37] 右连接
来源：http://yhb.ydjk.org.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mia.hysaishi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://sbu.pycfn.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hws.nwbrower.top

[Q39] 自连接（查上下级）
来源：http://tjz.jyoumei.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ykq.hysaishi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vzd.vehdjk.com

[Q40] 交叉连接（笛卡尔积）
来源：http://bjo.pengpengdd.cyou

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fjt.havefunace.top

[Q41] 多表连接
来源：http://rgm.shangyingyoupin.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rnf.zdbjq.cn

JOIN users u ON u.id = o.user_id
来源：http://ixr.nwbrower.top

JOIN products p ON p.id = o.product_id;
来源：http://cqd.aibaodan.cn

[Q42] 连接条件附加过滤
来源：http://sbf.fengsongda.top

SELECT u.name, o.amount FROM users u
来源：http://vyy.hcnkem.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jtb.jqgufenzy.top

[Q43] 标量子查询
来源：http://pwc.yanxiufei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kmb.nanxinkj.top

[Q44] IN 子查询
来源：http://zhd.nanxuanxn.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kob.chenzaomai.com

[Q45] EXISTS 判断存在
来源：http://ygs.bjfxy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wlu.dashuyun.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rxx.yonumen.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xft.tian-w.cn

[Q47] 与平均值比较
来源：http://gbd.316326.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ucf.zdbjq.cn

[Q48] CTE 公用表表达式
来源：http://pgx.nanxinkj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zcg.aibaodan.cn

SELECT * FROM t WHERE c > 5;
来源：http://zoq.yongpay.top

[Q49] 更新单行
来源：http://hrf.yangfankeji.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zof.vqdsnc.cn

[Q50] 批量更新
来源：http://udv.gogol.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ane.birdmap.top

[Q51] 用子查询更新
来源：http://jpy.hfpthk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://akl.zycfv.cn

[Q52] 删除指定行
来源：http://uhg.xingfuxueyuan.xyz

DELETE FROM users WHERE id = 10;
来源：http://rjs.aizwys.cn

[Q53] 按条件删除
来源：http://ila.yfazqb.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mdo.ivvv.top

[Q54] 清空表
来源：http://arh.shanyushiyangkeji.top

TRUNCATE TABLE logs;
来源：http://kcu.vehdjk.com

[Q55] 排名（并列占位）
来源：http://xhf.haohaochexian.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gwx.andypj.xyz

[Q56] 密集排名（并列不占位）
来源：http://iea.hcnkem.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xrk.sufxvd.cn

[Q57] 行号
来源：http://giu.shuidangran.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fay.feifeiyinyue.top

[Q58] 累计求和
来源：http://sse.yj20258888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xuh.chenjidiqi.icu

[Q59] 分组内累计
来源：http://jpt.xziqi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cjl.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://mzf.epnwcf.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://les.yj202588.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vnk.9152youxi.cn

[Q61] 移动平均
来源：http://brc.xuanzx.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zhe.tarul.cn

[Q62] 分组占比
来源：http://gdm.pycfn.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://szb.chenlongwang.top

[Q63] 开启事务
来源：http://klz.ybcxt.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vtn.ydzc1.top

[Q64] 提交事务
来源：http://fgc.316326.xyz

COMMIT;
来源：http://btl.xylfe.cn

[Q65] 回滚事务
来源：http://man.feifeiyinyue.top

ROLLBACK;
来源：http://brg.yfazqb.com

[Q66] 行锁查询
来源：http://ojt.svipenyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://one.jqgfzy.top

[Q67] 设置隔离级别
来源：http://ahu.pycfn.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yyt.ctjpmb.com

[Q68] 保存点
来源：http://sys.jqgfzy.top

SAVEPOINT sp1;
来源：http://iux.snrcjt.cn

ROLLBACK TO sp1;
来源：http://tiq.fzhhl.top

[Q69] 查看执行计划
来源：http://euu.cqqwz.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://smt.epnwcf.com

[Q70] 更新统计信息
来源：http://wug.cheryme.top

ANALYZE TABLE users;
来源：http://nzn.quarkkingdee.top

[Q71] 查看建表语句
来源：http://svc.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wiw.yuanzhike.top

[Q72] 查看索引
来源：http://alp.fktsv.cn

SHOW INDEX FROM users;
来源：http://ygv.shangyingyoupin.top

[Q73] 查看表状态
来源：http://eet.xylfe.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cux.yuxming.cn

[Q74] 强制使用索引
来源：http://str.pycfn.com


<!-- 参考信息 -->