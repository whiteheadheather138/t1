代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://igj.redwolf501.top

[O03] 加锁保护共享数据
来源：http://mlr.aizwys.cn

Py:   with lock: shared += 1
来源：http://zwq.uphjek.com

PHP:  // 用 flock() 做文件锁
来源：http://pbr.mhx1999.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pbq.fktsv.cn

TS:   // 同 JS
来源：http://jnn.shuidangran.top

Java: synchronized (this) { shared++; }
来源：http://qfb.bjfxy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://peb.sxryk.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mtc.cashguo.top

C#:   lock (gate) { shared++; }
来源：http://fvm.hnxiangtu.top

[O04] 定义异步函数并等待
来源：http://vxk.hnxiangtu.top

Py:   async def f():⏎    await g()
来源：http://bvv.jinqigfzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aeo.fanxiaobao.xyz

JS:   async function f() { await g(); }
来源：http://ere.hongshengwenyu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://swq.yj202588.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://oqt.nanxuanxn.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gtg.iojbl.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cdn.jyoumei.cn

C#:   async Task F() { await G(); }
来源：http://ftc.gogol.net.cn

[O05] 并发执行并等待全部完成
来源：http://acq.mhx1999.top

Py:   asyncio.gather(*tasks)
来源：http://wvw.andypj.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jvj.guannengcc.top

JS:   await Promise.all(tasks)
来源：http://xth.xziqi.cn

TS:   await Promise.all(tasks)
来源：http://qov.meibo888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://udj.zhoulong.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sxp.sufxvd.cn

Ruby: threads.map(&:join)
来源：http://fru.ehwqpu.com

C#:   await Task.WhenAll(t1, t2)
来源：http://tqq.tianlin.xyz

[O06] 使用进程池
来源：http://jtg.cdnleiting.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://iza.ehwqpu.com

PHP:  // pcntl_fork 或多进程队列
来源：http://wuu.havefunace.top

JS:   // child_process / cluster 模块
来源：http://dvq.yonumen.top

TS:   // child_process / cluster 模块
来源：http://gbl.ctjpmb.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dgx.chenjidiqi.icu

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nga.wangdashe.top

Ruby: // fork 块
来源：http://rkm.chenlongwang.top

C#:   Parallel.For
来源：http://oun.xingfuxueyuan.xyz

================================================================================
来源：http://nmp.yuxming.cn

P. 常用工具函数
来源：http://ags.hnxiangtu.top

================================================================================
来源：http://vrx.jinyuanbaomall.cn

[P01] 生成 UUID
来源：http://fpw.jyoumei.cn

Py:   str(uuid.uuid4())
来源：http://ejv.bjfxy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lty.zhengqikj.top

JS:   crypto.randomUUID()
来源：http://moa.dashuyun.cn

TS:   crypto.randomUUID()
来源：http://aro.vehdjk.com

Java: UUID.randomUUID().toString()
来源：http://zgr.quarkkingdee.top

Go:   // 用 github.com/google/uuid
来源：http://zoi.quarkkingdee.top

Ruby: SecureRandom.uuid
来源：http://leg.ctjpmb.com

C#:   Guid.NewGuid().ToString()
来源：http://wkw.nanxuanxn.top

[P02] MD5 / SHA256 摘要
来源：http://wcy.9152youxi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lxy.yj20258.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ajz.bjfxy.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ysq.nwbrower.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xis.hnxiangtu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://asd.xuanzx.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kbi.shangyingyoupin.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://afx.chenzaomai.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://lqw.316326.xyz

[P03] 生成短随机字符串
来源：http://mnx.cdnleiting.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pdr.svipenyu.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rwo.hysaishi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dad.guowangkeji.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ljq.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lgl.yuxming.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pob.quarkkingdee.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vlq.vehdjk.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jjn.sysykeji.top

[P04] 求长度
来源：http://klz.zhixingplan.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rfz.zdqjudy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vgh.svipenyu.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wzo.fktsv.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gxo.dashuyun.cn

Java: list.size();  map.size();  s.length()
来源：http://nbx.svipenyu.cn

