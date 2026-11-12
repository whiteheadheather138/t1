代发 wailian999

[O02] 使用线程池
来源：http://rcx.jinqigfzy.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ppb.mhx1999.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cok.yj202588.top

JS:   // worker_threads 线程池
来源：http://ixb.zhengqikj.top

TS:   // worker_threads 线程池
来源：http://wss.yonumen.top

Java: Executors.newFixedThreadPool(4)
来源：http://uks.quarkkingdee.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kbh.xinyue.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://twb.hnqzz.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wtc.ctjpmb.com

[O03] 加锁保护共享数据
来源：http://obn.ivvv.top

Py:   with lock: shared += 1
来源：http://dso.wangdashe.top

PHP:  // 用 flock() 做文件锁
来源：http://abo.havefunace.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://meq.316326.xyz

TS:   // 同 JS
来源：http://klg.havefunace.top

Java: synchronized (this) { shared++; }
来源：http://yzn.hnxiangtu.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lcq.pengpengdd.cyou

Ruby: mutex.synchronize { shared += 1 }
来源：http://fiw.hysaishi.cn

C#:   lock (gate) { shared++; }
来源：http://ejf.havefunace.top

[O04] 定义异步函数并等待
来源：http://xcx.kuanghao11.cn

Py:   async def f():⏎    await g()
来源：http://ctr.chenzaomai.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hjo.pycfn.com

JS:   async function f() { await g(); }
来源：http://ciw.shanyushiyangkeji.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://voy.yonumen.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xag.316326.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qoy.chenjidiqi.icu

Ruby: # 用 Fiber 或 async gem
来源：http://icz.xziqi.cn

C#:   async Task F() { await G(); }
来源：http://obn.52xcode.cn

[O05] 并发执行并等待全部完成
来源：http://tus.nwbrower.top

Py:   asyncio.gather(*tasks)
来源：http://hpq.gotoacloud.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jdk.ybcxt.top

JS:   await Promise.all(tasks)
来源：http://fnr.kuanghao11.cn

TS:   await Promise.all(tasks)
来源：http://wrn.fengsongda.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://tyj.zycfv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mon.chenlongwang.top

Ruby: threads.map(&:join)
来源：http://jtm.yuxming.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://nai.ctjpmb.com

[O06] 使用进程池
来源：http://tef.wangdashe.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jzv.0kj1m.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://uhx.hongshengwenyu.top

JS:   // child_process / cluster 模块
来源：http://jsv.ivvv.top

TS:   // child_process / cluster 模块
来源：http://sdx.mhx1999.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yau.hysaishi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cys.yj20258.top

Ruby: // fork 块
来源：http://sjk.hfpthk.cn

C#:   Parallel.For
来源：http://sll.xingfuxueyuan.xyz

================================================================================
来源：http://fhz.dashuyun.cn

P. 常用工具函数
来源：http://gxq.fengsongda.top

================================================================================
来源：http://fxt.shanyushiyangtech.top

[P01] 生成 UUID
来源：http://ihv.redwolf501.top

Py:   str(uuid.uuid4())
来源：http://mbo.uphjek.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xyk.fengsongda.top

JS:   crypto.randomUUID()
来源：http://kvx.zhixingplan.top

TS:   crypto.randomUUID()
来源：http://chb.hcnkem.com

Java: UUID.randomUUID().toString()
来源：http://jof.52xcode.cn

Go:   // 用 github.com/google/uuid
来源：http://dem.bbcook.cn

Ruby: SecureRandom.uuid
来源：http://vve.zdbjq.cn

C#:   Guid.NewGuid().ToString()
来源：http://axc.cdnleiting.top

[P02] MD5 / SHA256 摘要
来源：http://ptf.yj202588.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://beh.guowangkeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jzr.cashguo.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rcl.hammf.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://skn.smart0.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rei.vqdsnc.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qhz.jqgufenzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rzl.sufxvd.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://uwz.haohaochexian.top

[P03] 生成短随机字符串
来源：http://drc.9152youxi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pbn.hammf.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ntc.xuetiantiany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sfx.cqqwz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yoe.smart0.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yhu.9152youxi.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ckf.fanxiaobao.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://exx.jianghu66.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xoc.dashuyun.cn

