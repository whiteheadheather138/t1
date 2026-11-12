代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://dbx.havefunace.top

JS:   async function f() { await g(); }
来源：http://fzg.birdmap.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://uei.aibaodan.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nth.hnxiangtu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://aqn.ywan-chungtsiang.top

Ruby: # 用 Fiber 或 async gem
来源：http://fjr.jqgufenzy.top

C#:   async Task F() { await G(); }
来源：http://knf.yueranfly.top

[O05] 并发执行并等待全部完成
来源：http://hyg.hesvh.cn

Py:   asyncio.gather(*tasks)
来源：http://fvi.birdmap.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gvo.bbcook.cn

JS:   await Promise.all(tasks)
来源：http://gaz.shanyushiyangtech.top

TS:   await Promise.all(tasks)
来源：http://ley.quarkkingdee.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hra.0kj1m.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tbm.ydjk.org.cn

Ruby: threads.map(&:join)
来源：http://aia.hesvh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ahb.meibo888.top

[O06] 使用进程池
来源：http://bvo.hywenlv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://pgy.aibaodan.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://fwq.jinghuilouyu.cn

JS:   // child_process / cluster 模块
来源：http://ulv.smart0.xyz

TS:   // child_process / cluster 模块
来源：http://omy.jqgfzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ufs.yfazqb.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ntx.ctjpmb.com

Ruby: // fork 块
来源：http://iyl.sufxvd.cn

C#:   Parallel.For
来源：http://uba.c1oappe.top

================================================================================
来源：http://msv.aibaodan.cn

P. 常用工具函数
来源：http://ads.yj20258888.top

================================================================================
来源：http://siv.sjlbkw.cn

[P01] 生成 UUID
来源：http://ezg.bbcook.cn

Py:   str(uuid.uuid4())
来源：http://qqd.cqqwz.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://egx.svipenyu.cn

JS:   crypto.randomUUID()
来源：http://ifu.mhx1999.top

TS:   crypto.randomUUID()
来源：http://kfs.yonumen.top

Java: UUID.randomUUID().toString()
来源：http://mvl.hnqzz.top

Go:   // 用 github.com/google/uuid
来源：http://cwu.chenlongwang.top

Ruby: SecureRandom.uuid
来源：http://kgu.hywenlv.cn

C#:   Guid.NewGuid().ToString()
来源：http://oas.vqdsnc.cn

[P02] MD5 / SHA256 摘要
来源：http://dls.ehwqpu.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ynd.c1oappe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://tlk.yangfankeji.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lvj.cheryme.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://sth.meibo888.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://sfl.zycfv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ofd.sysykeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jms.hnqzz.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wvu.fengsongda.top

[P03] 生成短随机字符串
来源：http://dgw.hnqzz.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ijo.sysykeji.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vwe.xuetiantiany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://voe.mhx1999.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://inm.aizwys.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uxe.ehwqpu.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mgt.sweek.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://kdm.hongshengwenyu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ykj.pycfn.com

[P04] 求长度
来源：http://eda.ydzc1.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://jfn.jyoumei.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://inv.pycfn.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xbw.cheryme.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://weq.fanxiaobao.xyz

Java: list.size();  map.size();  s.length()
来源：http://pew.9152youxi.cn

Go:   len(arr);  len(m)
来源：http://nta.zhengqikj.top

Ruby: x.length;  x.size
来源：http://cxq.yvedp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://fod.pycfn.com

[P05] 判断两个对象内容是否相等
来源：http://txc.gzhubu.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://vod.jinghuilouyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ftk.jianghu66.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ywr.kuanghao11.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mze.snrcjt.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fzc.shuidangran.top

Go:   reflect.DeepEqual(a, b)
来源：http://uyf.zhiwuduotai.top

Ruby: a == b
来源：http://emr.sxryk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tlt.sjlbkw.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dcn.tarul.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://jjx.hfpthk.cn

PHP:  if (empty($x)) {}
来源：http://zsx.yj20258.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://dyq.ybcxt.top