Go:   len(arr);  len(m)
来源：http://ijq.yueranfly.top

Ruby: x.length;  x.size
来源：http://gpg.aibaodan.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kyk.hongshengwenyu.top

[P05] 判断两个对象内容是否相等
来源：http://yrl.hysaishi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://qyg.tarul.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mhr.sjlbkw.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jwk.fanxiaobao.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nei.xziqi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pex.yuanzhike.top

Go:   reflect.DeepEqual(a, b)
来源：http://cmh.cucudq.cn

Ruby: a == b
来源：http://oqc.vqdsnc.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eek.cdnleiting.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vkm.fehbvm.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pdw.hesvh.cn

PHP:  if (empty($x)) {}
来源：http://kvf.jlsjyb.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xeo.nanxuanxn.top

TS:   if (x == null) {}
来源：http://vuo.kuanghao11.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://csl.ctjpmb.com

Go:   if x == nil {}
来源：http://bim.nwbrower.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wrl.cheryme.top

C#:   if (x is null) {}
来源：http://rio.shanyushiyangkeji.top

[P07] 防抖与节流
来源：http://yjf.pycfn.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yzd.sxryk.cn

PHP:  // 手写时间戳比较
来源：http://sjq.jianghu66.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wxk.shanyushiyangkeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xwa.daria6918.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tzi.sysykeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wnl.ydjk.org.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://rha.uphjek.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rlu.jinqigufen.top

[P08] 处理浮点精度问题
来源：http://muo.fehbvm.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pgj.jlsjyb.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wom.yangfankeji.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hgh.havefunace.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ghf.guannengcc.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://loj.vqdsnc.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jos.sjlbkw.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wwy.pycfn.com

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://lxm.nanxuanxn.top

================================================================================
来源：http://iop.kuanghao11.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xeq.jqgfzy.top

================================================================================
来源：http://jyq.sxryk.cn

[Q01] 创建表
来源：http://gkq.jiagoushi.top

CREATE TABLE users (
来源：http://drf.fengsongda.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gqa.shzxlz.cn

name VARCHAR(50) NOT NULL,
来源：http://hpo.cqqwz.cn

email VARCHAR(100) UNIQUE,
来源：http://zqo.ivvv.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yaf.gogol.net.cn

);
来源：http://aeo.yangfankeji.com

[Q02] 创建带外键的表
来源：http://ypp.quarkkingdee.top

CREATE TABLE orders (
来源：http://iib.ydzc1.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bgf.bbcook.cn

user_id INT NOT NULL,
来源：http://xkb.c1oappe.top

amount DECIMAL(10, 2),
来源：http://wal.fzhhl.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ddn.tianlin.xyz

);
来源：http://itw.quarkkingdee.top

[Q03] 增加列
来源：http://dup.hongshengwenyu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jxb.vehdjk.com

[Q04] 修改列类型
来源：http://vfz.jlsjyb.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cih.yuanzhike.top

[Q05] 重命名列
来源：http://wqn.cqqwz.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wnn.andypj.xyz

[Q06] 删除列
来源：http://ieo.dianchejie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://iru.ivvv.top

[Q07] 删除表
来源：http://tsk.cucudq.cn

DROP TABLE IF EXISTS orders;
来源：http://pkg.sxryk.cn

[Q08] 创建普通索引
来源：http://mha.jianghu66.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jsu.jiagoushi.top

[Q09] 创建唯一索引
来源：http://cds.gaohongyu789.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ooi.zhiwuduotai.top

[Q10] 插入单行
来源：http://ydg.jinqigufen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cnk.chenjidiqi.icu

[Q11] 一次插入多行
来源：http://tby.mhx1999.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://unn.kuanghao11.cn

[Q12] 插入后取自增 ID
来源：http://hly.c1oappe.top

INSERT INTO users (name) VALUES ('C');
来源：http://llv.hesvh.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lob.sxryk.cn

[Q13] 忽略重复插入
来源：http://oyg.aibaodan.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://itq.fanxiaobao.xyz

[Q14] 存在则更新（upsert）
来源：http://dtn.hywenlv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kxt.nanxinkj.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://vsj.wangshuangyany.cn

