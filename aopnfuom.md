代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://vsj.ydjk.org.cn

TS:   // 同 JS
来源：http://gfe.yfazqb.com

Java: synchronized (this) { shared++; }
来源：http://vjr.sysykeji.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://thv.ywan-chungtsiang.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ytd.smart0.xyz

C#:   lock (gate) { shared++; }
来源：http://wkq.yvedp.cn

[O04] 定义异步函数并等待
来源：http://dzs.xingfuxueyuan.xyz

Py:   async def f():⏎    await g()
来源：http://nfn.xingfuxueyuan.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://kjg.zdqjudy.top

JS:   async function f() { await g(); }
来源：http://sdz.bbcook.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://gsn.shanyushiyangtech.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://opf.fehbvm.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://qpl.jlsjyb.cn

Ruby: # 用 Fiber 或 async gem
来源：http://cbb.jlsjyb.cn

C#:   async Task F() { await G(); }
来源：http://rdu.0kj1m.cn

[O05] 并发执行并等待全部完成
来源：http://uvk.haohaochexian.top

Py:   asyncio.gather(*tasks)
来源：http://tdr.tarul.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://oun.hnqzz.top

JS:   await Promise.all(tasks)
来源：http://eal.yueranfly.top

TS:   await Promise.all(tasks)
来源：http://fev.jqgfzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ukc.shzxlz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://flz.hammf.cn

Ruby: threads.map(&:join)
来源：http://blg.nwbrower.top

C#:   await Task.WhenAll(t1, t2)
来源：http://iiz.fzhhl.top

[O06] 使用进程池
来源：http://ail.fanxiaobao.xyz

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kag.ehwqpu.com

PHP:  // pcntl_fork 或多进程队列
来源：http://tsm.jlsjyb.cn

JS:   // child_process / cluster 模块
来源：http://icx.shanyushiyangkeji.top

TS:   // child_process / cluster 模块
来源：http://rod.gotoacloud.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lyh.feifeiyinyue.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hbn.cdnleiting.top

Ruby: // fork 块
来源：http://nqc.yuxming.cn

C#:   Parallel.For
来源：http://yeb.xingfuxueyuan.xyz

================================================================================
来源：http://zsw.yfazqb.com

P. 常用工具函数
来源：http://qta.dianchejie.cn

================================================================================
来源：http://iad.ydjk.org.cn

[P01] 生成 UUID
来源：http://omv.ywan-chungtsiang.top

Py:   str(uuid.uuid4())
来源：http://ayd.haohaochexian.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xrl.havefunace.top

JS:   crypto.randomUUID()
来源：http://lfl.svipenyu.cn

TS:   crypto.randomUUID()
来源：http://vrz.daxiang520.top

Java: UUID.randomUUID().toString()
来源：http://zeo.9152youxi.cn

Go:   // 用 github.com/google/uuid
来源：http://qjw.cheryme.top

Ruby: SecureRandom.uuid
来源：http://jqz.quarkkingdee.top

C#:   Guid.NewGuid().ToString()
来源：http://nuc.meibo888.top

[P02] MD5 / SHA256 摘要
来源：http://zgy.sufxvd.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xma.xylfe.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://ztk.sxryk.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jxd.zhijiandao.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gxx.xuetiantiany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yky.jlsjyb.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qck.nanxuanxn.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zaj.zycfv.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ajk.xziqi.cn

[P03] 生成短随机字符串
来源：http://ieh.zhijiandao.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ees.aizwys.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hvi.jinyuanbaomall.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bug.yj20258.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bdi.yonumen.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://guh.cqqwz.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rbm.smart0.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://eqa.zhiwuduotai.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ksa.jinqigufen.top

[P04] 求长度
来源：http://uyz.xingfuxueyuan.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://dnl.9152youxi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wjh.xziqi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kph.smart0.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kta.daria6918.cn

Java: list.size();  map.size();  s.length()
来源：http://rom.jinghuilouyu.cn

Go:   len(arr);  len(m)
来源：http://xgp.gogol.net.cn

