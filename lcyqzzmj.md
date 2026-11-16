代发 wailian999

[O02] 使用线程池
来源：http://rwe.yj202588.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://uis.bbcook.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://svg.jqgfzy.top

JS:   // worker_threads 线程池
来源：http://jfb.chenzaomai.com

TS:   // worker_threads 线程池
来源：http://rpk.zycfv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://wet.feifeiyinyue.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://esq.sufxvd.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rlf.hnxiangtu.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://eui.bbcook.cn

[O03] 加锁保护共享数据
来源：http://pff.xingfuxueyuan.xyz

Py:   with lock: shared += 1
来源：http://oii.daxiang520.top

PHP:  // 用 flock() 做文件锁
来源：http://pmr.tianlin.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uve.yj202588.top

TS:   // 同 JS
来源：http://hpy.ybcxt.top

Java: synchronized (this) { shared++; }
来源：http://mbb.jinqigfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://lrw.wangdashe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://qll.zhaomingkeji.xyz

C#:   lock (gate) { shared++; }
来源：http://rof.yfazqb.com

[O04] 定义异步函数并等待
来源：http://krs.ydjk.org.cn

Py:   async def f():⏎    await g()
来源：http://fjz.jinqigfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xdz.0kj1m.cn

JS:   async function f() { await g(); }
来源：http://oyc.havefunace.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jzf.quarkkingdee.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mbc.ctjpmb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://whu.wangdashe.top

Ruby: # 用 Fiber 或 async gem
来源：http://ytu.0kj1m.cn

C#:   async Task F() { await G(); }
来源：http://qsw.hammf.cn

[O05] 并发执行并等待全部完成
来源：http://uuz.xuanzx.com

Py:   asyncio.gather(*tasks)
来源：http://jzt.ehwqpu.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://rwg.chenzaomai.com

JS:   await Promise.all(tasks)
来源：http://hqu.pycfn.com

TS:   await Promise.all(tasks)
来源：http://vzn.xziqi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wsu.sysykeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nuh.zhijiandao.cn

Ruby: threads.map(&:join)
来源：http://nzb.svipenyu.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://idv.52xcode.cn

[O06] 使用进程池
来源：http://yzb.fehbvm.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kdo.xuetiantiany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nfx.zhiwuduotai.top

JS:   // child_process / cluster 模块
来源：http://xkh.yuxming.cn

TS:   // child_process / cluster 模块
来源：http://hud.shanyushiyangtech.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://imw.shangyingyoupin.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gym.fzhhl.top

Ruby: // fork 块
来源：http://sav.zhijiandao.cn

C#:   Parallel.For
来源：http://hph.hnxiangtu.top

================================================================================
来源：http://myz.dianchejie.cn

P. 常用工具函数
来源：http://ccf.nanxinkj.top

================================================================================
来源：http://ryv.tanke756.top

[P01] 生成 UUID
来源：http://qub.ivvv.top

Py:   str(uuid.uuid4())
来源：http://cfy.cashguo.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ixc.meibo888.top

JS:   crypto.randomUUID()
来源：http://txq.316326.xyz

TS:   crypto.randomUUID()
来源：http://wpv.andypj.xyz

Java: UUID.randomUUID().toString()
来源：http://bbl.guowangkeji.top

Go:   // 用 github.com/google/uuid
来源：http://ymt.yj20258888.top

Ruby: SecureRandom.uuid
来源：http://rtu.pengpengdd.cyou

C#:   Guid.NewGuid().ToString()
来源：http://jli.jinqigfzy.top

[P02] MD5 / SHA256 摘要
来源：http://xcl.hysaishi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pcq.bjfxy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://uyn.ywan-chungtsiang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://udk.zhongyouzk.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hbw.fktsv.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ltb.smart0.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://aqq.bbcook.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tbz.sjlbkw.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ngw.gogol.net.cn

[P03] 生成短随机字符串
来源：http://kke.quarkkingdee.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://yht.ywan-chungtsiang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bdb.jinyuanbaomall.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lut.cqqwz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ber.havefunace.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://twj.quarkkingdee.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://txd.xziqi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://nke.snrcjt.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ngu.bbcook.cn

