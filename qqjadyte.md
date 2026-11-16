代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://rbo.zhengqikj.top

TS:   // 同 JS
来源：http://jeu.smart0.xyz

Java: synchronized (this) { shared++; }
来源：http://mpb.sxryk.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://rkd.yanxiufei.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://qvf.guannengcc.top

C#:   lock (gate) { shared++; }
来源：http://ahd.ydzc1.top

[O04] 定义异步函数并等待
来源：http://pnd.jinqigfzy.top

Py:   async def f():⏎    await g()
来源：http://ntt.ctjpmb.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://eje.haohaochexian.top

JS:   async function f() { await g(); }
来源：http://vea.hongshengwenyu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://jyv.fengsongda.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yty.yangfankeji.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bjt.ydjk.org.cn

Ruby: # 用 Fiber 或 async gem
来源：http://one.tanke756.top

C#:   async Task F() { await G(); }
来源：http://wni.jinghuilouyu.cn

[O05] 并发执行并等待全部完成
来源：http://rcy.sweek.top

Py:   asyncio.gather(*tasks)
来源：http://qsm.316326.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jej.xingfuxueyuan.xyz

JS:   await Promise.all(tasks)
来源：http://xto.xylfe.cn

TS:   await Promise.all(tasks)
来源：http://drp.hcnkem.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://pdk.xziqi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rrq.guannengcc.top

Ruby: threads.map(&:join)
来源：http://uvo.daria6918.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://qqi.jinghuilouyu.cn

[O06] 使用进程池
来源：http://lsh.vehdjk.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://syn.jqgfzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://wwy.yonumen.top

JS:   // child_process / cluster 模块
来源：http://ypj.hfpthk.cn

TS:   // child_process / cluster 模块
来源：http://wrl.ctjpmb.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://unq.gogol.net.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wrq.ybcxt.top

Ruby: // fork 块
来源：http://bjw.yj20258.top

C#:   Parallel.For
来源：http://oet.daxiang520.top

================================================================================
来源：http://isk.cashguo.top

P. 常用工具函数
来源：http://jts.zdbjq.cn

================================================================================
来源：http://jny.daxiang520.top

[P01] 生成 UUID
来源：http://sid.havefunace.top

Py:   str(uuid.uuid4())
来源：http://ooq.yj202588.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oiv.zhongyouzk.top

JS:   crypto.randomUUID()
来源：http://qnm.guannengcc.top

TS:   crypto.randomUUID()
来源：http://yce.hnxiangtu.top

Java: UUID.randomUUID().toString()
来源：http://hgy.fanxiaobao.xyz

Go:   // 用 github.com/google/uuid
来源：http://nzn.yuxming.cn

Ruby: SecureRandom.uuid
来源：http://guu.cheryme.top

C#:   Guid.NewGuid().ToString()
来源：http://wiw.feifeiyinyue.top

[P02] MD5 / SHA256 摘要
来源：http://jpg.yanxiufei.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gwz.fanxiaobao.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://txd.yfazqb.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fln.yvedp.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ehw.cqqwz.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oxb.zhijiandao.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lot.xuetiantiany.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ilj.gzhubu.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wvz.sjlbkw.cn

[P03] 生成短随机字符串
来源：http://cga.ivvv.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ubz.zdbjq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://adz.hesvh.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lyf.yuanzhike.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jtx.hesvh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ciy.snrcjt.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://shy.fengsongda.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lrw.hfpthk.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vrx.tanke756.top

[P04] 求长度
来源：http://plq.yj20258.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://rdt.hcnkem.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jsz.fktsv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xjo.xinyue.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://akk.jiagoushi.top

Java: list.size();  map.size();  s.length()
来源：http://fjz.zhiwuduotai.top

Go:   len(arr);  len(m)
来源：http://tdd.birdmap.top

Ruby: x.length;  x.size
来源：http://alu.fktsv.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gcw.jlsjyb.cn