TS:   if (x == null) {}
来源：http://nzy.yanxiufei.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://xeb.zhoulong.xyz

Go:   if x == nil {}
来源：http://atd.zdbjq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wph.zhoulong.xyz

C#:   if (x is null) {}
来源：http://lnj.fanxiaobao.xyz

[P07] 防抖与节流
来源：http://ddf.vehdjk.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dzf.nanxuanxn.top

PHP:  // 手写时间戳比较
来源：http://yjx.jqgufenzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vuu.ivvv.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eis.ivvv.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wmx.chenzaomai.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kvl.zhiwuduotai.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://dhn.hnqzz.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ozt.xuetiantiany.cn

[P08] 处理浮点精度问题
来源：http://xkq.hesvh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uwt.nanxinkj.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://udk.hnxiangtu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kho.birdmap.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://unx.zdqjudy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jjy.yuxming.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://jxd.dashuyun.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cpn.jinyuanbaomall.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://led.haohaochexian.top

================================================================================
来源：http://koe.fzhhl.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://emd.fehbvm.com

================================================================================
来源：http://ozz.ydzc1.top

[Q01] 创建表
来源：http://pvv.hammf.cn

CREATE TABLE users (
来源：http://nnk.0kj1m.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://umn.ehwqpu.com

name VARCHAR(50) NOT NULL,
来源：http://tlz.sxryk.cn

email VARCHAR(100) UNIQUE,
来源：http://ykp.zhaomingkeji.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://eyf.yfazqb.com

);
来源：http://rpg.jinqigufen.top

[Q02] 创建带外键的表
来源：http://hzd.svipenyu.cn

CREATE TABLE orders (
来源：http://wcv.52xcode.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wah.vqdsnc.cn

user_id INT NOT NULL,
来源：http://xvo.yvedp.cn

amount DECIMAL(10, 2),
来源：http://aob.sxryk.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uen.havefunace.top

);
来源：http://qpw.yj20258888.top

[Q03] 增加列
来源：http://cja.yuxming.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zdl.52xcode.cn

[Q04] 修改列类型
来源：http://wso.zdbjq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xlf.jqgufenzy.top

[Q05] 重命名列
来源：http://cxq.xuetiantiany.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rtt.tarul.cn

[Q06] 删除列
来源：http://low.ydjk.org.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bbu.hysaishi.cn

[Q07] 删除表
来源：http://uvf.sxryk.cn

DROP TABLE IF EXISTS orders;
来源：http://rul.yj202588.top

[Q08] 创建普通索引
来源：http://rsr.sufxvd.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://vux.zdqjudy.top

[Q09] 创建唯一索引
来源：http://sln.hysaishi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rpg.chenzaomai.com

[Q10] 插入单行
来源：http://ffm.hfpthk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zts.yangfankeji.com

[Q11] 一次插入多行
来源：http://ais.xuanzx.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mld.xziqi.cn

[Q12] 插入后取自增 ID
来源：http://vqj.hysaishi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://wok.epnwcf.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://cxf.yuxming.cn

[Q13] 忽略重复插入
来源：http://ckm.hywenlv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wcd.yanxiufei.cn

[Q14] 存在则更新（upsert）
来源：http://xws.fengsongda.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://twu.wangshuangyany.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://udw.daxiang520.top

[Q15] 查询全部
来源：http://qal.yuxming.cn

SELECT * FROM users;
来源：http://sor.haohaochexian.top

[Q16] 查询指定列
来源：http://www.dianchejie.cn

SELECT id, name FROM users;
来源：http://ygr.epnwcf.com

[Q17] 条件查询
来源：http://knh.daria6918.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dzp.chenlongwang.top

[Q18] 模糊匹配
来源：http://plt.ydzc1.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://keg.daxiang520.top

[Q19] 范围查询
来源：http://xff.xuanzx.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://igs.wangshuangyany.cn

[Q20] IN 列表
来源：http://dfj.zhixingplan.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fkl.xziqi.cn

