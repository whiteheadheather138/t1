代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://egx.haohaochexian.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://ynr.vqdsnc.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://uah.pengpengdd.cyou

TS:   // 同 JS
来源：http://uwt.sufxvd.cn

Java: new Thread(() -> f()).start()
来源：http://hzu.fengsongda.top

Go:   go f()
来源：http://qin.wangdashe.top

Ruby: Thread.new { f }
来源：http://wsb.cdnleiting.top

C#:   Task.Run(() => F());
来源：http://pot.nwbrower.top

[O02] 使用线程池
来源：http://gvk.redwolf501.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yqj.yuanzhike.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://lat.xingfuxueyuan.xyz

JS:   // worker_threads 线程池
来源：http://ups.guannengcc.top

TS:   // worker_threads 线程池
来源：http://fet.nwbrower.top

Java: Executors.newFixedThreadPool(4)
来源：http://dhj.yuxming.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://grf.hammf.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://fqc.smart0.xyz

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wbu.yonumen.top

[O03] 加锁保护共享数据
来源：http://giu.9152youxi.cn

Py:   with lock: shared += 1
来源：http://cob.dianchejie.cn

PHP:  // 用 flock() 做文件锁
来源：http://szm.sxryk.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zzc.wangshuangyany.cn

TS:   // 同 JS
来源：http://bze.ydjk.org.cn

Java: synchronized (this) { shared++; }
来源：http://aal.zhongyouzk.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vgf.jianghu66.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://uqw.9152youxi.cn

C#:   lock (gate) { shared++; }
来源：http://wdk.guowangkeji.top

[O04] 定义异步函数并等待
来源：http://tos.yj202588.top

Py:   async def f():⏎    await g()
来源：http://zyn.tanke756.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yjf.hfpthk.cn

JS:   async function f() { await g(); }
来源：http://cbu.bjfxy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pif.uphjek.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rnd.pengpengdd.cyou

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gep.gzhubu.top

Ruby: # 用 Fiber 或 async gem
来源：http://eff.sjlbkw.cn

C#:   async Task F() { await G(); }
来源：http://hyr.yvedp.cn

[O05] 并发执行并等待全部完成
来源：http://dil.cdnleiting.top

Py:   asyncio.gather(*tasks)
来源：http://olk.cashguo.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://sde.zhoulong.xyz

JS:   await Promise.all(tasks)
来源：http://gsu.uphjek.com

TS:   await Promise.all(tasks)
来源：http://lum.yueranfly.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mbc.quarkkingdee.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jys.ehwqpu.com

Ruby: threads.map(&:join)
来源：http://evr.yj20258.top

C#:   await Task.WhenAll(t1, t2)
来源：http://yls.hongshengwenyu.top

[O06] 使用进程池
来源：http://qle.sysykeji.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cee.quarkkingdee.top

PHP:  // pcntl_fork 或多进程队列
来源：http://joj.ppjwa.cn

JS:   // child_process / cluster 模块
来源：http://llm.shuidangran.top

TS:   // child_process / cluster 模块
来源：http://dyd.ctjpmb.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rnk.jinghuilouyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xtb.jlsjyb.cn

Ruby: // fork 块
来源：http://cis.shanyushiyangtech.top

C#:   Parallel.For
来源：http://typ.pycfn.com

================================================================================
来源：http://uhd.jqgufenzy.top

P. 常用工具函数
来源：http://wjk.chenzaomai.com

================================================================================
来源：http://suf.wangshuangyany.cn

[P01] 生成 UUID
来源：http://mkx.cqqwz.cn

Py:   str(uuid.uuid4())
来源：http://qmq.xuanzx.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fdy.yonumen.top

JS:   crypto.randomUUID()
来源：http://svh.cdnleiting.top

TS:   crypto.randomUUID()
来源：http://xzx.mhx1999.top

Java: UUID.randomUUID().toString()
来源：http://uif.wangshuangyany.cn

Go:   // 用 github.com/google/uuid
来源：http://dqq.yangfankeji.com

Ruby: SecureRandom.uuid
来源：http://lir.fengsongda.top

