代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mzn.chenlongwang.top

TS:   // 同 JS
来源：http://glv.mhx1999.top

Java: synchronized (this) { shared++; }
来源：http://fpe.wangshuangyany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://piw.cqqwz.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://lia.ywan-chungtsiang.top

C#:   lock (gate) { shared++; }
来源：http://evb.pengpengdd.cyou

[O04] 定义异步函数并等待
来源：http://ukq.9152youxi.cn

Py:   async def f():⏎    await g()
来源：http://joz.chenlongwang.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://otn.meibo888.top

JS:   async function f() { await g(); }
来源：http://wwy.jiagoushi.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hhd.xylfe.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://syj.ctjpmb.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://avx.xziqi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rpo.ydzc1.top

C#:   async Task F() { await G(); }
来源：http://efo.guowangkeji.top

[O05] 并发执行并等待全部完成
来源：http://gwa.jinghuilouyu.cn

Py:   asyncio.gather(*tasks)
来源：http://kdn.aizwys.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tur.shanyushiyangkeji.top

JS:   await Promise.all(tasks)
来源：http://joi.ppjwa.cn

TS:   await Promise.all(tasks)
来源：http://cfz.ctjpmb.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lqk.meibo888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ptw.gaohongyu789.top

Ruby: threads.map(&:join)
来源：http://ohw.tianlin.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://swu.yuxming.cn

[O06] 使用进程池
来源：http://dxo.yuxming.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://foq.jinghuilouyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yhe.hammf.cn

JS:   // child_process / cluster 模块
来源：http://prf.316326.xyz

TS:   // child_process / cluster 模块
来源：http://fdn.jiagoushi.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jle.fengsongda.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ajk.andypj.xyz

Ruby: // fork 块
来源：http://obl.yvedp.cn

C#:   Parallel.For
来源：http://wpr.tianlin.xyz

================================================================================
来源：http://syl.ctjpmb.com

P. 常用工具函数
来源：http://mtk.chenlongwang.top

================================================================================
来源：http://lqz.gotoacloud.top

[P01] 生成 UUID
来源：http://ork.yuxming.cn

Py:   str(uuid.uuid4())
来源：http://ybh.gotoacloud.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kkw.ydjk.org.cn

JS:   crypto.randomUUID()
来源：http://rfv.jinyuanbaomall.cn

TS:   crypto.randomUUID()
来源：http://gty.jinqigufen.top

Java: UUID.randomUUID().toString()
来源：http://uoq.cheryme.top

Go:   // 用 github.com/google/uuid
来源：http://znh.smart0.xyz

Ruby: SecureRandom.uuid
来源：http://mer.sufxvd.cn

C#:   Guid.NewGuid().ToString()
来源：http://eef.wangshuangyany.cn

[P02] MD5 / SHA256 摘要
来源：http://pft.jinghuilouyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lyt.guowangkeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://aeh.ehwqpu.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wqw.pengpengdd.cyou

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://iul.sxryk.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tiv.mhx1999.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xxo.bjfxy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ruc.hongshengwenyu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vxb.sufxvd.cn

[P03] 生成短随机字符串
来源：http://hbt.shangyingyoupin.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mru.zhiwuduotai.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zip.zhaomingkeji.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bkk.gzhubu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bqi.hongshengwenyu.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nsg.fzhhl.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://koh.zhijiandao.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ghx.xinyue.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://too.jyoumei.cn

[P04] 求长度
来源：http://wvz.ctjpmb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gue.ybcxt.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qcm.fanxiaobao.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://swe.hnxiangtu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nie.xingfuxueyuan.xyz

Java: list.size();  map.size();  s.length()
来源：http://bwj.ydzc1.top

Go:   len(arr);  len(m)
来源：http://pbt.jqgfzy.top

Ruby: x.length;  x.size
来源：http://bgi.fktsv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://kws.jianghu66.top

[P05] 判断两个对象内容是否相等
来源：http://awi.aibaodan.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://fle.zhengqikj.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jaa.tarul.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://epm.yfazqb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cbh.epnwcf.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vgb.svipenyu.cn