[P05] 判断两个对象内容是否相等
来源：http://sij.yangfankeji.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://kaw.nanxinkj.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gpb.cashguo.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yfc.cqqwz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rym.haohaochexian.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ijq.uphjek.com

Go:   reflect.DeepEqual(a, b)
来源：http://fkb.uphjek.com

Ruby: a == b
来源：http://dhc.fengsongda.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sgb.ydjk.org.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ttr.zdqjudy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wrn.ybcxt.top

PHP:  if (empty($x)) {}
来源：http://afu.jlsjyb.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://meg.yfazqb.com

TS:   if (x == null) {}
来源：http://oqz.zhaomingkeji.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://weu.zhongyouzk.top

Go:   if x == nil {}
来源：http://xgf.daria6918.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fcn.yj20258888.top

C#:   if (x is null) {}
来源：http://aaf.smart0.xyz

[P07] 防抖与节流
来源：http://imc.shuidangran.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://laj.cqqwz.cn

PHP:  // 手写时间戳比较
来源：http://hcb.yvedp.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yuo.snrcjt.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vnb.tian-w.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xvd.xinyue.icu

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://osg.chenlongwang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wtj.ivvv.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://yje.jyoumei.cn

[P08] 处理浮点精度问题
来源：http://zsb.guannengcc.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://tjf.zycfv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bei.tianlin.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://nxd.zhixingplan.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wsb.quarkkingdee.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dyp.xingfuxueyuan.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dfs.yuxming.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mps.316326.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tqf.ydjk.org.cn

================================================================================
来源：http://hjo.ybcxt.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wtb.cashguo.top

================================================================================
来源：http://evm.redwolf501.top

[Q01] 创建表
来源：http://qvi.zdqjudy.top

CREATE TABLE users (
来源：http://vmu.feifeiyinyue.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cma.gotoacloud.top

name VARCHAR(50) NOT NULL,
来源：http://rgl.hnxiangtu.top

email VARCHAR(100) UNIQUE,
来源：http://wlm.jqgufenzy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ozu.xziqi.cn

);
来源：http://qpm.epnwcf.com

[Q02] 创建带外键的表
来源：http://ffy.birdmap.top

CREATE TABLE orders (
来源：http://bra.zhongyouzk.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pyb.yfazqb.com

user_id INT NOT NULL,
来源：http://idg.cheryme.top

amount DECIMAL(10, 2),
来源：http://pzt.vehdjk.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://myu.zhoulong.xyz

);
来源：http://sho.tanke756.top

[Q03] 增加列
来源：http://zfe.yuanzhike.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nyx.zhoulong.xyz

[Q04] 修改列类型
来源：http://iev.xuetiantiany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ptz.ivvv.top

[Q05] 重命名列
来源：http://gpk.andypj.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vsm.gzhubu.top

[Q06] 删除列
来源：http://ksz.zhaomingkeji.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://hmn.andypj.xyz

[Q07] 删除表
来源：http://zzg.yj20258888.top

DROP TABLE IF EXISTS orders;
来源：http://eey.nanxuanxn.top

[Q08] 创建普通索引
来源：http://ktu.zhiwuduotai.top

CREATE INDEX idx_users_email ON users(email);
来源：http://uqz.zdqjudy.top

[Q09] 创建唯一索引
来源：http://sig.iojbl.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://smp.havefunace.top

[Q10] 插入单行
来源：http://nrc.dashuyun.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fri.ivvv.top

[Q11] 一次插入多行
来源：http://agj.yangfankeji.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iof.tianlin.xyz

[Q12] 插入后取自增 ID
来源：http://xkg.sufxvd.cn

INSERT INTO users (name) VALUES ('C');
来源：http://kji.fanxiaobao.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ewk.jinyuanbaomall.cn

[Q13] 忽略重复插入
来源：http://xmy.gogol.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ddj.jiagoushi.top

[Q14] 存在则更新（upsert）
来源：http://xze.ehwqpu.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vgt.smart0.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mqm.ydzc1.top

[Q15] 查询全部
来源：http://cgs.yvedp.cn

