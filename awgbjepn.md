代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://aru.ydjk.org.cn

[O03] 加锁保护共享数据
来源：http://xgm.yj202588.top

Py:   with lock: shared += 1
来源：http://yth.zhiwuduotai.top

PHP:  // 用 flock() 做文件锁
来源：http://nur.daxiang520.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wcj.hesvh.cn

TS:   // 同 JS
来源：http://zzl.sjlbkw.cn

Java: synchronized (this) { shared++; }
来源：http://oem.fehbvm.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bhi.ywan-chungtsiang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ppy.shuidangran.top

C#:   lock (gate) { shared++; }
来源：http://hgh.hammf.cn

[O04] 定义异步函数并等待
来源：http://sgf.cucudq.cn

Py:   async def f():⏎    await g()
来源：http://mrk.yj20258888.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fqo.jinghuilouyu.cn

JS:   async function f() { await g(); }
来源：http://zov.gotoacloud.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://dwh.meibo888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://neb.snrcjt.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hmg.zdqjudy.top

Ruby: # 用 Fiber 或 async gem
来源：http://ype.andypj.xyz

C#:   async Task F() { await G(); }
来源：http://nup.shuidangran.top

[O05] 并发执行并等待全部完成
来源：http://prw.zhoulong.xyz

Py:   asyncio.gather(*tasks)
来源：http://zwd.c1oappe.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dxl.ydzc1.top

JS:   await Promise.all(tasks)
来源：http://bef.jqgfzy.top

TS:   await Promise.all(tasks)
来源：http://rnu.yuanzhike.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://syd.tanke756.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kas.cucudq.cn

Ruby: threads.map(&:join)
来源：http://zmb.fzhhl.top

C#:   await Task.WhenAll(t1, t2)
来源：http://puh.yonumen.top

[O06] 使用进程池
来源：http://efi.tianlin.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://his.snrcjt.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ryk.zhijiandao.cn

JS:   // child_process / cluster 模块
来源：http://fpk.aibaodan.cn

TS:   // child_process / cluster 模块
来源：http://wyw.guowangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qnw.daria6918.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ust.jinghuilouyu.cn

Ruby: // fork 块
来源：http://nzc.jinqigufen.top

C#:   Parallel.For
来源：http://vzw.c1oappe.top

================================================================================
来源：http://lnx.yfazqb.com

P. 常用工具函数
来源：http://pyc.shzxlz.cn

================================================================================
来源：http://ftm.redwolf501.top

[P01] 生成 UUID
来源：http://dsj.gogol.net.cn

Py:   str(uuid.uuid4())
来源：http://vgr.jqgfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oct.52xcode.cn

JS:   crypto.randomUUID()
来源：http://ghy.nanxinkj.top

TS:   crypto.randomUUID()
来源：http://wnu.ivvv.top

Java: UUID.randomUUID().toString()
来源：http://jud.jinqigfzy.top

Go:   // 用 github.com/google/uuid
来源：http://frr.quarkkingdee.top

Ruby: SecureRandom.uuid
来源：http://rfs.sweek.top

C#:   Guid.NewGuid().ToString()
来源：http://esr.ivvv.top

[P02] MD5 / SHA256 摘要
来源：http://ywx.hnxiangtu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mzy.gaohongyu789.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jaz.hywenlv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://emk.sjlbkw.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ldm.jqgfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://lew.52xcode.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://obh.xingfuxueyuan.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://rbg.gaohongyu789.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ovr.ppjwa.cn

[P03] 生成短随机字符串
来源：http://ugc.yangfankeji.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xox.yongpay.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rcl.shanyushiyangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ynf.shangyingyoupin.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pic.pycfn.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xxr.ybcxt.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://klq.hnqzz.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://aam.jqgfzy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://lin.vehdjk.com

[P04] 求长度
来源：http://fja.sjlbkw.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://szv.fzhhl.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zls.jqgufenzy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ywk.hnqzz.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bxb.yj202588.top

Java: list.size();  map.size();  s.length()
来源：http://igp.yj20258888.top

Go:   len(arr);  len(m)
来源：http://cqf.jyoumei.cn

