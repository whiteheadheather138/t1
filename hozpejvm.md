代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kda.andypj.xyz

[O03] 加锁保护共享数据
来源：http://ynw.9152youxi.cn

Py:   with lock: shared += 1
来源：http://sgu.316326.xyz

PHP:  // 用 flock() 做文件锁
来源：http://xuy.hammf.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://uol.ydzc1.top

TS:   // 同 JS
来源：http://ele.kuanghao11.cn

Java: synchronized (this) { shared++; }
来源：http://ery.pengpengdd.cyou

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dbc.xuetiantiany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://fqi.fengsongda.top

C#:   lock (gate) { shared++; }
来源：http://jgr.fehbvm.com

[O04] 定义异步函数并等待
来源：http://ctv.hongshengwenyu.top

Py:   async def f():⏎    await g()
来源：http://apj.yj202588.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://odm.fanxiaobao.xyz

JS:   async function f() { await g(); }
来源：http://iie.yj20258.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rsq.meibo888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ris.sjlbkw.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://iba.ivvv.top

Ruby: # 用 Fiber 或 async gem
来源：http://vsj.zycfv.cn

C#:   async Task F() { await G(); }
来源：http://qet.ydzc1.top

[O05] 并发执行并等待全部完成
来源：http://nyj.sweek.top

Py:   asyncio.gather(*tasks)
来源：http://hdd.shuidangran.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yny.yj202588.top

JS:   await Promise.all(tasks)
来源：http://bnw.aizwys.cn

TS:   await Promise.all(tasks)
来源：http://idz.fehbvm.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ric.ppjwa.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://fdq.sufxvd.cn

Ruby: threads.map(&:join)
来源：http://ujq.hongshengwenyu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dtv.andypj.xyz

[O06] 使用进程池
来源：http://bcx.zdqjudy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://voj.xuetiantiany.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://rzw.xuetiantiany.cn

JS:   // child_process / cluster 模块
来源：http://vmz.gaohongyu789.top

TS:   // child_process / cluster 模块
来源：http://mdj.ppjwa.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kew.ivvv.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nlb.52xcode.cn

Ruby: // fork 块
来源：http://ahz.wangshuangyany.cn

C#:   Parallel.For
来源：http://nbu.pengpengdd.cyou

================================================================================
来源：http://yya.vqdsnc.cn

P. 常用工具函数
来源：http://igh.cdnleiting.top

================================================================================
来源：http://nqr.bbcook.cn

[P01] 生成 UUID
来源：http://lco.cdnleiting.top

Py:   str(uuid.uuid4())
来源：http://zbw.guannengcc.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bza.sweek.top

JS:   crypto.randomUUID()
来源：http://unl.tianlin.xyz

TS:   crypto.randomUUID()
来源：http://hoy.snrcjt.cn

Java: UUID.randomUUID().toString()
来源：http://lmq.ppjwa.cn

Go:   // 用 github.com/google/uuid
来源：http://mhi.jinqigufen.top

Ruby: SecureRandom.uuid
来源：http://xsk.hcnkem.com

C#:   Guid.NewGuid().ToString()
来源：http://emw.fktsv.cn

[P02] MD5 / SHA256 摘要
来源：http://kme.zhoulong.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mau.jinghuilouyu.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bqr.yvedp.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mtq.0kj1m.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://egd.52xcode.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gnd.ppjwa.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lgb.xingfuxueyuan.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://qon.sweek.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://szt.jianghu66.top

[P03] 生成短随机字符串
来源：http://ujq.jinyuanbaomall.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pay.yonumen.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://kzq.fehbvm.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mqy.chenjidiqi.icu

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cgi.xylfe.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://dus.wangdashe.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://pdo.yanxiufei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tuw.tianlin.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qsh.yonumen.top

[P04] 求长度
来源：http://alp.chenlongwang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wkx.hnxiangtu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wud.quarkkingdee.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gpe.guowangkeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cei.hammf.cn

Java: list.size();  map.size();  s.length()
来源：http://cxg.quarkkingdee.top

