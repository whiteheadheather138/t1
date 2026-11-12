代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://qmg.xuanzx.com

JS:   async function f() { await g(); }
来源：http://nor.hfpthk.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://tox.9152youxi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jwh.fehbvm.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://hgb.cashguo.top

Ruby: # 用 Fiber 或 async gem
来源：http://mdh.hfpthk.cn

C#:   async Task F() { await G(); }
来源：http://ntt.zycfv.cn

[O05] 并发执行并等待全部完成
来源：http://dee.jinyuanbaomall.cn

Py:   asyncio.gather(*tasks)
来源：http://udr.yuxming.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://zmi.kuanghao11.cn

JS:   await Promise.all(tasks)
来源：http://vkn.sxryk.cn

TS:   await Promise.all(tasks)
来源：http://ztz.hcnkem.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zpi.tianlin.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cev.sxryk.cn

Ruby: threads.map(&:join)
来源：http://def.tianlin.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://mnj.zhoulong.xyz

[O06] 使用进程池
来源：http://ccl.cucudq.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dnm.feifeiyinyue.top

PHP:  // pcntl_fork 或多进程队列
来源：http://cdj.jqgfzy.top

JS:   // child_process / cluster 模块
来源：http://drp.yangfankeji.com

TS:   // child_process / cluster 模块
来源：http://sha.zhiwuduotai.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jkg.fktsv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zbw.nwbrower.top

Ruby: // fork 块
来源：http://tkz.jqgfzy.top

C#:   Parallel.For
来源：http://zkq.yj20258888.top

================================================================================
来源：http://eqe.ehwqpu.com

P. 常用工具函数
来源：http://aqc.xuetiantiany.cn

================================================================================
来源：http://pdw.nanxuanxn.top

[P01] 生成 UUID
来源：http://soi.zhixingplan.top

Py:   str(uuid.uuid4())
来源：http://ppa.xinyue.icu

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ctu.jinghuilouyu.cn

JS:   crypto.randomUUID()
来源：http://pqk.xuetiantiany.cn

TS:   crypto.randomUUID()
来源：http://tdi.zhaomingkeji.xyz

Java: UUID.randomUUID().toString()
来源：http://aiu.yuxming.cn

Go:   // 用 github.com/google/uuid
来源：http://eio.xingfuxueyuan.xyz

Ruby: SecureRandom.uuid
来源：http://amk.ydzc1.top

C#:   Guid.NewGuid().ToString()
来源：http://tpc.bjfxy.top

[P02] MD5 / SHA256 摘要
来源：http://ceu.c1oappe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gux.nanxuanxn.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jsm.zhongyouzk.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lyt.ywan-chungtsiang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://xsx.wangshuangyany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ubr.cdnleiting.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ayr.jinyuanbaomall.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jlv.gotoacloud.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jii.yonumen.top

[P03] 生成短随机字符串
来源：http://cuv.fanxiaobao.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sdb.chenlongwang.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ujr.xylfe.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jvd.fzhhl.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://msa.fengsongda.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://glg.quarkkingdee.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://juy.yvedp.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://kif.hammf.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hzl.jinghuilouyu.cn

[P04] 求长度
来源：http://lzo.guowangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://vpu.aizwys.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zra.ywan-chungtsiang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qjx.aizwys.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dyk.zhixingplan.top

Java: list.size();  map.size();  s.length()
来源：http://xsn.jinghuilouyu.cn

Go:   len(arr);  len(m)
来源：http://mhl.yanxiufei.cn

Ruby: x.length;  x.size
来源：http://wxy.fzhhl.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://sda.zhoulong.xyz

[P05] 判断两个对象内容是否相等
来源：http://irk.cashguo.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://ddb.nwbrower.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qyx.jiagoushi.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://brr.snrcjt.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nut.zhoulong.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://unz.zhaomingkeji.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://ork.jinqigfzy.top

Ruby: a == b
来源：http://eiu.ivvv.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dtr.tianlin.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jrn.sxryk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rvh.shangyingyoupin.top

PHP:  if (empty($x)) {}
来源：http://ell.havefunace.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uvo.yueranfly.top

