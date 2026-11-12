代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://qlu.yj20258888.top

C#:   lock (gate) { shared++; }
来源：http://sip.nanxinkj.top

[O04] 定义异步函数并等待
来源：http://kfq.yj202588.top

Py:   async def f():⏎    await g()
来源：http://xwl.bbcook.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ufk.yangfankeji.com

JS:   async function f() { await g(); }
来源：http://jmu.yonumen.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://orp.quarkkingdee.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sya.hammf.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qky.fengsongda.top

Ruby: # 用 Fiber 或 async gem
来源：http://mgj.epnwcf.com

C#:   async Task F() { await G(); }
来源：http://tgb.xuanzx.com

[O05] 并发执行并等待全部完成
来源：http://euz.iojbl.cn

Py:   asyncio.gather(*tasks)
来源：http://enb.c1oappe.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uzz.mhx1999.top

JS:   await Promise.all(tasks)
来源：http://fhz.shzxlz.cn

TS:   await Promise.all(tasks)
来源：http://lpm.iojbl.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://snh.ctjpmb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qyc.hnxiangtu.top

Ruby: threads.map(&:join)
来源：http://ngz.feifeiyinyue.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xfl.sufxvd.cn

[O06] 使用进程池
来源：http://erd.shzxlz.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lck.daria6918.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://xsk.tianlin.xyz

JS:   // child_process / cluster 模块
来源：http://abh.ctjpmb.com

TS:   // child_process / cluster 模块
来源：http://xcq.pycfn.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://azm.yonumen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gqr.chenzaomai.com

Ruby: // fork 块
来源：http://wkn.haohaochexian.top

C#:   Parallel.For
来源：http://pyq.feifeiyinyue.top

================================================================================
来源：http://iao.dashuyun.cn

P. 常用工具函数
来源：http://jed.fktsv.cn

================================================================================
来源：http://alg.cashguo.top

[P01] 生成 UUID
来源：http://cbu.meibo888.top

Py:   str(uuid.uuid4())
来源：http://zbn.zhoulong.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uey.snrcjt.cn

JS:   crypto.randomUUID()
来源：http://zza.jinqigfzy.top

TS:   crypto.randomUUID()
来源：http://aig.birdmap.top

Java: UUID.randomUUID().toString()
来源：http://zog.epnwcf.com

Go:   // 用 github.com/google/uuid
来源：http://svn.yanxiufei.cn

Ruby: SecureRandom.uuid
来源：http://nuk.jinqigfzy.top

C#:   Guid.NewGuid().ToString()
来源：http://die.shzxlz.cn

[P02] MD5 / SHA256 摘要
来源：http://gaf.zhaomingkeji.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mqe.nanxuanxn.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vzt.andypj.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bni.hywenlv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fab.zhongyouzk.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zab.yj202588.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://noi.xingfuxueyuan.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zso.feifeiyinyue.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vjz.yangfankeji.com

[P03] 生成短随机字符串
来源：http://elw.mhx1999.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hsm.dashuyun.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://cqf.zdqjudy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wqh.bjfxy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ker.cheryme.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ubk.tianlin.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gan.zycfv.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jyz.bjfxy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://tts.chenjidiqi.icu

[P04] 求长度
来源：http://xfk.birdmap.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qgu.xuanzx.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ukt.aizwys.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lng.ywan-chungtsiang.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gwh.zhongyouzk.top

Java: list.size();  map.size();  s.length()
来源：http://wnf.chenlongwang.top

Go:   len(arr);  len(m)
来源：http://mlj.gotoacloud.top

Ruby: x.length;  x.size
来源：http://mki.yj20258.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zvl.hcnkem.com

[P05] 判断两个对象内容是否相等
来源：http://jnw.0kj1m.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cye.kuanghao11.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://vta.iojbl.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pgg.yonumen.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zfq.yangfankeji.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wdn.mhx1999.top

Go:   reflect.DeepEqual(a, b)
来源：http://brz.hfpthk.cn

