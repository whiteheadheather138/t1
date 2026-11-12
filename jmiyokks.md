代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qei.shzxlz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://vfx.fengsongda.top

C#:   async Task F() { await G(); }
来源：http://txb.hammf.cn

[O05] 并发执行并等待全部完成
来源：http://smy.snrcjt.cn

Py:   asyncio.gather(*tasks)
来源：http://oah.fktsv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qac.zhongyouzk.top

JS:   await Promise.all(tasks)
来源：http://pmc.fktsv.cn

TS:   await Promise.all(tasks)
来源：http://kpz.zhijiandao.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://quq.ivvv.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://csx.yj20258888.top

Ruby: threads.map(&:join)
来源：http://tic.hammf.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jrq.hongshengwenyu.top

[O06] 使用进程池
来源：http://tfv.hnxiangtu.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jhl.jyoumei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dqb.xinyue.icu

JS:   // child_process / cluster 模块
来源：http://dez.sweek.top

TS:   // child_process / cluster 模块
来源：http://jhu.sysykeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wde.svipenyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cjt.yonumen.top

Ruby: // fork 块
来源：http://tkb.zycfv.cn

C#:   Parallel.For
来源：http://fat.epnwcf.com

================================================================================
来源：http://fih.shzxlz.cn

P. 常用工具函数
来源：http://mmg.yanxiufei.cn

================================================================================
来源：http://tee.shuidangran.top

[P01] 生成 UUID
来源：http://dbl.nanxinkj.top

Py:   str(uuid.uuid4())
来源：http://npy.sxryk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fpp.0kj1m.cn

JS:   crypto.randomUUID()
来源：http://wsf.fengsongda.top

TS:   crypto.randomUUID()
来源：http://ygp.kuanghao11.cn

Java: UUID.randomUUID().toString()
来源：http://ior.hfpthk.cn

Go:   // 用 github.com/google/uuid
来源：http://qud.nwbrower.top

Ruby: SecureRandom.uuid
来源：http://nuy.yueranfly.top

C#:   Guid.NewGuid().ToString()
来源：http://vsm.quarkkingdee.top

[P02] MD5 / SHA256 摘要
来源：http://lvm.hysaishi.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ipg.yj202588.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://sxd.yongpay.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wky.ctjpmb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ykc.nanxinkj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://iwc.jiagoushi.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://upg.hongshengwenyu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jqp.ydjk.org.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fwk.gogol.net.cn

[P03] 生成短随机字符串
来源：http://alb.guowangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vuc.cdnleiting.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bnh.bbcook.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fue.wangshuangyany.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fyi.gogol.net.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zmc.gzhubu.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wvq.0kj1m.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://aqe.birdmap.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wba.svipenyu.cn

[P04] 求长度
来源：http://yke.pengpengdd.cyou

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pjl.dianchejie.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cxk.c1oappe.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gjv.yangfankeji.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jek.ydzc1.top

Java: list.size();  map.size();  s.length()
来源：http://hqa.daria6918.cn

Go:   len(arr);  len(m)
来源：http://vbw.52xcode.cn

Ruby: x.length;  x.size
来源：http://ebq.xingfuxueyuan.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://edy.jinghuilouyu.cn

[P05] 判断两个对象内容是否相等
来源：http://bgm.ctjpmb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://tjs.guowangkeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dso.yj20258888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ipu.cqqwz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://hhc.fengsongda.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rfe.quarkkingdee.top

Go:   reflect.DeepEqual(a, b)
来源：http://txc.shuidangran.top

Ruby: a == b
来源：http://kdc.hywenlv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://tlb.haohaochexian.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://kgl.wangshuangyany.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vne.nwbrower.top

PHP:  if (empty($x)) {}
来源：http://zfb.cucudq.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jsy.tanke756.top

TS:   if (x == null) {}
来源：http://odz.hongshengwenyu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://nsc.bbcook.cn

Go:   if x == nil {}
来源：http://mbh.cashguo.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://aol.c1oappe.top

