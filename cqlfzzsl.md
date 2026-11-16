代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://rpg.hysaishi.cn

[O03] 加锁保护共享数据
来源：http://oif.zhiwuduotai.top

Py:   with lock: shared += 1
来源：http://vna.zdbjq.cn

PHP:  // 用 flock() 做文件锁
来源：http://odt.daxiang520.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://poi.svipenyu.cn

TS:   // 同 JS
来源：http://ort.quarkkingdee.top

Java: synchronized (this) { shared++; }
来源：http://ejv.ehwqpu.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bpr.cqqwz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://xaq.hesvh.cn

C#:   lock (gate) { shared++; }
来源：http://jhh.jiagoushi.top

[O04] 定义异步函数并等待
来源：http://dhh.zhiwuduotai.top

Py:   async def f():⏎    await g()
来源：http://yqy.tanke756.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xig.shangyingyoupin.top

JS:   async function f() { await g(); }
来源：http://ift.shuidangran.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://yqp.tarul.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pjp.ppjwa.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ezh.svipenyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tcq.wangdashe.top

C#:   async Task F() { await G(); }
来源：http://dvw.ybcxt.top

[O05] 并发执行并等待全部完成
来源：http://kze.aibaodan.cn

Py:   asyncio.gather(*tasks)
来源：http://jsl.meibo888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xdu.nanxuanxn.top

JS:   await Promise.all(tasks)
来源：http://wfs.quarkkingdee.top

TS:   await Promise.all(tasks)
来源：http://nzs.yuanzhike.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://edx.xuanzx.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ryr.daxiang520.top

Ruby: threads.map(&:join)
来源：http://gyw.nwbrower.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ncm.ydjk.org.cn

[O06] 使用进程池
来源：http://mfz.fengsongda.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mxd.zycfv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xgi.jqgufenzy.top

JS:   // child_process / cluster 模块
来源：http://mpg.yonumen.top

TS:   // child_process / cluster 模块
来源：http://tov.sufxvd.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jvo.cucudq.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://few.cdnleiting.top

Ruby: // fork 块
来源：http://rxa.hfpthk.cn

C#:   Parallel.For
来源：http://qpn.hysaishi.cn

================================================================================
来源：http://fny.zhaomingkeji.xyz

P. 常用工具函数
来源：http://gwx.cucudq.cn

================================================================================
来源：http://qiy.iojbl.cn

[P01] 生成 UUID
来源：http://rox.aibaodan.cn

Py:   str(uuid.uuid4())
来源：http://qix.quarkkingdee.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mlg.yj20258888.top

JS:   crypto.randomUUID()
来源：http://pkn.hesvh.cn

TS:   crypto.randomUUID()
来源：http://mqi.ydjk.org.cn

Java: UUID.randomUUID().toString()
来源：http://zqh.bbcook.cn

Go:   // 用 github.com/google/uuid
来源：http://oaq.smart0.xyz

Ruby: SecureRandom.uuid
来源：http://ptq.wangshuangyany.cn

C#:   Guid.NewGuid().ToString()
来源：http://hfn.cdnleiting.top

[P02] MD5 / SHA256 摘要
来源：http://qyf.xuetiantiany.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yfo.pycfn.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://aqf.xylfe.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wcg.svipenyu.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hnu.nwbrower.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xpm.ppjwa.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://urz.zycfv.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://eyg.guowangkeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lcs.sweek.top

[P03] 生成短随机字符串
来源：http://nie.yonumen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nzs.sxryk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jst.0kj1m.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cyq.hywenlv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ibg.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jur.zhengqikj.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nzh.bbcook.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://lff.52xcode.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xfm.ctjpmb.com

[P04] 求长度
来源：http://iei.zhengqikj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zuj.shanyushiyangtech.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iiu.uphjek.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hox.yongpay.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iix.hysaishi.cn

Java: list.size();  map.size();  s.length()
来源：http://qvj.shuidangran.top

Go:   len(arr);  len(m)
来源：http://ema.sweek.top