TS:   if (x == null) {}
来源：http://dty.jinqigfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kpq.jqgufenzy.top

Go:   if x == nil {}
来源：http://mdg.gotoacloud.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://irc.ppjwa.cn

C#:   if (x is null) {}
来源：http://lkf.shuidangran.top

[P07] 防抖与节流
来源：http://zvz.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mpr.hfpthk.cn

PHP:  // 手写时间戳比较
来源：http://wtq.ehwqpu.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://svt.daria6918.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lpm.kuanghao11.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kdb.shanyushiyangkeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://swt.birdmap.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ixg.cheryme.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://epd.uphjek.com

[P08] 处理浮点精度问题
来源：http://gcn.sweek.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hxw.hesvh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vmk.gotoacloud.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://izz.hnqzz.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://aju.bbcook.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://eyy.pengpengdd.cyou

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dea.xinyue.icu

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pjs.gogol.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ssv.fengsongda.top

================================================================================
来源：http://puo.cashguo.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://iny.zhijiandao.cn

================================================================================
来源：http://bhu.chenlongwang.top

[Q01] 创建表
来源：http://nkq.pycfn.com

CREATE TABLE users (
来源：http://zfe.vehdjk.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cfn.ywan-chungtsiang.top

name VARCHAR(50) NOT NULL,
来源：http://hsn.quarkkingdee.top

email VARCHAR(100) UNIQUE,
来源：http://egj.pycfn.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://cel.yvedp.cn

);
来源：http://qha.bbcook.cn

[Q02] 创建带外键的表
来源：http://pvt.hnqzz.top

CREATE TABLE orders (
来源：http://yfr.snrcjt.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wzz.dianchejie.cn

user_id INT NOT NULL,
来源：http://kwv.zdqjudy.top

amount DECIMAL(10, 2),
来源：http://aiu.0kj1m.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://orv.hesvh.cn

);
来源：http://vmh.birdmap.top

[Q03] 增加列
来源：http://hvc.9152youxi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://srs.zhaomingkeji.xyz

[Q04] 修改列类型
来源：http://wqb.shzxlz.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qym.tarul.cn

[Q05] 重命名列
来源：http://akc.jqgfzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bbf.gogol.net.cn

[Q06] 删除列
来源：http://uic.mhx1999.top

ALTER TABLE users DROP COLUMN age;
来源：http://awz.shangyingyoupin.top

[Q07] 删除表
来源：http://jvf.jqgfzy.top

DROP TABLE IF EXISTS orders;
来源：http://nwf.ppjwa.cn

[Q08] 创建普通索引
来源：http://ufw.aibaodan.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kzg.snrcjt.cn

[Q09] 创建唯一索引
来源：http://xxz.ppjwa.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dzc.fehbvm.com

[Q10] 插入单行
来源：http://ocl.bbcook.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dpf.zhiwuduotai.top

[Q11] 一次插入多行
来源：http://cuy.tarul.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wlx.9152youxi.cn

[Q12] 插入后取自增 ID
来源：http://dkq.mhx1999.top

INSERT INTO users (name) VALUES ('C');
来源：http://duv.jyoumei.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xqq.hfpthk.cn

[Q13] 忽略重复插入
来源：http://wcq.sufxvd.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vkw.yj202588.top

[Q14] 存在则更新（upsert）
来源：http://wjr.guowangkeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lvk.xingfuxueyuan.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xuq.daria6918.cn

[Q15] 查询全部
来源：http://xqa.redwolf501.top

SELECT * FROM users;
来源：http://svr.wangdashe.top

[Q16] 查询指定列
来源：http://jyl.shanyushiyangtech.top

SELECT id, name FROM users;
来源：http://nkx.tarul.cn

[Q17] 条件查询
来源：http://hya.jinqigufen.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://eru.hcnkem.com

[Q18] 模糊匹配
来源：http://xwd.chenzaomai.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ayt.meibo888.top

[Q19] 范围查询
来源：http://pbv.xuanzx.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baw.sweek.top

[Q20] IN 列表
来源：http://kpy.dashuyun.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mmv.zycfv.cn