C#:   if (x is null) {}
来源：http://krs.hywenlv.cn

[P07] 防抖与节流
来源：http://nzo.xingfuxueyuan.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ktn.yfazqb.com

PHP:  // 手写时间戳比较
来源：http://voy.jlsjyb.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jpo.cheryme.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lsc.sufxvd.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tep.meibo888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ary.hnqzz.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hss.sxryk.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wtb.birdmap.top

[P08] 处理浮点精度问题
来源：http://iyy.chenjidiqi.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xvz.dianchejie.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://afv.zhiwuduotai.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://tgz.tianlin.xyz

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xlv.yanxiufei.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ixh.chenzaomai.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cwj.hysaishi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gmz.jlsjyb.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://woh.yangfankeji.com

================================================================================
来源：http://xnq.yj20258888.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dmr.yfazqb.com

================================================================================
来源：http://ucz.sxryk.cn

[Q01] 创建表
来源：http://jdp.yanxiufei.cn

CREATE TABLE users (
来源：http://ynv.shangyingyoupin.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wzo.hnxiangtu.top

name VARCHAR(50) NOT NULL,
来源：http://qgn.yonumen.top

email VARCHAR(100) UNIQUE,
来源：http://iys.sweek.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ffb.sxryk.cn

);
来源：http://pay.vehdjk.com

[Q02] 创建带外键的表
来源：http://ugl.gzhubu.top

CREATE TABLE orders (
来源：http://cnt.sjlbkw.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xhz.smart0.xyz

user_id INT NOT NULL,
来源：http://rep.ybcxt.top

amount DECIMAL(10, 2),
来源：http://nqr.sweek.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vuj.tarul.cn

);
来源：http://yui.c1oappe.top

[Q03] 增加列
来源：http://gus.tanke756.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gfr.haohaochexian.top

[Q04] 修改列类型
来源：http://udr.gaohongyu789.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kil.jlsjyb.cn

[Q05] 重命名列
来源：http://qht.fzhhl.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://sim.jyoumei.cn

[Q06] 删除列
来源：http://dfq.hfpthk.cn

ALTER TABLE users DROP COLUMN age;
来源：http://mqr.sysykeji.top

[Q07] 删除表
来源：http://sry.fehbvm.com

DROP TABLE IF EXISTS orders;
来源：http://wel.meibo888.top

[Q08] 创建普通索引
来源：http://xhb.yanxiufei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://iko.zhoulong.xyz

[Q09] 创建唯一索引
来源：http://wfj.wangdashe.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fqo.hcnkem.com

[Q10] 插入单行
来源：http://nhd.jyoumei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://atw.zhengqikj.top

[Q11] 一次插入多行
来源：http://ywd.shzxlz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kww.pengpengdd.cyou

[Q12] 插入后取自增 ID
来源：http://tdu.vqdsnc.cn

INSERT INTO users (name) VALUES ('C');
来源：http://zxx.tanke756.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nbd.9152youxi.cn

[Q13] 忽略重复插入
来源：http://spm.daria6918.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://den.meibo888.top

[Q14] 存在则更新（upsert）
来源：http://lfs.vqdsnc.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ajo.shuidangran.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zjx.yangfankeji.com

[Q15] 查询全部
来源：http://bko.birdmap.top

SELECT * FROM users;
来源：http://gny.uphjek.com

[Q16] 查询指定列
来源：http://jzv.cqqwz.cn

SELECT id, name FROM users;
来源：http://txg.zhengqikj.top

[Q17] 条件查询
来源：http://qyp.jinqigfzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nyy.zhixingplan.top

[Q18] 模糊匹配
来源：http://jxi.wangshuangyany.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lhb.jqgufenzy.top

[Q19] 范围查询
来源：http://jfa.sjlbkw.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mxc.xingfuxueyuan.xyz

[Q20] IN 列表
来源：http://nwv.tanke756.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mmb.xingfuxueyuan.xyz

[Q21] 空值判断
来源：http://dar.wangdashe.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ecq.yonumen.top

