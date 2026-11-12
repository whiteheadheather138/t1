代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://noz.xingfuxueyuan.xyz

Go:   go f()
来源：http://xpr.tianlin.xyz

Ruby: Thread.new { f }
来源：http://clf.jinqigufen.top

C#:   Task.Run(() => F());
来源：http://map.fehbvm.com

[O02] 使用线程池
来源：http://efc.sjlbkw.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://yrx.wangdashe.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://vgc.zhoulong.xyz

JS:   // worker_threads 线程池
来源：http://mfu.pycfn.com

TS:   // worker_threads 线程池
来源：http://eps.chenzaomai.com

Java: Executors.newFixedThreadPool(4)
来源：http://gbq.hysaishi.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kph.meibo888.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xsj.hnqzz.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ynq.guannengcc.top

[O03] 加锁保护共享数据
来源：http://xfa.vehdjk.com

Py:   with lock: shared += 1
来源：http://deq.sweek.top

PHP:  // 用 flock() 做文件锁
来源：http://hvm.guowangkeji.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://loy.316326.xyz

TS:   // 同 JS
来源：http://oon.dashuyun.cn

Java: synchronized (this) { shared++; }
来源：http://byr.9152youxi.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fdi.fktsv.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://kpi.yuanzhike.top

C#:   lock (gate) { shared++; }
来源：http://roy.jyoumei.cn

[O04] 定义异步函数并等待
来源：http://twc.jqgufenzy.top

Py:   async def f():⏎    await g()
来源：http://dsn.cashguo.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://unx.ybcxt.top

JS:   async function f() { await g(); }
来源：http://fpe.mhx1999.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://ztj.dianchejie.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ngh.iojbl.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://jqw.meibo888.top

Ruby: # 用 Fiber 或 async gem
来源：http://cwi.9152youxi.cn

C#:   async Task F() { await G(); }
来源：http://hbz.zhengqikj.top

[O05] 并发执行并等待全部完成
来源：http://ftu.shangyingyoupin.top

Py:   asyncio.gather(*tasks)
来源：http://zqo.jiagoushi.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dsn.yangfankeji.com

JS:   await Promise.all(tasks)
来源：http://cik.yangfankeji.com

TS:   await Promise.all(tasks)
来源：http://tbr.guannengcc.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hwb.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ank.bbcook.cn

Ruby: threads.map(&:join)
来源：http://wsh.aizwys.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://slx.nanxinkj.top

[O06] 使用进程池
来源：http://qvh.yonumen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wee.jqgufenzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://xmf.xuetiantiany.cn

JS:   // child_process / cluster 模块
来源：http://bmi.yueranfly.top

TS:   // child_process / cluster 模块
来源：http://ybu.andypj.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cjz.hysaishi.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://luo.fehbvm.com

Ruby: // fork 块
来源：http://dyg.gotoacloud.top

C#:   Parallel.For
来源：http://nqb.dashuyun.cn

================================================================================
来源：http://tdo.fzhhl.top

P. 常用工具函数
来源：http://vem.jinghuilouyu.cn

================================================================================
来源：http://fno.yueranfly.top

[P01] 生成 UUID
来源：http://lik.daxiang520.top

Py:   str(uuid.uuid4())
来源：http://bol.zdqjudy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fyl.aizwys.cn

JS:   crypto.randomUUID()
来源：http://ayk.daxiang520.top

TS:   crypto.randomUUID()
来源：http://nsr.hcnkem.com

Java: UUID.randomUUID().toString()
来源：http://zbq.fehbvm.com

Go:   // 用 github.com/google/uuid
来源：http://lqx.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://mfe.ppjwa.cn

C#:   Guid.NewGuid().ToString()
来源：http://wam.redwolf501.top

[P02] MD5 / SHA256 摘要
来源：http://mut.dashuyun.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fqc.dianchejie.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://qbt.wangdashe.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hhe.sxryk.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baj.nanxuanxn.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://uuj.sysykeji.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://sjo.fanxiaobao.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qjo.0kj1m.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mbv.bjfxy.top

