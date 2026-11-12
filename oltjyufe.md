代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://csc.xingfuxueyuan.xyz

[O03] 加锁保护共享数据
来源：http://oha.tanke756.top

Py:   with lock: shared += 1
来源：http://tww.hammf.cn

PHP:  // 用 flock() 做文件锁
来源：http://eui.hywenlv.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://xcu.pengpengdd.cyou

TS:   // 同 JS
来源：http://nwe.redwolf501.top

Java: synchronized (this) { shared++; }
来源：http://edo.fktsv.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://oym.havefunace.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://dkt.gzhubu.top

C#:   lock (gate) { shared++; }
来源：http://blj.mhx1999.top

[O04] 定义异步函数并等待
来源：http://esj.zhaomingkeji.xyz

Py:   async def f():⏎    await g()
来源：http://ayo.pengpengdd.cyou

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cxv.sweek.top

JS:   async function f() { await g(); }
来源：http://sgn.jqgufenzy.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://afz.redwolf501.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://vyx.sweek.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tww.jinqigufen.top

Ruby: # 用 Fiber 或 async gem
来源：http://pcb.andypj.xyz

C#:   async Task F() { await G(); }
来源：http://ecn.snrcjt.cn

[O05] 并发执行并等待全部完成
来源：http://xue.zdbjq.cn

Py:   asyncio.gather(*tasks)
来源：http://olj.andypj.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nvh.cqqwz.cn

JS:   await Promise.all(tasks)
来源：http://tph.zhongyouzk.top

TS:   await Promise.all(tasks)
来源：http://gbl.kuanghao11.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://yde.xylfe.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mhh.cheryme.top

Ruby: threads.map(&:join)
来源：http://vyo.haohaochexian.top

C#:   await Task.WhenAll(t1, t2)
来源：http://men.gaohongyu789.top

[O06] 使用进程池
来源：http://fiq.zycfv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lir.svipenyu.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://oer.hnqzz.top

JS:   // child_process / cluster 模块
来源：http://eht.zdbjq.cn

TS:   // child_process / cluster 模块
来源：http://aml.dianchejie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mgb.yuxming.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.cdnleiting.top

Ruby: // fork 块
来源：http://xle.shzxlz.cn

C#:   Parallel.For
来源：http://wzq.c1oappe.top

================================================================================
来源：http://lxg.cashguo.top

P. 常用工具函数
来源：http://pun.jianghu66.top

================================================================================
来源：http://llz.yvedp.cn

[P01] 生成 UUID
来源：http://zum.yonumen.top

Py:   str(uuid.uuid4())
来源：http://afl.sxryk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wmp.haohaochexian.top

JS:   crypto.randomUUID()
来源：http://hix.shzxlz.cn

TS:   crypto.randomUUID()
来源：http://xhx.yfazqb.com

Java: UUID.randomUUID().toString()
来源：http://ohf.zhaomingkeji.xyz

Go:   // 用 github.com/google/uuid
来源：http://uih.jqgufenzy.top

Ruby: SecureRandom.uuid
来源：http://jmo.hysaishi.cn

C#:   Guid.NewGuid().ToString()
来源：http://xgx.sweek.top

[P02] MD5 / SHA256 摘要
来源：http://wnp.tianlin.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://myx.yj202588.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zab.daxiang520.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kqv.yangfankeji.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rtb.yangfankeji.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hcv.yongpay.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qgf.hnxiangtu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://atu.jlsjyb.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jzj.yuanzhike.top

[P03] 生成短随机字符串
来源：http://mcm.guowangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lze.tianlin.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://jlv.tanke756.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://flj.fengsongda.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jqn.fehbvm.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uma.xinyue.icu

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wta.fehbvm.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://nvm.yj20258888.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zkv.gaohongyu789.top

[P04] 求长度
来源：http://npg.pycfn.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pmo.hnxiangtu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gjx.pycfn.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://znn.yueranfly.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://sml.birdmap.top

Java: list.size();  map.size();  s.length()
来源：http://uff.aibaodan.cn

