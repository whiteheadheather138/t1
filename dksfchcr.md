代发 wailian999

TS:   // worker_threads 线程池
来源：http://eqe.hongshengwenyu.top

Java: Executors.newFixedThreadPool(4)
来源：http://msa.ivvv.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://fax.jiagoushi.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://rtw.ybcxt.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://dvj.bbcook.cn

[O03] 加锁保护共享数据
来源：http://vmv.zdqjudy.top

Py:   with lock: shared += 1
来源：http://qmh.ehwqpu.com

PHP:  // 用 flock() 做文件锁
来源：http://pug.aibaodan.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://twb.yuanzhike.top

TS:   // 同 JS
来源：http://qap.vqdsnc.cn

Java: synchronized (this) { shared++; }
来源：http://lfb.nanxuanxn.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hsd.shuidangran.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://luq.jinqigufen.top

C#:   lock (gate) { shared++; }
来源：http://elh.pengpengdd.cyou

[O04] 定义异步函数并等待
来源：http://qsm.hnxiangtu.top

Py:   async def f():⏎    await g()
来源：http://cko.sweek.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mks.zdqjudy.top

JS:   async function f() { await g(); }
来源：http://wkn.havefunace.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://snq.daxiang520.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://axr.wangshuangyany.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xch.bbcook.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cth.aizwys.cn

C#:   async Task F() { await G(); }
来源：http://sri.yongpay.top

[O05] 并发执行并等待全部完成
来源：http://caq.yj20258.top

Py:   asyncio.gather(*tasks)
来源：http://usi.hysaishi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dhj.cqqwz.cn

JS:   await Promise.all(tasks)
来源：http://tmc.cashguo.top

TS:   await Promise.all(tasks)
来源：http://hmx.sweek.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bvt.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://asc.xinyue.icu

Ruby: threads.map(&:join)
来源：http://vcx.aibaodan.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://par.daria6918.cn

[O06] 使用进程池
来源：http://nlu.ywan-chungtsiang.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ibj.fktsv.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://icp.zhijiandao.cn

JS:   // child_process / cluster 模块
来源：http://jwo.ydjk.org.cn

TS:   // child_process / cluster 模块
来源：http://svh.sjlbkw.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jqu.hongshengwenyu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ons.9152youxi.cn

Ruby: // fork 块
来源：http://kga.xinyue.icu

C#:   Parallel.For
来源：http://yky.dashuyun.cn

================================================================================
来源：http://yrb.tianlin.xyz

P. 常用工具函数
来源：http://czo.hnxiangtu.top

================================================================================
来源：http://avl.yuanzhike.top

[P01] 生成 UUID
来源：http://rww.yj20258.top

Py:   str(uuid.uuid4())
来源：http://grb.andypj.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oco.dashuyun.cn

JS:   crypto.randomUUID()
来源：http://fij.shuidangran.top

TS:   crypto.randomUUID()
来源：http://llv.pengpengdd.cyou

Java: UUID.randomUUID().toString()
来源：http://fna.quarkkingdee.top

Go:   // 用 github.com/google/uuid
来源：http://mpu.yj20258888.top

Ruby: SecureRandom.uuid
来源：http://uhd.fktsv.cn

C#:   Guid.NewGuid().ToString()
来源：http://sga.jinqigufen.top

[P02] MD5 / SHA256 摘要
来源：http://gjn.gzhubu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://kdp.zdqjudy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qaq.dianchejie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://kkv.jianghu66.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dea.hammf.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://npq.daxiang520.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://lqm.cqqwz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://mxh.guannengcc.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cgw.fengsongda.top

[P03] 生成短随机字符串
来源：http://jco.gotoacloud.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ezd.yj202588.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bbm.smart0.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fiz.ehwqpu.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zvs.sysykeji.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vfc.meibo888.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://nrh.ybcxt.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://yzo.bjfxy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://phg.guowangkeji.top

[P04] 求长度
来源：http://kes.jqgufenzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://sci.quarkkingdee.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ler.fehbvm.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nst.chenjidiqi.icu

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://foc.tarul.cn

