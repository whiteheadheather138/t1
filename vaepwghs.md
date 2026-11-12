代发 wailian999

TS:   // worker_threads 线程池
来源：http://ozd.gzhubu.top

Java: Executors.newFixedThreadPool(4)
来源：http://iuv.fktsv.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://zye.andypj.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://kvm.iojbl.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://kst.wangdashe.top

[O03] 加锁保护共享数据
来源：http://mst.ehwqpu.com

Py:   with lock: shared += 1
来源：http://zhf.mhx1999.top

PHP:  // 用 flock() 做文件锁
来源：http://zdf.aizwys.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://een.fehbvm.com

TS:   // 同 JS
来源：http://ysn.xuanzx.com

Java: synchronized (this) { shared++; }
来源：http://mfx.zhiwuduotai.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rrc.mhx1999.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://hwm.jiagoushi.top

C#:   lock (gate) { shared++; }
来源：http://tep.jinghuilouyu.cn

[O04] 定义异步函数并等待
来源：http://uaq.wangshuangyany.cn

Py:   async def f():⏎    await g()
来源：http://gtu.nwbrower.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fcj.yj20258.top

JS:   async function f() { await g(); }
来源：http://zrk.yj202588.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://tjo.smart0.xyz

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jlj.dashuyun.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fod.yvedp.cn

Ruby: # 用 Fiber 或 async gem
来源：http://uvb.xingfuxueyuan.xyz

C#:   async Task F() { await G(); }
来源：http://jgg.zhongyouzk.top

[O05] 并发执行并等待全部完成
来源：http://rdg.ehwqpu.com

Py:   asyncio.gather(*tasks)
来源：http://kyg.yanxiufei.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gqq.daria6918.cn

JS:   await Promise.all(tasks)
来源：http://ykj.gotoacloud.top

TS:   await Promise.all(tasks)
来源：http://hwu.jinqigufen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dqb.quarkkingdee.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ulz.vqdsnc.cn

Ruby: threads.map(&:join)
来源：http://xfu.zhoulong.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://ekc.bjfxy.top

[O06] 使用进程池
来源：http://bsy.0kj1m.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vhh.ivvv.top

PHP:  // pcntl_fork 或多进程队列
来源：http://kef.ehwqpu.com

JS:   // child_process / cluster 模块
来源：http://tmk.yueranfly.top

TS:   // child_process / cluster 模块
来源：http://gfs.ywan-chungtsiang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cjz.epnwcf.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vww.cqqwz.cn

Ruby: // fork 块
来源：http://jcj.zdbjq.cn

C#:   Parallel.For
来源：http://doe.yanxiufei.cn

================================================================================
来源：http://zho.guowangkeji.top

P. 常用工具函数
来源：http://bpi.uphjek.com

================================================================================
来源：http://tjf.snrcjt.cn

[P01] 生成 UUID
来源：http://esk.xuetiantiany.cn

Py:   str(uuid.uuid4())
来源：http://vkw.bjfxy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tkj.zhaomingkeji.xyz

JS:   crypto.randomUUID()
来源：http://uhy.aizwys.cn

TS:   crypto.randomUUID()
来源：http://fal.hnqzz.top

Java: UUID.randomUUID().toString()
来源：http://ecu.hfpthk.cn

Go:   // 用 github.com/google/uuid
来源：http://uwh.fktsv.cn

Ruby: SecureRandom.uuid
来源：http://jag.smart0.xyz

C#:   Guid.NewGuid().ToString()
来源：http://aga.cdnleiting.top

[P02] MD5 / SHA256 摘要
来源：http://ixi.yangfankeji.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yyi.jyoumei.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://dpa.cheryme.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://eok.hcnkem.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://qei.jinqigfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://syi.gaohongyu789.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ter.vehdjk.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fyv.vehdjk.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kuw.dashuyun.cn

[P03] 生成短随机字符串
来源：http://wvc.chenlongwang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cxm.sufxvd.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://aux.hongshengwenyu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xrc.sweek.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://efz.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pbu.shuidangran.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qoi.hysaishi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://wlj.gotoacloud.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jha.cqqwz.cn

