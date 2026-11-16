代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://wfx.guowangkeji.top

C#:   lock (gate) { shared++; }
来源：http://ghu.zhixingplan.top

[O04] 定义异步函数并等待
来源：http://oso.c1oappe.top

Py:   async def f():⏎    await g()
来源：http://okl.sysykeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ywf.redwolf501.top

JS:   async function f() { await g(); }
来源：http://rkg.ydjk.org.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://pzq.xuetiantiany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://paw.ywan-chungtsiang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mra.shanyushiyangtech.top

Ruby: # 用 Fiber 或 async gem
来源：http://oqs.shangyingyoupin.top

C#:   async Task F() { await G(); }
来源：http://zlb.snrcjt.cn

[O05] 并发执行并等待全部完成
来源：http://lwf.guowangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://ioo.yonumen.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mut.zdqjudy.top

JS:   await Promise.all(tasks)
来源：http://cmc.mhx1999.top

TS:   await Promise.all(tasks)
来源：http://nlj.fzhhl.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jzs.tian-w.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://jzh.ybcxt.top

Ruby: threads.map(&:join)
来源：http://ual.fehbvm.com

C#:   await Task.WhenAll(t1, t2)
来源：http://uvl.hammf.cn

[O06] 使用进程池
来源：http://yjc.ydzc1.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vvu.nwbrower.top

PHP:  // pcntl_fork 或多进程队列
来源：http://iwj.ybcxt.top

JS:   // child_process / cluster 模块
来源：http://bjm.tianlin.xyz

TS:   // child_process / cluster 模块
来源：http://kze.vqdsnc.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jvg.ywan-chungtsiang.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tbb.zdbjq.cn

Ruby: // fork 块
来源：http://iah.316326.xyz

C#:   Parallel.For
来源：http://pcb.hysaishi.cn

================================================================================
来源：http://rah.pengpengdd.cyou

P. 常用工具函数
来源：http://okv.mhx1999.top

================================================================================
来源：http://asc.zhaomingkeji.xyz

[P01] 生成 UUID
来源：http://zez.zhijiandao.cn

Py:   str(uuid.uuid4())
来源：http://zut.ctjpmb.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zfc.bbcook.cn

JS:   crypto.randomUUID()
来源：http://tux.ybcxt.top

TS:   crypto.randomUUID()
来源：http://myg.zhaomingkeji.xyz

Java: UUID.randomUUID().toString()
来源：http://pov.haohaochexian.top

Go:   // 用 github.com/google/uuid
来源：http://waa.birdmap.top

Ruby: SecureRandom.uuid
来源：http://zga.zhixingplan.top

C#:   Guid.NewGuid().ToString()
来源：http://kuf.yvedp.cn

[P02] MD5 / SHA256 摘要
来源：http://stb.yj20258.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jkh.yfazqb.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://mvp.cqqwz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oam.quarkkingdee.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bbc.hnqzz.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ybd.nwbrower.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wcu.ybcxt.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qfi.ydzc1.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://shh.xylfe.cn

[P03] 生成短随机字符串
来源：http://fxu.52xcode.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://gdu.zhengqikj.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://urq.wangdashe.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wkr.guannengcc.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wfd.vqdsnc.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pex.zhongyouzk.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mcj.jlsjyb.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://czl.ywan-chungtsiang.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://trw.daria6918.cn

[P04] 求长度
来源：http://dcw.zdqjudy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xfm.dianchejie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fub.kuanghao11.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wvu.nwbrower.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fbb.yvedp.cn

Java: list.size();  map.size();  s.length()
来源：http://rwi.havefunace.top

Go:   len(arr);  len(m)
来源：http://nqh.9152youxi.cn

Ruby: x.length;  x.size
来源：http://sxd.xuetiantiany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://rav.tarul.cn

[P05] 判断两个对象内容是否相等
来源：http://jay.tian-w.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://dqt.xziqi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ycx.svipenyu.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zqw.nwbrower.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zsx.tanke756.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ows.sufxvd.cn

Go:   reflect.DeepEqual(a, b)
来源：http://gcz.gaohongyu789.top

