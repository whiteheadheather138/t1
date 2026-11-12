代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dft.sysykeji.top

[O03] 加锁保护共享数据
来源：http://vbv.birdmap.top

Py:   with lock: shared += 1
来源：http://vnr.chenlongwang.top

PHP:  // 用 flock() 做文件锁
来源：http://ocg.kuanghao11.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://krs.jiagoushi.top

TS:   // 同 JS
来源：http://hxn.vehdjk.com

Java: synchronized (this) { shared++; }
来源：http://shv.hammf.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cze.ivvv.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rfb.aibaodan.cn

C#:   lock (gate) { shared++; }
来源：http://izl.zycfv.cn

[O04] 定义异步函数并等待
来源：http://azh.cucudq.cn

Py:   async def f():⏎    await g()
来源：http://dox.hnqzz.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iri.pengpengdd.cyou

JS:   async function f() { await g(); }
来源：http://gyb.cqqwz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://aup.wangshuangyany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hcj.chenjidiqi.icu

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wjq.wangshuangyany.cn

Ruby: # 用 Fiber 或 async gem
来源：http://rba.zhaomingkeji.xyz

C#:   async Task F() { await G(); }
来源：http://dsu.fengsongda.top

[O05] 并发执行并等待全部完成
来源：http://wdc.jqgfzy.top

Py:   asyncio.gather(*tasks)
来源：http://pru.nanxinkj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vtp.vehdjk.com

JS:   await Promise.all(tasks)
来源：http://odq.wangshuangyany.cn

TS:   await Promise.all(tasks)
来源：http://hry.sufxvd.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qew.yonumen.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ils.yfazqb.com

Ruby: threads.map(&:join)
来源：http://hpf.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://eve.sxryk.cn

[O06] 使用进程池
来源：http://wtj.jinyuanbaomall.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://way.wangdashe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ycy.zhoulong.xyz

JS:   // child_process / cluster 模块
来源：http://trt.chenzaomai.com

TS:   // child_process / cluster 模块
来源：http://bkq.cucudq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yjs.gogol.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bdr.ctjpmb.com

Ruby: // fork 块
来源：http://smw.fzhhl.top

C#:   Parallel.For
来源：http://pji.daxiang520.top

================================================================================
来源：http://ovb.kuanghao11.cn

P. 常用工具函数
来源：http://idb.fehbvm.com

================================================================================
来源：http://ymy.dashuyun.cn

[P01] 生成 UUID
来源：http://jze.xylfe.cn

Py:   str(uuid.uuid4())
来源：http://ugq.jqgfzy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jxz.pengpengdd.cyou

JS:   crypto.randomUUID()
来源：http://wzd.52xcode.cn

TS:   crypto.randomUUID()
来源：http://spn.ctjpmb.com

Java: UUID.randomUUID().toString()
来源：http://atc.yfazqb.com

Go:   // 用 github.com/google/uuid
来源：http://arh.andypj.xyz

Ruby: SecureRandom.uuid
来源：http://mfz.gotoacloud.top

C#:   Guid.NewGuid().ToString()
来源：http://vfa.zhijiandao.cn

[P02] MD5 / SHA256 摘要
来源：http://ufr.zhongyouzk.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://qrj.jinghuilouyu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hji.ctjpmb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pbj.vehdjk.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://olb.9152youxi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rgi.ywan-chungtsiang.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yqp.jqgfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qvb.yangfankeji.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://djq.aizwys.cn

[P03] 生成短随机字符串
来源：http://onq.yangfankeji.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mtr.ehwqpu.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bnw.xziqi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yux.zhixingplan.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bqt.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kfc.hcnkem.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mzj.jianghu66.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://vwz.shuidangran.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://cwo.guowangkeji.top

[P04] 求长度
来源：http://wbv.tianlin.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hnw.jinqigufen.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bnq.yuxming.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hdj.yongpay.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zvy.ydjk.org.cn

Java: list.size();  map.size();  s.length()
来源：http://uen.jinyuanbaomall.cn

Go:   len(arr);  len(m)
来源：http://zjx.meibo888.top

