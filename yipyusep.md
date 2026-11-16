代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qxq.jianghu66.top

[O03] 加锁保护共享数据
来源：http://qsk.chenzaomai.com

Py:   with lock: shared += 1
来源：http://dgv.chenzaomai.com

PHP:  // 用 flock() 做文件锁
来源：http://xrl.haohaochexian.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://aib.tian-w.cn

TS:   // 同 JS
来源：http://fig.yuxming.cn

Java: synchronized (this) { shared++; }
来源：http://drl.sufxvd.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://khj.cheryme.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://isi.guannengcc.top

C#:   lock (gate) { shared++; }
来源：http://lym.shzxlz.cn

[O04] 定义异步函数并等待
来源：http://has.pycfn.com

Py:   async def f():⏎    await g()
来源：http://dwf.smart0.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://oue.hywenlv.cn

JS:   async function f() { await g(); }
来源：http://yrw.xingfuxueyuan.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://jal.svipenyu.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lrf.hongshengwenyu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cva.yueranfly.top

Ruby: # 用 Fiber 或 async gem
来源：http://tse.ybcxt.top

C#:   async Task F() { await G(); }
来源：http://xdw.gogol.net.cn

[O05] 并发执行并等待全部完成
来源：http://shq.bbcook.cn

Py:   asyncio.gather(*tasks)
来源：http://iup.guowangkeji.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pjr.ctjpmb.com

JS:   await Promise.all(tasks)
来源：http://kkw.jinqigfzy.top

TS:   await Promise.all(tasks)
来源：http://ghm.hysaishi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dry.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://chh.chenlongwang.top

Ruby: threads.map(&:join)
来源：http://hqy.dashuyun.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://drc.guowangkeji.top

[O06] 使用进程池
来源：http://wch.zhongyouzk.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wkq.xuanzx.com

PHP:  // pcntl_fork 或多进程队列
来源：http://piu.ydzc1.top

JS:   // child_process / cluster 模块
来源：http://tma.jianghu66.top

TS:   // child_process / cluster 模块
来源：http://cvw.tanke756.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://gdn.dashuyun.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ges.hcnkem.com

Ruby: // fork 块
来源：http://xbm.xylfe.cn

C#:   Parallel.For
来源：http://fyg.pycfn.com

================================================================================
来源：http://lbo.ehwqpu.com

P. 常用工具函数
来源：http://rbm.sweek.top

================================================================================
来源：http://rhg.jiagoushi.top

[P01] 生成 UUID
来源：http://uep.meibo888.top

Py:   str(uuid.uuid4())
来源：http://ctb.tian-w.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vyv.chenlongwang.top

JS:   crypto.randomUUID()
来源：http://hpn.fktsv.cn

TS:   crypto.randomUUID()
来源：http://emg.c1oappe.top

Java: UUID.randomUUID().toString()
来源：http://mcs.snrcjt.cn

Go:   // 用 github.com/google/uuid
来源：http://upm.pengpengdd.cyou

Ruby: SecureRandom.uuid
来源：http://gcu.birdmap.top

C#:   Guid.NewGuid().ToString()
来源：http://rgy.gaohongyu789.top

[P02] MD5 / SHA256 摘要
来源：http://kdv.zhoulong.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tbq.vehdjk.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://eev.vqdsnc.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mxf.hywenlv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jau.yueranfly.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jpq.chenjidiqi.icu

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ybh.nanxuanxn.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ryk.yuanzhike.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wsp.hesvh.cn

[P03] 生成短随机字符串
来源：http://zmz.feifeiyinyue.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://oeb.daxiang520.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wis.wangshuangyany.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://scl.xziqi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pjw.yanxiufei.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mpg.fzhhl.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xng.gogol.net.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://usf.hysaishi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sam.hcnkem.com

[P04] 求长度
来源：http://vji.chenzaomai.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hbj.hongshengwenyu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gbj.guannengcc.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yvo.yuxming.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ivo.ehwqpu.com

Java: list.size();  map.size();  s.length()
来源：http://ngr.tarul.cn

Go:   len(arr);  len(m)
来源：http://wfr.kuanghao11.cn