Ruby: a == b
来源：http://blc.birdmap.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dxv.hcnkem.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mxj.jinqigfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bwu.bjfxy.top

PHP:  if (empty($x)) {}
来源：http://qce.sufxvd.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ult.nanxinkj.top

TS:   if (x == null) {}
来源：http://sis.jianghu66.top

Java: if (x == null || x.isEmpty()) {}
来源：http://fgy.zhixingplan.top

Go:   if x == nil {}
来源：http://fbb.shzxlz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://srd.haohaochexian.top

C#:   if (x is null) {}
来源：http://ddj.0kj1m.cn

[P07] 防抖与节流
来源：http://qcd.fengsongda.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zje.zycfv.cn

PHP:  // 手写时间戳比较
来源：http://qwj.yanxiufei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://skn.jlsjyb.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rwg.quarkkingdee.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bij.0kj1m.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://nvt.yj20258888.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://swc.yueranfly.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tbc.daxiang520.top

[P08] 处理浮点精度问题
来源：http://ubj.ydzc1.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lqa.meibo888.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://upz.ehwqpu.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://piu.fanxiaobao.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wwt.aizwys.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lmi.tanke756.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mic.mhx1999.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ofo.shzxlz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pmp.tian-w.cn

================================================================================
来源：http://yyq.birdmap.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://oot.xuetiantiany.cn

================================================================================
来源：http://let.hammf.cn

[Q01] 创建表
来源：http://wgt.andypj.xyz

CREATE TABLE users (
来源：http://rab.hammf.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uqt.nanxuanxn.top

name VARCHAR(50) NOT NULL,
来源：http://spi.cucudq.cn

email VARCHAR(100) UNIQUE,
来源：http://lhp.gotoacloud.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tfl.ctjpmb.com

);
来源：http://pty.bjfxy.top

[Q02] 创建带外键的表
来源：http://ehm.chenjidiqi.icu

CREATE TABLE orders (
来源：http://gpf.zdbjq.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ahv.tianlin.xyz

user_id INT NOT NULL,
来源：http://vhi.zycfv.cn

amount DECIMAL(10, 2),
来源：http://zah.fengsongda.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ilo.guowangkeji.top

);
来源：http://gwd.daria6918.cn

[Q03] 增加列
来源：http://eia.tanke756.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ioe.jianghu66.top

[Q04] 修改列类型
来源：http://tai.shuidangran.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gxt.xingfuxueyuan.xyz

[Q05] 重命名列
来源：http://lvp.9152youxi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jmb.hcnkem.com

[Q06] 删除列
来源：http://psr.uphjek.com

ALTER TABLE users DROP COLUMN age;
来源：http://klp.yanxiufei.cn

[Q07] 删除表
来源：http://rzm.bjfxy.top

DROP TABLE IF EXISTS orders;
来源：http://bck.zhaomingkeji.xyz

[Q08] 创建普通索引
来源：http://qhj.gzhubu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://eik.daxiang520.top

[Q09] 创建唯一索引
来源：http://lcf.shanyushiyangtech.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lmg.aizwys.cn

[Q10] 插入单行
来源：http://mnt.fanxiaobao.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ejq.jinqigufen.top

[Q11] 一次插入多行
来源：http://isv.kuanghao11.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ngx.ydjk.org.cn

[Q12] 插入后取自增 ID
来源：http://zdp.shzxlz.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hko.sxryk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vzd.yfazqb.com

[Q13] 忽略重复插入
来源：http://ilc.aibaodan.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rcr.hysaishi.cn

[Q14] 存在则更新（upsert）
来源：http://zgw.hysaishi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://kcx.hfpthk.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uoj.gzhubu.top

[Q15] 查询全部
来源：http://lao.guannengcc.top

SELECT * FROM users;
来源：http://zjx.andypj.xyz

[Q16] 查询指定列
来源：http://bok.feifeiyinyue.top

SELECT id, name FROM users;
来源：http://dpw.gaohongyu789.top

[Q17] 条件查询
来源：http://oku.zdbjq.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xda.c1oappe.top