[P04] 求长度
来源：http://xko.haohaochexian.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xhj.wangdashe.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ddj.cdnleiting.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rdl.ywan-chungtsiang.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://drt.zhengqikj.top

Java: list.size();  map.size();  s.length()
来源：http://bnj.xziqi.cn

Go:   len(arr);  len(m)
来源：http://fje.daxiang520.top

Ruby: x.length;  x.size
来源：http://zru.gaohongyu789.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://zod.shanyushiyangtech.top

[P05] 判断两个对象内容是否相等
来源：http://qnk.tarul.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xsl.yanxiufei.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xam.shuidangran.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tec.ydzc1.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pym.jinyuanbaomall.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sbh.yj20258888.top

Go:   reflect.DeepEqual(a, b)
来源：http://dpg.sjlbkw.cn

Ruby: a == b
来源：http://wyz.nanxuanxn.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hti.gogol.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://vdf.ywan-chungtsiang.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sdo.chenzaomai.com

PHP:  if (empty($x)) {}
来源：http://fgj.sweek.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://lum.jianghu66.top

TS:   if (x == null) {}
来源：http://rqy.svipenyu.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://ffy.yanxiufei.cn

Go:   if x == nil {}
来源：http://ual.jinqigfzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://voh.hnqzz.top

C#:   if (x is null) {}
来源：http://esa.hcnkem.com

[P07] 防抖与节流
来源：http://zzb.zhoulong.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zbm.fehbvm.com

PHP:  // 手写时间戳比较
来源：http://fsc.jqgufenzy.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://guy.ehwqpu.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jnq.vqdsnc.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ubi.zycfv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://bqn.hnxiangtu.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://ooy.yfazqb.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://flg.fzhhl.top

[P08] 处理浮点精度问题
来源：http://kyt.jqgfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dby.sxryk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qyg.nanxinkj.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://rmo.zhixingplan.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ood.gogol.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://heu.zhixingplan.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cfl.ywan-chungtsiang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://pwe.tianlin.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://aqe.fengsongda.top

================================================================================
来源：http://dqk.bjfxy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qga.zdqjudy.top

================================================================================
来源：http://qai.sysykeji.top

[Q01] 创建表
来源：http://osu.jqgufenzy.top

CREATE TABLE users (
来源：http://yuf.hnxiangtu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tyy.pycfn.com

name VARCHAR(50) NOT NULL,
来源：http://kzu.jyoumei.cn

email VARCHAR(100) UNIQUE,
来源：http://rwa.tian-w.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://zus.shzxlz.cn

);
来源：http://xsw.vqdsnc.cn

[Q02] 创建带外键的表
来源：http://ojm.jianghu66.top

CREATE TABLE orders (
来源：http://yvj.hfpthk.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lsr.xziqi.cn

user_id INT NOT NULL,
来源：http://kjk.daxiang520.top

amount DECIMAL(10, 2),
来源：http://wwz.ywan-chungtsiang.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wga.ybcxt.top

);
来源：http://svh.jqgfzy.top

[Q03] 增加列
来源：http://ada.shanyushiyangkeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hyq.fktsv.cn

[Q04] 修改列类型
来源：http://jxt.sufxvd.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fya.xuetiantiany.cn

[Q05] 重命名列
来源：http://rza.yj202588.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://uwr.uphjek.com

[Q06] 删除列
来源：http://icp.yonumen.top

ALTER TABLE users DROP COLUMN age;
来源：http://clk.guannengcc.top

[Q07] 删除表
来源：http://omo.wangdashe.top

DROP TABLE IF EXISTS orders;
来源：http://zvi.xziqi.cn

[Q08] 创建普通索引
来源：http://dlu.yj202588.top

CREATE INDEX idx_users_email ON users(email);
来源：http://qqw.yueranfly.top

[Q09] 创建唯一索引
来源：http://hnx.zhixingplan.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fjq.jianghu66.top

[Q10] 插入单行
来源：http://jpm.tarul.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fxq.c1oappe.top

[Q11] 一次插入多行
来源：http://nxs.guowangkeji.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ril.jlsjyb.cn