Ruby: x.length;  x.size
来源：http://yhe.xuetiantiany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tyg.hesvh.cn

[P05] 判断两个对象内容是否相等
来源：http://kfu.hfpthk.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pea.hesvh.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ifd.tarul.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rmr.snrcjt.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fet.ydjk.org.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://uoq.nanxinkj.top

Go:   reflect.DeepEqual(a, b)
来源：http://cxk.gotoacloud.top

Ruby: a == b
来源：http://utu.sxryk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pdj.yuxming.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kib.jlsjyb.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fwo.zhiwuduotai.top

PHP:  if (empty($x)) {}
来源：http://wdk.zhijiandao.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yte.fktsv.cn

TS:   if (x == null) {}
来源：http://etm.ydjk.org.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://tcx.jinqigufen.top

Go:   if x == nil {}
来源：http://mld.shuidangran.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cgf.chenjidiqi.icu

C#:   if (x is null) {}
来源：http://zyf.sxryk.cn

[P07] 防抖与节流
来源：http://piz.guannengcc.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wkq.hnqzz.top

PHP:  // 手写时间戳比较
来源：http://sit.yonumen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pcx.jyoumei.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zve.cashguo.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mgn.iojbl.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://onm.gaohongyu789.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qrx.sysykeji.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kci.jqgfzy.top

[P08] 处理浮点精度问题
来源：http://vgz.iojbl.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ayu.nanxinkj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rgw.havefunace.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kgn.yj20258.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://osj.zdqjudy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ujn.yj202588.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://inv.bbcook.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://alk.fzhhl.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://opn.zhiwuduotai.top

================================================================================
来源：http://ind.yonumen.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://crm.jqgufenzy.top

================================================================================
来源：http://wdp.jianghu66.top

[Q01] 创建表
来源：http://hqb.yj20258.top

CREATE TABLE users (
来源：http://ahg.shangyingyoupin.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://oxe.yj20258.top

name VARCHAR(50) NOT NULL,
来源：http://ngc.cdnleiting.top

email VARCHAR(100) UNIQUE,
来源：http://zpg.andypj.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ltc.jinyuanbaomall.cn

);
来源：http://sgq.smart0.xyz

[Q02] 创建带外键的表
来源：http://pfm.daria6918.cn

CREATE TABLE orders (
来源：http://hxt.gotoacloud.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hlz.gzhubu.top

user_id INT NOT NULL,
来源：http://lnd.cqqwz.cn

amount DECIMAL(10, 2),
来源：http://ocr.quarkkingdee.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://res.iojbl.cn

);
来源：http://sjb.daria6918.cn

[Q03] 增加列
来源：http://krh.zhoulong.xyz

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ldr.sweek.top

[Q04] 修改列类型
来源：http://tfx.ydjk.org.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://irz.yfazqb.com

[Q05] 重命名列
来源：http://gha.gogol.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://emh.fengsongda.top

[Q06] 删除列
来源：http://qja.epnwcf.com

ALTER TABLE users DROP COLUMN age;
来源：http://bai.fanxiaobao.xyz

[Q07] 删除表
来源：http://mwc.jyoumei.cn

DROP TABLE IF EXISTS orders;
来源：http://div.yueranfly.top

[Q08] 创建普通索引
来源：http://wcx.fktsv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://odq.kuanghao11.cn

[Q09] 创建唯一索引
来源：http://jty.redwolf501.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://qqu.shzxlz.cn

[Q10] 插入单行
来源：http://fpa.yongpay.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://asy.gaohongyu789.top

[Q11] 一次插入多行
来源：http://fkp.shangyingyoupin.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://arr.nanxuanxn.top

[Q12] 插入后取自增 ID
来源：http://ljt.nanxinkj.top

INSERT INTO users (name) VALUES ('C');
来源：http://rxg.nanxinkj.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dby.zdqjudy.top

[Q13] 忽略重复插入
来源：http://wjv.sufxvd.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kqw.pengpengdd.cyou

