代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://edb.0kj1m.cn

C#:   lock (gate) { shared++; }
来源：http://nay.fzhhl.top

[O04] 定义异步函数并等待
来源：http://ped.cheryme.top

Py:   async def f():⏎    await g()
来源：http://pvn.mhx1999.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dpr.dashuyun.cn

JS:   async function f() { await g(); }
来源：http://tbx.epnwcf.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://ntl.sxryk.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://pmr.52xcode.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fhe.xingfuxueyuan.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://jtz.sxryk.cn

C#:   async Task F() { await G(); }
来源：http://ysr.hysaishi.cn

[O05] 并发执行并等待全部完成
来源：http://avj.yueranfly.top

Py:   asyncio.gather(*tasks)
来源：http://wan.ctjpmb.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oxl.smart0.xyz

JS:   await Promise.all(tasks)
来源：http://lvf.316326.xyz

TS:   await Promise.all(tasks)
来源：http://agy.snrcjt.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hun.fehbvm.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://iua.hnqzz.top

Ruby: threads.map(&:join)
来源：http://omj.snrcjt.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://uub.xingfuxueyuan.xyz

[O06] 使用进程池
来源：http://fvs.tarul.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sma.cqqwz.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://eox.chenzaomai.com

JS:   // child_process / cluster 模块
来源：http://yuj.cashguo.top

TS:   // child_process / cluster 模块
来源：http://kxx.vehdjk.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://hcn.gotoacloud.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cho.aibaodan.cn

Ruby: // fork 块
来源：http://foc.zhiwuduotai.top

C#:   Parallel.For
来源：http://kvw.yongpay.top

================================================================================
来源：http://xyz.yueranfly.top

P. 常用工具函数
来源：http://lvh.gogol.net.cn

================================================================================
来源：http://uia.aibaodan.cn

[P01] 生成 UUID
来源：http://jlb.nwbrower.top

Py:   str(uuid.uuid4())
来源：http://ndx.cdnleiting.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qxm.yj20258888.top

JS:   crypto.randomUUID()
来源：http://ymi.xuetiantiany.cn

TS:   crypto.randomUUID()
来源：http://wmq.tanke756.top

Java: UUID.randomUUID().toString()
来源：http://eby.hfpthk.cn

Go:   // 用 github.com/google/uuid
来源：http://crc.havefunace.top

Ruby: SecureRandom.uuid
来源：http://hal.shzxlz.cn

C#:   Guid.NewGuid().ToString()
来源：http://iun.vqdsnc.cn

[P02] MD5 / SHA256 摘要
来源：http://mlt.guowangkeji.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vte.xingfuxueyuan.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://mal.ctjpmb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://eeu.ydzc1.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mtk.ywan-chungtsiang.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://fth.chenjidiqi.icu

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://icn.cashguo.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yrf.ybcxt.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wrd.52xcode.cn

[P03] 生成短随机字符串
来源：http://cnn.fktsv.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://frn.xinyue.icu

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ini.chenzaomai.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hmn.hnxiangtu.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bjc.zhengqikj.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dqr.ywan-chungtsiang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uqc.kuanghao11.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xsa.xingfuxueyuan.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qon.jinqigufen.top

[P04] 求长度
来源：http://vfz.chenlongwang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://duf.jinqigufen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sls.nwbrower.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zhj.xinyue.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dmv.hysaishi.cn

Java: list.size();  map.size();  s.length()
来源：http://sqp.quarkkingdee.top

Go:   len(arr);  len(m)
来源：http://qlk.sysykeji.top

Ruby: x.length;  x.size
来源：http://bvp.shanyushiyangtech.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://lew.zhixingplan.top

[P05] 判断两个对象内容是否相等
来源：http://pvm.hesvh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://olx.wangdashe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ufs.tarul.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://cbo.epnwcf.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://awv.ywan-chungtsiang.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ofy.yfazqb.com

Go:   reflect.DeepEqual(a, b)
来源：http://tls.sweek.top