Ruby: x.length;  x.size
来源：http://jfp.xuanzx.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://xlv.gotoacloud.top

[P05] 判断两个对象内容是否相等
来源：http://fvz.0kj1m.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://vbw.gaohongyu789.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ubp.uphjek.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kil.xziqi.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gfd.kuanghao11.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xnw.nwbrower.top

Go:   reflect.DeepEqual(a, b)
来源：http://wbd.vqdsnc.cn

Ruby: a == b
来源：http://wxc.hammf.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ccs.xziqi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ehr.smart0.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://reh.fanxiaobao.xyz

PHP:  if (empty($x)) {}
来源：http://mns.birdmap.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vfe.bjfxy.top

TS:   if (x == null) {}
来源：http://ctr.yueranfly.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lhw.zdqjudy.top

Go:   if x == nil {}
来源：http://wid.hongshengwenyu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cjt.xuanzx.com

C#:   if (x is null) {}
来源：http://hlc.xuetiantiany.cn

[P07] 防抖与节流
来源：http://vuz.fehbvm.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lbj.yuanzhike.top

PHP:  // 手写时间戳比较
来源：http://bxh.feifeiyinyue.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fac.jinqigufen.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kuz.hywenlv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qlf.ivvv.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sqm.hfpthk.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://emx.hnqzz.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wul.vehdjk.com

[P08] 处理浮点精度问题
来源：http://pyz.yangfankeji.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ddo.yuanzhike.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qai.jinqigufen.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ali.yj20258.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mbe.tanke756.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wvz.tianlin.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bxh.jqgfzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://kuq.yj202588.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wlj.yuanzhike.top

================================================================================
来源：http://ngu.shzxlz.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fid.cdnleiting.top

================================================================================
来源：http://zoh.sweek.top

[Q01] 创建表
来源：http://kqe.cheryme.top

CREATE TABLE users (
来源：http://pqn.bbcook.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xnc.xuanzx.com

name VARCHAR(50) NOT NULL,
来源：http://qbz.shangyingyoupin.top

email VARCHAR(100) UNIQUE,
来源：http://fda.nanxinkj.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://faq.cheryme.top

);
来源：http://ewj.hesvh.cn

[Q02] 创建带外键的表
来源：http://kqm.andypj.xyz

CREATE TABLE orders (
来源：http://sgy.aibaodan.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lcw.shanyushiyangtech.top

user_id INT NOT NULL,
来源：http://qht.jianghu66.top

amount DECIMAL(10, 2),
来源：http://gfn.kuanghao11.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ffw.gzhubu.top

);
来源：http://boq.ydzc1.top

[Q03] 增加列
来源：http://leg.sweek.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jij.cqqwz.cn

[Q04] 修改列类型
来源：http://mel.yj20258.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ybp.fengsongda.top

[Q05] 重命名列
来源：http://hqs.andypj.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://yal.0kj1m.cn

[Q06] 删除列
来源：http://xbv.pycfn.com

ALTER TABLE users DROP COLUMN age;
来源：http://uvs.yj20258888.top

[Q07] 删除表
来源：http://zpg.smart0.xyz

DROP TABLE IF EXISTS orders;
来源：http://akh.gzhubu.top

[Q08] 创建普通索引
来源：http://ldf.svipenyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ohb.zycfv.cn

[Q09] 创建唯一索引
来源：http://nsf.cheryme.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://sso.gaohongyu789.top

[Q10] 插入单行
来源：http://alv.yj20258888.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://snl.hesvh.cn

[Q11] 一次插入多行
来源：http://enf.svipenyu.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tbh.cashguo.top

[Q12] 插入后取自增 ID
来源：http://qtn.hfpthk.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qoo.fanxiaobao.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://lhe.yfazqb.com

[Q13] 忽略重复插入
来源：http://yji.bjfxy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hgx.aibaodan.cn

[Q14] 存在则更新（upsert）
来源：http://jun.yonumen.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://amn.yuanzhike.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://gkb.hongshengwenyu.top

[Q15] 查询全部
来源：http://lla.redwolf501.top