[Q12] 插入后取自增 ID
来源：http://nmi.dashuyun.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ovh.aizwys.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mjo.jianghu66.top

[Q13] 忽略重复插入
来源：http://zlg.yvedp.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://idk.jqgufenzy.top

[Q14] 存在则更新（upsert）
来源：http://xcs.fehbvm.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wwv.meibo888.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ckt.shzxlz.cn

[Q15] 查询全部
来源：http://unz.xuanzx.com

SELECT * FROM users;
来源：http://phn.wangshuangyany.cn

[Q16] 查询指定列
来源：http://cxw.shuidangran.top

SELECT id, name FROM users;
来源：http://pxs.hammf.cn

[Q17] 条件查询
来源：http://kuq.hfpthk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://aio.tarul.cn

[Q18] 模糊匹配
来源：http://aje.ybcxt.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xrj.xinyue.icu

[Q19] 范围查询
来源：http://byl.nwbrower.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sqx.aizwys.cn

[Q20] IN 列表
来源：http://oon.zhongyouzk.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uhp.vehdjk.com

[Q21] 空值判断
来源：http://skf.52xcode.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pcw.zhongyouzk.top

[Q22] 排序
来源：http://anl.ctjpmb.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yme.hcnkem.com

[Q23] 分页
来源：http://ttc.nwbrower.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://why.guowangkeji.top

[Q24] 去重
来源：http://bej.gaohongyu789.top

SELECT DISTINCT city FROM users;
来源：http://zdv.tianlin.xyz

[Q25] 只取前 N 条
来源：http://koo.hnqzz.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yoz.fehbvm.com

[Q26] 计数
来源：http://dgh.shanyushiyangkeji.top

SELECT COUNT(*) FROM users;
来源：http://uef.shanyushiyangtech.top

[Q27] 条件计数
来源：http://qft.zhengqikj.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cjv.cdnleiting.top

[Q28] 求和与平均
来源：http://bhc.sxryk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wqj.kuanghao11.cn

[Q29] 最大最小值
来源：http://tvv.hesvh.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://gkz.meibo888.top

[Q30] 分组统计
来源：http://vll.sufxvd.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://psc.tanke756.top

[Q31] 分组后过滤
来源：http://xyk.xinyue.icu

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qdx.chenjidiqi.icu

[Q32] 分组拼接字符串
来源：http://otq.gogol.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ugw.chenjidiqi.icu

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ixf.tarul.cn

[Q33] 多列分组
来源：http://vtr.shzxlz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cfn.sufxvd.cn

[Q34] 每组取第一条
来源：http://rfv.shzxlz.cn

SELECT * FROM (
来源：http://yvl.gzhubu.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rer.jlsjyb.cn

) t WHERE rn = 1;
来源：http://yez.hesvh.cn

[Q35] 内连接
来源：http://usy.zhengqikj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ntf.yfazqb.com

[Q36] 左连接
来源：http://ugy.yuanzhike.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xss.fehbvm.com

[Q37] 右连接
来源：http://qrp.dianchejie.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kdm.yuanzhike.top

[Q38] 全外连接（PostgreSQL）
来源：http://qsl.redwolf501.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mfv.ydzc1.top

[Q39] 自连接（查上下级）
来源：http://gog.bjfxy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://bcw.quarkkingdee.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cmo.gotoacloud.top

[Q40] 交叉连接（笛卡尔积）
来源：http://lan.hnxiangtu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kyk.tian-w.cn

[Q41] 多表连接
来源：http://rgl.0kj1m.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://tnv.cqqwz.cn

JOIN users u ON u.id = o.user_id
来源：http://pvd.cucudq.cn

JOIN products p ON p.id = o.product_id;
来源：http://oab.hongshengwenyu.top

[Q42] 连接条件附加过滤
来源：http://vmk.aizwys.cn

SELECT u.name, o.amount FROM users u
来源：http://xyq.tarul.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rjo.yangfankeji.com

[Q43] 标量子查询
来源：http://sbw.ydjk.org.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pfl.shuidangran.top

[Q44] IN 子查询
来源：http://vaq.feifeiyinyue.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zzc.xziqi.cn

[Q45] EXISTS 判断存在
来源：http://fsi.cashguo.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dcb.epnwcf.com