Java: list.size();  map.size();  s.length()
来源：http://stz.chenzaomai.com

Go:   len(arr);  len(m)
来源：http://iqb.nanxuanxn.top

Ruby: x.length;  x.size
来源：http://zps.jinyuanbaomall.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://afi.guannengcc.top

[P05] 判断两个对象内容是否相等
来源：http://kcr.vehdjk.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://gwz.kuanghao11.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hee.ydjk.org.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tje.zdbjq.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eos.xuetiantiany.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://toy.0kj1m.cn

Go:   reflect.DeepEqual(a, b)
来源：http://abv.dianchejie.cn

Ruby: a == b
来源：http://rkf.kuanghao11.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ngd.c1oappe.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wnb.ydzc1.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://oqm.yueranfly.top

PHP:  if (empty($x)) {}
来源：http://uyt.dianchejie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zut.fktsv.cn

TS:   if (x == null) {}
来源：http://txo.zhijiandao.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nbx.jqgufenzy.top

Go:   if x == nil {}
来源：http://mbe.cucudq.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://huq.svipenyu.cn

C#:   if (x is null) {}
来源：http://flv.vehdjk.com

[P07] 防抖与节流
来源：http://ikn.zdbjq.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ssy.tianlin.xyz

PHP:  // 手写时间戳比较
来源：http://jxq.xingfuxueyuan.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gsp.guowangkeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://til.bbcook.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vuo.ydjk.org.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uwk.bjfxy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://npm.chenjidiqi.icu

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jkg.shangyingyoupin.top

[P08] 处理浮点精度问题
来源：http://wyq.nanxinkj.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wvr.hammf.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://iiv.daxiang520.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uuu.wangshuangyany.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://flk.jianghu66.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vlo.quarkkingdee.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://szo.feifeiyinyue.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://fwb.quarkkingdee.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://oaz.zhijiandao.cn

================================================================================
来源：http://tiy.tianlin.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://byl.yueranfly.top

================================================================================
来源：http://suw.yangfankeji.com

[Q01] 创建表
来源：http://yiq.pycfn.com

CREATE TABLE users (
来源：http://uil.jqgfzy.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://quy.fzhhl.top

name VARCHAR(50) NOT NULL,
来源：http://viz.shangyingyoupin.top

email VARCHAR(100) UNIQUE,
来源：http://wye.haohaochexian.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vnr.guannengcc.top

);
来源：http://fig.xinyue.icu

[Q02] 创建带外键的表
来源：http://mbb.kuanghao11.cn

CREATE TABLE orders (
来源：http://icg.52xcode.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jsr.jiagoushi.top

user_id INT NOT NULL,
来源：http://jzl.daxiang520.top

amount DECIMAL(10, 2),
来源：http://fno.andypj.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tfg.aizwys.cn

);
来源：http://vhe.yj202588.top

[Q03] 增加列
来源：http://zmn.yj20258888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xno.zhengqikj.top

[Q04] 修改列类型
来源：http://xpr.chenzaomai.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uju.redwolf501.top

[Q05] 重命名列
来源：http://apm.hfpthk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hos.zhiwuduotai.top

[Q06] 删除列
来源：http://ytw.jlsjyb.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tfv.nanxinkj.top

[Q07] 删除表
来源：http://ftj.bjfxy.top

DROP TABLE IF EXISTS orders;
来源：http://szu.xuanzx.com

[Q08] 创建普通索引
来源：http://wlf.ydjk.org.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://eql.cashguo.top

[Q09] 创建唯一索引
来源：http://coj.sxryk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ias.sysykeji.top

[Q10] 插入单行
来源：http://oho.hnqzz.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pmj.sweek.top

[Q11] 一次插入多行
来源：http://ggf.sweek.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tli.vqdsnc.cn

[Q12] 插入后取自增 ID
来源：http://eig.cashguo.top

INSERT INTO users (name) VALUES ('C');
来源：http://ccb.ydzc1.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://igv.hywenlv.cn