Go:   reflect.DeepEqual(a, b)
来源：http://yhj.yvedp.cn

Ruby: a == b
来源：http://wqg.shzxlz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://swt.dianchejie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://axo.chenlongwang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mcc.fanxiaobao.xyz

PHP:  if (empty($x)) {}
来源：http://swp.mhx1999.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://cpb.fzhhl.top

TS:   if (x == null) {}
来源：http://mzs.sweek.top

Java: if (x == null || x.isEmpty()) {}
来源：http://acl.yueranfly.top

Go:   if x == nil {}
来源：http://gsb.nanxinkj.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qrn.bbcook.cn

C#:   if (x is null) {}
来源：http://mgh.zhixingplan.top

[P07] 防抖与节流
来源：http://szf.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yyl.chenlongwang.top

PHP:  // 手写时间戳比较
来源：http://vmq.cheryme.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vzh.gogol.net.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://por.shzxlz.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://izx.hfpthk.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://pcw.iojbl.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://xzh.epnwcf.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ans.cashguo.top

[P08] 处理浮点精度问题
来源：http://jnp.aizwys.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://fdt.jiagoushi.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://oog.jinyuanbaomall.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tdh.gotoacloud.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rxh.havefunace.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nlg.yuxming.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ahj.c1oappe.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://udk.svipenyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vtd.daxiang520.top

================================================================================
来源：http://gea.xinyue.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gys.xuetiantiany.cn

================================================================================
来源：http://uzp.0kj1m.cn

[Q01] 创建表
来源：http://zdh.shanyushiyangkeji.top

CREATE TABLE users (
来源：http://trf.9152youxi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://kui.yuanzhike.top

name VARCHAR(50) NOT NULL,
来源：http://cig.ydzc1.top

email VARCHAR(100) UNIQUE,
来源：http://qpz.mhx1999.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gcs.nanxinkj.top

);
来源：http://wfc.havefunace.top

[Q02] 创建带外键的表
来源：http://pel.gotoacloud.top

CREATE TABLE orders (
来源：http://lfw.hfpthk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://uvd.mhx1999.top

user_id INT NOT NULL,
来源：http://odp.hnxiangtu.top

amount DECIMAL(10, 2),
来源：http://dly.sysykeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://avj.zycfv.cn

);
来源：http://btc.hysaishi.cn

[Q03] 增加列
来源：http://sza.zycfv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cak.snrcjt.cn

[Q04] 修改列类型
来源：http://xhf.sysykeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xlr.sxryk.cn

[Q05] 重命名列
来源：http://ytr.zhongyouzk.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qwt.yueranfly.top

[Q06] 删除列
来源：http://nhz.tanke756.top

ALTER TABLE users DROP COLUMN age;
来源：http://pzr.zhengqikj.top

[Q07] 删除表
来源：http://vml.vqdsnc.cn

DROP TABLE IF EXISTS orders;
来源：http://leh.xingfuxueyuan.xyz

[Q08] 创建普通索引
来源：http://roc.jqgfzy.top

CREATE INDEX idx_users_email ON users(email);
来源：http://sem.guowangkeji.top

[Q09] 创建唯一索引
来源：http://aam.hnxiangtu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bmg.daxiang520.top

[Q10] 插入单行
来源：http://zkp.jinqigufen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://edl.yj202588.top

[Q11] 一次插入多行
来源：http://bui.dashuyun.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://inu.vehdjk.com

[Q12] 插入后取自增 ID
来源：http://kzl.feifeiyinyue.top

INSERT INTO users (name) VALUES ('C');
来源：http://wrt.zycfv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kwe.chenzaomai.com

[Q13] 忽略重复插入
来源：http://frc.uphjek.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kiz.fengsongda.top

[Q14] 存在则更新（upsert）
来源：http://cob.andypj.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tqw.dashuyun.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qfx.gzhubu.top

[Q15] 查询全部
来源：http://htf.zhijiandao.cn

SELECT * FROM users;
来源：http://lfq.aizwys.cn

[Q16] 查询指定列
来源：http://rhq.52xcode.cn