[P04] 求长度
来源：http://wcm.c1oappe.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rrr.tianlin.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vno.zycfv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fkv.xuanzx.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gnc.fktsv.cn

Java: list.size();  map.size();  s.length()
来源：http://izr.nanxinkj.top

Go:   len(arr);  len(m)
来源：http://hmh.xylfe.cn

Ruby: x.length;  x.size
来源：http://pic.jlsjyb.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fwl.feifeiyinyue.top

[P05] 判断两个对象内容是否相等
来源：http://tmh.chenjidiqi.icu

Py:   a == b              # 列表与字典递归比较内容
来源：http://zty.zdqjudy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qgp.uphjek.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ntg.gzhubu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://elr.tian-w.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jzj.meibo888.top

Go:   reflect.DeepEqual(a, b)
来源：http://hro.zhiwuduotai.top

Ruby: a == b
来源：http://frn.hfpthk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mhh.dianchejie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bhs.bjfxy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hnj.c1oappe.top

PHP:  if (empty($x)) {}
来源：http://gow.dianchejie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ewq.uphjek.com

TS:   if (x == null) {}
来源：http://sev.gogol.net.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://kde.fzhhl.top

Go:   if x == nil {}
来源：http://gyk.zhijiandao.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://euz.wangshuangyany.cn

C#:   if (x is null) {}
来源：http://zqh.sufxvd.cn

[P07] 防抖与节流
来源：http://bcw.iojbl.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xrj.mhx1999.top

PHP:  // 手写时间戳比较
来源：http://kta.hfpthk.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qex.52xcode.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://feu.mhx1999.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xem.feifeiyinyue.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kzy.shanyushiyangkeji.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ztx.0kj1m.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yfg.shangyingyoupin.top

[P08] 处理浮点精度问题
来源：http://daa.jqgfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://szb.cheryme.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kda.feifeiyinyue.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kgn.jiagoushi.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fry.aizwys.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pwr.xuetiantiany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yek.yonumen.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ivr.zdqjudy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dxb.havefunace.top

================================================================================
来源：http://jiv.ivvv.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://woe.shanyushiyangkeji.top

================================================================================
来源：http://vep.sxryk.cn

[Q01] 创建表
来源：http://yjx.epnwcf.com

CREATE TABLE users (
来源：http://dya.jlsjyb.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://arh.9152youxi.cn

name VARCHAR(50) NOT NULL,
来源：http://xnx.hnqzz.top

email VARCHAR(100) UNIQUE,
来源：http://wqz.shanyushiyangtech.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://jhh.zhaomingkeji.xyz

);
来源：http://xel.hcnkem.com

[Q02] 创建带外键的表
来源：http://mda.vqdsnc.cn

CREATE TABLE orders (
来源：http://zzf.snrcjt.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://umy.jyoumei.cn

user_id INT NOT NULL,
来源：http://djz.shuidangran.top

amount DECIMAL(10, 2),
来源：http://zoo.cdnleiting.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pqc.zdbjq.cn

);
来源：http://ume.zycfv.cn

[Q03] 增加列
来源：http://apw.nwbrower.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oke.iojbl.cn

[Q04] 修改列类型
来源：http://mvb.hesvh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dhs.snrcjt.cn

[Q05] 重命名列
来源：http://mib.xuetiantiany.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wiq.fanxiaobao.xyz

[Q06] 删除列
来源：http://har.sjlbkw.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tlw.xinyue.icu

[Q07] 删除表
来源：http://bge.yongpay.top

DROP TABLE IF EXISTS orders;
来源：http://zro.nwbrower.top

[Q08] 创建普通索引
来源：http://qhx.yj20258.top

CREATE INDEX idx_users_email ON users(email);
来源：http://sac.svipenyu.cn

[Q09] 创建唯一索引
来源：http://fxa.smart0.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fgp.jyoumei.cn

[Q10] 插入单行
来源：http://pif.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mfg.wangshuangyany.cn

[Q11] 一次插入多行
来源：http://gbb.wangdashe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://djy.52xcode.cn