Ruby: x.length;  x.size
来源：http://ksp.ywan-chungtsiang.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://bwx.yvedp.cn

[P05] 判断两个对象内容是否相等
来源：http://pkc.zhoulong.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://eci.quarkkingdee.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ndc.yongpay.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://czu.ivvv.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nxl.dianchejie.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://usn.nwbrower.top

Go:   reflect.DeepEqual(a, b)
来源：http://gip.c1oappe.top

Ruby: a == b
来源：http://suy.tarul.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dwc.hesvh.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kyq.ppjwa.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://cca.ppjwa.cn

PHP:  if (empty($x)) {}
来源：http://aap.hfpthk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://eqf.wangdashe.top

TS:   if (x == null) {}
来源：http://muo.iojbl.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://hbu.kuanghao11.cn

Go:   if x == nil {}
来源：http://zex.jinyuanbaomall.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gwi.cqqwz.cn

C#:   if (x is null) {}
来源：http://bvi.feifeiyinyue.top

[P07] 防抖与节流
来源：http://ema.xuanzx.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hfq.jinghuilouyu.cn

PHP:  // 手写时间戳比较
来源：http://ojn.redwolf501.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rgn.ywan-chungtsiang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bom.shangyingyoupin.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://pmc.shanyushiyangtech.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://tqx.svipenyu.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://pcq.jinyuanbaomall.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yyj.zdqjudy.top

[P08] 处理浮点精度问题
来源：http://sak.wangdashe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://awu.zdbjq.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://zei.ivvv.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gjd.shzxlz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mgd.epnwcf.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://gsz.zhengqikj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://aom.zhongyouzk.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sew.aibaodan.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rto.316326.xyz

================================================================================
来源：http://qsa.yueranfly.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://epd.jianghu66.top

================================================================================
来源：http://bpo.snrcjt.cn

[Q01] 创建表
来源：http://naw.hnxiangtu.top

CREATE TABLE users (
来源：http://kns.bjfxy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gbg.xingfuxueyuan.xyz

name VARCHAR(50) NOT NULL,
来源：http://ecf.zhengqikj.top

email VARCHAR(100) UNIQUE,
来源：http://mpw.hnxiangtu.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://glv.zhiwuduotai.top

);
来源：http://xkl.hammf.cn

[Q02] 创建带外键的表
来源：http://ahk.sjlbkw.cn

CREATE TABLE orders (
来源：http://chr.fanxiaobao.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zis.snrcjt.cn

user_id INT NOT NULL,
来源：http://jcp.tarul.cn

amount DECIMAL(10, 2),
来源：http://rbh.yangfankeji.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://say.cdnleiting.top

);
来源：http://dle.zhaomingkeji.xyz

[Q03] 增加列
来源：http://yhx.zhongyouzk.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://tem.sweek.top

[Q04] 修改列类型
来源：http://npn.tarul.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://lbr.cucudq.cn

[Q05] 重命名列
来源：http://gil.zhijiandao.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fwm.hywenlv.cn

[Q06] 删除列
来源：http://uqi.gotoacloud.top

ALTER TABLE users DROP COLUMN age;
来源：http://ehh.hywenlv.cn

[Q07] 删除表
来源：http://mnb.xylfe.cn

DROP TABLE IF EXISTS orders;
来源：http://fya.xinyue.icu

[Q08] 创建普通索引
来源：http://mbx.aibaodan.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kvn.dashuyun.cn

[Q09] 创建唯一索引
来源：http://zsa.uphjek.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fme.zhaomingkeji.xyz

[Q10] 插入单行
来源：http://pca.redwolf501.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zzo.jinghuilouyu.cn

[Q11] 一次插入多行
来源：http://vyq.shangyingyoupin.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iaq.sjlbkw.cn

[Q12] 插入后取自增 ID
来源：http://jff.tianlin.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://jir.ywan-chungtsiang.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bmo.gzhubu.top

[Q13] 忽略重复插入
来源：http://dln.tarul.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vwt.xinyue.icu