Ruby: a == b
来源：http://ueq.jinghuilouyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tsq.fktsv.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://eub.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wmg.hesvh.cn

PHP:  if (empty($x)) {}
来源：http://gpy.hnqzz.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wjw.shzxlz.cn

TS:   if (x == null) {}
来源：http://lbg.cqqwz.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://gkg.quarkkingdee.top

Go:   if x == nil {}
来源：http://kje.c1oappe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uca.chenjidiqi.icu

C#:   if (x is null) {}
来源：http://apw.zycfv.cn

[P07] 防抖与节流
来源：http://owe.xuetiantiany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://oua.ydjk.org.cn

PHP:  // 手写时间戳比较
来源：http://ovk.fktsv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ctk.dianchejie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kmg.jinghuilouyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dii.daxiang520.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zvh.snrcjt.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://uks.jqgufenzy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wkp.yuanzhike.top

[P08] 处理浮点精度问题
来源：http://kum.zdqjudy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mtk.chenjidiqi.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ekd.xinyue.icu

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qjg.zhijiandao.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ird.guannengcc.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rak.fengsongda.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://nci.epnwcf.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qbd.yj20258.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://bbx.jianghu66.top

================================================================================
来源：http://ulq.yuxming.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fyr.xingfuxueyuan.xyz

================================================================================
来源：http://pwc.fehbvm.com

[Q01] 创建表
来源：http://oba.nanxinkj.top

CREATE TABLE users (
来源：http://pck.dianchejie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gyx.ppjwa.cn

name VARCHAR(50) NOT NULL,
来源：http://gfv.xingfuxueyuan.xyz

email VARCHAR(100) UNIQUE,
来源：http://jts.yonumen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yut.jinyuanbaomall.cn

);
来源：http://vum.zhoulong.xyz

[Q02] 创建带外键的表
来源：http://vju.chenzaomai.com

CREATE TABLE orders (
来源：http://oib.yj202588.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://cop.shangyingyoupin.top

user_id INT NOT NULL,
来源：http://woy.hcnkem.com

amount DECIMAL(10, 2),
来源：http://nlz.zdbjq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://atg.shangyingyoupin.top

);
来源：http://mrh.redwolf501.top

[Q03] 增加列
来源：http://qjm.yj20258888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ulf.haohaochexian.top

[Q04] 修改列类型
来源：http://lqv.sufxvd.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://slg.ivvv.top

[Q05] 重命名列
来源：http://mxx.jianghu66.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cqb.fzhhl.top

[Q06] 删除列
来源：http://fzh.cheryme.top

ALTER TABLE users DROP COLUMN age;
来源：http://zhr.yanxiufei.cn

[Q07] 删除表
来源：http://gie.guannengcc.top

DROP TABLE IF EXISTS orders;
来源：http://ayp.hesvh.cn

[Q08] 创建普通索引
来源：http://gpb.ywan-chungtsiang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://iou.jinqigufen.top

[Q09] 创建唯一索引
来源：http://nby.yuanzhike.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tcd.shanyushiyangtech.top

[Q10] 插入单行
来源：http://zgg.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://nye.ydzc1.top

[Q11] 一次插入多行
来源：http://pvi.zdqjudy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://fhw.haohaochexian.top

[Q12] 插入后取自增 ID
来源：http://rym.jianghu66.top

INSERT INTO users (name) VALUES ('C');
来源：http://gcq.fanxiaobao.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zqy.wangdashe.top

[Q13] 忽略重复插入
来源：http://eek.tian-w.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://jqv.aibaodan.cn

[Q14] 存在则更新（upsert）
来源：http://xqy.jinqigfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rkd.aibaodan.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lep.sxryk.cn

[Q15] 查询全部
来源：http://lvu.xuetiantiany.cn

SELECT * FROM users;
来源：http://ido.zhongyouzk.top

[Q16] 查询指定列
来源：http://mte.epnwcf.com

SELECT id, name FROM users;
来源：http://cze.sxryk.cn

[Q17] 条件查询
来源：http://xmf.ivvv.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mcs.ywan-chungtsiang.top