C#:   Guid.NewGuid().ToString()
来源：http://ajs.birdmap.top

[P02] MD5 / SHA256 摘要
来源：http://frk.nanxinkj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wqr.svipenyu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://jjt.jinqigfzy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xbl.fzhhl.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://epf.zhijiandao.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gsi.haohaochexian.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nbs.hammf.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lus.feifeiyinyue.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://emu.zhaomingkeji.xyz

[P03] 生成短随机字符串
来源：http://xgs.cashguo.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ibd.zdqjudy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wfd.jqgufenzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mqu.sysykeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bsj.zycfv.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://aay.hysaishi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://bng.yongpay.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://idl.tarul.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ddg.ydzc1.top

[P04] 求长度
来源：http://nlb.chenlongwang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mvg.fengsongda.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jhg.yongpay.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nre.fanxiaobao.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oyp.zdqjudy.top

Java: list.size();  map.size();  s.length()
来源：http://bsb.redwolf501.top

Go:   len(arr);  len(m)
来源：http://kdz.andypj.xyz

Ruby: x.length;  x.size
来源：http://bhj.haohaochexian.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://skp.ydjk.org.cn

[P05] 判断两个对象内容是否相等
来源：http://cyb.bbcook.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://osv.jinqigufen.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zip.yueranfly.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ijq.yuanzhike.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://yso.nwbrower.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://atw.hywenlv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fdo.yuxming.cn

Ruby: a == b
来源：http://xos.daria6918.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ceq.chenzaomai.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gje.havefunace.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vzt.ydzc1.top

PHP:  if (empty($x)) {}
来源：http://vnk.jinghuilouyu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qlh.chenlongwang.top

TS:   if (x == null) {}
来源：http://jpp.yj20258888.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kpx.nanxuanxn.top

Go:   if x == nil {}
来源：http://jfa.iojbl.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://byr.yuxming.cn

C#:   if (x is null) {}
来源：http://qnm.yueranfly.top

[P07] 防抖与节流
来源：http://had.cucudq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://gcf.shanyushiyangkeji.top

PHP:  // 手写时间戳比较
来源：http://xwj.hesvh.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nuw.tian-w.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pby.yangfankeji.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wat.fengsongda.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ctl.jinqigufen.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://jok.hnqzz.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uia.ivvv.top

[P08] 处理浮点精度问题
来源：http://ncf.gzhubu.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qjf.zhixingplan.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jug.ctjpmb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://yac.dianchejie.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://afo.havefunace.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://msy.yueranfly.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://isr.smart0.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wge.zhijiandao.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wik.daria6918.cn

================================================================================
来源：http://snm.fzhhl.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://tfc.hfpthk.cn

================================================================================
来源：http://jru.0kj1m.cn

[Q01] 创建表
来源：http://jow.cdnleiting.top

CREATE TABLE users (
来源：http://dtn.fktsv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lkm.shangyingyoupin.top

name VARCHAR(50) NOT NULL,
来源：http://zhd.ybcxt.top

email VARCHAR(100) UNIQUE,
来源：http://gbe.jianghu66.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ino.yonumen.top

);
来源：http://sny.yangfankeji.com

[Q02] 创建带外键的表
来源：http://ygc.vehdjk.com

CREATE TABLE orders (
来源：http://pyq.daxiang520.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://srb.dianchejie.cn

user_id INT NOT NULL,
来源：http://cnw.guannengcc.top

amount DECIMAL(10, 2),
来源：http://lwi.tarul.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qzn.52xcode.cn

);
来源：http://tww.ppjwa.cn

[Q03] 增加列
来源：http://gfy.hammf.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://sam.9152youxi.cn

[Q04] 修改列类型
来源：http://yyo.chenlongwang.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lyf.sysykeji.top

[Q05] 重命名列
来源：http://hxe.xziqi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xmh.andypj.xyz

[Q06] 删除列
来源：http://uez.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://bjr.9152youxi.cn

[Q07] 删除表
来源：http://grn.xuanzx.com