Ruby: x.length;  x.size
来源：http://zdb.yanxiufei.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://jup.sxryk.cn

[P05] 判断两个对象内容是否相等
来源：http://bec.yvedp.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://yvm.sxryk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zbp.andypj.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://txb.tarul.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wmy.hcnkem.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://efw.zhiwuduotai.top

Go:   reflect.DeepEqual(a, b)
来源：http://kzp.cucudq.cn

Ruby: a == b
来源：http://tam.jqgufenzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ecp.jinqigufen.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://cte.xingfuxueyuan.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vvu.yonumen.top

PHP:  if (empty($x)) {}
来源：http://amd.9152youxi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://eoz.daxiang520.top

TS:   if (x == null) {}
来源：http://ihc.hnqzz.top

Java: if (x == null || x.isEmpty()) {}
来源：http://umx.jinqigfzy.top

Go:   if x == nil {}
来源：http://ems.0kj1m.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ehn.mhx1999.top

C#:   if (x is null) {}
来源：http://tiz.fktsv.cn

[P07] 防抖与节流
来源：http://cbv.shangyingyoupin.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bvp.cdnleiting.top

PHP:  // 手写时间戳比较
来源：http://rzm.zhongyouzk.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fij.daxiang520.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cbl.jlsjyb.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kqs.52xcode.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wkr.yj20258.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://yav.gogol.net.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mds.feifeiyinyue.top

[P08] 处理浮点精度问题
来源：http://fsz.xziqi.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lhk.chenzaomai.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lwb.jiagoushi.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ysj.ivvv.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pja.nanxinkj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mjs.snrcjt.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dlr.gaohongyu789.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qtu.hfpthk.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://syu.sweek.top

================================================================================
来源：http://dvs.epnwcf.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mny.yj20258.top

================================================================================
来源：http://tam.ppjwa.cn

[Q01] 创建表
来源：http://xxh.sjlbkw.cn

CREATE TABLE users (
来源：http://rnn.tanke756.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jad.yanxiufei.cn

name VARCHAR(50) NOT NULL,
来源：http://yni.hnqzz.top

email VARCHAR(100) UNIQUE,
来源：http://cvx.chenlongwang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://var.dianchejie.cn

);
来源：http://mur.fengsongda.top

[Q02] 创建带外键的表
来源：http://epr.fengsongda.top

CREATE TABLE orders (
来源：http://jka.cashguo.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://liw.shzxlz.cn

user_id INT NOT NULL,
来源：http://wdc.sufxvd.cn

amount DECIMAL(10, 2),
来源：http://sau.0kj1m.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qbg.vqdsnc.cn

);
来源：http://jef.smart0.xyz

[Q03] 增加列
来源：http://nyq.yangfankeji.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://cgv.feifeiyinyue.top

[Q04] 修改列类型
来源：http://dsg.jinqigufen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yoi.0kj1m.cn

[Q05] 重命名列
来源：http://bgg.sweek.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ama.bjfxy.top

[Q06] 删除列
来源：http://tlf.jiagoushi.top

ALTER TABLE users DROP COLUMN age;
来源：http://hlu.yj20258888.top

[Q07] 删除表
来源：http://pop.ydzc1.top

DROP TABLE IF EXISTS orders;
来源：http://ujw.guowangkeji.top

[Q08] 创建普通索引
来源：http://tnq.gogol.net.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kdi.jqgufenzy.top

[Q09] 创建唯一索引
来源：http://bul.zdbjq.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jxm.hammf.cn

[Q10] 插入单行
来源：http://cua.andypj.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hgo.52xcode.cn

[Q11] 一次插入多行
来源：http://iye.nwbrower.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sqz.yonumen.top

[Q12] 插入后取自增 ID
来源：http://tzc.fehbvm.com

INSERT INTO users (name) VALUES ('C');
来源：http://sde.jiagoushi.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jnh.shanyushiyangtech.top

[Q13] 忽略重复插入
来源：http://zjd.xziqi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gzf.ctjpmb.com