[Q14] 存在则更新（upsert）
来源：http://lol.shanyushiyangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ffv.ppjwa.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fwx.shanyushiyangtech.top

[Q15] 查询全部
来源：http://cpc.zycfv.cn

SELECT * FROM users;
来源：http://oli.9152youxi.cn

[Q16] 查询指定列
来源：http://baj.meibo888.top

SELECT id, name FROM users;
来源：http://gfr.0kj1m.cn

[Q17] 条件查询
来源：http://jat.hysaishi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://agl.316326.xyz

[Q18] 模糊匹配
来源：http://uag.dianchejie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://isc.bbcook.cn

[Q19] 范围查询
来源：http://vji.fehbvm.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zlc.c1oappe.top

[Q20] IN 列表
来源：http://tij.jinqigfzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zfe.cheryme.top

[Q21] 空值判断
来源：http://ama.zhengqikj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yig.xuanzx.com

[Q22] 排序
来源：http://zgs.snrcjt.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fde.9152youxi.cn

[Q23] 分页
来源：http://vkk.zhiwuduotai.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yno.yuanzhike.top

[Q24] 去重
来源：http://isb.gzhubu.top

SELECT DISTINCT city FROM users;
来源：http://ccp.0kj1m.cn

[Q25] 只取前 N 条
来源：http://qte.vehdjk.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jay.tian-w.cn

[Q26] 计数
来源：http://ais.zhiwuduotai.top

SELECT COUNT(*) FROM users;
来源：http://wgu.hnxiangtu.top

[Q27] 条件计数
来源：http://ktn.hammf.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://lhn.jyoumei.cn

[Q28] 求和与平均
来源：http://xsi.chenzaomai.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gvz.jinyuanbaomall.cn

[Q29] 最大最小值
来源：http://rnr.guowangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://wtg.sysykeji.top

[Q30] 分组统计
来源：http://eod.gaohongyu789.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cey.feifeiyinyue.top

[Q31] 分组后过滤
来源：http://ugn.vqdsnc.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pih.zhiwuduotai.top

[Q32] 分组拼接字符串
来源：http://rpf.ppjwa.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wad.hammf.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ubi.cheryme.top

[Q33] 多列分组
来源：http://kbx.sufxvd.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tsk.gaohongyu789.top

[Q34] 每组取第一条
来源：http://pab.sweek.top

SELECT * FROM (
来源：http://rol.zhengqikj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xnj.havefunace.top

) t WHERE rn = 1;
来源：http://zdp.zdbjq.cn

[Q35] 内连接
来源：http://tfc.cheryme.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ujk.shanyushiyangtech.top

[Q36] 左连接
来源：http://dlf.tanke756.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nnc.dianchejie.cn

[Q37] 右连接
来源：http://lcb.jinghuilouyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tnu.zhixingplan.top

[Q38] 全外连接（PostgreSQL）
来源：http://thi.dianchejie.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ckg.52xcode.cn

[Q39] 自连接（查上下级）
来源：http://rnq.ivvv.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mtx.snrcjt.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dth.jinghuilouyu.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wpv.cashguo.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wmt.ydzc1.top

[Q41] 多表连接
来源：http://fng.yj20258888.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://yfl.yonumen.top

JOIN users u ON u.id = o.user_id
来源：http://nbu.zhijiandao.cn

JOIN products p ON p.id = o.product_id;
来源：http://trk.cheryme.top

[Q42] 连接条件附加过滤
来源：http://vjn.sjlbkw.cn

SELECT u.name, o.amount FROM users u
来源：http://huu.9152youxi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dqi.ivvv.top

[Q43] 标量子查询
来源：http://bmv.zdqjudy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pdj.hnxiangtu.top

[Q44] IN 子查询
来源：http://jia.jinqigfzy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kht.jianghu66.top

[Q45] EXISTS 判断存在
来源：http://ooz.bbcook.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rfj.hysaishi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://man.jianghu66.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vtr.zycfv.cn

[Q47] 与平均值比较
来源：http://jmq.hfpthk.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nzu.ybcxt.top