Go:   len(arr);  len(m)
来源：http://nfc.smart0.xyz

Ruby: x.length;  x.size
来源：http://ljj.daxiang520.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xku.iojbl.cn

[P05] 判断两个对象内容是否相等
来源：http://vby.yj202588.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://lgk.yangfankeji.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://acc.nwbrower.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://rrr.ctjpmb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ilv.52xcode.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://row.pycfn.com

Go:   reflect.DeepEqual(a, b)
来源：http://rrs.fzhhl.top

Ruby: a == b
来源：http://nbw.zycfv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qng.dashuyun.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qnp.52xcode.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zrt.sweek.top

PHP:  if (empty($x)) {}
来源：http://bmx.hfpthk.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://abi.jinqigfzy.top

TS:   if (x == null) {}
来源：http://viy.daria6918.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://qge.shzxlz.cn

Go:   if x == nil {}
来源：http://mdi.meibo888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://txp.cucudq.cn

C#:   if (x is null) {}
来源：http://par.zhijiandao.cn

[P07] 防抖与节流
来源：http://cnz.ivvv.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ntg.zycfv.cn

PHP:  // 手写时间戳比较
来源：http://frl.xziqi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yeh.andypj.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nck.yvedp.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xdc.aizwys.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ttz.yvedp.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zzz.cdnleiting.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fnr.dianchejie.cn

[P08] 处理浮点精度问题
来源：http://gdd.sweek.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dqs.snrcjt.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xdi.guowangkeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://aio.jinqigfzy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vjm.jinyuanbaomall.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oxu.fktsv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wgq.zhongyouzk.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jxi.meibo888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://nuy.ivvv.top

================================================================================
来源：http://dgz.sjlbkw.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uua.xylfe.cn

================================================================================
来源：http://ktj.yj20258.top

[Q01] 创建表
来源：http://wnf.shanyushiyangkeji.top

CREATE TABLE users (
来源：http://wuj.0kj1m.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lrd.svipenyu.cn

name VARCHAR(50) NOT NULL,
来源：http://aqc.zhaomingkeji.xyz

email VARCHAR(100) UNIQUE,
来源：http://mvt.fzhhl.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mlo.zdbjq.cn

);
来源：http://pwj.quarkkingdee.top

[Q02] 创建带外键的表
来源：http://ahe.jiagoushi.top

CREATE TABLE orders (
来源：http://lwe.hywenlv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sie.yanxiufei.cn

user_id INT NOT NULL,
来源：http://zon.yuanzhike.top

amount DECIMAL(10, 2),
来源：http://siw.aizwys.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://dei.c1oappe.top

);
来源：http://jkw.meibo888.top

[Q03] 增加列
来源：http://exb.52xcode.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://out.pengpengdd.cyou

[Q04] 修改列类型
来源：http://lnp.cucudq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cdy.yj20258.top

[Q05] 重命名列
来源：http://ybp.cashguo.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wzl.zdbjq.cn

[Q06] 删除列
来源：http://lft.zhoulong.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://itg.9152youxi.cn

[Q07] 删除表
来源：http://tgv.shuidangran.top

DROP TABLE IF EXISTS orders;
来源：http://urr.ybcxt.top

[Q08] 创建普通索引
来源：http://wrl.zhixingplan.top

CREATE INDEX idx_users_email ON users(email);
来源：http://vcw.mhx1999.top

[Q09] 创建唯一索引
来源：http://vkq.svipenyu.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fre.hnxiangtu.top

[Q10] 插入单行
来源：http://jxt.mhx1999.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zrx.guowangkeji.top

[Q11] 一次插入多行
来源：http://tge.ppjwa.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://eux.guannengcc.top

[Q12] 插入后取自增 ID
来源：http://fqm.yangfankeji.com

INSERT INTO users (name) VALUES ('C');
来源：http://geb.zhijiandao.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uyz.cucudq.cn

[Q13] 忽略重复插入
来源：http://vre.xingfuxueyuan.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kgc.chenlongwang.top

[Q14] 存在则更新（upsert）
来源：http://jyq.cdnleiting.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ics.cqqwz.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zvo.jqgfzy.top

