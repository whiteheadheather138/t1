代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fxb.hammf.cn

[O03] 加锁保护共享数据
来源：http://xtf.uphjek.com

Py:   with lock: shared += 1
来源：http://zku.andypj.xyz

PHP:  // 用 flock() 做文件锁
来源：http://iez.gaohongyu789.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dya.epnwcf.com

TS:   // 同 JS
来源：http://ffw.jqgufenzy.top

Java: synchronized (this) { shared++; }
来源：http://kkq.pengpengdd.cyou

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dzf.cashguo.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://nqt.yj20258.top

C#:   lock (gate) { shared++; }
来源：http://rqj.shuidangran.top

[O04] 定义异步函数并等待
来源：http://wmj.xinyue.icu

Py:   async def f():⏎    await g()
来源：http://osm.uphjek.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ibc.shangyingyoupin.top

JS:   async function f() { await g(); }
来源：http://ibf.xuetiantiany.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://chq.feifeiyinyue.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bem.tarul.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gia.jiagoushi.top

Ruby: # 用 Fiber 或 async gem
来源：http://lqa.redwolf501.top

C#:   async Task F() { await G(); }
来源：http://oxp.daxiang520.top

[O05] 并发执行并等待全部完成
来源：http://svl.cucudq.cn

Py:   asyncio.gather(*tasks)
来源：http://pmx.zycfv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ppk.hesvh.cn

JS:   await Promise.all(tasks)
来源：http://oou.tian-w.cn

TS:   await Promise.all(tasks)
来源：http://nbb.shzxlz.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fac.ehwqpu.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qhr.chenzaomai.com

Ruby: threads.map(&:join)
来源：http://ujf.redwolf501.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hxx.sweek.top

[O06] 使用进程池
来源：http://oum.sweek.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qxw.vqdsnc.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://csp.yonumen.top

JS:   // child_process / cluster 模块
来源：http://aci.yuxming.cn

TS:   // child_process / cluster 模块
来源：http://iea.ctjpmb.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://sip.fzhhl.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ktd.chenlongwang.top

Ruby: // fork 块
来源：http://mgc.fehbvm.com

C#:   Parallel.For
来源：http://uev.hcnkem.com

================================================================================
来源：http://aym.tian-w.cn

P. 常用工具函数
来源：http://syf.hywenlv.cn

================================================================================
来源：http://wja.xuetiantiany.cn

[P01] 生成 UUID
来源：http://cjm.dashuyun.cn

Py:   str(uuid.uuid4())
来源：http://ets.hesvh.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uys.yvedp.cn

JS:   crypto.randomUUID()
来源：http://ovw.xinyue.icu

TS:   crypto.randomUUID()
来源：http://elk.guannengcc.top

Java: UUID.randomUUID().toString()
来源：http://lgp.hesvh.cn

Go:   // 用 github.com/google/uuid
来源：http://atb.hfpthk.cn

Ruby: SecureRandom.uuid
来源：http://rqk.zhijiandao.cn

C#:   Guid.NewGuid().ToString()
来源：http://tag.nanxuanxn.top

[P02] MD5 / SHA256 摘要
来源：http://pdp.bjfxy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://coe.svipenyu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://spd.nwbrower.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mte.xuanzx.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jzi.tanke756.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mfj.52xcode.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qrp.daria6918.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tya.vehdjk.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vvz.jinghuilouyu.cn

[P03] 生成短随机字符串
来源：http://swo.sxryk.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hko.yj202588.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://sqz.chenzaomai.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rdv.ppjwa.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xqt.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fie.zhaomingkeji.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://fne.yanxiufei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://hyq.zhaomingkeji.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jgu.smart0.xyz

[P04] 求长度
来源：http://flq.iojbl.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ppk.smart0.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nen.pycfn.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qke.yj202588.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://akd.yuanzhike.top

Java: list.size();  map.size();  s.length()
来源：http://dwz.jqgufenzy.top

Go:   len(arr);  len(m)
来源：http://aru.chenzaomai.com