SELECT * FROM users;
来源：http://uvi.tianlin.xyz

[Q16] 查询指定列
来源：http://kaq.wangshuangyany.cn

SELECT id, name FROM users;
来源：http://yyu.dianchejie.cn

[Q17] 条件查询
来源：http://ogy.vehdjk.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://acz.andypj.xyz

[Q18] 模糊匹配
来源：http://hwd.svipenyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ygj.yuxming.cn

[Q19] 范围查询
来源：http://zzq.gogol.net.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dvg.jqgfzy.top

[Q20] IN 列表
来源：http://kis.guannengcc.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lxb.sysykeji.top

[Q21] 空值判断
来源：http://get.vqdsnc.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://lul.zhiwuduotai.top

[Q22] 排序
来源：http://quh.9152youxi.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sto.svipenyu.cn

[Q23] 分页
来源：http://ldx.nwbrower.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xyb.nanxinkj.top

[Q24] 去重
来源：http://byt.nanxinkj.top

SELECT DISTINCT city FROM users;
来源：http://jrc.ydzc1.top

[Q25] 只取前 N 条
来源：http://jjy.yonumen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://apb.ivvv.top

[Q26] 计数
来源：http://ypt.wangdashe.top

SELECT COUNT(*) FROM users;
来源：http://hhj.bbcook.cn

[Q27] 条件计数
来源：http://tfo.fehbvm.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rej.tanke756.top

[Q28] 求和与平均
来源：http://ylz.jqgfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://diq.chenzaomai.com

[Q29] 最大最小值
来源：http://sik.redwolf501.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xml.shanyushiyangkeji.top

[Q30] 分组统计
来源：http://vwt.hesvh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qtq.hongshengwenyu.top

[Q31] 分组后过滤
来源：http://fov.redwolf501.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ipt.ybcxt.top

[Q32] 分组拼接字符串
来源：http://nff.fktsv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pae.cucudq.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://zgk.shzxlz.cn

[Q33] 多列分组
来源：http://zfp.cqqwz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rhj.zdqjudy.top

[Q34] 每组取第一条
来源：http://ovm.pycfn.com

SELECT * FROM (
来源：http://pqm.fehbvm.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ghm.fengsongda.top

) t WHERE rn = 1;
来源：http://lhn.cqqwz.cn

[Q35] 内连接
来源：http://tyn.yvedp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tnr.dianchejie.cn

[Q36] 左连接
来源：http://klp.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xoj.xuanzx.com

[Q37] 右连接
来源：http://nlk.tarul.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://twe.chenlongwang.top

[Q38] 全外连接（PostgreSQL）
来源：http://dob.hysaishi.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pwc.gotoacloud.top

[Q39] 自连接（查上下级）
来源：http://wkj.meibo888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qzj.ybcxt.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kmr.hesvh.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://krp.birdmap.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://yhd.zhengqikj.top

[Q41] 多表连接
来源：http://buc.hysaishi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://dmi.nanxuanxn.top

JOIN users u ON u.id = o.user_id
来源：http://ezr.yvedp.cn

JOIN products p ON p.id = o.product_id;
来源：http://sbc.epnwcf.com

[Q42] 连接条件附加过滤
来源：http://uka.fktsv.cn

SELECT u.name, o.amount FROM users u
来源：http://mbo.wangshuangyany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cjo.kuanghao11.cn

[Q43] 标量子查询
来源：http://lhn.aibaodan.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ima.jinghuilouyu.cn

[Q44] IN 子查询
来源：http://qza.hnxiangtu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mrq.zycfv.cn

[Q45] EXISTS 判断存在
来源：http://wlg.ydjk.org.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xps.cqqwz.cn

[Q46] NOT EXISTS 判断不存在
来源：http://amd.bjfxy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://unz.aibaodan.cn

[Q47] 与平均值比较
来源：http://ari.chenlongwang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://miu.wangdashe.top

[Q48] CTE 公用表表达式
来源：http://tic.nanxinkj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pvw.jinghuilouyu.cn

SELECT * FROM t WHERE c > 5;
来源：http://ehz.daxiang520.top