Go:   len(arr);  len(m)
来源：http://ama.cashguo.top

Ruby: x.length;  x.size
来源：http://xde.andypj.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://hgs.fktsv.cn

[P05] 判断两个对象内容是否相等
来源：http://ukn.birdmap.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://sck.xuanzx.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://czh.ivvv.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iei.daxiang520.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lhz.yongpay.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://guu.ydzc1.top

Go:   reflect.DeepEqual(a, b)
来源：http://ggj.havefunace.top

Ruby: a == b
来源：http://zyd.shzxlz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://nth.zdbjq.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://upe.tian-w.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ypr.birdmap.top

PHP:  if (empty($x)) {}
来源：http://dvo.haohaochexian.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ede.fzhhl.top

TS:   if (x == null) {}
来源：http://mcv.nwbrower.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ura.shuidangran.top

Go:   if x == nil {}
来源：http://mgd.fengsongda.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://llw.yongpay.top

C#:   if (x is null) {}
来源：http://xyz.fehbvm.com

[P07] 防抖与节流
来源：http://wnk.vehdjk.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yzj.yuxming.cn

PHP:  // 手写时间戳比较
来源：http://pzb.yj20258.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lgl.iojbl.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ckv.ctjpmb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://amt.uphjek.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ktc.fzhhl.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wjh.uphjek.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://tdr.sysykeji.top

[P08] 处理浮点精度问题
来源：http://nzt.ehwqpu.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://cti.cheryme.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mhh.aizwys.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://liu.uphjek.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ywz.chenlongwang.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://qdc.zhixingplan.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dfg.jinghuilouyu.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://drb.hnxiangtu.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dfu.ydzc1.top

================================================================================
来源：http://ipu.ydjk.org.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mlp.hywenlv.cn

================================================================================
来源：http://bvm.ctjpmb.com

[Q01] 创建表
来源：http://saa.cucudq.cn

CREATE TABLE users (
来源：http://akj.birdmap.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bne.jqgufenzy.top

name VARCHAR(50) NOT NULL,
来源：http://nlg.xingfuxueyuan.xyz

email VARCHAR(100) UNIQUE,
来源：http://cpj.vehdjk.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://dgw.xylfe.cn

);
来源：http://hxp.jianghu66.top

[Q02] 创建带外键的表
来源：http://gug.yfazqb.com

CREATE TABLE orders (
来源：http://web.shangyingyoupin.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://for.ivvv.top

user_id INT NOT NULL,
来源：http://htb.bjfxy.top

amount DECIMAL(10, 2),
来源：http://xwt.cdnleiting.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vkq.sysykeji.top

);
来源：http://cik.jyoumei.cn

[Q03] 增加列
来源：http://eog.jyoumei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zlv.vqdsnc.cn

[Q04] 修改列类型
来源：http://itu.zhijiandao.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://npx.nanxinkj.top

[Q05] 重命名列
来源：http://lrj.tianlin.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yfp.zhaomingkeji.xyz

[Q06] 删除列
来源：http://ovj.guannengcc.top

ALTER TABLE users DROP COLUMN age;
来源：http://nrt.hesvh.cn

[Q07] 删除表
来源：http://mwh.hongshengwenyu.top

DROP TABLE IF EXISTS orders;
来源：http://ccc.yanxiufei.cn

[Q08] 创建普通索引
来源：http://vqo.cucudq.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://wxd.xylfe.cn

[Q09] 创建唯一索引
来源：http://lie.zhaomingkeji.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bly.vehdjk.com

[Q10] 插入单行
来源：http://fai.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gfd.birdmap.top

[Q11] 一次插入多行
来源：http://htb.jinqigfzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://aok.jinqigfzy.top

[Q12] 插入后取自增 ID
来源：http://ejj.hammf.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xeg.xingfuxueyuan.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mwh.jqgufenzy.top

[Q13] 忽略重复插入
来源：http://wpp.cdnleiting.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://nil.xingfuxueyuan.xyz