Ruby: x.length;  x.size
来源：http://iee.svipenyu.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ztr.sufxvd.cn

[P05] 判断两个对象内容是否相等
来源：http://htf.sufxvd.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bgn.epnwcf.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jbb.yj20258888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jas.iojbl.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xab.hcnkem.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://tvi.hywenlv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://awo.wangshuangyany.cn

Ruby: a == b
来源：http://nmt.dianchejie.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qes.tanke756.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://dok.zycfv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fkn.ivvv.top

PHP:  if (empty($x)) {}
来源：http://eoh.vehdjk.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fpt.fengsongda.top

TS:   if (x == null) {}
来源：http://gzk.guannengcc.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ixy.zhijiandao.cn

Go:   if x == nil {}
来源：http://nvi.jyoumei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yds.yongpay.top

C#:   if (x is null) {}
来源：http://tff.xingfuxueyuan.xyz

[P07] 防抖与节流
来源：http://qfb.pycfn.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yyn.jqgfzy.top

PHP:  // 手写时间戳比较
来源：http://ptt.chenjidiqi.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lwh.shzxlz.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yxj.uphjek.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ann.yuxming.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hgm.haohaochexian.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cpj.fktsv.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://hzb.xinyue.icu

[P08] 处理浮点精度问题
来源：http://oeo.zhixingplan.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qao.zhoulong.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vsw.shanyushiyangkeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xao.jiagoushi.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wkx.9152youxi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zhr.sysykeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wxp.epnwcf.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dmo.gotoacloud.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://see.chenjidiqi.icu

================================================================================
来源：http://cty.haohaochexian.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://azn.vqdsnc.cn

================================================================================
来源：http://wts.xinyue.icu

[Q01] 创建表
来源：http://ejf.jlsjyb.cn

CREATE TABLE users (
来源：http://eqr.zycfv.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pof.yfazqb.com

name VARCHAR(50) NOT NULL,
来源：http://bte.nanxinkj.top

email VARCHAR(100) UNIQUE,
来源：http://wwt.hywenlv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xtn.uphjek.com

);
来源：http://yba.hysaishi.cn

[Q02] 创建带外键的表
来源：http://wgj.sjlbkw.cn

CREATE TABLE orders (
来源：http://ulj.birdmap.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://avq.nanxuanxn.top

user_id INT NOT NULL,
来源：http://zcn.tianlin.xyz

amount DECIMAL(10, 2),
来源：http://out.xylfe.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://fzx.sweek.top

);
来源：http://cen.kuanghao11.cn

[Q03] 增加列
来源：http://wzx.jqgufenzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://oav.kuanghao11.cn

[Q04] 修改列类型
来源：http://qiy.sxryk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://evq.snrcjt.cn

[Q05] 重命名列
来源：http://xui.hcnkem.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bwu.fzhhl.top

[Q06] 删除列
来源：http://sla.zdbjq.cn

ALTER TABLE users DROP COLUMN age;
来源：http://oaz.yanxiufei.cn

[Q07] 删除表
来源：http://qod.sjlbkw.cn

DROP TABLE IF EXISTS orders;
来源：http://jgx.shzxlz.cn

[Q08] 创建普通索引
来源：http://fsx.tian-w.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lhu.jinyuanbaomall.cn

[Q09] 创建唯一索引
来源：http://tuh.jqgfzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dxi.sweek.top

[Q10] 插入单行
来源：http://svj.birdmap.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vtb.zhijiandao.cn

[Q11] 一次插入多行
来源：http://dsa.xziqi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kqe.tian-w.cn

[Q12] 插入后取自增 ID
来源：http://egb.yuanzhike.top

INSERT INTO users (name) VALUES ('C');
来源：http://wsn.dashuyun.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yoa.shuidangran.top

[Q13] 忽略重复插入
来源：http://piq.jinyuanbaomall.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hrx.zhoulong.xyz

[Q14] 存在则更新（upsert）
来源：http://zhm.fehbvm.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://trv.redwolf501.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gim.gotoacloud.top

[Q15] 查询全部
来源：http://jey.tianlin.xyz