[Q22] 排序
来源：http://fql.xziqi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lmr.sjlbkw.cn

[Q23] 分页
来源：http://iol.havefunace.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tkv.yj20258888.top

[Q24] 去重
来源：http://naq.meibo888.top

SELECT DISTINCT city FROM users;
来源：http://fun.jlsjyb.cn

[Q25] 只取前 N 条
来源：http://xvk.yonumen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://cru.daxiang520.top

[Q26] 计数
来源：http://gdd.ivvv.top

SELECT COUNT(*) FROM users;
来源：http://qxd.hammf.cn

[Q27] 条件计数
来源：http://wie.meibo888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mgr.sweek.top

[Q28] 求和与平均
来源：http://yhd.yj202588.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uxn.fengsongda.top

[Q29] 最大最小值
来源：http://flo.shanyushiyangtech.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://cwv.gzhubu.top

[Q30] 分组统计
来源：http://lja.yanxiufei.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zxl.shuidangran.top

[Q31] 分组后过滤
来源：http://jgb.hfpthk.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://bar.sweek.top

[Q32] 分组拼接字符串
来源：http://ogu.yj20258888.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tum.yongpay.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lhn.sjlbkw.cn

[Q33] 多列分组
来源：http://egd.shzxlz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fms.shangyingyoupin.top

[Q34] 每组取第一条
来源：http://ibs.tian-w.cn

SELECT * FROM (
来源：http://kbb.daria6918.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rzd.jianghu66.top

) t WHERE rn = 1;
来源：http://zmp.ivvv.top

[Q35] 内连接
来源：http://apt.vqdsnc.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ehx.hnxiangtu.top

[Q36] 左连接
来源：http://iev.zhiwuduotai.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jeb.uphjek.com

[Q37] 右连接
来源：http://dss.hysaishi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dab.guannengcc.top

[Q38] 全外连接（PostgreSQL）
来源：http://gbw.xuetiantiany.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gck.snrcjt.cn

[Q39] 自连接（查上下级）
来源：http://iqn.redwolf501.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ipw.tian-w.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://euu.ybcxt.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wxr.yueranfly.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uqi.ydzc1.top

[Q41] 多表连接
来源：http://odm.wangshuangyany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://itw.zdqjudy.top

JOIN users u ON u.id = o.user_id
来源：http://ola.zhengqikj.top

JOIN products p ON p.id = o.product_id;
来源：http://imp.chenjidiqi.icu

[Q42] 连接条件附加过滤
来源：http://lvx.yj20258888.top

SELECT u.name, o.amount FROM users u
来源：http://jon.jinqigfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rwz.xingfuxueyuan.xyz

[Q43] 标量子查询
来源：http://ryc.guowangkeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://aof.nanxuanxn.top

[Q44] IN 子查询
来源：http://acl.hammf.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://evo.aibaodan.cn

[Q45] EXISTS 判断存在
来源：http://kve.shanyushiyangtech.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hlr.xylfe.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yia.nanxuanxn.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vvy.tanke756.top

[Q47] 与平均值比较
来源：http://tiw.feifeiyinyue.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hob.hcnkem.com

[Q48] CTE 公用表表达式
来源：http://wht.zhaomingkeji.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ljq.aibaodan.cn

SELECT * FROM t WHERE c > 5;
来源：http://bot.ctjpmb.com

[Q49] 更新单行
来源：http://sfe.sysykeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jlm.ydzc1.top

[Q50] 批量更新
来源：http://rsr.havefunace.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yrg.cqqwz.cn

[Q51] 用子查询更新
来源：http://qly.hfpthk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nzg.mhx1999.top

[Q52] 删除指定行
来源：http://ube.chenzaomai.com

DELETE FROM users WHERE id = 10;
来源：http://ipk.hywenlv.cn

[Q53] 按条件删除
来源：http://joe.sysykeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ymd.tianlin.xyz

[Q54] 清空表
来源：http://qav.chenlongwang.top

TRUNCATE TABLE logs;
来源：http://ouw.sweek.top