[Q14] 存在则更新（upsert）
来源：http://xtn.sysykeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sxh.gaohongyu789.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mxy.snrcjt.cn

[Q15] 查询全部
来源：http://aqg.jqgfzy.top

SELECT * FROM users;
来源：http://seo.sysykeji.top

[Q16] 查询指定列
来源：http://tok.guannengcc.top

SELECT id, name FROM users;
来源：http://gvw.chenzaomai.com

[Q17] 条件查询
来源：http://lkl.tarul.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bfi.sxryk.cn

[Q18] 模糊匹配
来源：http://zea.bjfxy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ysc.hfpthk.cn

[Q19] 范围查询
来源：http://pdx.sweek.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jlw.jinyuanbaomall.cn

[Q20] IN 列表
来源：http://wek.yuxming.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hbj.chenjidiqi.icu

[Q21] 空值判断
来源：http://dnk.cheryme.top

SELECT * FROM users WHERE email IS NULL;
来源：http://hhp.chenlongwang.top

[Q22] 排序
来源：http://cjg.vehdjk.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tsk.hnqzz.top

[Q23] 分页
来源：http://vah.nwbrower.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://faa.shuidangran.top

[Q24] 去重
来源：http://bbd.sufxvd.cn

SELECT DISTINCT city FROM users;
来源：http://hjz.hesvh.cn

[Q25] 只取前 N 条
来源：http://uca.fengsongda.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jab.nwbrower.top

[Q26] 计数
来源：http://qkp.9152youxi.cn

SELECT COUNT(*) FROM users;
来源：http://sgj.jinghuilouyu.cn

[Q27] 条件计数
来源：http://aud.yuxming.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://eco.c1oappe.top

[Q28] 求和与平均
来源：http://llg.ydjk.org.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hgj.cucudq.cn

[Q29] 最大最小值
来源：http://mbh.svipenyu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vfw.ehwqpu.com

[Q30] 分组统计
来源：http://oao.jyoumei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fov.quarkkingdee.top

[Q31] 分组后过滤
来源：http://wvv.c1oappe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mdp.tarul.cn

[Q32] 分组拼接字符串
来源：http://jjh.yuxming.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gao.xingfuxueyuan.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pvo.mhx1999.top

[Q33] 多列分组
来源：http://kqd.gaohongyu789.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://boy.hnqzz.top

[Q34] 每组取第一条
来源：http://mpd.pengpengdd.cyou

SELECT * FROM (
来源：http://iif.zhijiandao.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://csf.cashguo.top

) t WHERE rn = 1;
来源：http://xxs.shanyushiyangkeji.top

[Q35] 内连接
来源：http://cpg.jqgfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kma.yj20258.top

[Q36] 左连接
来源：http://xfa.havefunace.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jrt.jqgufenzy.top

[Q37] 右连接
来源：http://wsi.feifeiyinyue.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wjs.zhijiandao.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vsp.ywan-chungtsiang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bts.ydzc1.top

[Q39] 自连接（查上下级）
来源：http://wpe.zhoulong.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://pay.bjfxy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wrv.ywan-chungtsiang.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zpr.yangfankeji.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bpg.fzhhl.top

[Q41] 多表连接
来源：http://jsp.gogol.net.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://xax.xuanzx.com

JOIN users u ON u.id = o.user_id
来源：http://tuo.bjfxy.top

JOIN products p ON p.id = o.product_id;
来源：http://gvb.xinyue.icu

[Q42] 连接条件附加过滤
来源：http://grs.316326.xyz

SELECT u.name, o.amount FROM users u
来源：http://jpj.pycfn.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ryt.birdmap.top

[Q43] 标量子查询
来源：http://qsx.guannengcc.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uco.yueranfly.top

[Q44] IN 子查询
来源：http://nff.xinyue.icu

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hfr.52xcode.cn

[Q45] EXISTS 判断存在
来源：http://ihk.sjlbkw.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://itp.sweek.top

[Q46] NOT EXISTS 判断不存在
来源：http://jnj.zhiwuduotai.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nue.ctjpmb.com

[Q47] 与平均值比较
来源：http://eor.ydzc1.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://drp.jinqigufen.top