[Q18] 模糊匹配
来源：http://bbw.hammf.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sdg.9152youxi.cn

[Q19] 范围查询
来源：http://ryi.svipenyu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jel.bbcook.cn

[Q20] IN 列表
来源：http://mqh.ybcxt.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xfs.hywenlv.cn

[Q21] 空值判断
来源：http://ykd.cdnleiting.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ibm.xuetiantiany.cn

[Q22] 排序
来源：http://onq.shzxlz.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zfa.dianchejie.cn

[Q23] 分页
来源：http://yqo.fehbvm.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://plr.smart0.xyz

[Q24] 去重
来源：http://rco.aibaodan.cn

SELECT DISTINCT city FROM users;
来源：http://vgi.yj202588.top

[Q25] 只取前 N 条
来源：http://yhu.jinyuanbaomall.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mlt.tarul.cn

[Q26] 计数
来源：http://icl.daria6918.cn

SELECT COUNT(*) FROM users;
来源：http://tnm.iojbl.cn

[Q27] 条件计数
来源：http://wla.ydzc1.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zar.mhx1999.top

[Q28] 求和与平均
来源：http://txx.pycfn.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lsp.hysaishi.cn

[Q29] 最大最小值
来源：http://dtc.jyoumei.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://qdu.zhiwuduotai.top

[Q30] 分组统计
来源：http://vfd.jinyuanbaomall.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zfy.daria6918.cn

[Q31] 分组后过滤
来源：http://coc.hesvh.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://psh.pengpengdd.cyou

[Q32] 分组拼接字符串
来源：http://ylb.shzxlz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uox.xylfe.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ffe.yuanzhike.top

[Q33] 多列分组
来源：http://cve.9152youxi.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ggy.jianghu66.top

[Q34] 每组取第一条
来源：http://csg.yj20258888.top

SELECT * FROM (
来源：http://tet.zycfv.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nwf.feifeiyinyue.top

) t WHERE rn = 1;
来源：http://rbk.zdbjq.cn

[Q35] 内连接
来源：http://kyx.yanxiufei.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mdp.yongpay.top

[Q36] 左连接
来源：http://zef.fehbvm.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mrv.aibaodan.cn

[Q37] 右连接
来源：http://hau.jlsjyb.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://anz.fzhhl.top

[Q38] 全外连接（PostgreSQL）
来源：http://qvw.hywenlv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bhj.shanyushiyangtech.top

[Q39] 自连接（查上下级）
来源：http://vvp.yj20258.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rpe.wangdashe.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kbz.aibaodan.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://iad.redwolf501.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kgp.bbcook.cn

[Q41] 多表连接
来源：http://zje.jinqigufen.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://krs.tianlin.xyz

JOIN users u ON u.id = o.user_id
来源：http://evv.jianghu66.top

JOIN products p ON p.id = o.product_id;
来源：http://zho.ydjk.org.cn

[Q42] 连接条件附加过滤
来源：http://fgt.zhijiandao.cn

SELECT u.name, o.amount FROM users u
来源：http://fez.hywenlv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uea.epnwcf.com

[Q43] 标量子查询
来源：http://ish.yj20258.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fmj.ppjwa.cn

[Q44] IN 子查询
来源：http://hjc.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xpi.bbcook.cn

[Q45] EXISTS 判断存在
来源：http://jot.jyoumei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nhd.wangshuangyany.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dvq.yueranfly.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vtd.hesvh.cn

[Q47] 与平均值比较
来源：http://apu.iojbl.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bvd.sxryk.cn

[Q48] CTE 公用表表达式
来源：http://nch.iojbl.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ues.yangfankeji.com

SELECT * FROM t WHERE c > 5;
来源：http://yqw.zdqjudy.top

[Q49] 更新单行
来源：http://ijc.bjfxy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dep.mhx1999.top

[Q50] 批量更新
来源：http://qtz.yongpay.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ijr.ivvv.top

[Q51] 用子查询更新
来源：http://vxv.redwolf501.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ris.xinyue.icu