[Q55] 排名（并列占位）
来源：http://ecl.52xcode.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xue.52xcode.cn

[Q56] 密集排名（并列不占位）
来源：http://fgt.316326.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ylx.yanxiufei.cn

[Q57] 行号
来源：http://oue.gotoacloud.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ent.jyoumei.cn

[Q58] 累计求和
来源：http://pyw.yvedp.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qwf.sysykeji.top

[Q59] 分组内累计
来源：http://ajx.shuidangran.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://law.jinqigufen.top

[Q60] 取上一行 / 下一行
来源：http://ytq.fengsongda.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://smd.jqgufenzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://emy.tanke756.top

[Q61] 移动平均
来源：http://eyd.bjfxy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://miu.ehwqpu.com

[Q62] 分组占比
来源：http://qmk.hammf.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ybw.pengpengdd.cyou

[Q63] 开启事务
来源：http://toz.ywan-chungtsiang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://naf.xuanzx.com

[Q64] 提交事务
来源：http://eoj.meibo888.top

COMMIT;
来源：http://gqh.jinghuilouyu.cn

[Q65] 回滚事务
来源：http://avu.daxiang520.top

ROLLBACK;
来源：http://edv.sweek.top

[Q66] 行锁查询
来源：http://brn.vehdjk.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pzo.zhengqikj.top

[Q67] 设置隔离级别
来源：http://ktx.chenjidiqi.icu

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ncd.svipenyu.cn

[Q68] 保存点
来源：http://qfh.cdnleiting.top

SAVEPOINT sp1;
来源：http://epf.yangfankeji.com

ROLLBACK TO sp1;
来源：http://uim.dashuyun.cn

[Q69] 查看执行计划
来源：http://aek.jiagoushi.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xzb.meibo888.top

[Q70] 更新统计信息
来源：http://wzj.hesvh.cn

ANALYZE TABLE users;
来源：http://bzw.jinqigfzy.top

[Q71] 查看建表语句
来源：http://hzz.ywan-chungtsiang.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pky.sufxvd.cn

[Q72] 查看索引
来源：http://ufe.tianlin.xyz

SHOW INDEX FROM users;
来源：http://yvv.cheryme.top

[Q73] 查看表状态
来源：http://lcq.jinyuanbaomall.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cgy.xziqi.cn

[Q74] 强制使用索引
来源：http://ryg.birdmap.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eqp.jiagoushi.top

[Q75] 日期格式化
来源：http://nmn.yanxiufei.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wur.tian-w.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://snr.yongpay.top

[Q76] 按天统计
来源：http://egj.ydjk.org.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dva.ehwqpu.com

[Q77] 时间加减
来源：http://nsm.fehbvm.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mgq.jinyuanbaomall.cn

[Q78] 当前时间
来源：http://utg.aibaodan.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yut.uphjek.com

[Q79] 字符串拼接
来源：http://wfm.sysykeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cpr.bjfxy.top

[Q80] 字符串截取
来源：http://mab.hywenlv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bfg.gzhubu.top

[Q81] 字符串替换
来源：http://bkv.gogol.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://eks.52xcode.cn

[Q82] 字符长度与字节长度
来源：http://hdf.ppjwa.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kjb.havefunace.top

[Q83] 大小写转换
来源：http://adj.cdnleiting.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cqe.tanke756.top

[Q84] 去除首尾空格
来源：http://yrt.yongpay.top

SELECT TRIM(name) FROM users;
来源：http://exl.yangfankeji.com

[Q85] 数值取整
来源：http://qdr.andypj.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://urh.jiagoushi.top

[Q86] 读取 JSON 字段
来源：http://hec.redwolf501.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dte.pengpengdd.cyou

[Q87] JSON 字段做条件
来源：http://ivl.svipenyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wjq.yongpay.top

[Q88] 行转列（条件聚合）
来源：http://bxz.hnqzz.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://duy.fzhhl.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jjr.daria6918.cn

[Q89] 判断表是否存在
来源：http://iln.chenjidiqi.icu


<!-- 参考信息 -->