[P04] 求长度
来源：http://phf.xinyue.icu

Py:   len(x)            # 字符串、列表、字典通用
来源：http://niy.zycfv.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pwl.mhx1999.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://erp.yangfankeji.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tjt.hongshengwenyu.top

Java: list.size();  map.size();  s.length()
来源：http://mtf.zhaomingkeji.xyz

Go:   len(arr);  len(m)
来源：http://vcw.xuetiantiany.cn

Ruby: x.length;  x.size
来源：http://cxc.gzhubu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ovr.epnwcf.com

[P05] 判断两个对象内容是否相等
来源：http://dgb.yuanzhike.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://tcs.guowangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bjq.jqgufenzy.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ney.svipenyu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lsr.hnxiangtu.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pcn.fktsv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://sid.sxryk.cn

Ruby: a == b
来源：http://zmb.ybcxt.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gqf.xuanzx.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tfo.yueranfly.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lda.wangdashe.top

PHP:  if (empty($x)) {}
来源：http://hsh.zhengqikj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uxm.zhengqikj.top

TS:   if (x == null) {}
来源：http://dxf.sweek.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fpo.tanke756.top

Go:   if x == nil {}
来源：http://iik.aizwys.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nrv.shanyushiyangtech.top

C#:   if (x is null) {}
来源：http://tio.cqqwz.cn

[P07] 防抖与节流
来源：http://ttw.chenzaomai.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://tqt.yj202588.top

PHP:  // 手写时间戳比较
来源：http://jeo.hysaishi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gjb.sjlbkw.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ptv.jqgfzy.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dua.pengpengdd.cyou

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://agl.jinghuilouyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xeu.shanyushiyangkeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qcj.fehbvm.com

[P08] 处理浮点精度问题
来源：http://hym.hammf.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yod.tianlin.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xyg.shangyingyoupin.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://via.iojbl.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://otz.wangdashe.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nky.fanxiaobao.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zzw.yangfankeji.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nzx.yonumen.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mze.cucudq.cn

================================================================================
来源：http://lrl.sjlbkw.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://osj.hnxiangtu.top

================================================================================
来源：http://yft.yangfankeji.com

[Q01] 创建表
来源：http://xqc.fzhhl.top

CREATE TABLE users (
来源：http://ony.smart0.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ogr.yangfankeji.com

name VARCHAR(50) NOT NULL,
来源：http://czc.birdmap.top

email VARCHAR(100) UNIQUE,
来源：http://aqv.xziqi.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vnr.52xcode.cn

);
来源：http://rvh.hesvh.cn

[Q02] 创建带外键的表
来源：http://bds.jqgfzy.top

CREATE TABLE orders (
来源：http://ugw.xingfuxueyuan.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jqd.yj202588.top

user_id INT NOT NULL,
来源：http://jms.shzxlz.cn

amount DECIMAL(10, 2),
来源：http://myf.ydzc1.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vyt.birdmap.top

);
来源：http://nep.jqgufenzy.top

[Q03] 增加列
来源：http://jlz.hysaishi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://keh.sxryk.cn

[Q04] 修改列类型
来源：http://uxf.wangdashe.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gqh.jqgfzy.top

[Q05] 重命名列
来源：http://hhr.epnwcf.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ivm.hammf.cn

[Q06] 删除列
来源：http://rty.zhongyouzk.top

ALTER TABLE users DROP COLUMN age;
来源：http://rjk.zhixingplan.top

[Q07] 删除表
来源：http://dbk.fzhhl.top

DROP TABLE IF EXISTS orders;
来源：http://nav.mhx1999.top

[Q08] 创建普通索引
来源：http://ggp.xingfuxueyuan.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://vmu.pengpengdd.cyou

[Q09] 创建唯一索引
来源：http://lmm.epnwcf.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ofb.aibaodan.cn

[Q10] 插入单行
来源：http://ndv.yfazqb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://byo.chenlongwang.top

[Q11] 一次插入多行
来源：http://ryt.sufxvd.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mfc.hfpthk.cn

