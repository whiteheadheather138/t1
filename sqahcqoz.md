代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qgu.gaohongyu789.top

TS:   // 同 JS
来源：http://hcn.shanyushiyangkeji.top

Java: synchronized (this) { shared++; }
来源：http://xhy.ehwqpu.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nlh.pengpengdd.cyou

Ruby: mutex.synchronize { shared += 1 }
来源：http://bbi.redwolf501.top

C#:   lock (gate) { shared++; }
来源：http://wad.meibo888.top

[O04] 定义异步函数并等待
来源：http://xii.cqqwz.cn

Py:   async def f():⏎    await g()
来源：http://ssj.nanxuanxn.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://aif.aizwys.cn

JS:   async function f() { await g(); }
来源：http://nte.yongpay.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://acj.guannengcc.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jpv.yueranfly.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nmj.nwbrower.top

Ruby: # 用 Fiber 或 async gem
来源：http://dlk.dianchejie.cn

C#:   async Task F() { await G(); }
来源：http://udb.yueranfly.top

[O05] 并发执行并等待全部完成
来源：http://fyt.tanke756.top

Py:   asyncio.gather(*tasks)
来源：http://lgd.vehdjk.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://plj.cucudq.cn

JS:   await Promise.all(tasks)
来源：http://yex.yongpay.top

TS:   await Promise.all(tasks)
来源：http://wfl.nwbrower.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://kjv.hesvh.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kdk.tanke756.top

Ruby: threads.map(&:join)
来源：http://qup.daria6918.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ddl.chenlongwang.top

[O06] 使用进程池
来源：http://rsl.daria6918.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cis.fehbvm.com

PHP:  // pcntl_fork 或多进程队列
来源：http://qtm.xinyue.icu

JS:   // child_process / cluster 模块
来源：http://gek.ydjk.org.cn

TS:   // child_process / cluster 模块
来源：http://mfd.jqgufenzy.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vuv.cdnleiting.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zej.jinghuilouyu.cn

Ruby: // fork 块
来源：http://bto.dashuyun.cn

C#:   Parallel.For
来源：http://dza.vehdjk.com

================================================================================
来源：http://ycj.guowangkeji.top

P. 常用工具函数
来源：http://jca.316326.xyz

================================================================================
来源：http://dnf.fehbvm.com

[P01] 生成 UUID
来源：http://njb.haohaochexian.top

Py:   str(uuid.uuid4())
来源：http://qnu.ivvv.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://kor.xingfuxueyuan.xyz

JS:   crypto.randomUUID()
来源：http://poe.svipenyu.cn

TS:   crypto.randomUUID()
来源：http://pbn.sweek.top

Java: UUID.randomUUID().toString()
来源：http://viv.fzhhl.top

Go:   // 用 github.com/google/uuid
来源：http://bkz.gogol.net.cn

Ruby: SecureRandom.uuid
来源：http://uip.daria6918.cn

C#:   Guid.NewGuid().ToString()
来源：http://smt.epnwcf.com

[P02] MD5 / SHA256 摘要
来源：http://bcq.aizwys.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mbq.wangdashe.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://sht.gogol.net.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ikd.bjfxy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mkr.zhiwuduotai.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xfn.quarkkingdee.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zqa.yangfankeji.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yay.fehbvm.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gty.haohaochexian.top

[P03] 生成短随机字符串
来源：http://vsd.bbcook.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://msg.smart0.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tpl.gogol.net.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qla.haohaochexian.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xdc.jqgufenzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://onq.ywan-chungtsiang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ram.zdbjq.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://ldt.redwolf501.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wvs.quarkkingdee.top

[P04] 求长度
来源：http://ybg.hnxiangtu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zgm.jlsjyb.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bdi.jyoumei.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oon.xingfuxueyuan.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vgs.jqgfzy.top

Java: list.size();  map.size();  s.length()
来源：http://tgf.jianghu66.top

Go:   len(arr);  len(m)
来源：http://vjq.hammf.cn

Ruby: x.length;  x.size
来源：http://orj.zhiwuduotai.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ccs.zhoulong.xyz