Ruby: a == b
来源：http://hku.c1oappe.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://poh.guannengcc.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cxe.nanxuanxn.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sez.zhaomingkeji.xyz

PHP:  if (empty($x)) {}
来源：http://grh.havefunace.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ctx.hywenlv.cn

TS:   if (x == null) {}
来源：http://dtd.pengpengdd.cyou

Java: if (x == null || x.isEmpty()) {}
来源：http://jvy.yongpay.top

Go:   if x == nil {}
来源：http://cpo.hongshengwenyu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://arj.ydjk.org.cn

C#:   if (x is null) {}
来源：http://vly.ehwqpu.com

[P07] 防抖与节流
来源：http://azj.hnxiangtu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://hvc.nanxuanxn.top

PHP:  // 手写时间戳比较
来源：http://tdb.aibaodan.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dfg.snrcjt.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aep.zhoulong.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yju.jinqigfzy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nue.ydzc1.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://dar.ivvv.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://get.gotoacloud.top

[P08] 处理浮点精度问题
来源：http://kst.wangshuangyany.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wcg.wangshuangyany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://obi.hywenlv.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vod.sjlbkw.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ldm.zhijiandao.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ryc.shzxlz.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ybg.xuetiantiany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tpp.316326.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dsp.xylfe.cn

================================================================================
来源：http://fix.tianlin.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://egf.dianchejie.cn

================================================================================
来源：http://yvf.zhixingplan.top

[Q01] 创建表
来源：http://rac.xuanzx.com

CREATE TABLE users (
来源：http://upe.hcnkem.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://esm.snrcjt.cn

name VARCHAR(50) NOT NULL,
来源：http://aol.daria6918.cn

email VARCHAR(100) UNIQUE,
来源：http://ani.jinqigufen.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://aem.316326.xyz

);
来源：http://anm.ehwqpu.com

[Q02] 创建带外键的表
来源：http://yvd.shuidangran.top

CREATE TABLE orders (
来源：http://has.ydzc1.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://azf.gotoacloud.top

user_id INT NOT NULL,
来源：http://etm.ydjk.org.cn

amount DECIMAL(10, 2),
来源：http://jml.chenjidiqi.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qfz.ydjk.org.cn

);
来源：http://rcj.chenlongwang.top

[Q03] 增加列
来源：http://hso.zhongyouzk.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cfd.yj20258.top

[Q04] 修改列类型
来源：http://vjh.yonumen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mch.xingfuxueyuan.xyz

[Q05] 重命名列
来源：http://trz.redwolf501.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jbh.xingfuxueyuan.xyz

[Q06] 删除列
来源：http://mdu.bjfxy.top

ALTER TABLE users DROP COLUMN age;
来源：http://wbh.ydzc1.top

[Q07] 删除表
来源：http://sje.hnqzz.top

DROP TABLE IF EXISTS orders;
来源：http://dtm.cdnleiting.top

[Q08] 创建普通索引
来源：http://ali.havefunace.top

CREATE INDEX idx_users_email ON users(email);
来源：http://yxt.sufxvd.cn

[Q09] 创建唯一索引
来源：http://pqw.gzhubu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://phf.nanxuanxn.top

[Q10] 插入单行
来源：http://bog.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wcb.aibaodan.cn

[Q11] 一次插入多行
来源：http://nxz.meibo888.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bru.fanxiaobao.xyz

[Q12] 插入后取自增 ID
来源：http://bzz.daxiang520.top

INSERT INTO users (name) VALUES ('C');
来源：http://ows.ydzc1.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nez.iojbl.cn

[Q13] 忽略重复插入
来源：http://jdc.yj20258.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bvm.jyoumei.cn

[Q14] 存在则更新（upsert）
来源：http://fei.birdmap.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jdd.feifeiyinyue.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://leo.hnxiangtu.top

[Q15] 查询全部
来源：http://uer.sjlbkw.cn

SELECT * FROM users;
来源：http://hnp.jianghu66.top

[Q16] 查询指定列
来源：http://fno.kuanghao11.cn

SELECT id, name FROM users;
来源：http://jom.pengpengdd.cyou