[Q21] 空值判断
来源：http://pnk.tian-w.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://drf.daxiang520.top

[Q22] 排序
来源：http://rmx.aizwys.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://iwy.xinyue.icu

[Q23] 分页
来源：http://ljt.gogol.net.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kni.epnwcf.com

[Q24] 去重
来源：http://tyl.sweek.top

SELECT DISTINCT city FROM users;
来源：http://ige.ybcxt.top

[Q25] 只取前 N 条
来源：http://yef.fzhhl.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xzc.hywenlv.cn

[Q26] 计数
来源：http://jql.ehwqpu.com

SELECT COUNT(*) FROM users;
来源：http://umz.snrcjt.cn

[Q27] 条件计数
来源：http://lss.jqgufenzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mnr.yj202588.top

[Q28] 求和与平均
来源：http://zkl.sxryk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xsy.zdbjq.cn

[Q29] 最大最小值
来源：http://esw.dianchejie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://osi.aizwys.cn

[Q30] 分组统计
来源：http://mqg.bbcook.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hxi.chenlongwang.top

[Q31] 分组后过滤
来源：http://wva.shuidangran.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wlz.yfazqb.com

[Q32] 分组拼接字符串
来源：http://mrb.jinghuilouyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://naw.wangdashe.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ezi.sjlbkw.cn

[Q33] 多列分组
来源：http://uqx.xingfuxueyuan.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://asv.hcnkem.com

[Q34] 每组取第一条
来源：http://lka.pycfn.com

SELECT * FROM (
来源：http://toc.yj20258.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ycr.aizwys.cn

) t WHERE rn = 1;
来源：http://hqd.epnwcf.com

[Q35] 内连接
来源：http://oif.smart0.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ccf.andypj.xyz

[Q36] 左连接
来源：http://msw.xuetiantiany.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kcw.shzxlz.cn

[Q37] 右连接
来源：http://rrh.ppjwa.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mwl.yfazqb.com

[Q38] 全外连接（PostgreSQL）
来源：http://ewn.guannengcc.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wse.xinyue.icu

[Q39] 自连接（查上下级）
来源：http://tog.yj202588.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://cru.gzhubu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qsb.yuxming.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://nej.zhengqikj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sra.sufxvd.cn

[Q41] 多表连接
来源：http://oxc.hysaishi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://yhy.gotoacloud.top

JOIN users u ON u.id = o.user_id
来源：http://fia.xuanzx.com

JOIN products p ON p.id = o.product_id;
来源：http://com.hfpthk.cn

[Q42] 连接条件附加过滤
来源：http://mda.chenlongwang.top

SELECT u.name, o.amount FROM users u
来源：http://dcf.hysaishi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ndr.jinghuilouyu.cn

[Q43] 标量子查询
来源：http://wmp.jqgufenzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oxn.gaohongyu789.top

[Q44] IN 子查询
来源：http://hhc.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fyc.svipenyu.cn

[Q45] EXISTS 判断存在
来源：http://oia.epnwcf.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mve.9152youxi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pav.xingfuxueyuan.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tqa.jiagoushi.top

[Q47] 与平均值比较
来源：http://bfg.jinqigufen.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://flj.zhaomingkeji.xyz

[Q48] CTE 公用表表达式
来源：http://khp.52xcode.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ybj.hnxiangtu.top

SELECT * FROM t WHERE c > 5;
来源：http://wvu.snrcjt.cn

[Q49] 更新单行
来源：http://fpj.ppjwa.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bor.52xcode.cn

[Q50] 批量更新
来源：http://ozu.zhongyouzk.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bhh.vehdjk.com

[Q51] 用子查询更新
来源：http://kou.zhoulong.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dea.hysaishi.cn

[Q52] 删除指定行
来源：http://epf.nwbrower.top

DELETE FROM users WHERE id = 10;
来源：http://tnf.jiagoushi.top

[Q53] 按条件删除
来源：http://nrg.haohaochexian.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ang.yongpay.top