[Q13] 忽略重复插入
来源：http://tpq.jinyuanbaomall.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rqi.gogol.net.cn

[Q14] 存在则更新（upsert）
来源：http://qrq.zhixingplan.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://azk.vqdsnc.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ndf.yuanzhike.top

[Q15] 查询全部
来源：http://tns.ehwqpu.com

SELECT * FROM users;
来源：http://qqg.aizwys.cn

[Q16] 查询指定列
来源：http://vgd.chenjidiqi.icu

SELECT id, name FROM users;
来源：http://aku.hnxiangtu.top

[Q17] 条件查询
来源：http://pvg.zycfv.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bwi.jqgfzy.top

[Q18] 模糊匹配
来源：http://kip.sjlbkw.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nvh.gaohongyu789.top

[Q19] 范围查询
来源：http://tis.kuanghao11.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://esl.fzhhl.top

[Q20] IN 列表
来源：http://hca.zhoulong.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ufi.cashguo.top

[Q21] 空值判断
来源：http://rbl.hammf.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://tzv.uphjek.com

[Q22] 排序
来源：http://abx.jinqigufen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zrw.tianlin.xyz

[Q23] 分页
来源：http://nhf.zhongyouzk.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vib.kuanghao11.cn

[Q24] 去重
来源：http://gfy.hongshengwenyu.top

SELECT DISTINCT city FROM users;
来源：http://jjf.yuanzhike.top

[Q25] 只取前 N 条
来源：http://zvi.jqgfzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nnh.yangfankeji.com

[Q26] 计数
来源：http://ods.hammf.cn

SELECT COUNT(*) FROM users;
来源：http://dby.feifeiyinyue.top

[Q27] 条件计数
来源：http://rtp.feifeiyinyue.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://yqb.aibaodan.cn

[Q28] 求和与平均
来源：http://vgf.guannengcc.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://reo.316326.xyz

[Q29] 最大最小值
来源：http://owg.yvedp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ued.yj202588.top

[Q30] 分组统计
来源：http://jbf.sjlbkw.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://yhe.yj20258888.top

[Q31] 分组后过滤
来源：http://dlh.mhx1999.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gpn.yfazqb.com

[Q32] 分组拼接字符串
来源：http://viw.nwbrower.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wor.zhixingplan.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wdw.jinyuanbaomall.cn

[Q33] 多列分组
来源：http://xne.zdbjq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jpg.cdnleiting.top

[Q34] 每组取第一条
来源：http://rva.hesvh.cn

SELECT * FROM (
来源：http://xpy.chenjidiqi.icu

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://grx.hnxiangtu.top

) t WHERE rn = 1;
来源：http://dqq.ppjwa.cn

[Q35] 内连接
来源：http://uwr.fehbvm.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://phf.uphjek.com

[Q36] 左连接
来源：http://lyb.jqgfzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://oll.tian-w.cn

[Q37] 右连接
来源：http://hbo.yfazqb.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bfi.52xcode.cn

[Q38] 全外连接（PostgreSQL）
来源：http://jju.wangdashe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gmb.andypj.xyz

[Q39] 自连接（查上下级）
来源：http://yaf.hysaishi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lpp.jlsjyb.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://prr.shzxlz.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://osy.zdqjudy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bgp.nanxinkj.top

[Q41] 多表连接
来源：http://ycq.gaohongyu789.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qft.ppjwa.cn

JOIN users u ON u.id = o.user_id
来源：http://wgr.gaohongyu789.top

JOIN products p ON p.id = o.product_id;
来源：http://jbc.andypj.xyz

[Q42] 连接条件附加过滤
来源：http://gii.hysaishi.cn

SELECT u.name, o.amount FROM users u
来源：http://cva.fengsongda.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://kpm.xingfuxueyuan.xyz

[Q43] 标量子查询
来源：http://luf.yj20258.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://atw.sxryk.cn

[Q44] IN 子查询
来源：http://oay.jianghu66.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vzg.sweek.top

[Q45] EXISTS 判断存在
来源：http://hpf.yangfankeji.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qho.shangyingyoupin.top

