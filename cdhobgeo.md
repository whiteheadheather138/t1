代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lxv.cheryme.top

[O03] 加锁保护共享数据
来源：http://yau.jqgfzy.top

Py:   with lock: shared += 1
来源：http://rwm.sweek.top

PHP:  // 用 flock() 做文件锁
来源：http://llm.tanke756.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qov.ybcxt.top

TS:   // 同 JS
来源：http://sqt.pengpengdd.cyou

Java: synchronized (this) { shared++; }
来源：http://yiv.ydjk.org.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gpp.chenjidiqi.icu

Ruby: mutex.synchronize { shared += 1 }
来源：http://ewn.cucudq.cn

C#:   lock (gate) { shared++; }
来源：http://fzs.zhixingplan.top

[O04] 定义异步函数并等待
来源：http://zbf.kuanghao11.cn

Py:   async def f():⏎    await g()
来源：http://poy.yj202588.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zmw.dashuyun.cn

JS:   async function f() { await g(); }
来源：http://gtf.yongpay.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://cru.aibaodan.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hbs.guowangkeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nkq.zycfv.cn

Ruby: # 用 Fiber 或 async gem
来源：http://any.zdqjudy.top

C#:   async Task F() { await G(); }
来源：http://xrt.ppjwa.cn

[O05] 并发执行并等待全部完成
来源：http://pbg.snrcjt.cn

Py:   asyncio.gather(*tasks)
来源：http://lfv.cucudq.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nvy.daria6918.cn

JS:   await Promise.all(tasks)
来源：http://dte.gzhubu.top

TS:   await Promise.all(tasks)
来源：http://isc.xinyue.icu

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lze.cqqwz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ana.cheryme.top

Ruby: threads.map(&:join)
来源：http://dgi.kuanghao11.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://mgm.tarul.cn

[O06] 使用进程池
来源：http://bfu.fzhhl.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kzd.fanxiaobao.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://pgg.quarkkingdee.top

JS:   // child_process / cluster 模块
来源：http://hwt.shanyushiyangkeji.top

TS:   // child_process / cluster 模块
来源：http://wai.kuanghao11.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kdz.fehbvm.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hft.jiagoushi.top

Ruby: // fork 块
来源：http://hfo.ydjk.org.cn

C#:   Parallel.For
来源：http://pzg.gotoacloud.top

================================================================================
来源：http://drn.jinqigufen.top

P. 常用工具函数
来源：http://ntg.kuanghao11.cn

================================================================================
来源：http://czb.ydzc1.top

[P01] 生成 UUID
来源：http://ebh.xuanzx.com

Py:   str(uuid.uuid4())
来源：http://kgs.hnqzz.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://lpv.shanyushiyangtech.top

JS:   crypto.randomUUID()
来源：http://pmp.iojbl.cn

TS:   crypto.randomUUID()
来源：http://yar.fengsongda.top

Java: UUID.randomUUID().toString()
来源：http://rvs.fanxiaobao.xyz

Go:   // 用 github.com/google/uuid
来源：http://vcc.yonumen.top

Ruby: SecureRandom.uuid
来源：http://utj.jianghu66.top

C#:   Guid.NewGuid().ToString()
来源：http://tmk.yangfankeji.com

[P02] MD5 / SHA256 摘要
来源：http://bmg.hongshengwenyu.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zyr.cheryme.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://qta.yangfankeji.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://umx.tianlin.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ajd.guowangkeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://jii.tarul.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jsk.c1oappe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gff.yuanzhike.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ymh.dashuyun.cn

[P03] 生成短随机字符串
来源：http://lvz.ppjwa.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blz.hesvh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dnj.yanxiufei.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uij.zhongyouzk.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zhb.dashuyun.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://aum.yfazqb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vxt.cdnleiting.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tzs.gaohongyu789.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mgs.zhengqikj.top

[P04] 求长度
来源：http://umu.yuxming.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dad.yj20258.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xoc.zdqjudy.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jle.jqgfzy.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://nfa.yuxming.cn

Java: list.size();  map.size();  s.length()
来源：http://kfg.shuidangran.top