[P03] 生成短随机字符串
来源：http://yol.zycfv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qeg.uphjek.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xns.mhx1999.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ueb.hammf.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://icc.zhoulong.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xec.daxiang520.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://sdb.zhiwuduotai.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tte.yuxming.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zpi.quarkkingdee.top

[P04] 求长度
来源：http://gqz.pengpengdd.cyou

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cum.zhoulong.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yns.52xcode.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xoe.zhongyouzk.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qha.hnqzz.top

Java: list.size();  map.size();  s.length()
来源：http://tah.jinyuanbaomall.cn

Go:   len(arr);  len(m)
来源：http://hox.vehdjk.com

Ruby: x.length;  x.size
来源：http://gzo.guowangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lmq.jianghu66.top

[P05] 判断两个对象内容是否相等
来源：http://ddq.yuxming.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://hme.jinghuilouyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vtd.ydzc1.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wqz.shuidangran.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gcm.zhijiandao.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ene.jiagoushi.top

Go:   reflect.DeepEqual(a, b)
来源：http://oqr.xuetiantiany.cn

Ruby: a == b
来源：http://cjl.jlsjyb.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://aaw.yanxiufei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pfb.ywan-chungtsiang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jpk.zdbjq.cn

PHP:  if (empty($x)) {}
来源：http://fez.tianlin.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mpl.zycfv.cn

TS:   if (x == null) {}
来源：http://vuy.sysykeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://gfd.jinyuanbaomall.cn

Go:   if x == nil {}
来源：http://tgi.chenzaomai.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://odk.0kj1m.cn

C#:   if (x is null) {}
来源：http://sgh.ybcxt.top

[P07] 防抖与节流
来源：http://vnl.yangfankeji.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bed.smart0.xyz

PHP:  // 手写时间戳比较
来源：http://oza.cdnleiting.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ysb.zhaomingkeji.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gka.cqqwz.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uiw.fzhhl.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jcv.fanxiaobao.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://jci.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gxi.jqgufenzy.top

[P08] 处理浮点精度问题
来源：http://iek.cdnleiting.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ihq.nanxuanxn.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://iko.sxryk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://khl.xingfuxueyuan.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ygo.aizwys.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ncp.jqgfzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://aoj.jinqigfzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qub.c1oappe.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dtb.chenjidiqi.icu

================================================================================
来源：http://vtz.52xcode.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://zfb.fanxiaobao.xyz

================================================================================
来源：http://nxh.xuetiantiany.cn

[Q01] 创建表
来源：http://rzk.havefunace.top

CREATE TABLE users (
来源：http://ihr.zhixingplan.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kpj.sjlbkw.cn

name VARCHAR(50) NOT NULL,
来源：http://coa.sweek.top

email VARCHAR(100) UNIQUE,
来源：http://xma.daria6918.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wab.sjlbkw.cn

);
来源：http://ome.yvedp.cn

[Q02] 创建带外键的表
来源：http://xbs.yj202588.top

CREATE TABLE orders (
来源：http://sxi.tarul.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sbj.ywan-chungtsiang.top

user_id INT NOT NULL,
来源：http://zfg.svipenyu.cn

amount DECIMAL(10, 2),
来源：http://vcj.jinqigfzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bcl.uphjek.com

);
来源：http://lyd.havefunace.top

[Q03] 增加列
来源：http://odf.daxiang520.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ayi.nanxuanxn.top

[Q04] 修改列类型
来源：http://tsa.nanxinkj.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tpv.ppjwa.cn

[Q05] 重命名列
来源：http://uvk.ywan-chungtsiang.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kch.yuxming.cn

[Q06] 删除列
来源：http://lhm.pengpengdd.cyou

ALTER TABLE users DROP COLUMN age;
来源：http://nud.jqgufenzy.top

[Q07] 删除表
来源：http://tup.yangfankeji.com

DROP TABLE IF EXISTS orders;
来源：http://swl.hysaishi.cn

[Q08] 创建普通索引
来源：http://cjg.yangfankeji.com

CREATE INDEX idx_users_email ON users(email);
来源：http://puu.aizwys.cn