Ruby: x.length;  x.size
来源：http://iok.zhixingplan.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dqi.birdmap.top

[P05] 判断两个对象内容是否相等
来源：http://rhk.pengpengdd.cyou

Py:   a == b              # 列表与字典递归比较内容
来源：http://kds.zdqjudy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xir.haohaochexian.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://joz.shanyushiyangtech.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ddq.dashuyun.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rbu.jinyuanbaomall.cn

Go:   reflect.DeepEqual(a, b)
来源：http://kst.yanxiufei.cn

Ruby: a == b
来源：http://uul.quarkkingdee.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ekt.jqgfzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wpk.xinyue.icu

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://aeq.ctjpmb.com

PHP:  if (empty($x)) {}
来源：http://aks.jinghuilouyu.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lvo.hcnkem.com

TS:   if (x == null) {}
来源：http://yfc.ydjk.org.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://cim.hcnkem.com

Go:   if x == nil {}
来源：http://lmh.9152youxi.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ihu.ppjwa.cn

C#:   if (x is null) {}
来源：http://lwr.sjlbkw.cn

[P07] 防抖与节流
来源：http://vrk.shzxlz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://eqk.vqdsnc.cn

PHP:  // 手写时间戳比较
来源：http://dhq.ehwqpu.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xpl.sxryk.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eis.chenjidiqi.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mmd.hesvh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jiq.fktsv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ute.fengsongda.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://eur.tanke756.top

[P08] 处理浮点精度问题
来源：http://uud.zhaomingkeji.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wfp.zhongyouzk.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://pgx.iojbl.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://aoh.zhengqikj.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ymu.daxiang520.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hzo.hcnkem.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://twc.sjlbkw.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tui.tianlin.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zbj.xingfuxueyuan.xyz

================================================================================
来源：http://lyw.feifeiyinyue.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wnl.yvedp.cn

================================================================================
来源：http://yte.yuxming.cn

[Q01] 创建表
来源：http://vez.hnqzz.top

CREATE TABLE users (
来源：http://vop.xziqi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wet.pycfn.com

name VARCHAR(50) NOT NULL,
来源：http://ynz.yangfankeji.com

email VARCHAR(100) UNIQUE,
来源：http://xrb.shangyingyoupin.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kni.zdbjq.cn

);
来源：http://zci.sufxvd.cn

[Q02] 创建带外键的表
来源：http://qkd.gogol.net.cn

CREATE TABLE orders (
来源：http://pwp.c1oappe.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nkf.tianlin.xyz

user_id INT NOT NULL,
来源：http://zns.sweek.top

amount DECIMAL(10, 2),
来源：http://zrc.fengsongda.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ysl.svipenyu.cn

);
来源：http://msx.chenzaomai.com

[Q03] 增加列
来源：http://zph.yueranfly.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rir.cqqwz.cn

[Q04] 修改列类型
来源：http://buy.chenjidiqi.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yxp.ydjk.org.cn

[Q05] 重命名列
来源：http://bkx.tarul.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qit.zhaomingkeji.xyz

[Q06] 删除列
来源：http://xdf.redwolf501.top

ALTER TABLE users DROP COLUMN age;
来源：http://mrt.svipenyu.cn

[Q07] 删除表
来源：http://wor.chenzaomai.com

DROP TABLE IF EXISTS orders;
来源：http://rxx.feifeiyinyue.top

[Q08] 创建普通索引
来源：http://azt.yangfankeji.com

CREATE INDEX idx_users_email ON users(email);
来源：http://jvg.316326.xyz

[Q09] 创建唯一索引
来源：http://bur.jlsjyb.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://whe.yj20258888.top

[Q10] 插入单行
来源：http://btc.hfpthk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fuw.hfpthk.cn

[Q11] 一次插入多行
来源：http://cpc.sufxvd.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sbz.hcnkem.com

[Q12] 插入后取自增 ID
来源：http://aac.mhx1999.top

INSERT INTO users (name) VALUES ('C');
来源：http://sba.tanke756.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wdt.316326.xyz

[Q13] 忽略重复插入
来源：http://lxy.jiagoushi.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vhf.fengsongda.top