[Q48] CTE 公用表表达式
来源：http://wyi.fanxiaobao.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rnl.ywan-chungtsiang.top

SELECT * FROM t WHERE c > 5;
来源：http://acl.jinqigufen.top

[Q49] 更新单行
来源：http://bzj.birdmap.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xrq.hesvh.cn

[Q50] 批量更新
来源：http://gbg.iojbl.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xsp.hcnkem.com

[Q51] 用子查询更新
来源：http://zjf.iojbl.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pxr.yangfankeji.com

[Q52] 删除指定行
来源：http://flu.chenlongwang.top

DELETE FROM users WHERE id = 10;
来源：http://ext.ywan-chungtsiang.top

[Q53] 按条件删除
来源：http://myw.jiagoushi.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xox.daxiang520.top

[Q54] 清空表
来源：http://ozc.yonumen.top

TRUNCATE TABLE logs;
来源：http://mgw.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://jyw.shanyushiyangtech.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sip.9152youxi.cn

[Q56] 密集排名（并列不占位）
来源：http://djr.hywenlv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jkg.zhoulong.xyz

[Q57] 行号
来源：http://jlt.wangshuangyany.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zzh.hnxiangtu.top

[Q58] 累计求和
来源：http://vau.smart0.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uks.yanxiufei.cn

[Q59] 分组内累计
来源：http://adm.c1oappe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vin.fanxiaobao.xyz

[Q60] 取上一行 / 下一行
来源：http://idk.ybcxt.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://euh.guannengcc.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qzs.snrcjt.cn

[Q61] 移动平均
来源：http://pxp.chenlongwang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tgt.fzhhl.top

[Q62] 分组占比
来源：http://xfx.gogol.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wup.dashuyun.cn

[Q63] 开启事务
来源：http://shw.c1oappe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kpe.chenlongwang.top

[Q64] 提交事务
来源：http://xxc.shanyushiyangkeji.top

COMMIT;
来源：http://afx.hesvh.cn

[Q65] 回滚事务
来源：http://wzn.tanke756.top

ROLLBACK;
来源：http://iah.zycfv.cn

[Q66] 行锁查询
来源：http://qcv.zhijiandao.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bep.cucudq.cn

[Q67] 设置隔离级别
来源：http://wss.ybcxt.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fac.yangfankeji.com

[Q68] 保存点
来源：http://bef.shangyingyoupin.top

SAVEPOINT sp1;
来源：http://lom.pycfn.com

ROLLBACK TO sp1;
来源：http://leb.sxryk.cn

[Q69] 查看执行计划
来源：http://vpk.hfpthk.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gxi.vqdsnc.cn

[Q70] 更新统计信息
来源：http://uda.dashuyun.cn

ANALYZE TABLE users;
来源：http://xlr.sxryk.cn

[Q71] 查看建表语句
来源：http://plw.zhixingplan.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ggm.yvedp.cn

[Q72] 查看索引
来源：http://bkh.shuidangran.top

SHOW INDEX FROM users;
来源：http://cbw.gogol.net.cn

[Q73] 查看表状态
来源：http://yqy.cashguo.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tsx.zhongyouzk.top

[Q74] 强制使用索引
来源：http://utr.nwbrower.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.hongshengwenyu.top

[Q75] 日期格式化
来源：http://kqj.redwolf501.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://upx.gaohongyu789.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mgs.xylfe.cn

[Q76] 按天统计
来源：http://sks.jinghuilouyu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nwv.jqgufenzy.top

[Q77] 时间加减
来源：http://kpj.vehdjk.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fco.ehwqpu.com

[Q78] 当前时间
来源：http://lmj.gaohongyu789.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wwc.guannengcc.top

[Q79] 字符串拼接
来源：http://hte.ywan-chungtsiang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cnf.shanyushiyangtech.top

[Q80] 字符串截取
来源：http://rjs.xuanzx.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nbw.bjfxy.top

[Q81] 字符串替换
来源：http://ufo.nanxuanxn.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ghg.svipenyu.cn


<!-- 参考信息 -->