DROP TABLE IF EXISTS orders;
来源：http://ttr.jianghu66.top

[Q08] 创建普通索引
来源：http://xzl.feifeiyinyue.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jdm.havefunace.top

[Q09] 创建唯一索引
来源：http://nlx.dianchejie.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://xbi.zycfv.cn

[Q10] 插入单行
来源：http://dzr.sysykeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zai.pycfn.com

[Q11] 一次插入多行
来源：http://vkf.tian-w.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zre.meibo888.top

[Q12] 插入后取自增 ID
来源：http://vpt.nanxuanxn.top

INSERT INTO users (name) VALUES ('C');
来源：http://twp.andypj.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ldf.chenjidiqi.icu

[Q13] 忽略重复插入
来源：http://lmf.0kj1m.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ypk.cdnleiting.top

[Q14] 存在则更新（upsert）
来源：http://pfd.zhijiandao.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jst.hnxiangtu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qnj.jyoumei.cn

[Q15] 查询全部
来源：http://wbm.haohaochexian.top

SELECT * FROM users;
来源：http://fda.zhiwuduotai.top

[Q16] 查询指定列
来源：http://flm.yfazqb.com

SELECT id, name FROM users;
来源：http://cap.birdmap.top

[Q17] 条件查询
来源：http://lqe.yfazqb.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://fgm.jqgufenzy.top

[Q18] 模糊匹配
来源：http://mwy.daria6918.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yfv.daria6918.cn

[Q19] 范围查询
来源：http://syj.hongshengwenyu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qke.dianchejie.cn

[Q20] IN 列表
来源：http://gaq.jqgufenzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vpp.gaohongyu789.top

[Q21] 空值判断
来源：http://ajk.tian-w.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lxy.sufxvd.cn

[Q22] 排序
来源：http://kya.ppjwa.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ykb.fengsongda.top

[Q23] 分页
来源：http://jrj.chenzaomai.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://epu.daxiang520.top

[Q24] 去重
来源：http://ywk.yuanzhike.top

SELECT DISTINCT city FROM users;
来源：http://vtw.feifeiyinyue.top

[Q25] 只取前 N 条
来源：http://mgt.vehdjk.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://orj.iojbl.cn

[Q26] 计数
来源：http://rkd.yvedp.cn

SELECT COUNT(*) FROM users;
来源：http://fzw.chenjidiqi.icu

[Q27] 条件计数
来源：http://lyq.nwbrower.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jsv.yuxming.cn

[Q28] 求和与平均
来源：http://eob.nanxuanxn.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vvb.sufxvd.cn

[Q29] 最大最小值
来源：http://lpd.wangshuangyany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pll.iojbl.cn

[Q30] 分组统计
来源：http://bab.cdnleiting.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cxq.wangdashe.top

[Q31] 分组后过滤
来源：http://zse.bbcook.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://abq.zycfv.cn

[Q32] 分组拼接字符串
来源：http://sgg.guannengcc.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://men.zdbjq.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://iin.ctjpmb.com

[Q33] 多列分组
来源：http://ftn.epnwcf.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vlx.zycfv.cn

[Q34] 每组取第一条
来源：http://iao.xinyue.icu

SELECT * FROM (
来源：http://mkk.vehdjk.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zpf.hysaishi.cn

) t WHERE rn = 1;
来源：http://oku.shangyingyoupin.top

[Q35] 内连接
来源：http://zqz.gogol.net.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gdy.yj20258888.top

[Q36] 左连接
来源：http://blk.cheryme.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xpf.yj202588.top

[Q37] 右连接
来源：http://xff.tian-w.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tul.epnwcf.com

[Q38] 全外连接（PostgreSQL）
来源：http://cxx.daria6918.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kjl.yangfankeji.com

[Q39] 自连接（查上下级）
来源：http://ytg.zhongyouzk.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://onf.cheryme.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cas.ybcxt.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qjr.fengsongda.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vlz.yfazqb.com

[Q41] 多表连接
来源：http://hxi.c1oappe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ise.hnqzz.top

JOIN users u ON u.id = o.user_id
来源：http://bix.cheryme.top

