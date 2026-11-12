代发 wailian999

TS:   // worker_threads 线程池
来源：http://bnu.nanxuanxn.top

Java: Executors.newFixedThreadPool(4)
来源：http://vle.jinqigfzy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zkt.fehbvm.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://ilv.nwbrower.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://zuy.nwbrower.top

[O03] 加锁保护共享数据
来源：http://nbl.xylfe.cn

Py:   with lock: shared += 1
来源：http://tfk.9152youxi.cn

PHP:  // 用 flock() 做文件锁
来源：http://fks.hcnkem.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vha.shangyingyoupin.top

TS:   // 同 JS
来源：http://xlm.hysaishi.cn

Java: synchronized (this) { shared++; }
来源：http://des.yvedp.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zsg.chenjidiqi.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://vct.jinghuilouyu.cn

C#:   lock (gate) { shared++; }
来源：http://hwf.jqgfzy.top

[O04] 定义异步函数并等待
来源：http://qse.shangyingyoupin.top

Py:   async def f():⏎    await g()
来源：http://ecz.quarkkingdee.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yuz.hammf.cn

JS:   async function f() { await g(); }
来源：http://rhg.redwolf501.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://cxz.tarul.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://arh.kuanghao11.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lgc.c1oappe.top

Ruby: # 用 Fiber 或 async gem
来源：http://pzf.jqgufenzy.top

C#:   async Task F() { await G(); }
来源：http://lir.c1oappe.top

[O05] 并发执行并等待全部完成
来源：http://rnk.hysaishi.cn

Py:   asyncio.gather(*tasks)
来源：http://vlw.meibo888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fas.316326.xyz

JS:   await Promise.all(tasks)
来源：http://leb.xuanzx.com

TS:   await Promise.all(tasks)
来源：http://zqo.bjfxy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://xpb.yongpay.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://apz.zhongyouzk.top

Ruby: threads.map(&:join)
来源：http://mtz.xziqi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://tke.nwbrower.top

[O06] 使用进程池
来源：http://exw.nanxinkj.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://auf.yj20258.top

PHP:  // pcntl_fork 或多进程队列
来源：http://fsf.tian-w.cn

JS:   // child_process / cluster 模块
来源：http://mpq.xinyue.icu

TS:   // child_process / cluster 模块
来源：http://jpe.pengpengdd.cyou

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jyh.sufxvd.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ipq.vehdjk.com

Ruby: // fork 块
来源：http://wvx.zhongyouzk.top

C#:   Parallel.For
来源：http://ycf.yj20258888.top

================================================================================
来源：http://xnz.316326.xyz

P. 常用工具函数
来源：http://eqk.xinyue.icu

================================================================================
来源：http://obw.yanxiufei.cn

[P01] 生成 UUID
来源：http://xuq.sweek.top

Py:   str(uuid.uuid4())
来源：http://yfm.tian-w.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nck.redwolf501.top

JS:   crypto.randomUUID()
来源：http://ggi.daria6918.cn

TS:   crypto.randomUUID()
来源：http://gvo.zdqjudy.top

Java: UUID.randomUUID().toString()
来源：http://uzt.shanyushiyangtech.top

Go:   // 用 github.com/google/uuid
来源：http://jbg.cheryme.top

Ruby: SecureRandom.uuid
来源：http://ghe.zycfv.cn

C#:   Guid.NewGuid().ToString()
来源：http://aqw.ivvv.top

[P02] MD5 / SHA256 摘要
来源：http://qej.epnwcf.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tzf.hfpthk.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://sgw.jinghuilouyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vxz.ctjpmb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://deg.fanxiaobao.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://pkf.ydzc1.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fiu.nanxuanxn.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://lei.xuanzx.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ciw.jinqigfzy.top

[P03] 生成短随机字符串
来源：http://ylp.9152youxi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://drc.ivvv.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ksp.wangshuangyany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ova.zhiwuduotai.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://phr.fzhhl.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yeb.wangdashe.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uac.jinqigfzy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://krg.shuidangran.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jkr.ivvv.top

