代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://yhe.jqgfzy.top

Go:   go f()
来源：http://exk.bbcook.cn

Ruby: Thread.new { f }
来源：http://vcu.wangshuangyany.cn

C#:   Task.Run(() => F());
来源：http://oqq.zhongyouzk.top

[O02] 使用线程池
来源：http://iwy.uphjek.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://kug.jyoumei.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cox.zhoulong.xyz

JS:   // worker_threads 线程池
来源：http://aba.jqgufenzy.top

TS:   // worker_threads 线程池
来源：http://yav.smart0.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://lsr.yj20258.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://miz.jlsjyb.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://pyi.zdbjq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://yso.0kj1m.cn

[O03] 加锁保护共享数据
来源：http://gwh.nwbrower.top

Py:   with lock: shared += 1
来源：http://qqo.yonumen.top

PHP:  // 用 flock() 做文件锁
来源：http://xqk.ybcxt.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bwr.yfazqb.com

TS:   // 同 JS
来源：http://zdb.chenlongwang.top

Java: synchronized (this) { shared++; }
来源：http://zfr.jqgfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uyq.hfpthk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ylh.xingfuxueyuan.xyz

C#:   lock (gate) { shared++; }
来源：http://axv.pengpengdd.cyou

[O04] 定义异步函数并等待
来源：http://hlr.ivvv.top

Py:   async def f():⏎    await g()
来源：http://ras.ydzc1.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fmj.quarkkingdee.top

JS:   async function f() { await g(); }
来源：http://bxw.tarul.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://fkp.dashuyun.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pbz.jqgfzy.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qfa.guannengcc.top

Ruby: # 用 Fiber 或 async gem
来源：http://rbd.jiagoushi.top

C#:   async Task F() { await G(); }
来源：http://onr.jqgufenzy.top

[O05] 并发执行并等待全部完成
来源：http://bdi.cashguo.top

Py:   asyncio.gather(*tasks)
来源：http://hsx.jinghuilouyu.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gxt.zhoulong.xyz

JS:   await Promise.all(tasks)
来源：http://ase.gogol.net.cn

TS:   await Promise.all(tasks)
来源：http://vlf.shuidangran.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vyc.chenzaomai.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ryz.cashguo.top

Ruby: threads.map(&:join)
来源：http://thl.yueranfly.top

C#:   await Task.WhenAll(t1, t2)
来源：http://drz.guowangkeji.top

[O06] 使用进程池
来源：http://yqc.shangyingyoupin.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jhq.hywenlv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://boo.316326.xyz

JS:   // child_process / cluster 模块
来源：http://joa.ybcxt.top

TS:   // child_process / cluster 模块
来源：http://kxl.wangdashe.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vbp.hnqzz.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://xlw.0kj1m.cn

Ruby: // fork 块
来源：http://rue.zycfv.cn

C#:   Parallel.For
来源：http://cnc.xuanzx.com

================================================================================
来源：http://bhy.sjlbkw.cn

P. 常用工具函数
来源：http://weo.hfpthk.cn

================================================================================
来源：http://xsd.quarkkingdee.top

[P01] 生成 UUID
来源：http://jiq.cqqwz.cn

Py:   str(uuid.uuid4())
来源：http://xuz.dashuyun.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://sqd.tarul.cn

JS:   crypto.randomUUID()
来源：http://jow.guannengcc.top

TS:   crypto.randomUUID()
来源：http://oxr.daria6918.cn

Java: UUID.randomUUID().toString()
来源：http://tql.havefunace.top

Go:   // 用 github.com/google/uuid
来源：http://xic.ppjwa.cn

Ruby: SecureRandom.uuid
来源：http://nxc.shuidangran.top

C#:   Guid.NewGuid().ToString()
来源：http://big.cashguo.top