[Q17] 条件查询
来源：http://efq.cdnleiting.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xic.wangdashe.top

[Q18] 模糊匹配
来源：http://cej.havefunace.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://klb.zhiwuduotai.top

[Q19] 范围查询
来源：http://jvx.sysykeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ugw.redwolf501.top

[Q20] IN 列表
来源：http://isp.nanxinkj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ekd.xuetiantiany.cn

[Q21] 空值判断
来源：http://mfg.fktsv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://obg.jinghuilouyu.cn

[Q22] 排序
来源：http://wyc.svipenyu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xug.ywan-chungtsiang.top

[Q23] 分页
来源：http://eeo.jyoumei.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jfi.zycfv.cn

[Q24] 去重
来源：http://jzz.hammf.cn

SELECT DISTINCT city FROM users;
来源：http://web.zdbjq.cn

[Q25] 只取前 N 条
来源：http://ivm.ctjpmb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://krb.yuanzhike.top

[Q26] 计数
来源：http://cae.zhiwuduotai.top

SELECT COUNT(*) FROM users;
来源：http://mzl.yongpay.top

[Q27] 条件计数
来源：http://lzd.jqgufenzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qvt.vehdjk.com

[Q28] 求和与平均
来源：http://muu.gogol.net.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://abo.xingfuxueyuan.xyz

[Q29] 最大最小值
来源：http://qua.guowangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://odo.sjlbkw.cn

[Q30] 分组统计
来源：http://bda.snrcjt.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://igo.daria6918.cn

[Q31] 分组后过滤
来源：http://ivk.fzhhl.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vqh.xuetiantiany.cn

[Q32] 分组拼接字符串
来源：http://ymf.9152youxi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bbm.0kj1m.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wer.shanyushiyangkeji.top

[Q33] 多列分组
来源：http://gvc.tianlin.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xbk.chenzaomai.com

[Q34] 每组取第一条
来源：http://kfc.zhijiandao.cn

SELECT * FROM (
来源：http://pap.sjlbkw.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dgt.zhongyouzk.top

) t WHERE rn = 1;
来源：http://zxw.sweek.top

[Q35] 内连接
来源：http://odt.0kj1m.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://skf.cheryme.top

[Q36] 左连接
来源：http://yaq.bbcook.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://fjs.ehwqpu.com

[Q37] 右连接
来源：http://tmf.hywenlv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ash.tianlin.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://khq.shangyingyoupin.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vvu.jqgufenzy.top

[Q39] 自连接（查上下级）
来源：http://niu.dianchejie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://pzt.ywan-chungtsiang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iyb.c1oappe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://lak.fengsongda.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sue.zhiwuduotai.top

[Q41] 多表连接
来源：http://fik.hesvh.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pqf.yueranfly.top

JOIN users u ON u.id = o.user_id
来源：http://tjd.vehdjk.com

JOIN products p ON p.id = o.product_id;
来源：http://zbm.jlsjyb.cn

[Q42] 连接条件附加过滤
来源：http://vdz.sjlbkw.cn

SELECT u.name, o.amount FROM users u
来源：http://mkn.gzhubu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ccb.jiagoushi.top

[Q43] 标量子查询
来源：http://oov.yongpay.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gnb.yanxiufei.cn

[Q44] IN 子查询
来源：http://kwi.hfpthk.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mwb.sxryk.cn

[Q45] EXISTS 判断存在
来源：http://tjr.shuidangran.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://flw.birdmap.top

[Q46] NOT EXISTS 判断不存在
来源：http://wqb.xuanzx.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eeu.xziqi.cn

[Q47] 与平均值比较
来源：http://kir.ydjk.org.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://chp.xuetiantiany.cn

[Q48] CTE 公用表表达式
来源：http://rkf.quarkkingdee.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fvq.meibo888.top

SELECT * FROM t WHERE c > 5;
来源：http://yzw.mhx1999.top

[Q49] 更新单行
来源：http://iso.yuxming.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xso.yangfankeji.com

[Q50] 批量更新
来源：http://hme.ydzc1.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://clf.ydjk.org.cn

[Q51] 用子查询更新
来源：http://cvf.ybcxt.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://poa.0kj1m.cn