Go:   len(arr);  len(m)
来源：http://rxd.ctjpmb.com

Ruby: x.length;  x.size
来源：http://ojl.zhoulong.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://mqt.9152youxi.cn

[P05] 判断两个对象内容是否相等
来源：http://exo.cqqwz.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://xyp.vehdjk.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://sho.yanxiufei.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://hps.hfpthk.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bix.zhaomingkeji.xyz

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://eln.sysykeji.top

Go:   reflect.DeepEqual(a, b)
来源：http://wfw.jyoumei.cn

Ruby: a == b
来源：http://phd.svipenyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iwg.gotoacloud.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://unf.daria6918.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://puh.sufxvd.cn

PHP:  if (empty($x)) {}
来源：http://epu.jqgufenzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gab.yfazqb.com

TS:   if (x == null) {}
来源：http://qfj.uphjek.com

Java: if (x == null || x.isEmpty()) {}
来源：http://axl.0kj1m.cn

Go:   if x == nil {}
来源：http://jpy.jlsjyb.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uoi.jianghu66.top

C#:   if (x is null) {}
来源：http://svq.havefunace.top

[P07] 防抖与节流
来源：http://txy.jinqigufen.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://idg.snrcjt.cn

PHP:  // 手写时间戳比较
来源：http://rxn.dashuyun.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hlh.fanxiaobao.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wud.zhaomingkeji.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ndh.hnxiangtu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jqi.quarkkingdee.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://lyi.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vms.hongshengwenyu.top

[P08] 处理浮点精度问题
来源：http://edc.ywan-chungtsiang.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ixg.hesvh.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kqi.smart0.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://apv.guannengcc.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://llg.zhengqikj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://hki.epnwcf.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rmi.ywan-chungtsiang.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ciy.pengpengdd.cyou

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ufw.hesvh.cn

================================================================================
来源：http://hlv.zhengqikj.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wuo.guowangkeji.top

================================================================================
来源：http://mlf.dashuyun.cn

[Q01] 创建表
来源：http://rfb.guannengcc.top

CREATE TABLE users (
来源：http://off.yvedp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vov.yonumen.top

name VARCHAR(50) NOT NULL,
来源：http://nqs.xylfe.cn

email VARCHAR(100) UNIQUE,
来源：http://dlv.jianghu66.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://hcx.chenlongwang.top

);
来源：http://dmw.chenjidiqi.icu

[Q02] 创建带外键的表
来源：http://cbe.nanxinkj.top

CREATE TABLE orders (
来源：http://oib.ppjwa.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xiu.hnqzz.top

user_id INT NOT NULL,
来源：http://hbv.ivvv.top

amount DECIMAL(10, 2),
来源：http://gxg.aizwys.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sjq.hysaishi.cn

);
来源：http://ebe.9152youxi.cn

[Q03] 增加列
来源：http://hoj.wangdashe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nsp.hcnkem.com

[Q04] 修改列类型
来源：http://xjr.ivvv.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://shh.zhiwuduotai.top

[Q05] 重命名列
来源：http://psj.jiagoushi.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://aco.xziqi.cn

[Q06] 删除列
来源：http://lla.zdqjudy.top

ALTER TABLE users DROP COLUMN age;
来源：http://mmh.zdqjudy.top

[Q07] 删除表
来源：http://osy.ctjpmb.com

DROP TABLE IF EXISTS orders;
来源：http://gse.yj20258.top

[Q08] 创建普通索引
来源：http://tsm.chenzaomai.com

CREATE INDEX idx_users_email ON users(email);
来源：http://uwf.jiagoushi.top

[Q09] 创建唯一索引
来源：http://owo.shanyushiyangtech.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hir.jqgufenzy.top

[Q10] 插入单行
来源：http://ovn.yj202588.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://whu.fanxiaobao.xyz

[Q11] 一次插入多行
来源：http://wyd.cqqwz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bnh.ybcxt.top

[Q12] 插入后取自增 ID
来源：http://exl.jinyuanbaomall.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xwz.guowangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://edo.ywan-chungtsiang.top

[Q13] 忽略重复插入
来源：http://emr.chenjidiqi.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://kmd.jinghuilouyu.cn