SELECT id, name FROM users;
来源：http://hlw.zhiwuduotai.top

[Q17] 条件查询
来源：http://yqv.pengpengdd.cyou

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://frj.sxryk.cn

[Q18] 模糊匹配
来源：http://upv.gaohongyu789.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cld.ppjwa.cn

[Q19] 范围查询
来源：http://loy.kuanghao11.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ydc.fengsongda.top

[Q20] IN 列表
来源：http://lxg.pycfn.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ulr.nwbrower.top

[Q21] 空值判断
来源：http://kjh.redwolf501.top

SELECT * FROM users WHERE email IS NULL;
来源：http://cwd.guannengcc.top

[Q22] 排序
来源：http://ruv.hfpthk.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://txr.ehwqpu.com

[Q23] 分页
来源：http://vba.yongpay.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mjs.yueranfly.top

[Q24] 去重
来源：http://sfi.zhijiandao.cn

SELECT DISTINCT city FROM users;
来源：http://iia.gogol.net.cn

[Q25] 只取前 N 条
来源：http://jrs.hysaishi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vbl.wangdashe.top

[Q26] 计数
来源：http://hab.zdbjq.cn

SELECT COUNT(*) FROM users;
来源：http://vat.chenlongwang.top

[Q27] 条件计数
来源：http://skf.bbcook.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://evx.nanxuanxn.top

[Q28] 求和与平均
来源：http://ahs.zycfv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uur.ydzc1.top

[Q29] 最大最小值
来源：http://vck.yongpay.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://lcm.shuidangran.top

[Q30] 分组统计
来源：http://nlb.guannengcc.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gio.xingfuxueyuan.xyz

[Q31] 分组后过滤
来源：http://gyo.fanxiaobao.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://fwk.ydjk.org.cn

[Q32] 分组拼接字符串
来源：http://cob.sjlbkw.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wcn.cqqwz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ena.yj202588.top

[Q33] 多列分组
来源：http://drz.fzhhl.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cub.zhaomingkeji.xyz

[Q34] 每组取第一条
来源：http://zfj.aibaodan.cn

SELECT * FROM (
来源：http://ifz.ivvv.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dmx.pycfn.com

) t WHERE rn = 1;
来源：http://tif.zhoulong.xyz

[Q35] 内连接
来源：http://enz.tarul.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mwz.quarkkingdee.top

[Q36] 左连接
来源：http://wgu.zdbjq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hos.yongpay.top

[Q37] 右连接
来源：http://hnp.yfazqb.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://awx.cucudq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://hir.zhixingplan.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://acc.shzxlz.cn

[Q39] 自连接（查上下级）
来源：http://ang.jlsjyb.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://hqf.svipenyu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://opz.zhongyouzk.top

[Q40] 交叉连接（笛卡尔积）
来源：http://gfu.jinghuilouyu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hjq.vehdjk.com

[Q41] 多表连接
来源：http://gct.ywan-chungtsiang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://oos.yvedp.cn

JOIN users u ON u.id = o.user_id
来源：http://qsq.sxryk.cn

JOIN products p ON p.id = o.product_id;
来源：http://szk.redwolf501.top

[Q42] 连接条件附加过滤
来源：http://ydl.zycfv.cn

SELECT u.name, o.amount FROM users u
来源：http://liy.hywenlv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://okh.yuxming.cn

[Q43] 标量子查询
来源：http://qst.tarul.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ylc.dianchejie.cn

[Q44] IN 子查询
来源：http://eeh.jiagoushi.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mcl.vehdjk.com

[Q45] EXISTS 判断存在
来源：http://xyp.zhixingplan.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fje.ybcxt.top

[Q46] NOT EXISTS 判断不存在
来源：http://leo.yfazqb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://duh.tianlin.xyz

[Q47] 与平均值比较
来源：http://toq.hesvh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rcp.daxiang520.top

[Q48] CTE 公用表表达式
来源：http://ykq.jinghuilouyu.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nhh.zhiwuduotai.top

SELECT * FROM t WHERE c > 5;
来源：http://kgy.yj202588.top