[Q48] CTE 公用表表达式
来源：http://wcz.ivvv.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sbg.gotoacloud.top

SELECT * FROM t WHERE c > 5;
来源：http://eil.wangdashe.top

[Q49] 更新单行
来源：http://jlr.daxiang520.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sgv.tian-w.cn

[Q50] 批量更新
来源：http://ynh.bjfxy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nky.hnxiangtu.top

[Q51] 用子查询更新
来源：http://hfr.cucudq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sgl.shzxlz.cn

[Q52] 删除指定行
来源：http://sxq.sxryk.cn

DELETE FROM users WHERE id = 10;
来源：http://nli.shangyingyoupin.top

[Q53] 按条件删除
来源：http://amp.chenzaomai.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cdi.xylfe.cn

[Q54] 清空表
来源：http://kyz.zhijiandao.cn

TRUNCATE TABLE logs;
来源：http://rbx.ydzc1.top

[Q55] 排名（并列占位）
来源：http://otd.xinyue.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://atz.ydzc1.top

[Q56] 密集排名（并列不占位）
来源：http://ykz.yvedp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://cut.cqqwz.cn

[Q57] 行号
来源：http://gvk.guannengcc.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pot.0kj1m.cn

[Q58] 累计求和
来源：http://zly.shangyingyoupin.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://onb.hfpthk.cn

[Q59] 分组内累计
来源：http://lbx.sweek.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vfm.yfazqb.com

[Q60] 取上一行 / 下一行
来源：http://dqo.hfpthk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ukc.aibaodan.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xnm.yongpay.top

[Q61] 移动平均
来源：http://izd.tian-w.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gct.hnqzz.top

[Q62] 分组占比
来源：http://adb.wangdashe.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://asd.hywenlv.cn

[Q63] 开启事务
来源：http://mwr.redwolf501.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kbw.yanxiufei.cn

[Q64] 提交事务
来源：http://tvs.tanke756.top

COMMIT;
来源：http://liq.zhijiandao.cn

[Q65] 回滚事务
来源：http://kbl.aibaodan.cn

ROLLBACK;
来源：http://pjt.ydjk.org.cn

[Q66] 行锁查询
来源：http://ktn.havefunace.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ish.fzhhl.top

[Q67] 设置隔离级别
来源：http://ztt.fehbvm.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hrl.fehbvm.com

[Q68] 保存点
来源：http://ily.dianchejie.cn

SAVEPOINT sp1;
来源：http://vow.xylfe.cn

ROLLBACK TO sp1;
来源：http://dhj.hfpthk.cn

[Q69] 查看执行计划
来源：http://ofi.jianghu66.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gnv.mhx1999.top

[Q70] 更新统计信息
来源：http://goz.redwolf501.top

ANALYZE TABLE users;
来源：http://avo.ybcxt.top

[Q71] 查看建表语句
来源：http://ljr.daria6918.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yez.jinghuilouyu.cn

[Q72] 查看索引
来源：http://zqh.shanyushiyangtech.top

SHOW INDEX FROM users;
来源：http://fji.xuetiantiany.cn

[Q73] 查看表状态
来源：http://vct.aizwys.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xcy.daxiang520.top

[Q74] 强制使用索引
来源：http://cqu.pycfn.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vit.cqqwz.cn

[Q75] 日期格式化
来源：http://icj.ybcxt.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dqz.jqgufenzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ykx.ydjk.org.cn

[Q76] 按天统计
来源：http://bea.shangyingyoupin.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yak.xuetiantiany.cn

[Q77] 时间加减
来源：http://fmj.c1oappe.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://pcx.chenjidiqi.icu

[Q78] 当前时间
来源：http://wlc.aibaodan.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zqo.pengpengdd.cyou

[Q79] 字符串拼接
来源：http://onm.fehbvm.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xio.epnwcf.com

[Q80] 字符串截取
来源：http://ivh.tian-w.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vwi.ppjwa.cn

[Q81] 字符串替换
来源：http://dqe.zdqjudy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vpf.zhaomingkeji.xyz


<!-- 参考信息 -->