SELECT * FROM users;
来源：http://hrc.dashuyun.cn

[Q16] 查询指定列
来源：http://ksp.tarul.cn

SELECT id, name FROM users;
来源：http://eli.ydzc1.top

[Q17] 条件查询
来源：http://xmr.sufxvd.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ksn.havefunace.top

[Q18] 模糊匹配
来源：http://dud.aizwys.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://zas.hywenlv.cn

[Q19] 范围查询
来源：http://apg.0kj1m.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tus.hywenlv.cn

[Q20] IN 列表
来源：http://qzc.jiagoushi.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wbu.hammf.cn

[Q21] 空值判断
来源：http://mgo.xylfe.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://iha.jinyuanbaomall.cn

[Q22] 排序
来源：http://xll.cheryme.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://oyq.52xcode.cn

[Q23] 分页
来源：http://lyz.dashuyun.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xqt.ydjk.org.cn

[Q24] 去重
来源：http://kew.hammf.cn

SELECT DISTINCT city FROM users;
来源：http://gkd.feifeiyinyue.top

[Q25] 只取前 N 条
来源：http://eqp.hammf.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jpy.xinyue.icu

[Q26] 计数
来源：http://tjs.jinghuilouyu.cn

SELECT COUNT(*) FROM users;
来源：http://etk.hnxiangtu.top

[Q27] 条件计数
来源：http://edp.aibaodan.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jzg.tianlin.xyz

[Q28] 求和与平均
来源：http://rua.wangshuangyany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://psh.nanxinkj.top

[Q29] 最大最小值
来源：http://sok.shuidangran.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://avb.chenzaomai.com

[Q30] 分组统计
来源：http://rsl.jinghuilouyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://roz.zhengqikj.top

[Q31] 分组后过滤
来源：http://clh.guowangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qlv.guowangkeji.top

[Q32] 分组拼接字符串
来源：http://ibs.chenlongwang.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://cef.hywenlv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vff.yvedp.cn

[Q33] 多列分组
来源：http://zro.pycfn.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vuw.hongshengwenyu.top

[Q34] 每组取第一条
来源：http://iiz.guannengcc.top

SELECT * FROM (
来源：http://tjx.gotoacloud.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lnj.yj202588.top

) t WHERE rn = 1;
来源：http://vzd.sysykeji.top

[Q35] 内连接
来源：http://drc.cashguo.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://evz.sxryk.cn

[Q36] 左连接
来源：http://ibn.zhongyouzk.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nem.yuanzhike.top

[Q37] 右连接
来源：http://vob.jianghu66.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jxu.jqgufenzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://yit.52xcode.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pcn.hfpthk.cn

[Q39] 自连接（查上下级）
来源：http://ozl.zhijiandao.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://gye.bjfxy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://azv.sjlbkw.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://hyb.zhixingplan.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://isn.shzxlz.cn

[Q41] 多表连接
来源：http://amj.zhixingplan.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://iju.smart0.xyz

JOIN users u ON u.id = o.user_id
来源：http://iss.zdqjudy.top

JOIN products p ON p.id = o.product_id;
来源：http://czb.ppjwa.cn

[Q42] 连接条件附加过滤
来源：http://jmb.yj202588.top

SELECT u.name, o.amount FROM users u
来源：http://cxo.sysykeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fgt.dashuyun.cn

[Q43] 标量子查询
来源：http://xbd.0kj1m.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jyi.shanyushiyangkeji.top

[Q44] IN 子查询
来源：http://fmr.hammf.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mda.jinghuilouyu.cn

[Q45] EXISTS 判断存在
来源：http://cbc.jinqigfzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nqh.0kj1m.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sku.fktsv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dfk.kuanghao11.cn

[Q47] 与平均值比较
来源：http://pql.andypj.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kvy.hnxiangtu.top

[Q48] CTE 公用表表达式
来源：http://xom.cucudq.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zvb.jinghuilouyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://fha.fanxiaobao.xyz

[Q49] 更新单行
来源：http://yet.yuxming.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lqp.xinyue.icu