[Q14] 存在则更新（upsert）
来源：http://hna.cqqwz.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://csm.jyoumei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://hfq.xziqi.cn

[Q15] 查询全部
来源：http://kzw.52xcode.cn

SELECT * FROM users;
来源：http://wjd.hammf.cn

[Q16] 查询指定列
来源：http://ldr.redwolf501.top

SELECT id, name FROM users;
来源：http://onv.shanyushiyangtech.top

[Q17] 条件查询
来源：http://mel.hongshengwenyu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ytw.ivvv.top

[Q18] 模糊匹配
来源：http://roq.birdmap.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oba.vehdjk.com

[Q19] 范围查询
来源：http://sbf.fehbvm.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nun.guowangkeji.top

[Q20] IN 列表
来源：http://xrq.zdbjq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dyk.hfpthk.cn

[Q21] 空值判断
来源：http://rqt.hongshengwenyu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://gfy.aizwys.cn

[Q22] 排序
来源：http://avz.xylfe.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fii.gotoacloud.top

[Q23] 分页
来源：http://xqu.sysykeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wej.tanke756.top

[Q24] 去重
来源：http://fjz.dashuyun.cn

SELECT DISTINCT city FROM users;
来源：http://oej.pycfn.com

[Q25] 只取前 N 条
来源：http://zjw.meibo888.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ejw.smart0.xyz

[Q26] 计数
来源：http://zto.tian-w.cn

SELECT COUNT(*) FROM users;
来源：http://jru.gaohongyu789.top

[Q27] 条件计数
来源：http://fjl.aizwys.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hug.cashguo.top

[Q28] 求和与平均
来源：http://aev.pycfn.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jzx.dashuyun.cn

[Q29] 最大最小值
来源：http://hbh.iojbl.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://yka.zycfv.cn

[Q30] 分组统计
来源：http://frx.svipenyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://juw.aibaodan.cn

[Q31] 分组后过滤
来源：http://rja.andypj.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mjc.zdbjq.cn

[Q32] 分组拼接字符串
来源：http://gkb.chenjidiqi.icu

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lkx.fehbvm.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xzv.yanxiufei.cn

[Q33] 多列分组
来源：http://gzj.jiagoushi.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rsy.hongshengwenyu.top

[Q34] 每组取第一条
来源：http://iyo.ywan-chungtsiang.top

SELECT * FROM (
来源：http://ibk.vehdjk.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qwk.pengpengdd.cyou

) t WHERE rn = 1;
来源：http://nhm.fehbvm.com

[Q35] 内连接
来源：http://otm.ydjk.org.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ehy.yuanzhike.top

[Q36] 左连接
来源：http://kzq.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gee.jianghu66.top

[Q37] 右连接
来源：http://who.ppjwa.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ggc.cheryme.top

[Q38] 全外连接（PostgreSQL）
来源：http://yxu.xingfuxueyuan.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zvw.bbcook.cn

[Q39] 自连接（查上下级）
来源：http://mer.xinyue.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://yzd.chenjidiqi.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://guz.havefunace.top

[Q40] 交叉连接（笛卡尔积）
来源：http://cze.chenjidiqi.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://prd.guowangkeji.top

[Q41] 多表连接
来源：http://wuk.ybcxt.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://yhc.ppjwa.cn

JOIN users u ON u.id = o.user_id
来源：http://gyj.haohaochexian.top

JOIN products p ON p.id = o.product_id;
来源：http://pga.wangshuangyany.cn

[Q42] 连接条件附加过滤
来源：http://rgp.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u
来源：http://oyq.ydjk.org.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xww.uphjek.com

[Q43] 标量子查询
来源：http://ecz.yj20258888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xnm.sxryk.cn

[Q44] IN 子查询
来源：http://yei.havefunace.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xtn.hnqzz.top

[Q45] EXISTS 判断存在
来源：http://jvg.yj20258888.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ppw.hnxiangtu.top

[Q46] NOT EXISTS 判断不存在
来源：http://lhs.tianlin.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qiz.tian-w.cn

[Q47] 与平均值比较
来源：http://sbd.dashuyun.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vco.dianchejie.cn