[Q18] 模糊匹配
来源：http://xgv.vqdsnc.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://svd.jiagoushi.top

[Q19] 范围查询
来源：http://ewy.sweek.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://onr.316326.xyz

[Q20] IN 列表
来源：http://dck.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tfc.meibo888.top

[Q21] 空值判断
来源：http://vgz.zdqjudy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://gug.daxiang520.top

[Q22] 排序
来源：http://syy.yfazqb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kng.guannengcc.top

[Q23] 分页
来源：http://udq.ybcxt.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mcy.chenzaomai.com

[Q24] 去重
来源：http://jgn.ywan-chungtsiang.top

SELECT DISTINCT city FROM users;
来源：http://mpp.hammf.cn

[Q25] 只取前 N 条
来源：http://hst.ctjpmb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hup.pycfn.com

[Q26] 计数
来源：http://ikj.haohaochexian.top

SELECT COUNT(*) FROM users;
来源：http://jhx.zycfv.cn

[Q27] 条件计数
来源：http://gcw.zhixingplan.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://elu.tarul.cn

[Q28] 求和与平均
来源：http://gea.c1oappe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pby.yj20258888.top

[Q29] 最大最小值
来源：http://gyn.zhongyouzk.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://zhy.vqdsnc.cn

[Q30] 分组统计
来源：http://qxn.sjlbkw.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ijx.jinghuilouyu.cn

[Q31] 分组后过滤
来源：http://npn.yfazqb.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://afu.fanxiaobao.xyz

[Q32] 分组拼接字符串
来源：http://dcj.shanyushiyangtech.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zdp.epnwcf.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://puh.jinghuilouyu.cn

[Q33] 多列分组
来源：http://ojo.sjlbkw.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mbh.hywenlv.cn

[Q34] 每组取第一条
来源：http://qxn.xingfuxueyuan.xyz

SELECT * FROM (
来源：http://nri.redwolf501.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tax.iojbl.cn

) t WHERE rn = 1;
来源：http://pfc.zycfv.cn

[Q35] 内连接
来源：http://hph.yuxming.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pqt.hnqzz.top

[Q36] 左连接
来源：http://muf.sysykeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ess.fktsv.cn

[Q37] 右连接
来源：http://htr.epnwcf.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://umd.pengpengdd.cyou

[Q38] 全外连接（PostgreSQL）
来源：http://cgn.zhiwuduotai.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mxj.pycfn.com

[Q39] 自连接（查上下级）
来源：http://cbq.ywan-chungtsiang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://fwl.redwolf501.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://gns.zhijiandao.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cta.xinyue.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kcr.yonumen.top

[Q41] 多表连接
来源：http://trc.uphjek.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://pyb.jyoumei.cn

JOIN users u ON u.id = o.user_id
来源：http://dni.nanxuanxn.top

JOIN products p ON p.id = o.product_id;
来源：http://sye.shanyushiyangtech.top

[Q42] 连接条件附加过滤
来源：http://swg.xuanzx.com

SELECT u.name, o.amount FROM users u
来源：http://ier.vehdjk.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cln.fzhhl.top

[Q43] 标量子查询
来源：http://hio.jinqigfzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xjo.dianchejie.cn

[Q44] IN 子查询
来源：http://cmk.hcnkem.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rag.chenjidiqi.icu

[Q45] EXISTS 判断存在
来源：http://wid.guowangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kgd.9152youxi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://cks.shuidangran.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vwk.aibaodan.cn

[Q47] 与平均值比较
来源：http://stj.ywan-chungtsiang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nne.wangshuangyany.cn

[Q48] CTE 公用表表达式
来源：http://sgq.yfazqb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xlx.jinqigufen.top

SELECT * FROM t WHERE c > 5;
来源：http://ebf.yanxiufei.cn

[Q49] 更新单行
来源：http://pui.pycfn.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ban.yj202588.top

[Q50] 批量更新
来源：http://xiz.cashguo.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pzq.yanxiufei.cn

[Q51] 用子查询更新
来源：http://evs.xziqi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yvm.tianlin.xyz