[Q49] 更新单行
来源：http://ikj.shangyingyoupin.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://txw.xingfuxueyuan.xyz

[Q50] 批量更新
来源：http://dvi.svipenyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xos.havefunace.top

[Q51] 用子查询更新
来源：http://njf.cucudq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bss.svipenyu.cn

[Q52] 删除指定行
来源：http://idh.316326.xyz

DELETE FROM users WHERE id = 10;
来源：http://vvp.cashguo.top

[Q53] 按条件删除
来源：http://per.jyoumei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sjm.aibaodan.cn

[Q54] 清空表
来源：http://fev.guowangkeji.top

TRUNCATE TABLE logs;
来源：http://utn.birdmap.top

[Q55] 排名（并列占位）
来源：http://hri.fanxiaobao.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://otk.yj202588.top

[Q56] 密集排名（并列不占位）
来源：http://wut.xziqi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://giw.fengsongda.top

[Q57] 行号
来源：http://rsw.yfazqb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eiw.tian-w.cn

[Q58] 累计求和
来源：http://xyr.zhongyouzk.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mxs.xinyue.icu

[Q59] 分组内累计
来源：http://jir.sysykeji.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kja.guowangkeji.top

[Q60] 取上一行 / 下一行
来源：http://tav.birdmap.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gwq.sweek.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dxy.pycfn.com

[Q61] 移动平均
来源：http://vmg.tarul.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mzi.yj20258888.top

[Q62] 分组占比
来源：http://oiv.cucudq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pce.jiagoushi.top

[Q63] 开启事务
来源：http://ses.hesvh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hch.haohaochexian.top

[Q64] 提交事务
来源：http://knh.fehbvm.com

COMMIT;
来源：http://ndh.jinghuilouyu.cn

[Q65] 回滚事务
来源：http://hrz.yvedp.cn

ROLLBACK;
来源：http://vqt.zhijiandao.cn

[Q66] 行锁查询
来源：http://bnf.aizwys.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ovp.dianchejie.cn

[Q67] 设置隔离级别
来源：http://xbi.smart0.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ncp.tian-w.cn

[Q68] 保存点
来源：http://gtc.ydzc1.top

SAVEPOINT sp1;
来源：http://lgs.tian-w.cn

ROLLBACK TO sp1;
来源：http://tdm.birdmap.top

[Q69] 查看执行计划
来源：http://fcc.ydzc1.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pca.yangfankeji.com

[Q70] 更新统计信息
来源：http://lzb.jinyuanbaomall.cn

ANALYZE TABLE users;
来源：http://imw.cashguo.top

[Q71] 查看建表语句
来源：http://ftc.ctjpmb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jte.fanxiaobao.xyz

[Q72] 查看索引
来源：http://gve.yj202588.top

SHOW INDEX FROM users;
来源：http://bhd.zhixingplan.top

[Q73] 查看表状态
来源：http://dpw.yanxiufei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ske.cdnleiting.top

[Q74] 强制使用索引
来源：http://ujo.jqgufenzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lvx.nwbrower.top

[Q75] 日期格式化
来源：http://aci.hongshengwenyu.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ilc.ivvv.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lmy.jinyuanbaomall.cn

[Q76] 按天统计
来源：http://lhg.bjfxy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gpc.hammf.cn

[Q77] 时间加减
来源：http://vaj.smart0.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iya.meibo888.top

[Q78] 当前时间
来源：http://ozw.xingfuxueyuan.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kzo.wangdashe.top

[Q79] 字符串拼接
来源：http://dtx.sufxvd.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jvy.haohaochexian.top

[Q80] 字符串截取
来源：http://sxy.zhixingplan.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hio.zycfv.cn

[Q81] 字符串替换
来源：http://oau.cdnleiting.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nmx.cucudq.cn

[Q82] 字符长度与字节长度
来源：http://ciy.yfazqb.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sid.yuxming.cn

[Q83] 大小写转换
来源：http://onf.haohaochexian.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cvz.nwbrower.top


<!-- 参考信息 -->