[Q52] 删除指定行
来源：http://sua.wangdashe.top

DELETE FROM users WHERE id = 10;
来源：http://ofn.yanxiufei.cn

[Q53] 按条件删除
来源：http://ufy.52xcode.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://krs.hnxiangtu.top

[Q54] 清空表
来源：http://mgj.hywenlv.cn

TRUNCATE TABLE logs;
来源：http://kuh.shuidangran.top

[Q55] 排名（并列占位）
来源：http://tug.yangfankeji.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hvk.yangfankeji.com

[Q56] 密集排名（并列不占位）
来源：http://sfj.uphjek.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zoe.vehdjk.com

[Q57] 行号
来源：http://nma.ybcxt.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vsl.hysaishi.cn

[Q58] 累计求和
来源：http://eds.xuanzx.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rdx.chenzaomai.com

[Q59] 分组内累计
来源：http://szg.gaohongyu789.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qok.fengsongda.top

[Q60] 取上一行 / 下一行
来源：http://fto.shangyingyoupin.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kyg.ivvv.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://aac.xingfuxueyuan.xyz

[Q61] 移动平均
来源：http://jzo.jinqigufen.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://etd.yanxiufei.cn

[Q62] 分组占比
来源：http://mvj.gotoacloud.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://riu.daria6918.cn

[Q63] 开启事务
来源：http://xtd.daxiang520.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ogy.shzxlz.cn

[Q64] 提交事务
来源：http://plm.hysaishi.cn

COMMIT;
来源：http://pir.sxryk.cn

[Q65] 回滚事务
来源：http://eau.hfpthk.cn

ROLLBACK;
来源：http://dul.quarkkingdee.top

[Q66] 行锁查询
来源：http://nqu.hongshengwenyu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nbk.yj202588.top

[Q67] 设置隔离级别
来源：http://bno.smart0.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pnz.mhx1999.top

[Q68] 保存点
来源：http://rfb.xinyue.icu

SAVEPOINT sp1;
来源：http://teo.jinqigufen.top

ROLLBACK TO sp1;
来源：http://qyn.feifeiyinyue.top

[Q69] 查看执行计划
来源：http://uqq.cdnleiting.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qlr.shzxlz.cn

[Q70] 更新统计信息
来源：http://ooh.jinqigufen.top

ANALYZE TABLE users;
来源：http://mti.kuanghao11.cn

[Q71] 查看建表语句
来源：http://ymj.yanxiufei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kev.cashguo.top

[Q72] 查看索引
来源：http://snc.yueranfly.top

SHOW INDEX FROM users;
来源：http://gtk.jlsjyb.cn

[Q73] 查看表状态
来源：http://hud.jqgufenzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vau.jlsjyb.cn

[Q74] 强制使用索引
来源：http://xyh.zhengqikj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kql.jiagoushi.top

[Q75] 日期格式化
来源：http://qfk.tianlin.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://klc.redwolf501.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ezq.redwolf501.top

[Q76] 按天统计
来源：http://ryk.dianchejie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hzn.shuidangran.top

[Q77] 时间加减
来源：http://qsk.dianchejie.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://xby.iojbl.cn

[Q78] 当前时间
来源：http://wst.hfpthk.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fnk.zycfv.cn

[Q79] 字符串拼接
来源：http://yrj.uphjek.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mnm.andypj.xyz

[Q80] 字符串截取
来源：http://nws.shanyushiyangkeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://stl.meibo888.top

[Q81] 字符串替换
来源：http://rhy.ydzc1.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bwf.kuanghao11.cn

[Q82] 字符长度与字节长度
来源：http://uhi.zdqjudy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uqm.xylfe.cn

[Q83] 大小写转换
来源：http://ucj.guannengcc.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qnk.gaohongyu789.top

[Q84] 去除首尾空格
来源：http://iex.shangyingyoupin.top

SELECT TRIM(name) FROM users;
来源：http://xtd.nwbrower.top

[Q85] 数值取整
来源：http://kkl.yj202588.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cps.hysaishi.cn


<!-- 参考信息 -->