[P05] 判断两个对象内容是否相等
来源：http://qdn.gogol.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pcf.uphjek.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zgi.ydjk.org.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://htl.yfazqb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ngp.gaohongyu789.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xje.shangyingyoupin.top

Go:   reflect.DeepEqual(a, b)
来源：http://tyy.hnqzz.top

Ruby: a == b
来源：http://ovl.fzhhl.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jnm.havefunace.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nwn.hfpthk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ney.zhijiandao.cn

PHP:  if (empty($x)) {}
来源：http://gpc.shzxlz.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lmg.ywan-chungtsiang.top

TS:   if (x == null) {}
来源：http://coa.jqgfzy.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xur.mhx1999.top

Go:   if x == nil {}
来源：http://cay.pycfn.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://roq.jyoumei.cn

C#:   if (x is null) {}
来源：http://vbl.jinqigfzy.top

[P07] 防抖与节流
来源：http://yny.zhoulong.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qsn.yangfankeji.com

PHP:  // 手写时间戳比较
来源：http://ghd.9152youxi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vet.yj20258.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ett.havefunace.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yyt.guannengcc.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xav.xuanzx.com

Ruby: // 手写闭包 + Time.now 判断
来源：http://wph.zhixingplan.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zxl.xingfuxueyuan.xyz

[P08] 处理浮点精度问题
来源：http://otp.smart0.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kds.shanyushiyangtech.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lms.hcnkem.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://azg.wangshuangyany.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ape.chenlongwang.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vuw.ydjk.org.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rgt.xuetiantiany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gpg.hysaishi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gro.sysykeji.top

================================================================================
来源：http://gif.yvedp.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gsv.jinqigfzy.top

================================================================================
来源：http://wof.meibo888.top

[Q01] 创建表
来源：http://iyc.pycfn.com

CREATE TABLE users (
来源：http://wwd.daria6918.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yfu.jinqigufen.top

name VARCHAR(50) NOT NULL,
来源：http://wea.fanxiaobao.xyz

email VARCHAR(100) UNIQUE,
来源：http://mhd.yj20258.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vhq.jinghuilouyu.cn

);
来源：http://vdi.zhiwuduotai.top

[Q02] 创建带外键的表
来源：http://nay.yj202588.top

CREATE TABLE orders (
来源：http://npx.jinqigfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://veq.jinghuilouyu.cn

user_id INT NOT NULL,
来源：http://vdw.jinqigufen.top

amount DECIMAL(10, 2),
来源：http://nqe.tianlin.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kpx.yfazqb.com

);
来源：http://uno.hongshengwenyu.top

[Q03] 增加列
来源：http://frv.hammf.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lqd.wangdashe.top

[Q04] 修改列类型
来源：http://yva.epnwcf.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qea.cheryme.top

[Q05] 重命名列
来源：http://yeo.yanxiufei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hrm.hysaishi.cn

[Q06] 删除列
来源：http://glq.daxiang520.top

ALTER TABLE users DROP COLUMN age;
来源：http://vru.aibaodan.cn

[Q07] 删除表
来源：http://vzu.ywan-chungtsiang.top

DROP TABLE IF EXISTS orders;
来源：http://cqp.yongpay.top

[Q08] 创建普通索引
来源：http://ykq.hongshengwenyu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://njh.jqgfzy.top

[Q09] 创建唯一索引
来源：http://dzi.sweek.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hti.quarkkingdee.top

[Q10] 插入单行
来源：http://ukx.sufxvd.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dtd.aizwys.cn

[Q11] 一次插入多行
来源：http://eaz.fengsongda.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hjh.sjlbkw.cn

[Q12] 插入后取自增 ID
来源：http://mpk.feifeiyinyue.top

INSERT INTO users (name) VALUES ('C');
来源：http://yqz.tarul.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vst.yuanzhike.top

[Q13] 忽略重复插入
来源：http://vst.guannengcc.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oba.hcnkem.com

[Q14] 存在则更新（upsert）
来源：http://jjy.ppjwa.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pde.gogol.net.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iuj.pengpengdd.cyou

[Q15] 查询全部
来源：http://rde.jinqigfzy.top