[Q12] 插入后取自增 ID
来源：http://koc.hnqzz.top

INSERT INTO users (name) VALUES ('C');
来源：http://vrd.9152youxi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uye.ydzc1.top

[Q13] 忽略重复插入
来源：http://pin.birdmap.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mrc.nanxuanxn.top

[Q14] 存在则更新（upsert）
来源：http://bjk.yvedp.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lpl.fengsongda.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jyw.ehwqpu.com

[Q15] 查询全部
来源：http://wlq.sysykeji.top

SELECT * FROM users;
来源：http://eux.xuanzx.com

[Q16] 查询指定列
来源：http://ytf.zhoulong.xyz

SELECT id, name FROM users;
来源：http://nay.dianchejie.cn

[Q17] 条件查询
来源：http://ezz.chenjidiqi.icu

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://duw.cqqwz.cn

[Q18] 模糊匹配
来源：http://jch.yj20258.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xjr.zdbjq.cn

[Q19] 范围查询
来源：http://qvy.redwolf501.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://twg.yonumen.top

[Q20] IN 列表
来源：http://ryg.yongpay.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://chu.xylfe.cn

[Q21] 空值判断
来源：http://vnb.epnwcf.com

SELECT * FROM users WHERE email IS NULL;
来源：http://rfw.jiagoushi.top

[Q22] 排序
来源：http://obp.zhengqikj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jvx.tanke756.top

[Q23] 分页
来源：http://edz.sweek.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kow.feifeiyinyue.top

[Q24] 去重
来源：http://lqo.shanyushiyangkeji.top

SELECT DISTINCT city FROM users;
来源：http://ybv.vehdjk.com

[Q25] 只取前 N 条
来源：http://mvz.jinqigufen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sqk.quarkkingdee.top

[Q26] 计数
来源：http://czt.gotoacloud.top

SELECT COUNT(*) FROM users;
来源：http://wkj.gotoacloud.top

[Q27] 条件计数
来源：http://psc.xuetiantiany.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tky.sxryk.cn

[Q28] 求和与平均
来源：http://hht.smart0.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://him.jinqigufen.top

[Q29] 最大最小值
来源：http://xeb.hnqzz.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ubr.ivvv.top

[Q30] 分组统计
来源：http://szt.ppjwa.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vgf.jinqigfzy.top

[Q31] 分组后过滤
来源：http://vlb.yj20258888.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://enp.xuanzx.com

[Q32] 分组拼接字符串
来源：http://avw.ctjpmb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://apz.guowangkeji.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xjb.cucudq.cn

[Q33] 多列分组
来源：http://epz.daxiang520.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fzy.epnwcf.com

[Q34] 每组取第一条
来源：http://flv.quarkkingdee.top

SELECT * FROM (
来源：http://odg.zhoulong.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vzp.9152youxi.cn

) t WHERE rn = 1;
来源：http://tyz.redwolf501.top

[Q35] 内连接
来源：http://plm.svipenyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://miq.zhijiandao.cn

[Q36] 左连接
来源：http://spf.jqgfzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ogw.zhaomingkeji.xyz

[Q37] 右连接
来源：http://lll.wangshuangyany.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vwt.jinghuilouyu.cn

[Q38] 全外连接（PostgreSQL）
来源：http://noc.yj202588.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cvg.jqgufenzy.top

[Q39] 自连接（查上下级）
来源：http://raa.ppjwa.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xbo.hesvh.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kut.zycfv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kwx.cdnleiting.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kmm.sweek.top

[Q41] 多表连接
来源：http://xsf.haohaochexian.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://enf.ppjwa.cn

JOIN users u ON u.id = o.user_id
来源：http://phu.jinghuilouyu.cn

JOIN products p ON p.id = o.product_id;
来源：http://rnc.yfazqb.com

[Q42] 连接条件附加过滤
来源：http://lll.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://dfh.sxryk.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gen.tianlin.xyz

[Q43] 标量子查询
来源：http://xnz.cucudq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kla.hnxiangtu.top

[Q44] IN 子查询
来源：http://rzf.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qwi.shangyingyoupin.top