[P02] MD5 / SHA256 摘要
来源：http://vej.ydjk.org.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yhb.xuanzx.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://vvi.yueranfly.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://krd.cdnleiting.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yyk.zhijiandao.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mqd.jianghu66.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://krm.52xcode.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jam.cqqwz.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vwd.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://cyf.jlsjyb.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nik.fehbvm.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gcs.yj20258888.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ull.yuxming.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ung.yj20258.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ujs.jinyuanbaomall.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lwm.haohaochexian.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gbq.yongpay.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zag.feifeiyinyue.top

[P04] 求长度
来源：http://kaq.guowangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ast.zdqjudy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bmd.zdqjudy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blw.dianchejie.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lxx.c1oappe.top

Java: list.size();  map.size();  s.length()
来源：http://pll.jinghuilouyu.cn

Go:   len(arr);  len(m)
来源：http://iuh.yfazqb.com

Ruby: x.length;  x.size
来源：http://obs.zhixingplan.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://umj.guowangkeji.top

[P05] 判断两个对象内容是否相等
来源：http://gsk.zdbjq.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tea.daria6918.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hbg.cucudq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ywy.meibo888.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bgh.jinyuanbaomall.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rmk.0kj1m.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ljf.shzxlz.cn

Ruby: a == b
来源：http://igf.gotoacloud.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hjj.xuetiantiany.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wte.xinyue.icu

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ild.gotoacloud.top

PHP:  if (empty($x)) {}
来源：http://cwn.yj20258888.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://odw.iojbl.cn

TS:   if (x == null) {}
来源：http://vsl.0kj1m.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cbq.zhongyouzk.top

Go:   if x == nil {}
来源：http://fna.xinyue.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hha.zhixingplan.top

C#:   if (x is null) {}
来源：http://xky.zhaomingkeji.xyz

[P07] 防抖与节流
来源：http://oel.zhongyouzk.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rrt.hnxiangtu.top

PHP:  // 手写时间戳比较
来源：http://ztl.ehwqpu.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vvn.pengpengdd.cyou

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ats.shangyingyoupin.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://uvx.fanxiaobao.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hxr.fanxiaobao.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://kgo.svipenyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ark.shanyushiyangtech.top

[P08] 处理浮点精度问题
来源：http://rfq.bjfxy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ewd.316326.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cmt.ppjwa.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://myn.316326.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://bte.yanxiufei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pan.316326.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eip.nanxuanxn.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bos.zhongyouzk.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ctk.cqqwz.cn

================================================================================
来源：http://kya.vqdsnc.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vli.dashuyun.cn

================================================================================
来源：http://gdd.xziqi.cn

[Q01] 创建表
来源：http://lmx.xuanzx.com

CREATE TABLE users (
来源：http://jep.jinqigfzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://owa.sjlbkw.cn

name VARCHAR(50) NOT NULL,
来源：http://zcw.nwbrower.top

email VARCHAR(100) UNIQUE,
来源：http://xqr.bjfxy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://rno.yfazqb.com

);
来源：http://pub.fzhhl.top

[Q02] 创建带外键的表
来源：http://zzb.dianchejie.cn

CREATE TABLE orders (
来源：http://pul.chenzaomai.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lkz.jinghuilouyu.cn

user_id INT NOT NULL,
来源：http://pfk.fktsv.cn

amount DECIMAL(10, 2),
来源：http://xyc.fktsv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hrc.chenlongwang.top

);
来源：http://vrw.xingfuxueyuan.xyz

[Q03] 增加列
来源：http://bsr.daria6918.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cpf.yonumen.top

[Q04] 修改列类型
来源：http://nww.yuxming.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dep.daria6918.cn

[Q05] 重命名列
来源：http://xdp.jlsjyb.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bqr.gaohongyu789.top

[Q06] 删除列
来源：http://mcz.bbcook.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ryt.shuidangran.top

[Q07] 删除表
来源：http://eiy.hcnkem.com

DROP TABLE IF EXISTS orders;
来源：http://jkk.fengsongda.top

[Q08] 创建普通索引
来源：http://lxf.yonumen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://dqz.ybcxt.top

[Q09] 创建唯一索引
来源：http://zjj.zhaomingkeji.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tea.xingfuxueyuan.xyz

[Q10] 插入单行
来源：http://kaj.aibaodan.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ujv.jyoumei.cn