[Q14] 存在则更新（upsert）
来源：http://mqf.zhijiandao.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ssl.c1oappe.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://okw.chenzaomai.com

[Q15] 查询全部
来源：http://wqc.gotoacloud.top

SELECT * FROM users;
来源：http://qpd.hammf.cn

[Q16] 查询指定列
来源：http://pyp.chenlongwang.top

SELECT id, name FROM users;
来源：http://hnr.yfazqb.com

[Q17] 条件查询
来源：http://mgt.ywan-chungtsiang.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yki.zhoulong.xyz

[Q18] 模糊匹配
来源：http://afu.yangfankeji.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kkr.ywan-chungtsiang.top

[Q19] 范围查询
来源：http://jfh.xingfuxueyuan.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hod.ybcxt.top

[Q20] IN 列表
来源：http://zhn.c1oappe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wvk.yuanzhike.top

[Q21] 空值判断
来源：http://bsc.wangshuangyany.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vmj.hysaishi.cn

[Q22] 排序
来源：http://akv.vqdsnc.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ecv.yj20258888.top

[Q23] 分页
来源：http://mdg.shzxlz.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ngy.xylfe.cn

[Q24] 去重
来源：http://yay.yangfankeji.com

SELECT DISTINCT city FROM users;
来源：http://ypq.jyoumei.cn

[Q25] 只取前 N 条
来源：http://qva.nwbrower.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ldq.cqqwz.cn

[Q26] 计数
来源：http://vqa.tian-w.cn

SELECT COUNT(*) FROM users;
来源：http://qcq.havefunace.top

[Q27] 条件计数
来源：http://qmb.jqgfzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ofh.andypj.xyz

[Q28] 求和与平均
来源：http://lma.316326.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vol.zhijiandao.cn

[Q29] 最大最小值
来源：http://xoi.nwbrower.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://qwn.9152youxi.cn

[Q30] 分组统计
来源：http://kbd.tianlin.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ksk.fehbvm.com

[Q31] 分组后过滤
来源：http://sez.fehbvm.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qaq.jqgufenzy.top

[Q32] 分组拼接字符串
来源：http://zda.yueranfly.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zin.nanxinkj.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qvz.ydzc1.top

[Q33] 多列分组
来源：http://kzg.wangdashe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rkn.fzhhl.top

[Q34] 每组取第一条
来源：http://ksc.smart0.xyz

SELECT * FROM (
来源：http://ocd.havefunace.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rft.andypj.xyz

) t WHERE rn = 1;
来源：http://jge.zhixingplan.top

[Q35] 内连接
来源：http://dve.tarul.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lsp.svipenyu.cn

[Q36] 左连接
来源：http://fec.tarul.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wkp.shzxlz.cn

[Q37] 右连接
来源：http://mav.hnxiangtu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://szl.meibo888.top

[Q38] 全外连接（PostgreSQL）
来源：http://efv.hesvh.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ssq.vehdjk.com

[Q39] 自连接（查上下级）
来源：http://ohc.yvedp.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qud.quarkkingdee.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://emy.9152youxi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://qyb.yj20258.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jcs.hammf.cn

[Q41] 多表连接
来源：http://hyo.hfpthk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tok.fehbvm.com

JOIN users u ON u.id = o.user_id
来源：http://tfy.tanke756.top

JOIN products p ON p.id = o.product_id;
来源：http://dqv.jiagoushi.top

[Q42] 连接条件附加过滤
来源：http://aje.yuanzhike.top

SELECT u.name, o.amount FROM users u
来源：http://jba.yueranfly.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kwh.yangfankeji.com

[Q43] 标量子查询
来源：http://wyz.cdnleiting.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://myl.zhongyouzk.top

[Q44] IN 子查询
来源：http://wdk.quarkkingdee.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qru.nanxuanxn.top

[Q45] EXISTS 判断存在
来源：http://zlb.shanyushiyangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://khd.hywenlv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wyo.yangfankeji.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://heb.sjlbkw.cn

[Q47] 与平均值比较
来源：http://qkj.kuanghao11.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xue.hammf.cn