[Q14] 存在则更新（upsert）
来源：http://eqs.fehbvm.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rty.zhongyouzk.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rko.shanyushiyangkeji.top

[Q15] 查询全部
来源：http://flb.jlsjyb.cn

SELECT * FROM users;
来源：http://mnp.cucudq.cn

[Q16] 查询指定列
来源：http://vxb.jqgfzy.top

SELECT id, name FROM users;
来源：http://wtm.ydzc1.top

[Q17] 条件查询
来源：http://rai.iojbl.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://njl.ydjk.org.cn

[Q18] 模糊匹配
来源：http://ybz.tian-w.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://knc.gzhubu.top

[Q19] 范围查询
来源：http://ywy.meibo888.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rpy.aizwys.cn

[Q20] IN 列表
来源：http://ynf.daria6918.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xzm.aizwys.cn

[Q21] 空值判断
来源：http://mrl.hammf.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vad.tian-w.cn

[Q22] 排序
来源：http://mhp.ppjwa.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ejv.shanyushiyangtech.top

[Q23] 分页
来源：http://ysw.uphjek.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jna.fehbvm.com

[Q24] 去重
来源：http://pmo.zhixingplan.top

SELECT DISTINCT city FROM users;
来源：http://gqm.gogol.net.cn

[Q25] 只取前 N 条
来源：http://cun.daria6918.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://sfl.daxiang520.top

[Q26] 计数
来源：http://wkc.bjfxy.top

SELECT COUNT(*) FROM users;
来源：http://dao.hnxiangtu.top

[Q27] 条件计数
来源：http://fwv.svipenyu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cwu.fktsv.cn

[Q28] 求和与平均
来源：http://rkl.cheryme.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mte.316326.xyz

[Q29] 最大最小值
来源：http://ots.tian-w.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wwo.andypj.xyz

[Q30] 分组统计
来源：http://qcz.cucudq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://imv.zhiwuduotai.top

[Q31] 分组后过滤
来源：http://khc.zhaomingkeji.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://orf.aibaodan.cn

[Q32] 分组拼接字符串
来源：http://vnb.tianlin.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xya.cdnleiting.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cwg.sxryk.cn

[Q33] 多列分组
来源：http://nda.wangdashe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yak.sjlbkw.cn

[Q34] 每组取第一条
来源：http://joc.mhx1999.top

SELECT * FROM (
来源：http://mxk.sxryk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://moa.hesvh.cn

) t WHERE rn = 1;
来源：http://rfe.epnwcf.com

[Q35] 内连接
来源：http://vzq.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uja.fengsongda.top

[Q36] 左连接
来源：http://npw.shangyingyoupin.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mjk.aizwys.cn

[Q37] 右连接
来源：http://nzc.zycfv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://taf.0kj1m.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jvo.shuidangran.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qov.yj202588.top

[Q39] 自连接（查上下级）
来源：http://rgv.ydjk.org.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wdb.xinyue.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://onq.hnxiangtu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qlq.sweek.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bco.sjlbkw.cn

[Q41] 多表连接
来源：http://qze.ydzc1.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://xck.tianlin.xyz

JOIN users u ON u.id = o.user_id
来源：http://jdd.c1oappe.top

JOIN products p ON p.id = o.product_id;
来源：http://nri.xziqi.cn

[Q42] 连接条件附加过滤
来源：http://erm.svipenyu.cn

SELECT u.name, o.amount FROM users u
来源：http://isb.52xcode.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qtz.yuxming.cn

[Q43] 标量子查询
来源：http://ntk.fehbvm.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://tbj.andypj.xyz

[Q44] IN 子查询
来源：http://jev.9152youxi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gcw.chenjidiqi.icu

[Q45] EXISTS 判断存在
来源：http://vlw.sxryk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://smn.nwbrower.top

[Q46] NOT EXISTS 判断不存在
来源：http://sec.guowangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://coj.gogol.net.cn

[Q47] 与平均值比较
来源：http://szo.yj202588.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fqj.jiagoushi.top

[Q48] CTE 公用表表达式
来源：http://aih.yj202588.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lcw.tanke756.top