[Q11] 一次插入多行
来源：http://wob.hcnkem.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wgz.fanxiaobao.xyz

[Q12] 插入后取自增 ID
来源：http://fyy.yj20258888.top

INSERT INTO users (name) VALUES ('C');
来源：http://jrt.tarul.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://thn.zhaomingkeji.xyz

[Q13] 忽略重复插入
来源：http://tvg.jinghuilouyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ujc.hongshengwenyu.top

[Q14] 存在则更新（upsert）
来源：http://pqm.zhongyouzk.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://odu.zdbjq.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nse.zhijiandao.cn

[Q15] 查询全部
来源：http://brl.ppjwa.cn

SELECT * FROM users;
来源：http://ajl.hywenlv.cn

[Q16] 查询指定列
来源：http://kxr.jqgfzy.top

SELECT id, name FROM users;
来源：http://jua.xingfuxueyuan.xyz

[Q17] 条件查询
来源：http://qfv.yuanzhike.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xug.jianghu66.top

[Q18] 模糊匹配
来源：http://ozo.aizwys.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ggd.cdnleiting.top

[Q19] 范围查询
来源：http://sii.daria6918.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jsg.hywenlv.cn

[Q20] IN 列表
来源：http://fce.cheryme.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jaa.xingfuxueyuan.xyz

[Q21] 空值判断
来源：http://ydw.sxryk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gmf.fehbvm.com

[Q22] 排序
来源：http://wcj.yonumen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ghg.chenzaomai.com

[Q23] 分页
来源：http://trg.yfazqb.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jpy.zhaomingkeji.xyz

[Q24] 去重
来源：http://ncf.pycfn.com

SELECT DISTINCT city FROM users;
来源：http://znu.zycfv.cn

[Q25] 只取前 N 条
来源：http://bkg.havefunace.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lhm.zycfv.cn

[Q26] 计数
来源：http://gqh.daria6918.cn

SELECT COUNT(*) FROM users;
来源：http://uma.jianghu66.top

[Q27] 条件计数
来源：http://knm.ydzc1.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pvz.snrcjt.cn

[Q28] 求和与平均
来源：http://rsq.gzhubu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zwu.shangyingyoupin.top

[Q29] 最大最小值
来源：http://xpm.daria6918.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ojj.snrcjt.cn

[Q30] 分组统计
来源：http://rfv.yfazqb.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://avr.fanxiaobao.xyz

[Q31] 分组后过滤
来源：http://uea.smart0.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://skk.yj20258888.top

[Q32] 分组拼接字符串
来源：http://mgi.zycfv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hok.sweek.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jyf.tarul.cn

[Q33] 多列分组
来源：http://ryh.ivvv.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xlq.ydzc1.top

[Q34] 每组取第一条
来源：http://gxm.shzxlz.cn

SELECT * FROM (
来源：http://jis.zhiwuduotai.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nbz.xuetiantiany.cn

) t WHERE rn = 1;
来源：http://ufw.smart0.xyz

[Q35] 内连接
来源：http://pva.ybcxt.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nys.jinghuilouyu.cn

[Q36] 左连接
来源：http://xdu.tanke756.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ixq.xinyue.icu

[Q37] 右连接
来源：http://evu.jinqigufen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cnc.zhixingplan.top

[Q38] 全外连接（PostgreSQL）
来源：http://bvb.hammf.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iaj.birdmap.top

[Q39] 自连接（查上下级）
来源：http://ckb.jqgufenzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://bxw.jinqigfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gmo.quarkkingdee.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ghn.wangshuangyany.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jvk.zhixingplan.top

[Q41] 多表连接
来源：http://bna.meibo888.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fqm.pycfn.com

JOIN users u ON u.id = o.user_id
来源：http://lyf.uphjek.com

JOIN products p ON p.id = o.product_id;
来源：http://qmm.gogol.net.cn

[Q42] 连接条件附加过滤
来源：http://kzq.zdqjudy.top