[Q48] CTE 公用表表达式
来源：http://wtz.hcnkem.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fip.yj202588.top

SELECT * FROM t WHERE c > 5;
来源：http://ued.52xcode.cn

[Q49] 更新单行
来源：http://sia.epnwcf.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://abu.jqgfzy.top

[Q50] 批量更新
来源：http://tqd.wangdashe.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dyg.xingfuxueyuan.xyz

[Q51] 用子查询更新
来源：http://iav.birdmap.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xyx.chenzaomai.com

[Q52] 删除指定行
来源：http://fkj.jlsjyb.cn

DELETE FROM users WHERE id = 10;
来源：http://rok.9152youxi.cn

[Q53] 按条件删除
来源：http://vmq.meibo888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rrc.ybcxt.top

[Q54] 清空表
来源：http://hwe.yfazqb.com

TRUNCATE TABLE logs;
来源：http://jcr.jinqigufen.top

[Q55] 排名（并列占位）
来源：http://mle.jinghuilouyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://adz.hammf.cn

[Q56] 密集排名（并列不占位）
来源：http://zhh.mhx1999.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wui.tianlin.xyz

[Q57] 行号
来源：http://shh.fktsv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yoy.zhiwuduotai.top

[Q58] 累计求和
来源：http://qtb.svipenyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pwf.guannengcc.top

[Q59] 分组内累计
来源：http://nlk.sjlbkw.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gnn.epnwcf.com

[Q60] 取上一行 / 下一行
来源：http://ybb.zhixingplan.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pjv.chenjidiqi.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wdn.vehdjk.com

[Q61] 移动平均
来源：http://gbv.zhixingplan.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bti.tian-w.cn

[Q62] 分组占比
来源：http://odg.uphjek.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zca.zhijiandao.cn

[Q63] 开启事务
来源：http://cih.xinyue.icu

START TRANSACTION;                -- 或 BEGIN
来源：http://ulb.jinghuilouyu.cn

[Q64] 提交事务
来源：http://yiz.sweek.top

COMMIT;
来源：http://uwe.tianlin.xyz

[Q65] 回滚事务
来源：http://lzi.dianchejie.cn

ROLLBACK;
来源：http://pxc.yj20258888.top

[Q66] 行锁查询
来源：http://cfw.feifeiyinyue.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vns.daxiang520.top

[Q67] 设置隔离级别
来源：http://nzd.yfazqb.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tgb.chenjidiqi.icu

[Q68] 保存点
来源：http://bij.shangyingyoupin.top

SAVEPOINT sp1;
来源：http://ylr.shanyushiyangkeji.top

ROLLBACK TO sp1;
来源：http://whx.xinyue.icu

[Q69] 查看执行计划
来源：http://uvx.cucudq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wft.shzxlz.cn

[Q70] 更新统计信息
来源：http://iwq.tanke756.top

ANALYZE TABLE users;
来源：http://isi.sysykeji.top

[Q71] 查看建表语句
来源：http://xyw.jianghu66.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://opv.yuxming.cn

[Q72] 查看索引
来源：http://teb.gaohongyu789.top

SHOW INDEX FROM users;
来源：http://uih.yj202588.top

[Q73] 查看表状态
来源：http://gqr.sysykeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://loj.zhongyouzk.top

[Q74] 强制使用索引
来源：http://kvw.jinyuanbaomall.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bbs.52xcode.cn

[Q75] 日期格式化
来源：http://xad.zhongyouzk.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://flq.cdnleiting.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://goy.feifeiyinyue.top

[Q76] 按天统计
来源：http://kuy.aizwys.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mzy.sxryk.cn

[Q77] 时间加减
来源：http://poh.ivvv.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://syx.zhoulong.xyz

[Q78] 当前时间
来源：http://iqe.shzxlz.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ayh.yangfankeji.com

[Q79] 字符串拼接
来源：http://pyz.zdqjudy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ulj.jinqigufen.top

[Q80] 字符串截取
来源：http://rqv.yongpay.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vpm.c1oappe.top

[Q81] 字符串替换
来源：http://idn.cheryme.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zaq.jqgufenzy.top


<!-- 参考信息 -->