[Q48] CTE 公用表表达式
来源：http://xns.zhixingplan.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xmb.hesvh.cn

SELECT * FROM t WHERE c > 5;
来源：http://xdn.ppjwa.cn

[Q49] 更新单行
来源：http://vkv.hammf.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://myo.quarkkingdee.top

[Q50] 批量更新
来源：http://znr.ydzc1.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gvr.jqgfzy.top

[Q51] 用子查询更新
来源：http://ttu.zdqjudy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kvf.c1oappe.top

[Q52] 删除指定行
来源：http://zqq.aibaodan.cn

DELETE FROM users WHERE id = 10;
来源：http://txj.cqqwz.cn

[Q53] 按条件删除
来源：http://qho.yueranfly.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oup.pycfn.com

[Q54] 清空表
来源：http://skl.ydjk.org.cn

TRUNCATE TABLE logs;
来源：http://guh.fktsv.cn

[Q55] 排名（并列占位）
来源：http://ewu.kuanghao11.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fyp.jlsjyb.cn

[Q56] 密集排名（并列不占位）
来源：http://enz.shzxlz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dxs.hfpthk.cn

[Q57] 行号
来源：http://mcu.ydzc1.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vsi.fzhhl.top

[Q58] 累计求和
来源：http://maw.zdbjq.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://iza.hnxiangtu.top

[Q59] 分组内累计
来源：http://sof.yfazqb.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cil.svipenyu.cn

[Q60] 取上一行 / 下一行
来源：http://ape.jlsjyb.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yve.uphjek.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ohe.zhiwuduotai.top

[Q61] 移动平均
来源：http://yup.zdbjq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fxv.vehdjk.com

[Q62] 分组占比
来源：http://vwz.sysykeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://azc.xuetiantiany.cn

[Q63] 开启事务
来源：http://abb.9152youxi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ifg.yangfankeji.com

[Q64] 提交事务
来源：http://kak.gzhubu.top

COMMIT;
来源：http://opx.xuanzx.com

[Q65] 回滚事务
来源：http://ogp.sjlbkw.cn

ROLLBACK;
来源：http://yaj.iojbl.cn

[Q66] 行锁查询
来源：http://cmh.ybcxt.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tcj.snrcjt.cn

[Q67] 设置隔离级别
来源：http://pqw.ydzc1.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jhl.wangdashe.top

[Q68] 保存点
来源：http://ckg.hammf.cn

SAVEPOINT sp1;
来源：http://mef.hcnkem.com

ROLLBACK TO sp1;
来源：http://swj.vehdjk.com

[Q69] 查看执行计划
来源：http://vdp.mhx1999.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uvv.hfpthk.cn

[Q70] 更新统计信息
来源：http://bwq.cdnleiting.top

ANALYZE TABLE users;
来源：http://lkr.dashuyun.cn

[Q71] 查看建表语句
来源：http://tmh.tianlin.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://irm.yonumen.top

[Q72] 查看索引
来源：http://guo.jlsjyb.cn

SHOW INDEX FROM users;
来源：http://hqb.yuanzhike.top

[Q73] 查看表状态
来源：http://yew.gzhubu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://kyx.chenjidiqi.icu

[Q74] 强制使用索引
来源：http://frb.shzxlz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dkz.yfazqb.com

[Q75] 日期格式化
来源：http://sbn.smart0.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://chs.nanxinkj.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iir.jqgufenzy.top

[Q76] 按天统计
来源：http://jxg.cdnleiting.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uvm.wangdashe.top

[Q77] 时间加减
来源：http://ipq.epnwcf.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bfc.tanke756.top

[Q78] 当前时间
来源：http://rsp.wangdashe.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hyb.nwbrower.top

[Q79] 字符串拼接
来源：http://rjg.guowangkeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://isl.fzhhl.top

[Q80] 字符串截取
来源：http://tlq.jqgufenzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jro.xuetiantiany.cn

[Q81] 字符串替换
来源：http://sgl.chenjidiqi.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kxq.gaohongyu789.top


<!-- 参考信息 -->