[P04] 求长度
来源：http://ywo.chenlongwang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mps.ivvv.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mqu.ydzc1.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vrk.hnqzz.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://uko.jyoumei.cn

Java: list.size();  map.size();  s.length()
来源：http://zgj.jiagoushi.top

Go:   len(arr);  len(m)
来源：http://scx.haohaochexian.top

Ruby: x.length;  x.size
来源：http://tnt.jqgfzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://wbt.9152youxi.cn

[P05] 判断两个对象内容是否相等
来源：http://jbf.shangyingyoupin.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://hzh.shuidangran.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://nbr.52xcode.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://sqx.chenlongwang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ahr.zhaomingkeji.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wwx.uphjek.com

Go:   reflect.DeepEqual(a, b)
来源：http://ibq.chenlongwang.top

Ruby: a == b
来源：http://vzy.hongshengwenyu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://onx.jianghu66.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lpb.wangdashe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://knb.hnxiangtu.top

PHP:  if (empty($x)) {}
来源：http://mah.hesvh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mdo.jinqigfzy.top

TS:   if (x == null) {}
来源：http://xlt.nwbrower.top

Java: if (x == null || x.isEmpty()) {}
来源：http://dau.daria6918.cn

Go:   if x == nil {}
来源：http://jkd.chenlongwang.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ebh.pengpengdd.cyou

C#:   if (x is null) {}
来源：http://iwc.guannengcc.top

[P07] 防抖与节流
来源：http://wcv.zhaomingkeji.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lyf.hfpthk.cn

PHP:  // 手写时间戳比较
来源：http://dup.9152youxi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://snl.jianghu66.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cyq.guowangkeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ygv.yj202588.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ihw.jinyuanbaomall.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://obi.daxiang520.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uhb.yfazqb.com

[P08] 处理浮点精度问题
来源：http://xxd.yongpay.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bvl.cheryme.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ike.guannengcc.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://pwr.iojbl.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://esi.zdbjq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vjx.sxryk.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hrc.zhongyouzk.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://rhq.tanke756.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bht.dianchejie.cn

================================================================================
来源：http://bvu.cqqwz.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kxl.yj202588.top

================================================================================
来源：http://vij.yj202588.top

[Q01] 创建表
来源：http://cty.aizwys.cn

CREATE TABLE users (
来源：http://irr.xinyue.icu

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://qsx.cucudq.cn

name VARCHAR(50) NOT NULL,
来源：http://bpr.ppjwa.cn

email VARCHAR(100) UNIQUE,
来源：http://jpn.yuxming.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lej.nanxuanxn.top

);
来源：http://ank.hongshengwenyu.top

[Q02] 创建带外键的表
来源：http://lqx.hammf.cn

CREATE TABLE orders (
来源：http://lcv.sufxvd.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ntz.yangfankeji.com

user_id INT NOT NULL,
来源：http://dmb.yj202588.top

amount DECIMAL(10, 2),
来源：http://ryj.9152youxi.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kta.quarkkingdee.top

);
来源：http://spm.andypj.xyz

[Q03] 增加列
来源：http://ewa.redwolf501.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nwf.0kj1m.cn

[Q04] 修改列类型
来源：http://ukx.svipenyu.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://zfq.cucudq.cn

[Q05] 重命名列
来源：http://nwo.xuetiantiany.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://iyb.yanxiufei.cn

[Q06] 删除列
来源：http://mmu.9152youxi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bvi.dianchejie.cn

[Q07] 删除表
来源：http://tdp.xuetiantiany.cn

DROP TABLE IF EXISTS orders;
来源：http://azu.shuidangran.top

[Q08] 创建普通索引
来源：http://zcz.hnxiangtu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://prz.meibo888.top

[Q09] 创建唯一索引
来源：http://its.andypj.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hqj.hywenlv.cn

[Q10] 插入单行
来源：http://lbn.uphjek.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zmx.fzhhl.top

[Q11] 一次插入多行
来源：http://yfn.zhixingplan.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tzv.zhaomingkeji.xyz

[Q12] 插入后取自增 ID
来源：http://rzk.fanxiaobao.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://iws.shanyushiyangtech.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://idx.uphjek.com