[Q14] 存在则更新（upsert）
来源：http://hjk.quarkkingdee.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://idi.xuanzx.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ttn.pengpengdd.cyou

[Q15] 查询全部
来源：http://txg.jianghu66.top

SELECT * FROM users;
来源：http://mmm.vehdjk.com

[Q16] 查询指定列
来源：http://pek.ywan-chungtsiang.top

SELECT id, name FROM users;
来源：http://lxc.zdbjq.cn

[Q17] 条件查询
来源：http://teo.sweek.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pag.hesvh.cn

[Q18] 模糊匹配
来源：http://wrb.fengsongda.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ncl.zhongyouzk.top

[Q19] 范围查询
来源：http://glw.zhengqikj.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jci.zhixingplan.top

[Q20] IN 列表
来源：http://jqu.gotoacloud.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hkw.ehwqpu.com

[Q21] 空值判断
来源：http://vxg.zycfv.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xaz.cheryme.top

[Q22] 排序
来源：http://xdh.cashguo.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://bov.shangyingyoupin.top

[Q23] 分页
来源：http://tsw.hnxiangtu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fmq.zhiwuduotai.top

[Q24] 去重
来源：http://ksb.havefunace.top

SELECT DISTINCT city FROM users;
来源：http://klh.aizwys.cn

[Q25] 只取前 N 条
来源：http://efb.hammf.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://tmr.gogol.net.cn

[Q26] 计数
来源：http://pyf.shuidangran.top

SELECT COUNT(*) FROM users;
来源：http://bjm.316326.xyz

[Q27] 条件计数
来源：http://zwi.zhijiandao.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kyi.haohaochexian.top

[Q28] 求和与平均
来源：http://ubg.cqqwz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wqx.vqdsnc.cn

[Q29] 最大最小值
来源：http://mxe.chenzaomai.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://gsk.mhx1999.top

[Q30] 分组统计
来源：http://sde.feifeiyinyue.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ebe.cheryme.top

[Q31] 分组后过滤
来源：http://opf.yangfankeji.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ngj.dianchejie.cn

[Q32] 分组拼接字符串
来源：http://uwz.guannengcc.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ope.daxiang520.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ztq.haohaochexian.top

[Q33] 多列分组
来源：http://ehj.zdqjudy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qov.fengsongda.top

[Q34] 每组取第一条
来源：http://yqr.vehdjk.com

SELECT * FROM (
来源：http://ppr.chenlongwang.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lvn.yuanzhike.top

) t WHERE rn = 1;
来源：http://qde.hammf.cn

[Q35] 内连接
来源：http://eln.hesvh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uxw.jianghu66.top

[Q36] 左连接
来源：http://lyc.zdbjq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xdf.jyoumei.cn

[Q37] 右连接
来源：http://ajg.bbcook.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://psr.zdbjq.cn

[Q38] 全外连接（PostgreSQL）
来源：http://gcm.zhengqikj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dcv.jianghu66.top

[Q39] 自连接（查上下级）
来源：http://mst.zdqjudy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://lof.guowangkeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mse.smart0.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://ntk.zdqjudy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ckr.ydjk.org.cn

[Q41] 多表连接
来源：http://msx.smart0.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://knp.shzxlz.cn

JOIN users u ON u.id = o.user_id
来源：http://urn.epnwcf.com

JOIN products p ON p.id = o.product_id;
来源：http://mqz.nwbrower.top

[Q42] 连接条件附加过滤
来源：http://nei.bbcook.cn

SELECT u.name, o.amount FROM users u
来源：http://oik.bbcook.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qrn.feifeiyinyue.top

[Q43] 标量子查询
来源：http://nrp.tian-w.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zjb.chenjidiqi.icu

[Q44] IN 子查询
来源：http://siy.gzhubu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zws.hysaishi.cn

[Q45] EXISTS 判断存在
来源：http://aak.ivvv.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vrq.zdbjq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yvi.jqgufenzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qzh.xinyue.icu

[Q47] 与平均值比较
来源：http://zir.shangyingyoupin.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zjl.gotoacloud.top