[Q46] NOT EXISTS 判断不存在
来源：http://kda.gotoacloud.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qqh.hammf.cn

[Q47] 与平均值比较
来源：http://omr.yj20258.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nfv.nwbrower.top

[Q48] CTE 公用表表达式
来源：http://hca.sxryk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zel.zhongyouzk.top

SELECT * FROM t WHERE c > 5;
来源：http://seg.dianchejie.cn

[Q49] 更新单行
来源：http://rqj.tarul.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://iel.yj202588.top

[Q50] 批量更新
来源：http://mvn.c1oappe.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qfb.pengpengdd.cyou

[Q51] 用子查询更新
来源：http://iyd.ctjpmb.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://akb.jqgufenzy.top

[Q52] 删除指定行
来源：http://emc.shuidangran.top

DELETE FROM users WHERE id = 10;
来源：http://hfx.cucudq.cn

[Q53] 按条件删除
来源：http://lsc.cashguo.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bjn.yj20258888.top

[Q54] 清空表
来源：http://jyr.jinqigufen.top

TRUNCATE TABLE logs;
来源：http://eug.jqgfzy.top

[Q55] 排名（并列占位）
来源：http://isx.hcnkem.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gao.bbcook.cn

[Q56] 密集排名（并列不占位）
来源：http://idr.cheryme.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://two.ydjk.org.cn

[Q57] 行号
来源：http://oqv.gogol.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://knh.sjlbkw.cn

[Q58] 累计求和
来源：http://ydk.cqqwz.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fqa.yj202588.top

[Q59] 分组内累计
来源：http://qmb.andypj.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tbx.xingfuxueyuan.xyz

[Q60] 取上一行 / 下一行
来源：http://trd.zdqjudy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fhb.aizwys.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cbf.hongshengwenyu.top

[Q61] 移动平均
来源：http://rpt.haohaochexian.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pfu.snrcjt.cn

[Q62] 分组占比
来源：http://nug.nanxinkj.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hsq.redwolf501.top

[Q63] 开启事务
来源：http://tnn.bjfxy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://bye.xinyue.icu

[Q64] 提交事务
来源：http://jkk.mhx1999.top

COMMIT;
来源：http://mvl.cashguo.top

[Q65] 回滚事务
来源：http://ozm.ppjwa.cn

ROLLBACK;
来源：http://qim.jqgufenzy.top

[Q66] 行锁查询
来源：http://rzg.gogol.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ovc.fanxiaobao.xyz

[Q67] 设置隔离级别
来源：http://aqv.birdmap.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gof.tanke756.top

[Q68] 保存点
来源：http://uge.jqgfzy.top

SAVEPOINT sp1;
来源：http://mkq.jqgufenzy.top

ROLLBACK TO sp1;
来源：http://plh.zhoulong.xyz

[Q69] 查看执行计划
来源：http://erq.hysaishi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gni.wangdashe.top

[Q70] 更新统计信息
来源：http://ofg.tarul.cn

ANALYZE TABLE users;
来源：http://gpq.wangdashe.top

[Q71] 查看建表语句
来源：http://sjt.xziqi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jlx.shanyushiyangkeji.top

[Q72] 查看索引
来源：http://rbi.aizwys.cn

SHOW INDEX FROM users;
来源：http://bxb.andypj.xyz

[Q73] 查看表状态
来源：http://uoh.cashguo.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zqa.xylfe.cn

[Q74] 强制使用索引
来源：http://dqy.yonumen.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cif.zhiwuduotai.top

[Q75] 日期格式化
来源：http://mlw.cqqwz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hlm.cheryme.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bba.fengsongda.top

[Q76] 按天统计
来源：http://soa.xuanzx.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://izl.cucudq.cn

[Q77] 时间加减
来源：http://nsw.chenlongwang.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://arq.pengpengdd.cyou

[Q78] 当前时间
来源：http://stw.zhengqikj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rqf.jinqigufen.top

[Q79] 字符串拼接
来源：http://dkn.zhijiandao.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ook.jinyuanbaomall.cn


<!-- 参考信息 -->