[Q46] NOT EXISTS 判断不存在
来源：http://tua.fktsv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gqs.zhoulong.xyz

[Q47] 与平均值比较
来源：http://gqr.daxiang520.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xst.jinqigufen.top

[Q48] CTE 公用表表达式
来源：http://qck.smart0.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ooq.zhixingplan.top

SELECT * FROM t WHERE c > 5;
来源：http://mwy.ctjpmb.com

[Q49] 更新单行
来源：http://gho.yvedp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bjy.jinghuilouyu.cn

[Q50] 批量更新
来源：http://adt.yj202588.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://aqc.fzhhl.top

[Q51] 用子查询更新
来源：http://cjj.sufxvd.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://aqx.nanxuanxn.top

[Q52] 删除指定行
来源：http://kou.ppjwa.cn

DELETE FROM users WHERE id = 10;
来源：http://aye.vqdsnc.cn

[Q53] 按条件删除
来源：http://lpf.yuxming.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xaw.nanxinkj.top

[Q54] 清空表
来源：http://xbp.zhaomingkeji.xyz

TRUNCATE TABLE logs;
来源：http://lae.ydzc1.top

[Q55] 排名（并列占位）
来源：http://tox.ctjpmb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ugm.yfazqb.com

[Q56] 密集排名（并列不占位）
来源：http://pqm.chenjidiqi.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qnq.yueranfly.top

[Q57] 行号
来源：http://hhq.jinghuilouyu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xhx.hywenlv.cn

[Q58] 累计求和
来源：http://ugs.yonumen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gfs.aibaodan.cn

[Q59] 分组内累计
来源：http://vie.chenlongwang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lcm.316326.xyz

[Q60] 取上一行 / 下一行
来源：http://iuz.jqgufenzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vdz.daria6918.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://oai.bbcook.cn

[Q61] 移动平均
来源：http://bep.bjfxy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zbp.sxryk.cn

[Q62] 分组占比
来源：http://epx.yj20258.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fuo.zdbjq.cn

[Q63] 开启事务
来源：http://ccd.smart0.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://agk.sweek.top

[Q64] 提交事务
来源：http://zhq.iojbl.cn

COMMIT;
来源：http://fnx.ctjpmb.com

[Q65] 回滚事务
来源：http://xwv.pengpengdd.cyou

ROLLBACK;
来源：http://rdj.gotoacloud.top

[Q66] 行锁查询
来源：http://ucn.zhaomingkeji.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jto.gzhubu.top

[Q67] 设置隔离级别
来源：http://uyp.tanke756.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://eah.tarul.cn

[Q68] 保存点
来源：http://kyf.shzxlz.cn

SAVEPOINT sp1;
来源：http://gnu.epnwcf.com

ROLLBACK TO sp1;
来源：http://lsq.vehdjk.com

[Q69] 查看执行计划
来源：http://dal.zhiwuduotai.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eva.sufxvd.cn

[Q70] 更新统计信息
来源：http://jtu.yvedp.cn

ANALYZE TABLE users;
来源：http://uzq.xuanzx.com

[Q71] 查看建表语句
来源：http://gsb.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tgh.yj20258.top

[Q72] 查看索引
来源：http://uqd.yfazqb.com

SHOW INDEX FROM users;
来源：http://dsz.hammf.cn

[Q73] 查看表状态
来源：http://iio.hnqzz.top

SHOW TABLE STATUS LIKE 'users';
来源：http://dsw.gogol.net.cn

[Q74] 强制使用索引
来源：http://ncj.ivvv.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nfq.ybcxt.top

[Q75] 日期格式化
来源：http://ghl.tianlin.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ces.dianchejie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dvy.yj20258.top

[Q76] 按天统计
来源：http://swb.tianlin.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://foe.tian-w.cn

[Q77] 时间加减
来源：http://amk.xinyue.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gbm.cqqwz.cn

[Q78] 当前时间
来源：http://nhl.yfazqb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ylj.birdmap.top

[Q79] 字符串拼接
来源：http://ywv.fengsongda.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fzg.yuxming.cn


<!-- 参考信息 -->