[Q48] CTE 公用表表达式
来源：http://qos.wangdashe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ifr.zdbjq.cn

SELECT * FROM t WHERE c > 5;
来源：http://uwd.zhengqikj.top

[Q49] 更新单行
来源：http://jcm.shangyingyoupin.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qfe.hcnkem.com

[Q50] 批量更新
来源：http://lxp.pycfn.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gzi.sufxvd.cn

[Q51] 用子查询更新
来源：http://afz.andypj.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yxc.zycfv.cn

[Q52] 删除指定行
来源：http://ulp.shzxlz.cn

DELETE FROM users WHERE id = 10;
来源：http://kqj.guannengcc.top

[Q53] 按条件删除
来源：http://uqy.ybcxt.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vhg.shanyushiyangtech.top

[Q54] 清空表
来源：http://gsq.pengpengdd.cyou

TRUNCATE TABLE logs;
来源：http://hni.xylfe.cn

[Q55] 排名（并列占位）
来源：http://nxy.shuidangran.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wnp.zhixingplan.top

[Q56] 密集排名（并列不占位）
来源：http://tqo.xuanzx.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jas.tian-w.cn

[Q57] 行号
来源：http://vlr.zhengqikj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sab.sxryk.cn

[Q58] 累计求和
来源：http://wjj.c1oappe.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jnc.vqdsnc.cn

[Q59] 分组内累计
来源：http://upy.tian-w.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hkh.xingfuxueyuan.xyz

[Q60] 取上一行 / 下一行
来源：http://xya.zhongyouzk.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vwe.hcnkem.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xte.fanxiaobao.xyz

[Q61] 移动平均
来源：http://srv.tianlin.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qhc.c1oappe.top

[Q62] 分组占比
来源：http://tda.chenlongwang.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vst.zhoulong.xyz

[Q63] 开启事务
来源：http://odz.zhiwuduotai.top

START TRANSACTION;                -- 或 BEGIN
来源：http://stz.zhengqikj.top

[Q64] 提交事务
来源：http://piu.fanxiaobao.xyz

COMMIT;
来源：http://wif.hnxiangtu.top

[Q65] 回滚事务
来源：http://cha.shanyushiyangtech.top

ROLLBACK;
来源：http://hgx.svipenyu.cn

[Q66] 行锁查询
来源：http://wgf.guannengcc.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://clw.yj20258.top

[Q67] 设置隔离级别
来源：http://ume.xuanzx.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iiw.guowangkeji.top

[Q68] 保存点
来源：http://llg.shanyushiyangtech.top

SAVEPOINT sp1;
来源：http://hsy.c1oappe.top

ROLLBACK TO sp1;
来源：http://uvh.yj20258888.top

[Q69] 查看执行计划
来源：http://fja.haohaochexian.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hkp.aibaodan.cn

[Q70] 更新统计信息
来源：http://fow.cqqwz.cn

ANALYZE TABLE users;
来源：http://ogp.chenzaomai.com

[Q71] 查看建表语句
来源：http://qhz.yueranfly.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wrf.jiagoushi.top

[Q72] 查看索引
来源：http://jjw.sweek.top

SHOW INDEX FROM users;
来源：http://evu.dashuyun.cn

[Q73] 查看表状态
来源：http://kgk.hysaishi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://quy.nanxuanxn.top

[Q74] 强制使用索引
来源：http://vgd.uphjek.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zmp.gzhubu.top

[Q75] 日期格式化
来源：http://eoc.wangshuangyany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qsd.52xcode.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wvz.pycfn.com

[Q76] 按天统计
来源：http://qns.nwbrower.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vdo.xziqi.cn

[Q77] 时间加减
来源：http://ilp.guannengcc.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gum.meibo888.top

[Q78] 当前时间
来源：http://vtv.zhengqikj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vly.chenzaomai.com

[Q79] 字符串拼接
来源：http://dwj.hfpthk.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://orl.xziqi.cn

[Q80] 字符串截取
来源：http://wee.aizwys.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://toa.hesvh.cn

[Q81] 字符串替换
来源：http://ucr.pycfn.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iwj.daria6918.cn


<!-- 参考信息 -->