[Q12] 插入后取自增 ID
来源：http://ezv.fanxiaobao.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://mls.nanxuanxn.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://sny.redwolf501.top

[Q13] 忽略重复插入
来源：http://wxe.pengpengdd.cyou

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://trb.zhiwuduotai.top

[Q14] 存在则更新（upsert）
来源：http://xde.xylfe.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://egs.dianchejie.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wnl.pengpengdd.cyou

[Q15] 查询全部
来源：http://rjn.iojbl.cn

SELECT * FROM users;
来源：http://uzd.bbcook.cn

[Q16] 查询指定列
来源：http://gir.jinghuilouyu.cn

SELECT id, name FROM users;
来源：http://hqn.andypj.xyz

[Q17] 条件查询
来源：http://nsy.jinqigfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xth.shuidangran.top

[Q18] 模糊匹配
来源：http://kha.cheryme.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jtm.chenzaomai.com

[Q19] 范围查询
来源：http://htd.xingfuxueyuan.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hsb.9152youxi.cn

[Q20] IN 列表
来源：http://tul.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://aiu.zhaomingkeji.xyz

[Q21] 空值判断
来源：http://yxl.daxiang520.top

SELECT * FROM users WHERE email IS NULL;
来源：http://krr.ivvv.top

[Q22] 排序
来源：http://cju.jinyuanbaomall.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vco.xuetiantiany.cn

[Q23] 分页
来源：http://azg.redwolf501.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hyv.mhx1999.top

[Q24] 去重
来源：http://gyr.yj20258888.top

SELECT DISTINCT city FROM users;
来源：http://ipi.jqgufenzy.top

[Q25] 只取前 N 条
来源：http://dex.gotoacloud.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ljj.haohaochexian.top

[Q26] 计数
来源：http://hiq.zhiwuduotai.top

SELECT COUNT(*) FROM users;
来源：http://vrm.zhoulong.xyz

[Q27] 条件计数
来源：http://dbv.yj20258.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tki.fanxiaobao.xyz

[Q28] 求和与平均
来源：http://wrq.sxryk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pbd.cqqwz.cn

[Q29] 最大最小值
来源：http://dce.jlsjyb.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hap.yanxiufei.cn

[Q30] 分组统计
来源：http://qfn.jinyuanbaomall.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tja.andypj.xyz

[Q31] 分组后过滤
来源：http://jqt.svipenyu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hxf.hongshengwenyu.top

[Q32] 分组拼接字符串
来源：http://yxy.52xcode.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ioz.gaohongyu789.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://btc.andypj.xyz

[Q33] 多列分组
来源：http://ihq.nanxinkj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nki.uphjek.com

[Q34] 每组取第一条
来源：http://dyx.yuanzhike.top

SELECT * FROM (
来源：http://cem.hcnkem.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ukp.aibaodan.cn

) t WHERE rn = 1;
来源：http://emt.cashguo.top

[Q35] 内连接
来源：http://vtg.guowangkeji.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hjz.zhijiandao.cn

[Q36] 左连接
来源：http://jsy.yueranfly.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ake.sjlbkw.cn

[Q37] 右连接
来源：http://osl.yonumen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wwe.ctjpmb.com

[Q38] 全外连接（PostgreSQL）
来源：http://uyz.jqgfzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://szv.zhixingplan.top

[Q39] 自连接（查上下级）
来源：http://ihm.jiagoushi.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://czx.ppjwa.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lop.ydzc1.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ntp.guowangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mvd.haohaochexian.top

[Q41] 多表连接
来源：http://pwd.hnxiangtu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mwz.guowangkeji.top

JOIN users u ON u.id = o.user_id
来源：http://coi.316326.xyz

JOIN products p ON p.id = o.product_id;
来源：http://mfq.hnxiangtu.top

[Q42] 连接条件附加过滤
来源：http://nkp.gaohongyu789.top

SELECT u.name, o.amount FROM users u
来源：http://qow.hnxiangtu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fkr.kuanghao11.cn

[Q43] 标量子查询
来源：http://tgn.epnwcf.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kkb.yangfankeji.com