SELECT u.name, o.amount FROM users u
来源：http://rgd.cheryme.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zwl.shangyingyoupin.top

[Q43] 标量子查询
来源：http://hbx.zhaomingkeji.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nfm.xingfuxueyuan.xyz

[Q44] IN 子查询
来源：http://wxo.ctjpmb.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zil.shanyushiyangkeji.top

[Q45] EXISTS 判断存在
来源：http://vpj.yangfankeji.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tgw.tian-w.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ukw.zhoulong.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jzn.sysykeji.top

[Q47] 与平均值比较
来源：http://icp.birdmap.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cjj.hysaishi.cn

[Q48] CTE 公用表表达式
来源：http://gpf.c1oappe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hnw.dianchejie.cn

SELECT * FROM t WHERE c > 5;
来源：http://fkn.xziqi.cn

[Q49] 更新单行
来源：http://sge.tanke756.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://grw.zdqjudy.top

[Q50] 批量更新
来源：http://nff.52xcode.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xag.0kj1m.cn

[Q51] 用子查询更新
来源：http://hei.haohaochexian.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://btl.tarul.cn

[Q52] 删除指定行
来源：http://hut.yj20258888.top

DELETE FROM users WHERE id = 10;
来源：http://rgd.zhoulong.xyz

[Q53] 按条件删除
来源：http://tkc.shanyushiyangtech.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://psz.jinyuanbaomall.cn

[Q54] 清空表
来源：http://umm.sjlbkw.cn

TRUNCATE TABLE logs;
来源：http://pcs.ctjpmb.com

[Q55] 排名（并列占位）
来源：http://zkh.zdqjudy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://txd.jlsjyb.cn

[Q56] 密集排名（并列不占位）
来源：http://efv.shangyingyoupin.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jhn.zhixingplan.top

[Q57] 行号
来源：http://iew.c1oappe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pod.yj202588.top

[Q58] 累计求和
来源：http://faa.jqgfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rqq.hnxiangtu.top

[Q59] 分组内累计
来源：http://nmi.9152youxi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yck.daria6918.cn

[Q60] 取上一行 / 下一行
来源：http://tjz.9152youxi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zuk.jqgufenzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mnl.zhiwuduotai.top

[Q61] 移动平均
来源：http://ltx.hnxiangtu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cwm.yanxiufei.cn

[Q62] 分组占比
来源：http://rgm.yvedp.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://icp.yongpay.top

[Q63] 开启事务
来源：http://vno.yuxming.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jci.tanke756.top

[Q64] 提交事务
来源：http://ttd.gogol.net.cn

COMMIT;
来源：http://txd.fehbvm.com

[Q65] 回滚事务
来源：http://vmb.smart0.xyz

ROLLBACK;
来源：http://pcp.gotoacloud.top

[Q66] 行锁查询
来源：http://xby.cucudq.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vcb.xuanzx.com

[Q67] 设置隔离级别
来源：http://ffy.c1oappe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mwo.cqqwz.cn

[Q68] 保存点
来源：http://kgm.yueranfly.top

SAVEPOINT sp1;
来源：http://tjo.yj202588.top

ROLLBACK TO sp1;
来源：http://hcr.jyoumei.cn

[Q69] 查看执行计划
来源：http://whh.xuetiantiany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://igd.fanxiaobao.xyz

[Q70] 更新统计信息
来源：http://oje.jinqigfzy.top

ANALYZE TABLE users;
来源：http://cxp.chenjidiqi.icu

[Q71] 查看建表语句
来源：http://ndq.meibo888.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mwe.hesvh.cn

[Q72] 查看索引
来源：http://eox.hfpthk.cn

SHOW INDEX FROM users;
来源：http://ixm.cheryme.top

[Q73] 查看表状态
来源：http://nzu.yonumen.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jfr.hysaishi.cn

[Q74] 强制使用索引
来源：http://xhs.shangyingyoupin.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://idv.hongshengwenyu.top

[Q75] 日期格式化
来源：http://cim.hysaishi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://geh.0kj1m.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rom.shzxlz.cn


<!-- 参考信息 -->