SELECT * FROM users;
来源：http://bhl.cashguo.top

[Q16] 查询指定列
来源：http://bbv.jqgfzy.top

SELECT id, name FROM users;
来源：http://txi.yueranfly.top

[Q17] 条件查询
来源：http://ltu.nwbrower.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://luu.fengsongda.top

[Q18] 模糊匹配
来源：http://aoc.316326.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wws.quarkkingdee.top

[Q19] 范围查询
来源：http://kjq.ydjk.org.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xdx.mhx1999.top

[Q20] IN 列表
来源：http://sgg.yj202588.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ejf.hammf.cn

[Q21] 空值判断
来源：http://mfv.aizwys.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gme.sxryk.cn

[Q22] 排序
来源：http://bxk.yuanzhike.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://abh.iojbl.cn

[Q23] 分页
来源：http://yfz.ehwqpu.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://nkc.ydzc1.top

[Q24] 去重
来源：http://suf.jqgfzy.top

SELECT DISTINCT city FROM users;
来源：http://nwb.zhaomingkeji.xyz

[Q25] 只取前 N 条
来源：http://neu.jlsjyb.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lns.yvedp.cn

[Q26] 计数
来源：http://hvn.chenzaomai.com

SELECT COUNT(*) FROM users;
来源：http://tno.xingfuxueyuan.xyz

[Q27] 条件计数
来源：http://efg.fanxiaobao.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kaf.yj20258888.top

[Q28] 求和与平均
来源：http://ofc.yuanzhike.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tit.iojbl.cn

[Q29] 最大最小值
来源：http://dfk.xinyue.icu

SELECT MAX(age), MIN(age) FROM users;
来源：http://vak.yuanzhike.top

[Q30] 分组统计
来源：http://qdl.zdqjudy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dzg.hywenlv.cn

[Q31] 分组后过滤
来源：http://nap.haohaochexian.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nnl.smart0.xyz

[Q32] 分组拼接字符串
来源：http://thp.c1oappe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lyj.snrcjt.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://aiv.fengsongda.top

[Q33] 多列分组
来源：http://ega.jyoumei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://uhy.9152youxi.cn

[Q34] 每组取第一条
来源：http://jxp.pengpengdd.cyou

SELECT * FROM (
来源：http://rjs.andypj.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nlm.snrcjt.cn

) t WHERE rn = 1;
来源：http://otn.hongshengwenyu.top

[Q35] 内连接
来源：http://uhu.hcnkem.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://iuu.fengsongda.top

[Q36] 左连接
来源：http://acc.hywenlv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rfr.shanyushiyangtech.top

[Q37] 右连接
来源：http://jpd.svipenyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wyq.bjfxy.top

[Q38] 全外连接（PostgreSQL）
来源：http://etv.xuetiantiany.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cjt.cqqwz.cn

[Q39] 自连接（查上下级）
来源：http://crq.sjlbkw.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://vkl.fktsv.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rmf.zhijiandao.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zja.epnwcf.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jyv.shangyingyoupin.top

[Q41] 多表连接
来源：http://tlp.ivvv.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://gnj.jianghu66.top

JOIN users u ON u.id = o.user_id
来源：http://nyb.pycfn.com

JOIN products p ON p.id = o.product_id;
来源：http://clr.fehbvm.com

[Q42] 连接条件附加过滤
来源：http://hrt.yangfankeji.com

SELECT u.name, o.amount FROM users u
来源：http://twk.pycfn.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sje.pengpengdd.cyou

[Q43] 标量子查询
来源：http://coc.yanxiufei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ily.zhaomingkeji.xyz

[Q44] IN 子查询
来源：http://oij.52xcode.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://obk.kuanghao11.cn

[Q45] EXISTS 判断存在
来源：http://mkq.nwbrower.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gsg.tianlin.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://odd.yfazqb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://daj.xinyue.icu

[Q47] 与平均值比较
来源：http://mnw.iojbl.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vrn.jinghuilouyu.cn

[Q48] CTE 公用表表达式
来源：http://gsg.aizwys.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kdg.ivvv.top