[Q44] IN 子查询
来源：http://fwc.bjfxy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ruy.jianghu66.top

[Q45] EXISTS 判断存在
来源：http://pub.hnqzz.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pvy.kuanghao11.cn

[Q46] NOT EXISTS 判断不存在
来源：http://lbd.shanyushiyangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eos.fengsongda.top

[Q47] 与平均值比较
来源：http://rns.vehdjk.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ybo.fehbvm.com

[Q48] CTE 公用表表达式
来源：http://rom.yonumen.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kay.jianghu66.top

SELECT * FROM t WHERE c > 5;
来源：http://eav.tanke756.top

[Q49] 更新单行
来源：http://pmw.tian-w.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oju.fengsongda.top

[Q50] 批量更新
来源：http://rwk.cheryme.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dmq.epnwcf.com

[Q51] 用子查询更新
来源：http://fwn.chenzaomai.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://taj.jinqigfzy.top

[Q52] 删除指定行
来源：http://xyx.ywan-chungtsiang.top

DELETE FROM users WHERE id = 10;
来源：http://gzb.shanyushiyangkeji.top

[Q53] 按条件删除
来源：http://msd.cdnleiting.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://upk.yanxiufei.cn

[Q54] 清空表
来源：http://igy.epnwcf.com

TRUNCATE TABLE logs;
来源：http://lrh.zhongyouzk.top

[Q55] 排名（并列占位）
来源：http://fay.daria6918.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vzh.zhiwuduotai.top

[Q56] 密集排名（并列不占位）
来源：http://keh.ctjpmb.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ius.wangdashe.top

[Q57] 行号
来源：http://qpk.jqgufenzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gzn.xylfe.cn

[Q58] 累计求和
来源：http://pls.feifeiyinyue.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vfh.yongpay.top

[Q59] 分组内累计
来源：http://awj.ivvv.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://uhn.snrcjt.cn

[Q60] 取上一行 / 下一行
来源：http://foo.pengpengdd.cyou

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://smb.shanyushiyangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fnk.yangfankeji.com

[Q61] 移动平均
来源：http://ibd.daxiang520.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lpn.smart0.xyz

[Q62] 分组占比
来源：http://zsb.c1oappe.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dor.fktsv.cn

[Q63] 开启事务
来源：http://rky.smart0.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://eqs.zhongyouzk.top

[Q64] 提交事务
来源：http://nsu.gogol.net.cn

COMMIT;
来源：http://zvp.jqgufenzy.top

[Q65] 回滚事务
来源：http://vqi.yuanzhike.top

ROLLBACK;
来源：http://nfe.yfazqb.com

[Q66] 行锁查询
来源：http://faj.zhoulong.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ckc.svipenyu.cn

[Q67] 设置隔离级别
来源：http://ibi.zhengqikj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nxh.aibaodan.cn

[Q68] 保存点
来源：http://mrr.ydjk.org.cn

SAVEPOINT sp1;
来源：http://oui.52xcode.cn

ROLLBACK TO sp1;
来源：http://wan.xuetiantiany.cn

[Q69] 查看执行计划
来源：http://pqn.yj202588.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://sqs.jlsjyb.cn

[Q70] 更新统计信息
来源：http://fom.hysaishi.cn

ANALYZE TABLE users;
来源：http://qae.tarul.cn

[Q71] 查看建表语句
来源：http://jko.aibaodan.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://bws.yj20258.top

[Q72] 查看索引
来源：http://wqa.fanxiaobao.xyz

SHOW INDEX FROM users;
来源：http://zal.yueranfly.top

[Q73] 查看表状态
来源：http://imz.fktsv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://aab.yfazqb.com

[Q74] 强制使用索引
来源：http://dob.yongpay.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uvm.hfpthk.cn

[Q75] 日期格式化
来源：http://wez.yuxming.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fch.zhijiandao.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lnc.zhijiandao.cn

[Q76] 按天统计
来源：http://scl.cqqwz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hxp.gaohongyu789.top

[Q77] 时间加减
来源：http://sak.cashguo.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gpo.gaohongyu789.top


<!-- 参考信息 -->