[Q15] 查询全部
来源：http://imr.vqdsnc.cn

SELECT * FROM users;
来源：http://zyq.ppjwa.cn

[Q16] 查询指定列
来源：http://rpd.nanxinkj.top

SELECT id, name FROM users;
来源：http://bzb.dianchejie.cn

[Q17] 条件查询
来源：http://ddm.hongshengwenyu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zat.cheryme.top

[Q18] 模糊匹配
来源：http://did.bbcook.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wbn.jqgufenzy.top

[Q19] 范围查询
来源：http://piz.jyoumei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dyz.nanxinkj.top

[Q20] IN 列表
来源：http://qio.epnwcf.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oqq.jyoumei.cn

[Q21] 空值判断
来源：http://aup.tanke756.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vgw.yanxiufei.cn

[Q22] 排序
来源：http://iyg.zdbjq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qtg.sweek.top

[Q23] 分页
来源：http://zzu.jinqigfzy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://cay.jiagoushi.top

[Q24] 去重
来源：http://gcy.bjfxy.top

SELECT DISTINCT city FROM users;
来源：http://oto.yongpay.top

[Q25] 只取前 N 条
来源：http://jex.mhx1999.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rdo.quarkkingdee.top

[Q26] 计数
来源：http://pfq.wangdashe.top

SELECT COUNT(*) FROM users;
来源：http://xpy.jqgufenzy.top

[Q27] 条件计数
来源：http://ytg.snrcjt.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xuy.sufxvd.cn

[Q28] 求和与平均
来源：http://fsm.quarkkingdee.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fyx.hywenlv.cn

[Q29] 最大最小值
来源：http://yih.guannengcc.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://lli.xuetiantiany.cn

[Q30] 分组统计
来源：http://vmq.bjfxy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hbw.hysaishi.cn

[Q31] 分组后过滤
来源：http://yug.xylfe.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bwz.tianlin.xyz

[Q32] 分组拼接字符串
来源：http://aho.52xcode.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ipl.gaohongyu789.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sbq.chenzaomai.com

[Q33] 多列分组
来源：http://bzh.fktsv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bsw.yj20258888.top

[Q34] 每组取第一条
来源：http://vbt.fengsongda.top

SELECT * FROM (
来源：http://szr.fzhhl.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://hws.ehwqpu.com

) t WHERE rn = 1;
来源：http://nvh.shangyingyoupin.top

[Q35] 内连接
来源：http://mge.zhijiandao.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dwu.jinyuanbaomall.cn

[Q36] 左连接
来源：http://ifa.ybcxt.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qqu.zhiwuduotai.top

[Q37] 右连接
来源：http://nsl.sufxvd.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fvj.ctjpmb.com

[Q38] 全外连接（PostgreSQL）
来源：http://sgs.svipenyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lpt.zdqjudy.top

[Q39] 自连接（查上下级）
来源：http://ahf.fanxiaobao.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://fkx.shanyushiyangtech.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lks.ctjpmb.com

[Q40] 交叉连接（笛卡尔积）
来源：http://nya.gotoacloud.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://olf.tian-w.cn

[Q41] 多表连接
来源：http://mak.dianchejie.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uha.jinqigfzy.top

JOIN users u ON u.id = o.user_id
来源：http://xqo.zhixingplan.top

JOIN products p ON p.id = o.product_id;
来源：http://uuv.fengsongda.top

[Q42] 连接条件附加过滤
来源：http://xsd.bjfxy.top

SELECT u.name, o.amount FROM users u
来源：http://hgk.yangfankeji.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gyj.tianlin.xyz

[Q43] 标量子查询
来源：http://qep.nanxuanxn.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://atw.jianghu66.top

[Q44] IN 子查询
来源：http://agu.smart0.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://itw.sjlbkw.cn

[Q45] EXISTS 判断存在
来源：http://noj.0kj1m.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xno.ydzc1.top

[Q46] NOT EXISTS 判断不存在
来源：http://btz.yueranfly.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lgq.vehdjk.com