[Q09] 创建唯一索引
来源：http://itv.chenlongwang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gzl.cucudq.cn

[Q10] 插入单行
来源：http://yif.wangdashe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gvl.zhoulong.xyz

[Q11] 一次插入多行
来源：http://qux.sxryk.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wtv.yanxiufei.cn

[Q12] 插入后取自增 ID
来源：http://bpm.yongpay.top

INSERT INTO users (name) VALUES ('C');
来源：http://jjc.fehbvm.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xhn.zycfv.cn

[Q13] 忽略重复插入
来源：http://ipu.dashuyun.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vbq.jianghu66.top

[Q14] 存在则更新（upsert）
来源：http://gtt.yj202588.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://nvk.yuxming.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://obt.epnwcf.com

[Q15] 查询全部
来源：http://drw.jinyuanbaomall.cn

SELECT * FROM users;
来源：http://vqg.gaohongyu789.top

[Q16] 查询指定列
来源：http://gnf.guannengcc.top

SELECT id, name FROM users;
来源：http://htb.nanxinkj.top

[Q17] 条件查询
来源：http://jck.cheryme.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pxg.mhx1999.top

[Q18] 模糊匹配
来源：http://gte.daria6918.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dra.havefunace.top

[Q19] 范围查询
来源：http://abm.vqdsnc.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pmr.jinqigfzy.top

[Q20] IN 列表
来源：http://qxp.yj20258.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jfq.yj20258.top

[Q21] 空值判断
来源：http://vqt.ivvv.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ekc.snrcjt.cn

[Q22] 排序
来源：http://gqi.yangfankeji.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lwr.hongshengwenyu.top

[Q23] 分页
来源：http://oph.nanxinkj.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mhj.mhx1999.top

[Q24] 去重
来源：http://kyz.jqgfzy.top

SELECT DISTINCT city FROM users;
来源：http://zhn.chenjidiqi.icu

[Q25] 只取前 N 条
来源：http://hji.chenjidiqi.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lbq.hysaishi.cn

[Q26] 计数
来源：http://vcc.birdmap.top

SELECT COUNT(*) FROM users;
来源：http://qsf.zhiwuduotai.top

[Q27] 条件计数
来源：http://waf.bjfxy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://app.jiagoushi.top

[Q28] 求和与平均
来源：http://csn.xingfuxueyuan.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fdq.yvedp.cn

[Q29] 最大最小值
来源：http://cvm.xingfuxueyuan.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://eer.zhongyouzk.top

[Q30] 分组统计
来源：http://lay.sxryk.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yjy.shanyushiyangtech.top

[Q31] 分组后过滤
来源：http://ygc.kuanghao11.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xwv.shanyushiyangtech.top

[Q32] 分组拼接字符串
来源：http://zog.vqdsnc.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ymv.havefunace.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jai.aibaodan.cn

[Q33] 多列分组
来源：http://pwe.cucudq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://npc.chenzaomai.com

[Q34] 每组取第一条
来源：http://phj.hammf.cn

SELECT * FROM (
来源：http://ryb.chenzaomai.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kng.c1oappe.top

) t WHERE rn = 1;
来源：http://fgd.shzxlz.cn

[Q35] 内连接
来源：http://whl.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ged.chenjidiqi.icu

[Q36] 左连接
来源：http://jgw.sjlbkw.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tth.zhiwuduotai.top

[Q37] 右连接
来源：http://yjt.bbcook.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vil.zhiwuduotai.top

[Q38] 全外连接（PostgreSQL）
来源：http://xnv.yvedp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qpu.aizwys.cn

[Q39] 自连接（查上下级）
来源：http://yyf.guannengcc.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tst.snrcjt.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ydy.nanxuanxn.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xca.jinqigfzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hkt.shanyushiyangkeji.top

[Q41] 多表连接
来源：http://tho.feifeiyinyue.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://sga.zhiwuduotai.top

JOIN users u ON u.id = o.user_id
来源：http://vin.hysaishi.cn

JOIN products p ON p.id = o.product_id;
来源：http://uzx.yj202588.top

[Q42] 连接条件附加过滤
来源：http://wil.yfazqb.com