SELECT * FROM t WHERE c > 5;
来源：http://ffd.vehdjk.com

[Q49] 更新单行
来源：http://zcj.andypj.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zhj.316326.xyz

[Q50] 批量更新
来源：http://pni.yanxiufei.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kkh.nwbrower.top

[Q51] 用子查询更新
来源：http://aya.ywan-chungtsiang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dgp.meibo888.top

[Q52] 删除指定行
来源：http://hkd.pengpengdd.cyou

DELETE FROM users WHERE id = 10;
来源：http://hvt.ydzc1.top

[Q53] 按条件删除
来源：http://bor.xuanzx.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vzm.yfazqb.com

[Q54] 清空表
来源：http://mfb.aizwys.cn

TRUNCATE TABLE logs;
来源：http://byz.quarkkingdee.top

[Q55] 排名（并列占位）
来源：http://icm.wangdashe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tbl.aibaodan.cn

[Q56] 密集排名（并列不占位）
来源：http://snz.shzxlz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pcg.fktsv.cn

[Q57] 行号
来源：http://rvf.yj202588.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xve.yonumen.top

[Q58] 累计求和
来源：http://lol.ydzc1.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zuf.jinqigufen.top

[Q59] 分组内累计
来源：http://hjv.hywenlv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ifk.daxiang520.top

[Q60] 取上一行 / 下一行
来源：http://nqf.iojbl.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://asx.ivvv.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mvk.hongshengwenyu.top

[Q61] 移动平均
来源：http://wti.0kj1m.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://llx.tanke756.top

[Q62] 分组占比
来源：http://gni.uphjek.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nds.pycfn.com

[Q63] 开启事务
来源：http://hlv.hywenlv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pxo.hywenlv.cn

[Q64] 提交事务
来源：http://sve.shuidangran.top

COMMIT;
来源：http://wtp.yvedp.cn

[Q65] 回滚事务
来源：http://ndi.hysaishi.cn

ROLLBACK;
来源：http://hrk.9152youxi.cn

[Q66] 行锁查询
来源：http://dhk.sweek.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://khy.zhongyouzk.top

[Q67] 设置隔离级别
来源：http://ibp.jiagoushi.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jwo.9152youxi.cn

[Q68] 保存点
来源：http://sdk.haohaochexian.top

SAVEPOINT sp1;
来源：http://wry.bjfxy.top

ROLLBACK TO sp1;
来源：http://dts.quarkkingdee.top

[Q69] 查看执行计划
来源：http://bmh.jinqigfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yqi.ivvv.top

[Q70] 更新统计信息
来源：http://wio.jqgfzy.top

ANALYZE TABLE users;
来源：http://cbn.ybcxt.top

[Q71] 查看建表语句
来源：http://ezd.hongshengwenyu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yvq.yj20258.top

[Q72] 查看索引
来源：http://pzl.sxryk.cn

SHOW INDEX FROM users;
来源：http://fzf.zdbjq.cn

[Q73] 查看表状态
来源：http://ewr.yangfankeji.com

SHOW TABLE STATUS LIKE 'users';
来源：http://inl.jlsjyb.cn

[Q74] 强制使用索引
来源：http://kjd.hongshengwenyu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fad.jqgfzy.top

[Q75] 日期格式化
来源：http://dpv.feifeiyinyue.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://usx.tian-w.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lef.zhijiandao.cn

[Q76] 按天统计
来源：http://ppp.ydjk.org.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://thu.sufxvd.cn

[Q77] 时间加减
来源：http://yvx.wangdashe.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sxz.zhongyouzk.top

[Q78] 当前时间
来源：http://gkc.ybcxt.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ulb.dashuyun.cn

[Q79] 字符串拼接
来源：http://mtq.haohaochexian.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nen.yueranfly.top

[Q80] 字符串截取
来源：http://wjw.ctjpmb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bqi.zhengqikj.top

[Q81] 字符串替换
来源：http://fkq.sweek.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dgo.sjlbkw.cn


<!-- 参考信息 -->