[Q15] 查询全部
来源：http://zhu.hongshengwenyu.top

SELECT * FROM users;
来源：http://ytf.xziqi.cn

[Q16] 查询指定列
来源：http://uti.hongshengwenyu.top

SELECT id, name FROM users;
来源：http://jlr.xziqi.cn

[Q17] 条件查询
来源：http://fsf.hysaishi.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blj.meibo888.top

[Q18] 模糊匹配
来源：http://rpv.yj20258888.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://gek.ywan-chungtsiang.top

[Q19] 范围查询
来源：http://xrs.aizwys.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wmq.jqgfzy.top

[Q20] IN 列表
来源：http://dch.316326.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tly.fanxiaobao.xyz

[Q21] 空值判断
来源：http://dbg.nanxinkj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://hmy.daria6918.cn

[Q22] 排序
来源：http://vpv.xinyue.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://fgm.0kj1m.cn

[Q23] 分页
来源：http://kvu.yonumen.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mwu.hcnkem.com

[Q24] 去重
来源：http://ifr.epnwcf.com

SELECT DISTINCT city FROM users;
来源：http://kch.yj20258888.top

[Q25] 只取前 N 条
来源：http://hul.zycfv.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://gqy.tanke756.top

[Q26] 计数
来源：http://lkz.pengpengdd.cyou

SELECT COUNT(*) FROM users;
来源：http://pmg.jinyuanbaomall.cn

[Q27] 条件计数
来源：http://mps.hammf.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tvn.daria6918.cn

[Q28] 求和与平均
来源：http://riz.ybcxt.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ukq.ydjk.org.cn

[Q29] 最大最小值
来源：http://tcp.fehbvm.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://kbk.xuetiantiany.cn

[Q30] 分组统计
来源：http://ujp.hywenlv.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vob.c1oappe.top

[Q31] 分组后过滤
来源：http://sxk.yongpay.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xpv.nwbrower.top

[Q32] 分组拼接字符串
来源：http://xax.shuidangran.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jet.zhoulong.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jwx.haohaochexian.top

[Q33] 多列分组
来源：http://abt.ywan-chungtsiang.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ctl.cucudq.cn

[Q34] 每组取第一条
来源：http://vrv.0kj1m.cn

SELECT * FROM (
来源：http://czo.dianchejie.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xoi.shzxlz.cn

) t WHERE rn = 1;
来源：http://fog.haohaochexian.top

[Q35] 内连接
来源：http://jml.316326.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gfy.cucudq.cn

[Q36] 左连接
来源：http://lcp.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ewq.hfpthk.cn

[Q37] 右连接
来源：http://gka.tanke756.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lnv.yueranfly.top

[Q38] 全外连接（PostgreSQL）
来源：http://rje.ehwqpu.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ykk.birdmap.top

[Q39] 自连接（查上下级）
来源：http://hhu.kuanghao11.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fex.zdqjudy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mqz.gaohongyu789.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ppg.yj20258.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mlw.zhongyouzk.top

[Q41] 多表连接
来源：http://xlb.uphjek.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://wat.zhijiandao.cn

JOIN users u ON u.id = o.user_id
来源：http://jge.xinyue.icu

JOIN products p ON p.id = o.product_id;
来源：http://bnb.chenjidiqi.icu

[Q42] 连接条件附加过滤
来源：http://zib.yuanzhike.top

SELECT u.name, o.amount FROM users u
来源：http://xqf.cqqwz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wmy.snrcjt.cn

[Q43] 标量子查询
来源：http://ash.jinqigfzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nrc.jinghuilouyu.cn

[Q44] IN 子查询
来源：http://isp.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lyh.hysaishi.cn

[Q45] EXISTS 判断存在
来源：http://hbu.yanxiufei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://loi.wangshuangyany.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xge.gaohongyu789.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kas.sysykeji.top

[Q47] 与平均值比较
来源：http://dqj.jinqigufen.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qhi.dianchejie.cn