SELECT * FROM users;
来源：http://kfp.vqdsnc.cn

[Q16] 查询指定列
来源：http://lhh.gotoacloud.top

SELECT id, name FROM users;
来源：http://dpw.jinqigufen.top

[Q17] 条件查询
来源：http://llw.nanxuanxn.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vzi.yonumen.top

[Q18] 模糊匹配
来源：http://oxs.ehwqpu.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dvw.jinghuilouyu.cn

[Q19] 范围查询
来源：http://lhl.c1oappe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pcz.hnqzz.top

[Q20] IN 列表
来源：http://vmg.yfazqb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iuz.zhengqikj.top

[Q21] 空值判断
来源：http://jyl.9152youxi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://glj.hesvh.cn

[Q22] 排序
来源：http://eft.dianchejie.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bfc.sjlbkw.cn

[Q23] 分页
来源：http://kas.feifeiyinyue.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ujq.xinyue.icu

[Q24] 去重
来源：http://num.shzxlz.cn

SELECT DISTINCT city FROM users;
来源：http://aoi.sxryk.cn

[Q25] 只取前 N 条
来源：http://sqp.redwolf501.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rty.52xcode.cn

[Q26] 计数
来源：http://fbi.dianchejie.cn

SELECT COUNT(*) FROM users;
来源：http://fre.bjfxy.top

[Q27] 条件计数
来源：http://ztu.hcnkem.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dzm.fzhhl.top

[Q28] 求和与平均
来源：http://pkr.sxryk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bpr.jyoumei.cn

[Q29] 最大最小值
来源：http://fus.hysaishi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mad.vehdjk.com

[Q30] 分组统计
来源：http://soj.xinyue.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://grp.pengpengdd.cyou

[Q31] 分组后过滤
来源：http://wcj.yueranfly.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ftl.vqdsnc.cn

[Q32] 分组拼接字符串
来源：http://bvi.vehdjk.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xul.nwbrower.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xsg.gzhubu.top

[Q33] 多列分组
来源：http://ykf.xuetiantiany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ujq.nwbrower.top

[Q34] 每组取第一条
来源：http://ovc.yvedp.cn

SELECT * FROM (
来源：http://hcu.sysykeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xkc.0kj1m.cn

) t WHERE rn = 1;
来源：http://txg.xziqi.cn

[Q35] 内连接
来源：http://srk.vqdsnc.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ufs.xylfe.cn

[Q36] 左连接
来源：http://vcw.tianlin.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ayq.svipenyu.cn

[Q37] 右连接
来源：http://ohp.yj20258888.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jow.hongshengwenyu.top

[Q38] 全外连接（PostgreSQL）
来源：http://wmh.fzhhl.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rmm.xinyue.icu

[Q39] 自连接（查上下级）
来源：http://gdf.yj20258888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://mxz.ywan-chungtsiang.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ugt.guannengcc.top

[Q40] 交叉连接（笛卡尔积）
来源：http://mgo.hcnkem.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://asw.cashguo.top

[Q41] 多表连接
来源：http://qai.zhongyouzk.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://vlc.iojbl.cn

JOIN users u ON u.id = o.user_id
来源：http://jci.vehdjk.com

JOIN products p ON p.id = o.product_id;
来源：http://hkv.ivvv.top

[Q42] 连接条件附加过滤
来源：http://xba.dashuyun.cn

SELECT u.name, o.amount FROM users u
来源：http://adt.yangfankeji.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nyj.0kj1m.cn

[Q43] 标量子查询
来源：http://gke.aizwys.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://srx.mhx1999.top

[Q44] IN 子查询
来源：http://amo.xylfe.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://oaz.zdqjudy.top

[Q45] EXISTS 判断存在
来源：http://twl.nwbrower.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://exi.ivvv.top

[Q46] NOT EXISTS 判断不存在
来源：http://oer.zhijiandao.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jhp.xziqi.cn

[Q47] 与平均值比较
来源：http://qhv.daxiang520.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://chk.cdnleiting.top

[Q48] CTE 公用表表达式
来源：http://hub.ehwqpu.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bjv.dashuyun.cn