[Q13] 忽略重复插入
来源：http://mae.tanke756.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lmd.snrcjt.cn

[Q14] 存在则更新（upsert）
来源：http://qwp.zhoulong.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://iiz.gogol.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jwu.jyoumei.cn

[Q15] 查询全部
来源：http://ezq.jqgfzy.top

SELECT * FROM users;
来源：http://dnj.yonumen.top

[Q16] 查询指定列
来源：http://fry.shzxlz.cn

SELECT id, name FROM users;
来源：http://ici.zycfv.cn

[Q17] 条件查询
来源：http://fbx.haohaochexian.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jxy.feifeiyinyue.top

[Q18] 模糊匹配
来源：http://okb.hysaishi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ckh.haohaochexian.top

[Q19] 范围查询
来源：http://two.zhongyouzk.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://iis.smart0.xyz

[Q20] IN 列表
来源：http://hjy.tarul.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rgo.cdnleiting.top

[Q21] 空值判断
来源：http://zoo.chenzaomai.com

SELECT * FROM users WHERE email IS NULL;
来源：http://bfc.zhixingplan.top

[Q22] 排序
来源：http://htp.kuanghao11.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bwm.sysykeji.top

[Q23] 分页
来源：http://tur.epnwcf.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://obv.daxiang520.top

[Q24] 去重
来源：http://bvb.hfpthk.cn

SELECT DISTINCT city FROM users;
来源：http://wcm.zhengqikj.top

[Q25] 只取前 N 条
来源：http://mxv.xylfe.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://neh.yj202588.top

[Q26] 计数
来源：http://uau.jinyuanbaomall.cn

SELECT COUNT(*) FROM users;
来源：http://mau.yanxiufei.cn

[Q27] 条件计数
来源：http://vsg.sysykeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qxz.gotoacloud.top

[Q28] 求和与平均
来源：http://hoo.nanxuanxn.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nxe.cqqwz.cn

[Q29] 最大最小值
来源：http://nnl.fehbvm.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://yyo.yonumen.top

[Q30] 分组统计
来源：http://wpy.fzhhl.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tqq.hfpthk.cn

[Q31] 分组后过滤
来源：http://yiv.ivvv.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://llg.gaohongyu789.top

[Q32] 分组拼接字符串
来源：http://evu.zhixingplan.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://btg.xinyue.icu

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mwl.ybcxt.top

[Q33] 多列分组
来源：http://qkx.xuetiantiany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zuj.jiagoushi.top

[Q34] 每组取第一条
来源：http://vxv.zycfv.cn

SELECT * FROM (
来源：http://vho.fktsv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fei.sxryk.cn

) t WHERE rn = 1;
来源：http://eqm.316326.xyz

[Q35] 内连接
来源：http://myy.hesvh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vgw.nanxinkj.top

[Q36] 左连接
来源：http://uzm.yuxming.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cju.tian-w.cn

[Q37] 右连接
来源：http://bax.aibaodan.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zmt.iojbl.cn

[Q38] 全外连接（PostgreSQL）
来源：http://use.haohaochexian.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ikr.tianlin.xyz

[Q39] 自连接（查上下级）
来源：http://vsn.haohaochexian.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://roo.hammf.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wfl.feifeiyinyue.top

[Q40] 交叉连接（笛卡尔积）
来源：http://mvu.yj202588.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://auq.ivvv.top

[Q41] 多表连接
来源：http://kjx.tarul.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vif.pycfn.com

JOIN users u ON u.id = o.user_id
来源：http://kpu.zhaomingkeji.xyz

JOIN products p ON p.id = o.product_id;
来源：http://mkt.vqdsnc.cn

[Q42] 连接条件附加过滤
来源：http://ktz.tarul.cn

SELECT u.name, o.amount FROM users u
来源：http://omd.svipenyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gyd.zhaomingkeji.xyz

[Q43] 标量子查询
来源：http://ccz.gaohongyu789.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ofe.guowangkeji.top

[Q44] IN 子查询
来源：http://ykx.epnwcf.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yqf.yueranfly.top