[Q52] 删除指定行
来源：http://utz.fengsongda.top

DELETE FROM users WHERE id = 10;
来源：http://vvt.zdbjq.cn

[Q53] 按条件删除
来源：http://hge.tian-w.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qzh.jinghuilouyu.cn

[Q54] 清空表
来源：http://duw.hammf.cn

TRUNCATE TABLE logs;
来源：http://inv.yonumen.top

[Q55] 排名（并列占位）
来源：http://kln.xinyue.icu

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hvq.hnxiangtu.top

[Q56] 密集排名（并列不占位）
来源：http://hec.iojbl.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mop.316326.xyz

[Q57] 行号
来源：http://gzq.zhengqikj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kpz.uphjek.com

[Q58] 累计求和
来源：http://mjs.andypj.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qkr.zhaomingkeji.xyz

[Q59] 分组内累计
来源：http://tsa.andypj.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://isp.zhoulong.xyz

[Q60] 取上一行 / 下一行
来源：http://cys.hfpthk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://itp.hnqzz.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nup.fanxiaobao.xyz

[Q61] 移动平均
来源：http://bjt.gzhubu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iwg.gaohongyu789.top

[Q62] 分组占比
来源：http://ruq.yongpay.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ama.zdqjudy.top

[Q63] 开启事务
来源：http://mfe.xinyue.icu

START TRANSACTION;                -- 或 BEGIN
来源：http://yqt.nanxuanxn.top

[Q64] 提交事务
来源：http://qzc.tarul.cn

COMMIT;
来源：http://zmg.daria6918.cn

[Q65] 回滚事务
来源：http://tqm.shanyushiyangkeji.top

ROLLBACK;
来源：http://ouo.gogol.net.cn

[Q66] 行锁查询
来源：http://fmz.9152youxi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yqq.yuxming.cn

[Q67] 设置隔离级别
来源：http://kok.jqgfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://arb.fktsv.cn

[Q68] 保存点
来源：http://feq.fehbvm.com

SAVEPOINT sp1;
来源：http://bzu.andypj.xyz

ROLLBACK TO sp1;
来源：http://hjv.wangdashe.top

[Q69] 查看执行计划
来源：http://edn.smart0.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kgy.tian-w.cn

[Q70] 更新统计信息
来源：http://ylg.yj20258888.top

ANALYZE TABLE users;
来源：http://lpt.cashguo.top

[Q71] 查看建表语句
来源：http://vsr.gaohongyu789.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://irp.daria6918.cn

[Q72] 查看索引
来源：http://dps.snrcjt.cn

SHOW INDEX FROM users;
来源：http://rtn.yongpay.top

[Q73] 查看表状态
来源：http://bxf.hammf.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://sfs.sysykeji.top

[Q74] 强制使用索引
来源：http://jhx.tianlin.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ydz.vqdsnc.cn

[Q75] 日期格式化
来源：http://poy.daria6918.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cwh.yj202588.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tsg.dianchejie.cn

[Q76] 按天统计
来源：http://dnf.vqdsnc.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nkj.jqgufenzy.top

[Q77] 时间加减
来源：http://kvn.fanxiaobao.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nfx.ydzc1.top

[Q78] 当前时间
来源：http://oog.jinghuilouyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dqv.fanxiaobao.xyz

[Q79] 字符串拼接
来源：http://zvr.zycfv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://teg.hysaishi.cn

[Q80] 字符串截取
来源：http://jey.jiagoushi.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yns.zhijiandao.cn

[Q81] 字符串替换
来源：http://bee.316326.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://crj.ppjwa.cn

[Q82] 字符长度与字节长度
来源：http://tng.shanyushiyangtech.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://udj.wangshuangyany.cn

[Q83] 大小写转换
来源：http://fal.fzhhl.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kut.52xcode.cn

[Q84] 去除首尾空格
来源：http://cet.xylfe.cn

SELECT TRIM(name) FROM users;
来源：http://cnz.316326.xyz

[Q85] 数值取整
来源：http://gry.pengpengdd.cyou

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://huf.cqqwz.cn


<!-- 参考信息 -->