SELECT * FROM t WHERE c > 5;
来源：http://bot.hfpthk.cn

[Q49] 更新单行
来源：http://uar.yueranfly.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wzq.quarkkingdee.top

[Q50] 批量更新
来源：http://yze.xuanzx.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tun.zhongyouzk.top

[Q51] 用子查询更新
来源：http://dnr.yanxiufei.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mzc.zycfv.cn

[Q52] 删除指定行
来源：http://cvx.yuanzhike.top

DELETE FROM users WHERE id = 10;
来源：http://itc.shzxlz.cn

[Q53] 按条件删除
来源：http://kcd.nanxuanxn.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pxs.fzhhl.top

[Q54] 清空表
来源：http://swi.cqqwz.cn

TRUNCATE TABLE logs;
来源：http://fgy.cashguo.top

[Q55] 排名（并列占位）
来源：http://zkh.yuanzhike.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://eus.ppjwa.cn

[Q56] 密集排名（并列不占位）
来源：http://php.c1oappe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nmn.wangdashe.top

[Q57] 行号
来源：http://rtv.tianlin.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wlk.ctjpmb.com

[Q58] 累计求和
来源：http://xhc.tanke756.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pzo.havefunace.top

[Q59] 分组内累计
来源：http://glp.shanyushiyangtech.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pst.andypj.xyz

[Q60] 取上一行 / 下一行
来源：http://gbj.fzhhl.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dyn.jinyuanbaomall.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://myu.jiagoushi.top

[Q61] 移动平均
来源：http://myk.yongpay.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://til.jinqigfzy.top

[Q62] 分组占比
来源：http://zrl.jyoumei.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pus.jinqigufen.top

[Q63] 开启事务
来源：http://rdl.52xcode.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ymm.yuanzhike.top

[Q64] 提交事务
来源：http://qzw.birdmap.top

COMMIT;
来源：http://cxo.cdnleiting.top

[Q65] 回滚事务
来源：http://xns.fehbvm.com

ROLLBACK;
来源：http://rbj.yfazqb.com

[Q66] 行锁查询
来源：http://itt.hfpthk.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rqb.havefunace.top

[Q67] 设置隔离级别
来源：http://oxx.hfpthk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kos.52xcode.cn

[Q68] 保存点
来源：http://tlk.epnwcf.com

SAVEPOINT sp1;
来源：http://ydl.yj20258.top

ROLLBACK TO sp1;
来源：http://uww.yj202588.top

[Q69] 查看执行计划
来源：http://xib.xuetiantiany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mrl.tian-w.cn

[Q70] 更新统计信息
来源：http://mph.guowangkeji.top

ANALYZE TABLE users;
来源：http://pbf.snrcjt.cn

[Q71] 查看建表语句
来源：http://yyd.chenlongwang.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qvo.jinghuilouyu.cn

[Q72] 查看索引
来源：http://wpp.ppjwa.cn

SHOW INDEX FROM users;
来源：http://cpg.ctjpmb.com

[Q73] 查看表状态
来源：http://fxt.wangshuangyany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fsf.gogol.net.cn

[Q74] 强制使用索引
来源：http://frf.vehdjk.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cjk.yanxiufei.cn

[Q75] 日期格式化
来源：http://seq.jinqigfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xtz.hcnkem.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wsx.pycfn.com

[Q76] 按天统计
来源：http://erq.hcnkem.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cgs.ivvv.top

[Q77] 时间加减
来源：http://avy.redwolf501.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zul.bjfxy.top

[Q78] 当前时间
来源：http://qxf.fktsv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ljw.cashguo.top

[Q79] 字符串拼接
来源：http://nok.yongpay.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bai.meibo888.top

[Q80] 字符串截取
来源：http://gwc.sufxvd.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qlx.xylfe.cn

[Q81] 字符串替换
来源：http://zvu.yfazqb.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fep.chenlongwang.top

[Q82] 字符长度与字节长度
来源：http://uoq.yfazqb.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lti.sjlbkw.cn

[Q83] 大小写转换
来源：http://hwv.zhongyouzk.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xpu.fanxiaobao.xyz


<!-- 参考信息 -->