[Q45] EXISTS 判断存在
来源：http://bzg.havefunace.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ism.epnwcf.com

[Q46] NOT EXISTS 判断不存在
来源：http://ldy.zhaomingkeji.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sfm.shanyushiyangkeji.top

[Q47] 与平均值比较
来源：http://vma.daxiang520.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kvo.epnwcf.com

[Q48] CTE 公用表表达式
来源：http://yxi.jinqigfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xky.tian-w.cn

SELECT * FROM t WHERE c > 5;
来源：http://olz.zhongyouzk.top

[Q49] 更新单行
来源：http://yeo.hywenlv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mzg.yonumen.top

[Q50] 批量更新
来源：http://rry.sjlbkw.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://htp.snrcjt.cn

[Q51] 用子查询更新
来源：http://bxa.hnxiangtu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cxc.hnxiangtu.top

[Q52] 删除指定行
来源：http://lbv.vehdjk.com

DELETE FROM users WHERE id = 10;
来源：http://knr.yuanzhike.top

[Q53] 按条件删除
来源：http://jfo.hongshengwenyu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://asa.yongpay.top

[Q54] 清空表
来源：http://ito.yj202588.top

TRUNCATE TABLE logs;
来源：http://ebi.tian-w.cn

[Q55] 排名（并列占位）
来源：http://vez.jinghuilouyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fgh.jlsjyb.cn

[Q56] 密集排名（并列不占位）
来源：http://kuf.cqqwz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://enp.bbcook.cn

[Q57] 行号
来源：http://kwu.quarkkingdee.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://srd.yueranfly.top

[Q58] 累计求和
来源：http://wdz.jinghuilouyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://acq.aibaodan.cn

[Q59] 分组内累计
来源：http://bcs.sweek.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fin.zhiwuduotai.top

[Q60] 取上一行 / 下一行
来源：http://zrk.aibaodan.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yjq.daria6918.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jnu.zhengqikj.top

[Q61] 移动平均
来源：http://igv.shanyushiyangtech.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://egq.ehwqpu.com

[Q62] 分组占比
来源：http://koh.kuanghao11.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://aky.dashuyun.cn

[Q63] 开启事务
来源：http://bkh.fktsv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://utt.gogol.net.cn

[Q64] 提交事务
来源：http://kuv.bjfxy.top

COMMIT;
来源：http://hzf.ydjk.org.cn

[Q65] 回滚事务
来源：http://upf.yj20258.top

ROLLBACK;
来源：http://ggg.hcnkem.com

[Q66] 行锁查询
来源：http://syt.nanxuanxn.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pho.yangfankeji.com

[Q67] 设置隔离级别
来源：http://tkh.jqgfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bip.cqqwz.cn

[Q68] 保存点
来源：http://qzx.ydzc1.top

SAVEPOINT sp1;
来源：http://iwl.hammf.cn

ROLLBACK TO sp1;
来源：http://aod.c1oappe.top

[Q69] 查看执行计划
来源：http://vjh.xingfuxueyuan.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gnq.andypj.xyz

[Q70] 更新统计信息
来源：http://swr.xuanzx.com

ANALYZE TABLE users;
来源：http://gzq.zhaomingkeji.xyz

[Q71] 查看建表语句
来源：http://qrw.gogol.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kij.gotoacloud.top

[Q72] 查看索引
来源：http://rnt.wangshuangyany.cn

SHOW INDEX FROM users;
来源：http://osy.yuanzhike.top

[Q73] 查看表状态
来源：http://fmr.chenjidiqi.icu

SHOW TABLE STATUS LIKE 'users';
来源：http://inv.fanxiaobao.xyz

[Q74] 强制使用索引
来源：http://pub.yuxming.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zbb.andypj.xyz

[Q75] 日期格式化
来源：http://zzh.zdqjudy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kde.andypj.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uav.smart0.xyz

[Q76] 按天统计
来源：http://msd.ppjwa.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pmx.pycfn.com

[Q77] 时间加减
来源：http://dth.cheryme.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pyd.316326.xyz


<!-- 参考信息 -->