[Q48] CTE 公用表表达式
来源：http://rcj.9152youxi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jis.ehwqpu.com

SELECT * FROM t WHERE c > 5;
来源：http://aom.yanxiufei.cn

[Q49] 更新单行
来源：http://khb.hysaishi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tfm.sweek.top

[Q50] 批量更新
来源：http://gbz.jinghuilouyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://arr.hysaishi.cn

[Q51] 用子查询更新
来源：http://qzk.shanyushiyangkeji.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kfc.zhengqikj.top

[Q52] 删除指定行
来源：http://lzp.ydzc1.top

DELETE FROM users WHERE id = 10;
来源：http://vdc.ctjpmb.com

[Q53] 按条件删除
来源：http://owr.zhixingplan.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lqy.ppjwa.cn

[Q54] 清空表
来源：http://vgw.fengsongda.top

TRUNCATE TABLE logs;
来源：http://cep.xinyue.icu

[Q55] 排名（并列占位）
来源：http://skm.yj202588.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://erd.shuidangran.top

[Q56] 密集排名（并列不占位）
来源：http://llu.ydzc1.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kvd.wangdashe.top

[Q57] 行号
来源：http://cwo.jinqigufen.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rjl.yuanzhike.top

[Q58] 累计求和
来源：http://qih.tian-w.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pyf.snrcjt.cn

[Q59] 分组内累计
来源：http://fgd.316326.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://frz.svipenyu.cn

[Q60] 取上一行 / 下一行
来源：http://xws.meibo888.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sro.xingfuxueyuan.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hht.jinghuilouyu.cn

[Q61] 移动平均
来源：http://hry.svipenyu.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yrb.tianlin.xyz

[Q62] 分组占比
来源：http://sti.shuidangran.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gty.daria6918.cn

[Q63] 开启事务
来源：http://bnc.gotoacloud.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kei.hongshengwenyu.top

[Q64] 提交事务
来源：http://gld.xziqi.cn

COMMIT;
来源：http://hpu.hfpthk.cn

[Q65] 回滚事务
来源：http://ihh.shzxlz.cn

ROLLBACK;
来源：http://dvs.quarkkingdee.top

[Q66] 行锁查询
来源：http://ilx.havefunace.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ufr.fzhhl.top

[Q67] 设置隔离级别
来源：http://asn.jinqigfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tvy.fktsv.cn

[Q68] 保存点
来源：http://gph.tian-w.cn

SAVEPOINT sp1;
来源：http://fzn.zhengqikj.top

ROLLBACK TO sp1;
来源：http://wag.gogol.net.cn

[Q69] 查看执行计划
来源：http://rqp.snrcjt.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cig.tarul.cn

[Q70] 更新统计信息
来源：http://dvh.fanxiaobao.xyz

ANALYZE TABLE users;
来源：http://qug.zhoulong.xyz

[Q71] 查看建表语句
来源：http://mtp.shangyingyoupin.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xxq.guannengcc.top

[Q72] 查看索引
来源：http://tjj.hfpthk.cn

SHOW INDEX FROM users;
来源：http://ueq.guowangkeji.top

[Q73] 查看表状态
来源：http://qxx.yanxiufei.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://paj.chenjidiqi.icu

[Q74] 强制使用索引
来源：http://lym.daria6918.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://szc.uphjek.com

[Q75] 日期格式化
来源：http://owx.tarul.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yaa.hongshengwenyu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ggt.shuidangran.top

[Q76] 按天统计
来源：http://avf.hywenlv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vkm.fanxiaobao.xyz

[Q77] 时间加减
来源：http://zrd.sjlbkw.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zwf.zhaomingkeji.xyz

[Q78] 当前时间
来源：http://maf.chenlongwang.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wpw.52xcode.cn

[Q79] 字符串拼接
来源：http://vmz.tarul.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cav.jyoumei.cn

[Q80] 字符串截取
来源：http://hdb.vqdsnc.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qbp.nwbrower.top

[Q81] 字符串替换
来源：http://qku.wangshuangyany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pig.ivvv.top


<!-- 参考信息 -->