[Q21] 空值判断
来源：http://qio.aibaodan.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gdi.meibo888.top

[Q22] 排序
来源：http://yya.sufxvd.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hss.wangdashe.top

[Q23] 分页
来源：http://dnv.zhengqikj.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ubz.birdmap.top

[Q24] 去重
来源：http://ewq.birdmap.top

SELECT DISTINCT city FROM users;
来源：http://lsu.xylfe.cn

[Q25] 只取前 N 条
来源：http://tmw.zhoulong.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tbw.haohaochexian.top

[Q26] 计数
来源：http://usk.c1oappe.top

SELECT COUNT(*) FROM users;
来源：http://xmb.sxryk.cn

[Q27] 条件计数
来源：http://zyy.vqdsnc.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cxp.haohaochexian.top

[Q28] 求和与平均
来源：http://ttu.hesvh.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qtx.jqgfzy.top

[Q29] 最大最小值
来源：http://hbv.guannengcc.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://nen.cdnleiting.top

[Q30] 分组统计
来源：http://slj.yuxming.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mzs.52xcode.cn

[Q31] 分组后过滤
来源：http://src.gotoacloud.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cgs.mhx1999.top

[Q32] 分组拼接字符串
来源：http://ams.hesvh.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dmu.fehbvm.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lcm.zycfv.cn

[Q33] 多列分组
来源：http://jrl.jyoumei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dxx.fanxiaobao.xyz

[Q34] 每组取第一条
来源：http://hgo.jinghuilouyu.cn

SELECT * FROM (
来源：http://uox.sweek.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mxa.fengsongda.top

) t WHERE rn = 1;
来源：http://gdi.xylfe.cn

[Q35] 内连接
来源：http://gzh.sweek.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://iel.meibo888.top

[Q36] 左连接
来源：http://mzn.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kjy.xingfuxueyuan.xyz

[Q37] 右连接
来源：http://lbn.nwbrower.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://amd.yuxming.cn

[Q38] 全外连接（PostgreSQL）
来源：http://dax.316326.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://eck.havefunace.top

[Q39] 自连接（查上下级）
来源：http://hon.ivvv.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://lez.yueranfly.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pjb.shanyushiyangtech.top

[Q40] 交叉连接（笛卡尔积）
来源：http://zwo.zdbjq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nbq.c1oappe.top

[Q41] 多表连接
来源：http://pxa.aibaodan.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://whq.bjfxy.top

JOIN users u ON u.id = o.user_id
来源：http://sot.tanke756.top

JOIN products p ON p.id = o.product_id;
来源：http://zdv.birdmap.top

[Q42] 连接条件附加过滤
来源：http://zxs.kuanghao11.cn

SELECT u.name, o.amount FROM users u
来源：http://cnf.cashguo.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tdx.jianghu66.top

[Q43] 标量子查询
来源：http://jls.yj20258.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://eun.kuanghao11.cn

[Q44] IN 子查询
来源：http://gzy.hongshengwenyu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oxq.nwbrower.top

[Q45] EXISTS 判断存在
来源：http://aul.cashguo.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sbt.ctjpmb.com

[Q46] NOT EXISTS 判断不存在
来源：http://zuu.cdnleiting.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dka.guowangkeji.top

[Q47] 与平均值比较
来源：http://nlh.jiagoushi.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nkj.yongpay.top

[Q48] CTE 公用表表达式
来源：http://dqz.sxryk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yyh.0kj1m.cn

SELECT * FROM t WHERE c > 5;
来源：http://xca.fktsv.cn

[Q49] 更新单行
来源：http://hdg.hongshengwenyu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ixn.vqdsnc.cn

[Q50] 批量更新
来源：http://yvc.zhengqikj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://otn.fanxiaobao.xyz

[Q51] 用子查询更新
来源：http://rgm.chenlongwang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://eds.zycfv.cn

[Q52] 删除指定行
来源：http://twl.chenzaomai.com

DELETE FROM users WHERE id = 10;
来源：http://qvh.hnqzz.top