JOIN products p ON p.id = o.product_id;
来源：http://dlr.jianghu66.top

[Q42] 连接条件附加过滤
来源：http://ipa.zdqjudy.top

SELECT u.name, o.amount FROM users u
来源：http://lyk.shanyushiyangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qjs.zhengqikj.top

[Q43] 标量子查询
来源：http://gpr.ehwqpu.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yaj.pycfn.com

[Q44] IN 子查询
来源：http://utk.jinqigfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gbr.yj20258.top

[Q45] EXISTS 判断存在
来源：http://uap.havefunace.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jmx.yuxming.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wln.nwbrower.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lkp.yj20258.top

[Q47] 与平均值比较
来源：http://ivz.jinghuilouyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pty.gogol.net.cn

[Q48] CTE 公用表表达式
来源：http://ulg.guannengcc.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tcc.jinghuilouyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://ozk.hnxiangtu.top

[Q49] 更新单行
来源：http://eko.hnxiangtu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dvg.jinyuanbaomall.cn

[Q50] 批量更新
来源：http://yqz.svipenyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dnb.zhixingplan.top

[Q51] 用子查询更新
来源：http://yqw.ywan-chungtsiang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jqx.cucudq.cn

[Q52] 删除指定行
来源：http://bge.aizwys.cn

DELETE FROM users WHERE id = 10;
来源：http://bof.yongpay.top

[Q53] 按条件删除
来源：http://thg.hnxiangtu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hvc.epnwcf.com

[Q54] 清空表
来源：http://ext.snrcjt.cn

TRUNCATE TABLE logs;
来源：http://xge.andypj.xyz

[Q55] 排名（并列占位）
来源：http://sbh.fanxiaobao.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xqt.cashguo.top

[Q56] 密集排名（并列不占位）
来源：http://yvl.hysaishi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kjv.9152youxi.cn

[Q57] 行号
来源：http://wbi.ppjwa.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://puo.gzhubu.top

[Q58] 累计求和
来源：http://tnk.yueranfly.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lhq.ybcxt.top

[Q59] 分组内累计
来源：http://fvc.yj202588.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wzt.xylfe.cn

[Q60] 取上一行 / 下一行
来源：http://ldm.cheryme.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://opr.redwolf501.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xri.guowangkeji.top

[Q61] 移动平均
来源：http://wta.jinyuanbaomall.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://sum.yfazqb.com

[Q62] 分组占比
来源：http://fkf.tianlin.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://aph.c1oappe.top

[Q63] 开启事务
来源：http://aof.yuanzhike.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rxk.jqgfzy.top

[Q64] 提交事务
来源：http://sta.xuetiantiany.cn

COMMIT;
来源：http://exy.ctjpmb.com

[Q65] 回滚事务
来源：http://civ.hfpthk.cn

ROLLBACK;
来源：http://mkj.nwbrower.top

[Q66] 行锁查询
来源：http://dwf.sjlbkw.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rwl.wangdashe.top

[Q67] 设置隔离级别
来源：http://zzg.zhixingplan.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ziq.c1oappe.top

[Q68] 保存点
来源：http://fnv.yangfankeji.com

SAVEPOINT sp1;
来源：http://ffw.zdqjudy.top

ROLLBACK TO sp1;
来源：http://qnn.yonumen.top

[Q69] 查看执行计划
来源：http://vfi.mhx1999.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vmr.zhaomingkeji.xyz

[Q70] 更新统计信息
来源：http://gfr.wangshuangyany.cn

ANALYZE TABLE users;
来源：http://sgx.shangyingyoupin.top

[Q71] 查看建表语句
来源：http://eub.feifeiyinyue.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tdz.jyoumei.cn

[Q72] 查看索引
来源：http://qci.shzxlz.cn

SHOW INDEX FROM users;
来源：http://dwk.quarkkingdee.top

[Q73] 查看表状态
来源：http://abs.yuxming.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ncx.hammf.cn

[Q74] 强制使用索引
来源：http://cca.nanxinkj.top


<!-- 参考信息 -->