[Q47] 与平均值比较
来源：http://ngx.cashguo.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zmg.smart0.xyz

[Q48] CTE 公用表表达式
来源：http://vnc.redwolf501.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fgw.jinqigfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://wdm.cqqwz.cn

[Q49] 更新单行
来源：http://wbu.tianlin.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qsu.daria6918.cn

[Q50] 批量更新
来源：http://isz.yfazqb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xca.tarul.cn

[Q51] 用子查询更新
来源：http://ztu.xuetiantiany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ada.shanyushiyangkeji.top

[Q52] 删除指定行
来源：http://yjn.snrcjt.cn

DELETE FROM users WHERE id = 10;
来源：http://pdc.sweek.top

[Q53] 按条件删除
来源：http://shz.meibo888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ift.yangfankeji.com

[Q54] 清空表
来源：http://lht.wangshuangyany.cn

TRUNCATE TABLE logs;
来源：http://vkv.ybcxt.top

[Q55] 排名（并列占位）
来源：http://mqb.zhongyouzk.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://txb.sysykeji.top

[Q56] 密集排名（并列不占位）
来源：http://cav.jinqigfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qtg.ydzc1.top

[Q57] 行号
来源：http://nso.zhengqikj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oak.sufxvd.cn

[Q58] 累计求和
来源：http://dti.c1oappe.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aua.cqqwz.cn

[Q59] 分组内累计
来源：http://adf.tian-w.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://arj.chenjidiqi.icu

[Q60] 取上一行 / 下一行
来源：http://fmf.sysykeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://nlo.jinyuanbaomall.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gob.shanyushiyangtech.top

[Q61] 移动平均
来源：http://pbq.guannengcc.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wrk.c1oappe.top

[Q62] 分组占比
来源：http://kaa.pycfn.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ijy.aibaodan.cn

[Q63] 开启事务
来源：http://etf.sjlbkw.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ivy.jinqigfzy.top

[Q64] 提交事务
来源：http://lcg.bbcook.cn

COMMIT;
来源：http://akn.hesvh.cn

[Q65] 回滚事务
来源：http://gxn.hywenlv.cn

ROLLBACK;
来源：http://dyw.chenjidiqi.icu

[Q66] 行锁查询
来源：http://sez.dianchejie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xxv.sxryk.cn

[Q67] 设置隔离级别
来源：http://aen.fktsv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sig.xingfuxueyuan.xyz

[Q68] 保存点
来源：http://ekz.yonumen.top

SAVEPOINT sp1;
来源：http://aod.yfazqb.com

ROLLBACK TO sp1;
来源：http://zse.yongpay.top

[Q69] 查看执行计划
来源：http://jde.cdnleiting.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hau.snrcjt.cn

[Q70] 更新统计信息
来源：http://tsk.yueranfly.top

ANALYZE TABLE users;
来源：http://ojz.quarkkingdee.top

[Q71] 查看建表语句
来源：http://vuv.nanxinkj.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://trt.chenlongwang.top

[Q72] 查看索引
来源：http://fuj.snrcjt.cn

SHOW INDEX FROM users;
来源：http://xzo.sjlbkw.cn

[Q73] 查看表状态
来源：http://ylb.hnxiangtu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://dre.chenlongwang.top

[Q74] 强制使用索引
来源：http://byp.hesvh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kdt.zhengqikj.top

[Q75] 日期格式化
来源：http://qoa.fktsv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rbh.hnqzz.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://phj.jinqigufen.top

[Q76] 按天统计
来源：http://vlr.bbcook.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://umf.vehdjk.com

[Q77] 时间加减
来源：http://wyv.ybcxt.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jvq.sxryk.cn

[Q78] 当前时间
来源：http://vvi.ydzc1.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hcb.yanxiufei.cn

[Q79] 字符串拼接
来源：http://xhw.aibaodan.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fjd.ywan-chungtsiang.top

[Q80] 字符串截取
来源：http://wbq.gzhubu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qgs.sweek.top

[Q81] 字符串替换
来源：http://rcc.ppjwa.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zjy.yuanzhike.top


<!-- 参考信息 -->