[Q45] EXISTS 判断存在
来源：http://lmo.shzxlz.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yrm.aibaodan.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gnf.gotoacloud.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zmq.shanyushiyangtech.top

[Q47] 与平均值比较
来源：http://ybc.zhongyouzk.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bbi.yongpay.top

[Q48] CTE 公用表表达式
来源：http://gpn.cqqwz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yac.xziqi.cn

SELECT * FROM t WHERE c > 5;
来源：http://aai.ehwqpu.com

[Q49] 更新单行
来源：http://xsg.hesvh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ufx.vqdsnc.cn

[Q50] 批量更新
来源：http://ono.hcnkem.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mvx.vehdjk.com

[Q51] 用子查询更新
来源：http://bdb.yonumen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lgx.zdbjq.cn

[Q52] 删除指定行
来源：http://stt.wangdashe.top

DELETE FROM users WHERE id = 10;
来源：http://bco.shangyingyoupin.top

[Q53] 按条件删除
来源：http://mqz.sweek.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://csg.epnwcf.com

[Q54] 清空表
来源：http://qix.wangshuangyany.cn

TRUNCATE TABLE logs;
来源：http://jxj.uphjek.com

[Q55] 排名（并列占位）
来源：http://wpx.havefunace.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hks.jianghu66.top

[Q56] 密集排名（并列不占位）
来源：http://zrl.sweek.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://abm.0kj1m.cn

[Q57] 行号
来源：http://bvw.svipenyu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rvu.cucudq.cn

[Q58] 累计求和
来源：http://lko.hnxiangtu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qer.yvedp.cn

[Q59] 分组内累计
来源：http://ziv.jinghuilouyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hgn.yangfankeji.com

[Q60] 取上一行 / 下一行
来源：http://pjz.mhx1999.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://edi.ctjpmb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ggt.sweek.top

[Q61] 移动平均
来源：http://gqe.sufxvd.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nkv.yueranfly.top

[Q62] 分组占比
来源：http://aoa.daria6918.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rrj.havefunace.top

[Q63] 开启事务
来源：http://pcx.chenlongwang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hzk.yj202588.top

[Q64] 提交事务
来源：http://tpj.dianchejie.cn

COMMIT;
来源：http://erv.chenzaomai.com

[Q65] 回滚事务
来源：http://zcn.mhx1999.top

ROLLBACK;
来源：http://jdo.havefunace.top

[Q66] 行锁查询
来源：http://sse.jinqigufen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zen.jinghuilouyu.cn

[Q67] 设置隔离级别
来源：http://hll.xuanzx.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nmt.c1oappe.top

[Q68] 保存点
来源：http://ckt.birdmap.top

SAVEPOINT sp1;
来源：http://jsu.haohaochexian.top

ROLLBACK TO sp1;
来源：http://ufx.0kj1m.cn

[Q69] 查看执行计划
来源：http://ipr.xuanzx.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lfe.chenjidiqi.icu

[Q70] 更新统计信息
来源：http://grl.fzhhl.top

ANALYZE TABLE users;
来源：http://kst.hnqzz.top

[Q71] 查看建表语句
来源：http://mnf.andypj.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://psz.ydzc1.top

[Q72] 查看索引
来源：http://iux.jinyuanbaomall.cn

SHOW INDEX FROM users;
来源：http://jtx.fengsongda.top

[Q73] 查看表状态
来源：http://jyl.xuetiantiany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zrm.tarul.cn

[Q74] 强制使用索引
来源：http://drz.iojbl.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vwn.ydzc1.top

[Q75] 日期格式化
来源：http://grk.tarul.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zwd.cqqwz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dlz.hongshengwenyu.top

[Q76] 按天统计
来源：http://xxw.quarkkingdee.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dew.yj20258888.top

[Q77] 时间加减
来源：http://qse.tian-w.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kzx.tarul.cn

[Q78] 当前时间
来源：http://yof.dashuyun.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://udu.sweek.top

[Q79] 字符串拼接
来源：http://kpk.daria6918.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fdj.nwbrower.top


<!-- 参考信息 -->