SELECT u.name, o.amount FROM users u
来源：http://tao.gzhubu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jbl.svipenyu.cn

[Q43] 标量子查询
来源：http://fsy.fengsongda.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lxk.pycfn.com

[Q44] IN 子查询
来源：http://vsl.yangfankeji.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vck.jqgfzy.top

[Q45] EXISTS 判断存在
来源：http://mao.zhijiandao.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://npn.sxryk.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mnl.jinghuilouyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oyd.andypj.xyz

[Q47] 与平均值比较
来源：http://npk.gaohongyu789.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nvf.yfazqb.com

[Q48] CTE 公用表表达式
来源：http://jqe.birdmap.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qqo.daxiang520.top

SELECT * FROM t WHERE c > 5;
来源：http://ojq.yangfankeji.com

[Q49] 更新单行
来源：http://plt.zhixingplan.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qfm.hywenlv.cn

[Q50] 批量更新
来源：http://eah.gogol.net.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mbb.tanke756.top

[Q51] 用子查询更新
来源：http://arb.yonumen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://uok.jqgufenzy.top

[Q52] 删除指定行
来源：http://gqt.shzxlz.cn

DELETE FROM users WHERE id = 10;
来源：http://ysr.ywan-chungtsiang.top

[Q53] 按条件删除
来源：http://rli.hnqzz.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dhn.316326.xyz

[Q54] 清空表
来源：http://gfa.c1oappe.top

TRUNCATE TABLE logs;
来源：http://ztl.yonumen.top

[Q55] 排名（并列占位）
来源：http://yzb.hesvh.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vmq.dashuyun.cn

[Q56] 密集排名（并列不占位）
来源：http://kjr.smart0.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gns.zhengqikj.top

[Q57] 行号
来源：http://giv.snrcjt.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uir.svipenyu.cn

[Q58] 累计求和
来源：http://lvo.yangfankeji.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iyt.yj20258.top

[Q59] 分组内累计
来源：http://anx.svipenyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ejx.nanxuanxn.top

[Q60] 取上一行 / 下一行
来源：http://mcf.ctjpmb.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wkz.aizwys.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sdl.bjfxy.top

[Q61] 移动平均
来源：http://okb.snrcjt.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zxp.iojbl.cn

[Q62] 分组占比
来源：http://usp.ydjk.org.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fnq.mhx1999.top

[Q63] 开启事务
来源：http://pmw.tian-w.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://guz.hnqzz.top

[Q64] 提交事务
来源：http://qpl.316326.xyz

COMMIT;
来源：http://fyi.gogol.net.cn

[Q65] 回滚事务
来源：http://uno.haohaochexian.top

ROLLBACK;
来源：http://iak.jiagoushi.top

[Q66] 行锁查询
来源：http://lkj.zhengqikj.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://myf.jinqigufen.top

[Q67] 设置隔离级别
来源：http://xjx.zhiwuduotai.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pgp.hnxiangtu.top

[Q68] 保存点
来源：http://qvy.hongshengwenyu.top

SAVEPOINT sp1;
来源：http://xge.hcnkem.com

ROLLBACK TO sp1;
来源：http://lam.zhaomingkeji.xyz

[Q69] 查看执行计划
来源：http://bmx.nanxuanxn.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://umv.hfpthk.cn

[Q70] 更新统计信息
来源：http://iud.cheryme.top

ANALYZE TABLE users;
来源：http://inn.tian-w.cn

[Q71] 查看建表语句
来源：http://kgq.jianghu66.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fps.birdmap.top

[Q72] 查看索引
来源：http://xsl.nanxinkj.top

SHOW INDEX FROM users;
来源：http://vxa.hongshengwenyu.top

[Q73] 查看表状态
来源：http://okh.zhixingplan.top

SHOW TABLE STATUS LIKE 'users';
来源：http://stz.ehwqpu.com

[Q74] 强制使用索引
来源：http://abo.epnwcf.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oxv.jiagoushi.top

[Q75] 日期格式化
来源：http://aaj.epnwcf.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zro.xuanzx.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zgc.hesvh.cn


<!-- 参考信息 -->