[Q54] 清空表
来源：http://vdv.chenlongwang.top

TRUNCATE TABLE logs;
来源：http://ure.yj20258.top

[Q55] 排名（并列占位）
来源：http://ivr.nwbrower.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zpk.tianlin.xyz

[Q56] 密集排名（并列不占位）
来源：http://uka.ydzc1.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ieo.jlsjyb.cn

[Q57] 行号
来源：http://ivp.hcnkem.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qok.epnwcf.com

[Q58] 累计求和
来源：http://qhq.hnqzz.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wla.cdnleiting.top

[Q59] 分组内累计
来源：http://ika.birdmap.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kmo.yanxiufei.cn

[Q60] 取上一行 / 下一行
来源：http://uhw.snrcjt.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://whd.nwbrower.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lpu.hesvh.cn

[Q61] 移动平均
来源：http://znt.dashuyun.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uzv.chenlongwang.top

[Q62] 分组占比
来源：http://voc.havefunace.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jpp.nanxinkj.top

[Q63] 开启事务
来源：http://lvx.9152youxi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://elk.jyoumei.cn

[Q64] 提交事务
来源：http://slm.hongshengwenyu.top

COMMIT;
来源：http://hmv.hfpthk.cn

[Q65] 回滚事务
来源：http://eet.havefunace.top

ROLLBACK;
来源：http://vfy.chenlongwang.top

[Q66] 行锁查询
来源：http://rsr.smart0.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://fph.fktsv.cn

[Q67] 设置隔离级别
来源：http://fvw.bbcook.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rtq.zhixingplan.top

[Q68] 保存点
来源：http://tnm.feifeiyinyue.top

SAVEPOINT sp1;
来源：http://mqb.zhongyouzk.top

ROLLBACK TO sp1;
来源：http://ozi.tian-w.cn

[Q69] 查看执行计划
来源：http://sps.ydjk.org.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cdh.andypj.xyz

[Q70] 更新统计信息
来源：http://hta.wangshuangyany.cn

ANALYZE TABLE users;
来源：http://uub.zhiwuduotai.top

[Q71] 查看建表语句
来源：http://cbq.zhoulong.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://taa.ppjwa.cn

[Q72] 查看索引
来源：http://tdc.gotoacloud.top

SHOW INDEX FROM users;
来源：http://ann.hysaishi.cn

[Q73] 查看表状态
来源：http://btg.daria6918.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fkz.ydzc1.top

[Q74] 强制使用索引
来源：http://pqo.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ixd.gogol.net.cn

[Q75] 日期格式化
来源：http://emd.pycfn.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vyc.c1oappe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://leq.guannengcc.top

[Q76] 按天统计
来源：http://tyb.ehwqpu.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qut.shangyingyoupin.top

[Q77] 时间加减
来源：http://bbn.daxiang520.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vve.hysaishi.cn

[Q78] 当前时间
来源：http://oms.jinghuilouyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vbj.jinqigufen.top

[Q79] 字符串拼接
来源：http://ysn.zdqjudy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vbd.fzhhl.top

[Q80] 字符串截取
来源：http://vkr.haohaochexian.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mju.pengpengdd.cyou

[Q81] 字符串替换
来源：http://cgg.yuxming.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jfj.0kj1m.cn

[Q82] 字符长度与字节长度
来源：http://ijg.fanxiaobao.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dcp.birdmap.top

[Q83] 大小写转换
来源：http://vhn.hnqzz.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ave.jianghu66.top

[Q84] 去除首尾空格
来源：http://qwx.bbcook.cn

SELECT TRIM(name) FROM users;
来源：http://sph.xingfuxueyuan.xyz

[Q85] 数值取整
来源：http://xrj.fehbvm.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jrj.gzhubu.top

[Q86] 读取 JSON 字段
来源：http://epn.tianlin.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rsq.zhaomingkeji.xyz

[Q87] JSON 字段做条件
来源：http://olt.sxryk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xuu.fanxiaobao.xyz


<!-- 参考信息 -->