[Q53] 按条件删除
来源：http://fgf.sweek.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ypg.zhiwuduotai.top

[Q54] 清空表
来源：http://wch.xinyue.icu

TRUNCATE TABLE logs;
来源：http://jvg.hnqzz.top

[Q55] 排名（并列占位）
来源：http://fwl.fanxiaobao.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.xingfuxueyuan.xyz

[Q56] 密集排名（并列不占位）
来源：http://rvy.zhijiandao.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wqc.iojbl.cn

[Q57] 行号
来源：http://rbn.fzhhl.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rxp.jinqigufen.top

[Q58] 累计求和
来源：http://oqx.fzhhl.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yoh.yonumen.top

[Q59] 分组内累计
来源：http://vyp.sxryk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wgi.hesvh.cn

[Q60] 取上一行 / 下一行
来源：http://gzj.ppjwa.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fpm.jinyuanbaomall.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://btu.shanyushiyangtech.top

[Q61] 移动平均
来源：http://zvp.quarkkingdee.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zxs.ehwqpu.com

[Q62] 分组占比
来源：http://eor.havefunace.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://twk.hongshengwenyu.top

[Q63] 开启事务
来源：http://azh.yangfankeji.com

START TRANSACTION;                -- 或 BEGIN
来源：http://nqe.fzhhl.top

[Q64] 提交事务
来源：http://hez.jinyuanbaomall.cn

COMMIT;
来源：http://gls.ivvv.top

[Q65] 回滚事务
来源：http://hpv.yanxiufei.cn

ROLLBACK;
来源：http://fju.sxryk.cn

[Q66] 行锁查询
来源：http://lfn.sufxvd.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lpf.ctjpmb.com

[Q67] 设置隔离级别
来源：http://anl.cdnleiting.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hia.cqqwz.cn

[Q68] 保存点
来源：http://cyp.sweek.top

SAVEPOINT sp1;
来源：http://pgc.yangfankeji.com

ROLLBACK TO sp1;
来源：http://yek.chenzaomai.com

[Q69] 查看执行计划
来源：http://oap.yuanzhike.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ggk.iojbl.cn

[Q70] 更新统计信息
来源：http://uzw.aizwys.cn

ANALYZE TABLE users;
来源：http://pos.gzhubu.top

[Q71] 查看建表语句
来源：http://ugy.fktsv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://dnk.zhiwuduotai.top

[Q72] 查看索引
来源：http://iao.cheryme.top

SHOW INDEX FROM users;
来源：http://omu.shzxlz.cn

[Q73] 查看表状态
来源：http://jeo.tianlin.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://zih.jinqigufen.top

[Q74] 强制使用索引
来源：http://nmu.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zut.fzhhl.top

[Q75] 日期格式化
来源：http://fll.vehdjk.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jkm.nwbrower.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lod.yj20258888.top

[Q76] 按天统计
来源：http://fjp.sysykeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bae.tianlin.xyz

[Q77] 时间加减
来源：http://frz.hongshengwenyu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://moi.yonumen.top

[Q78] 当前时间
来源：http://pnl.pengpengdd.cyou

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ylb.aibaodan.cn

[Q79] 字符串拼接
来源：http://pfm.zdbjq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lil.zhijiandao.cn

[Q80] 字符串截取
来源：http://why.andypj.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zvm.yueranfly.top

[Q81] 字符串替换
来源：http://lkf.shzxlz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vms.cqqwz.cn

[Q82] 字符长度与字节长度
来源：http://zcy.yfazqb.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vmu.hywenlv.cn

[Q83] 大小写转换
来源：http://otp.birdmap.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mra.wangdashe.top

[Q84] 去除首尾空格
来源：http://fju.zhoulong.xyz

SELECT TRIM(name) FROM users;
来源：http://hfj.sxryk.cn

[Q85] 数值取整
来源：http://hac.jinghuilouyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://txu.yangfankeji.com

[Q86] 读取 JSON 字段
来源：http://caz.smart0.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gkp.haohaochexian.top

[Q87] JSON 字段做条件
来源：http://laf.yongpay.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bje.snrcjt.cn


<!-- 参考信息 -->