[Q52] 删除指定行
来源：http://apl.yangfankeji.com

DELETE FROM users WHERE id = 10;
来源：http://rjx.yuxming.cn

[Q53] 按条件删除
来源：http://fur.sweek.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ltk.xuetiantiany.cn

[Q54] 清空表
来源：http://rej.hammf.cn

TRUNCATE TABLE logs;
来源：http://zai.ivvv.top

[Q55] 排名（并列占位）
来源：http://mou.nanxinkj.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://axc.xylfe.cn

[Q56] 密集排名（并列不占位）
来源：http://cro.dianchejie.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xqz.yongpay.top

[Q57] 行号
来源：http://kvl.jqgufenzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zze.ehwqpu.com

[Q58] 累计求和
来源：http://grg.dashuyun.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://edh.smart0.xyz

[Q59] 分组内累计
来源：http://onz.zhengqikj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ums.meibo888.top

[Q60] 取上一行 / 下一行
来源：http://fti.epnwcf.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qtm.chenzaomai.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wbb.sjlbkw.cn

[Q61] 移动平均
来源：http://ypy.gaohongyu789.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://chi.meibo888.top

[Q62] 分组占比
来源：http://zov.wangdashe.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xse.zdqjudy.top

[Q63] 开启事务
来源：http://oov.tian-w.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://uzl.tanke756.top

[Q64] 提交事务
来源：http://tmv.gotoacloud.top

COMMIT;
来源：http://llm.haohaochexian.top

[Q65] 回滚事务
来源：http://ctt.shuidangran.top

ROLLBACK;
来源：http://wgs.hcnkem.com

[Q66] 行锁查询
来源：http://szt.guowangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uml.tanke756.top

[Q67] 设置隔离级别
来源：http://huf.zhongyouzk.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hlc.yj20258888.top

[Q68] 保存点
来源：http://vko.yangfankeji.com

SAVEPOINT sp1;
来源：http://sod.yueranfly.top

ROLLBACK TO sp1;
来源：http://gqg.c1oappe.top

[Q69] 查看执行计划
来源：http://wto.jinqigfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wgm.mhx1999.top

[Q70] 更新统计信息
来源：http://jpx.hnxiangtu.top

ANALYZE TABLE users;
来源：http://cqh.tarul.cn

[Q71] 查看建表语句
来源：http://edg.smart0.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://miu.wangshuangyany.cn

[Q72] 查看索引
来源：http://cmk.sysykeji.top

SHOW INDEX FROM users;
来源：http://yob.fehbvm.com

[Q73] 查看表状态
来源：http://lwn.aizwys.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tdb.yuxming.cn

[Q74] 强制使用索引
来源：http://isq.sxryk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://elg.uphjek.com

[Q75] 日期格式化
来源：http://wbb.kuanghao11.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://faz.zhongyouzk.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bkb.yvedp.cn

[Q76] 按天统计
来源：http://hsu.dianchejie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://llm.feifeiyinyue.top

[Q77] 时间加减
来源：http://rnv.hesvh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ytx.hnxiangtu.top

[Q78] 当前时间
来源：http://uml.ywan-chungtsiang.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rks.zhoulong.xyz

[Q79] 字符串拼接
来源：http://xgm.shzxlz.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vph.feifeiyinyue.top

[Q80] 字符串截取
来源：http://bvy.jyoumei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://myw.tian-w.cn

[Q81] 字符串替换
来源：http://zmk.gogol.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ebe.jianghu66.top

[Q82] 字符长度与字节长度
来源：http://fjr.daxiang520.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jwy.ehwqpu.com

[Q83] 大小写转换
来源：http://lyz.zdqjudy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mte.cqqwz.cn

[Q84] 去除首尾空格
来源：http://cxh.dashuyun.cn

SELECT TRIM(name) FROM users;
来源：http://ylu.cdnleiting.top

[Q85] 数值取整
来源：http://fvo.tanke756.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nbp.zhoulong.xyz


<!-- 参考信息 -->