[Q50] 批量更新
来源：http://diy.52xcode.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://msb.jinqigfzy.top

[Q51] 用子查询更新
来源：http://jee.nwbrower.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qpw.smart0.xyz

[Q52] 删除指定行
来源：http://ogx.shzxlz.cn

DELETE FROM users WHERE id = 10;
来源：http://hwc.dianchejie.cn

[Q53] 按条件删除
来源：http://kft.yueranfly.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gku.epnwcf.com

[Q54] 清空表
来源：http://usz.shangyingyoupin.top

TRUNCATE TABLE logs;
来源：http://bud.feifeiyinyue.top

[Q55] 排名（并列占位）
来源：http://fgr.aibaodan.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://iet.ehwqpu.com

[Q56] 密集排名（并列不占位）
来源：http://zuf.yanxiufei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vsc.jinqigfzy.top

[Q57] 行号
来源：http://mvo.0kj1m.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cxs.fzhhl.top

[Q58] 累计求和
来源：http://iiw.yuxming.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pby.pengpengdd.cyou

[Q59] 分组内累计
来源：http://ago.cdnleiting.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://inr.hfpthk.cn

[Q60] 取上一行 / 下一行
来源：http://brd.aizwys.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ywl.ybcxt.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jvp.xinyue.icu

[Q61] 移动平均
来源：http://han.yueranfly.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tqb.hfpthk.cn

[Q62] 分组占比
来源：http://iwc.zhijiandao.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://squ.0kj1m.cn

[Q63] 开启事务
来源：http://emw.dashuyun.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kbw.cdnleiting.top

[Q64] 提交事务
来源：http://gpa.yj20258888.top

COMMIT;
来源：http://adj.sweek.top

[Q65] 回滚事务
来源：http://och.snrcjt.cn

ROLLBACK;
来源：http://umh.mhx1999.top

[Q66] 行锁查询
来源：http://uhn.guannengcc.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ypu.svipenyu.cn

[Q67] 设置隔离级别
来源：http://rfr.xingfuxueyuan.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://imc.jinyuanbaomall.cn

[Q68] 保存点
来源：http://ala.sufxvd.cn

SAVEPOINT sp1;
来源：http://dto.hammf.cn

ROLLBACK TO sp1;
来源：http://lsl.yuanzhike.top

[Q69] 查看执行计划
来源：http://aqr.0kj1m.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://woe.zhongyouzk.top

[Q70] 更新统计信息
来源：http://npf.zhixingplan.top

ANALYZE TABLE users;
来源：http://yca.zhengqikj.top

[Q71] 查看建表语句
来源：http://nqu.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ifk.ydzc1.top

[Q72] 查看索引
来源：http://pmj.hammf.cn

SHOW INDEX FROM users;
来源：http://xsq.chenlongwang.top

[Q73] 查看表状态
来源：http://ige.gzhubu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://usm.hcnkem.com

[Q74] 强制使用索引
来源：http://dhn.cheryme.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tpu.yj20258888.top

[Q75] 日期格式化
来源：http://zes.pycfn.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://utd.yueranfly.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://aud.ybcxt.top

[Q76] 按天统计
来源：http://xfy.vehdjk.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hsv.ywan-chungtsiang.top

[Q77] 时间加减
来源：http://qfy.xinyue.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jre.jiagoushi.top

[Q78] 当前时间
来源：http://gue.nwbrower.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://top.nanxuanxn.top

[Q79] 字符串拼接
来源：http://wtx.ydzc1.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bli.dianchejie.cn

[Q80] 字符串截取
来源：http://pgz.gotoacloud.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nki.nwbrower.top

[Q81] 字符串替换
来源：http://ioy.epnwcf.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hrp.hcnkem.com

[Q82] 字符长度与字节长度
来源：http://bze.sjlbkw.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://abq.xuetiantiany.cn

[Q83] 大小写转换
来源：http://wuk.havefunace.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vzc.zhixingplan.top


<!-- 参考信息 -->