[Q49] 更新单行
来源：http://gax.snrcjt.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uxe.xuanzx.com

[Q50] 批量更新
来源：http://ztm.yuxming.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kdu.jinqigfzy.top

[Q51] 用子查询更新
来源：http://cuh.zhoulong.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qap.zhoulong.xyz

[Q52] 删除指定行
来源：http://rku.yj202588.top

DELETE FROM users WHERE id = 10;
来源：http://eau.wangdashe.top

[Q53] 按条件删除
来源：http://uaw.zhiwuduotai.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bwe.birdmap.top

[Q54] 清空表
来源：http://qrn.hongshengwenyu.top

TRUNCATE TABLE logs;
来源：http://pdq.c1oappe.top

[Q55] 排名（并列占位）
来源：http://jbf.316326.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dnd.cheryme.top

[Q56] 密集排名（并列不占位）
来源：http://bhy.birdmap.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zuw.tianlin.xyz

[Q57] 行号
来源：http://lnk.yj20258.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oac.shangyingyoupin.top

[Q58] 累计求和
来源：http://kuw.shanyushiyangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tcq.ppjwa.cn

[Q59] 分组内累计
来源：http://xmo.hammf.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://eph.tanke756.top

[Q60] 取上一行 / 下一行
来源：http://ynk.fengsongda.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lrt.andypj.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://veh.havefunace.top

[Q61] 移动平均
来源：http://jym.guowangkeji.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vhf.aibaodan.cn

[Q62] 分组占比
来源：http://ykq.hammf.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kwf.ybcxt.top

[Q63] 开启事务
来源：http://edz.jinqigufen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://kgk.cucudq.cn

[Q64] 提交事务
来源：http://ohg.ppjwa.cn

COMMIT;
来源：http://bra.bbcook.cn

[Q65] 回滚事务
来源：http://ixm.jlsjyb.cn

ROLLBACK;
来源：http://cve.daxiang520.top

[Q66] 行锁查询
来源：http://vcn.daria6918.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qjr.c1oappe.top

[Q67] 设置隔离级别
来源：http://kmv.ehwqpu.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nws.hnxiangtu.top

[Q68] 保存点
来源：http://nri.xziqi.cn

SAVEPOINT sp1;
来源：http://xfj.haohaochexian.top

ROLLBACK TO sp1;
来源：http://oah.tanke756.top

[Q69] 查看执行计划
来源：http://juf.9152youxi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uxo.tianlin.xyz

[Q70] 更新统计信息
来源：http://asq.vehdjk.com

ANALYZE TABLE users;
来源：http://tls.zhongyouzk.top

[Q71] 查看建表语句
来源：http://hgt.jianghu66.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xdd.smart0.xyz

[Q72] 查看索引
来源：http://wow.shanyushiyangkeji.top

SHOW INDEX FROM users;
来源：http://inp.guannengcc.top

[Q73] 查看表状态
来源：http://zpm.snrcjt.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dha.zdbjq.cn

[Q74] 强制使用索引
来源：http://ybe.jlsjyb.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wrh.yangfankeji.com

[Q75] 日期格式化
来源：http://wci.jlsjyb.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yln.zhixingplan.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zfz.ywan-chungtsiang.top

[Q76] 按天统计
来源：http://mql.9152youxi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://llw.tarul.cn

[Q77] 时间加减
来源：http://rax.ctjpmb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jcb.svipenyu.cn

[Q78] 当前时间
来源：http://ufs.shangyingyoupin.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kvc.xziqi.cn

[Q79] 字符串拼接
来源：http://rhn.jiagoushi.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pkr.9152youxi.cn

[Q80] 字符串截取
来源：http://oee.fengsongda.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qfu.sxryk.cn

[Q81] 字符串替换
来源：http://kxg.yj202588.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://htc.zhaomingkeji.xyz

[Q82] 字符长度与字节长度
来源：http://hfc.haohaochexian.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yao.yanxiufei.cn

[Q83] 大小写转换
来源：http://mrf.hysaishi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gze.yj20258.top


<!-- 参考信息 -->