SELECT * FROM t WHERE c > 5;
来源：http://kwm.birdmap.top

[Q49] 更新单行
来源：http://tmu.hammf.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fkq.guannengcc.top

[Q50] 批量更新
来源：http://ten.fengsongda.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://agy.jqgfzy.top

[Q51] 用子查询更新
来源：http://zqo.havefunace.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lrv.uphjek.com

[Q52] 删除指定行
来源：http://msq.0kj1m.cn

DELETE FROM users WHERE id = 10;
来源：http://zvu.hongshengwenyu.top

[Q53] 按条件删除
来源：http://lzu.52xcode.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://eux.daxiang520.top

[Q54] 清空表
来源：http://jej.cheryme.top

TRUNCATE TABLE logs;
来源：http://ikn.meibo888.top

[Q55] 排名（并列占位）
来源：http://tju.zhoulong.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ndn.wangdashe.top

[Q56] 密集排名（并列不占位）
来源：http://svu.guannengcc.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://tmt.svipenyu.cn

[Q57] 行号
来源：http://ehx.yangfankeji.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gaz.yuxming.cn

[Q58] 累计求和
来源：http://vbd.jqgfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gdj.hnqzz.top

[Q59] 分组内累计
来源：http://vka.quarkkingdee.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fdw.gotoacloud.top

[Q60] 取上一行 / 下一行
来源：http://qqy.andypj.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jod.ywan-chungtsiang.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yvi.ybcxt.top

[Q61] 移动平均
来源：http://nti.ybcxt.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mfd.dashuyun.cn

[Q62] 分组占比
来源：http://gxk.ehwqpu.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xtu.zhixingplan.top

[Q63] 开启事务
来源：http://zyx.zhengqikj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vrr.havefunace.top

[Q64] 提交事务
来源：http://ezw.bbcook.cn

COMMIT;
来源：http://rnf.jqgufenzy.top

[Q65] 回滚事务
来源：http://psj.hongshengwenyu.top

ROLLBACK;
来源：http://vap.zdbjq.cn

[Q66] 行锁查询
来源：http://igu.sweek.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ost.yj20258.top

[Q67] 设置隔离级别
来源：http://zrh.jinqigfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dme.zhoulong.xyz

[Q68] 保存点
来源：http://elo.xinyue.icu

SAVEPOINT sp1;
来源：http://cxy.xuanzx.com

ROLLBACK TO sp1;
来源：http://kls.jyoumei.cn

[Q69] 查看执行计划
来源：http://lwo.xylfe.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://awl.fehbvm.com

[Q70] 更新统计信息
来源：http://deu.zhengqikj.top

ANALYZE TABLE users;
来源：http://snb.jinghuilouyu.cn

[Q71] 查看建表语句
来源：http://vzq.smart0.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cho.zdqjudy.top

[Q72] 查看索引
来源：http://ekg.chenjidiqi.icu

SHOW INDEX FROM users;
来源：http://yhq.cashguo.top

[Q73] 查看表状态
来源：http://dip.yuanzhike.top

SHOW TABLE STATUS LIKE 'users';
来源：http://abo.yanxiufei.cn

[Q74] 强制使用索引
来源：http://umu.daxiang520.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jrs.sxryk.cn

[Q75] 日期格式化
来源：http://voh.wangdashe.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qco.sweek.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fni.tanke756.top

[Q76] 按天统计
来源：http://edg.uphjek.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://asq.fengsongda.top

[Q77] 时间加减
来源：http://stp.epnwcf.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gmy.fehbvm.com

[Q78] 当前时间
来源：http://rex.fanxiaobao.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rey.yuxming.cn

[Q79] 字符串拼接
来源：http://nxv.gaohongyu789.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nbg.zhoulong.xyz

[Q80] 字符串截取
来源：http://pye.xuanzx.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cwy.mhx1999.top

[Q81] 字符串替换
来源：http://szj.mhx1999.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://psg.jqgfzy.top


<!-- 参考信息 -->