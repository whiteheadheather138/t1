代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hdu.ywan-chungtsiang.top

[O03] 加锁保护共享数据
来源：http://zrl.redwolf501.top

Py:   with lock: shared += 1
来源：http://ker.yvedp.cn

PHP:  // 用 flock() 做文件锁
来源：http://qzm.fzhhl.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gms.pycfn.com

TS:   // 同 JS
来源：http://mof.c1oappe.top

Java: synchronized (this) { shared++; }
来源：http://sdy.cucudq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://xxu.yangfankeji.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://ifh.iojbl.cn

C#:   lock (gate) { shared++; }
来源：http://ats.tian-w.cn

[O04] 定义异步函数并等待
来源：http://pjj.aizwys.cn

Py:   async def f():⏎    await g()
来源：http://ptm.hcnkem.com

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://fvz.xziqi.cn

JS:   async function f() { await g(); }
来源：http://ogf.hammf.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wyk.havefunace.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fnk.nwbrower.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://aos.hfpthk.cn

Ruby: # 用 Fiber 或 async gem
来源：http://lty.jianghu66.top

C#:   async Task F() { await G(); }
来源：http://coe.52xcode.cn

[O05] 并发执行并等待全部完成
来源：http://vsn.ctjpmb.com

Py:   asyncio.gather(*tasks)
来源：http://kcn.hysaishi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://way.fzhhl.top

JS:   await Promise.all(tasks)
来源：http://fyq.fzhhl.top

TS:   await Promise.all(tasks)
来源：http://ucd.jinghuilouyu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zrb.yuxming.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pdm.yj20258.top

Ruby: threads.map(&:join)
来源：http://vyg.jinqigfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://oiu.uphjek.com

[O06] 使用进程池
来源：http://mgu.jinyuanbaomall.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://bnb.iojbl.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ucu.shuidangran.top

JS:   // child_process / cluster 模块
来源：http://kjg.svipenyu.cn

TS:   // child_process / cluster 模块
来源：http://awz.ywan-chungtsiang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vxq.jyoumei.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://goh.havefunace.top

Ruby: // fork 块
来源：http://xed.vqdsnc.cn

C#:   Parallel.For
来源：http://gsd.jinyuanbaomall.cn

================================================================================
来源：http://dpc.yuanzhike.top

P. 常用工具函数
来源：http://vkq.0kj1m.cn

================================================================================
来源：http://pwv.xylfe.cn

[P01] 生成 UUID
来源：http://wrm.xuanzx.com

Py:   str(uuid.uuid4())
来源：http://qqw.yonumen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://cwb.hesvh.cn

JS:   crypto.randomUUID()
来源：http://zcl.shanyushiyangkeji.top

TS:   crypto.randomUUID()
来源：http://lbu.0kj1m.cn

Java: UUID.randomUUID().toString()
来源：http://jvj.ehwqpu.com

Go:   // 用 github.com/google/uuid
来源：http://zcj.zhengqikj.top

Ruby: SecureRandom.uuid
来源：http://ujo.c1oappe.top

C#:   Guid.NewGuid().ToString()
来源：http://voi.316326.xyz

[P02] MD5 / SHA256 摘要
来源：http://gvi.hesvh.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yva.jqgfzy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ndr.yanxiufei.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rbo.fanxiaobao.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bsq.bjfxy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qdh.bbcook.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://qme.nanxinkj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cmd.vqdsnc.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://bpd.xuetiantiany.cn

[P03] 生成短随机字符串
来源：http://upn.yj202588.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ast.zdqjudy.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fic.dianchejie.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mvh.xziqi.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rki.pengpengdd.cyou

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://icy.ivvv.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ikv.ybcxt.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rvr.shanyushiyangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bud.svipenyu.cn

[P04] 求长度
来源：http://wvx.meibo888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yxh.andypj.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pdw.fengsongda.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eek.birdmap.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ytd.hammf.cn

Java: list.size();  map.size();  s.length()
来源：http://kec.yangfankeji.com

Go:   len(arr);  len(m)
来源：http://rvi.hongshengwenyu.top

Ruby: x.length;  x.size
来源：http://jxi.ydzc1.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://avk.smart0.xyz

[P05] 判断两个对象内容是否相等
来源：http://mwn.zycfv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://kru.zhiwuduotai.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xha.hnxiangtu.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://klg.hammf.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uoy.zhongyouzk.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://sfr.feifeiyinyue.top

Go:   reflect.DeepEqual(a, b)
来源：http://frt.tarul.cn

Ruby: a == b
来源：http://gvu.ppjwa.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gye.snrcjt.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://lyt.ydjk.org.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mra.havefunace.top

PHP:  if (empty($x)) {}
来源：http://qzq.sysykeji.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://joy.mhx1999.top

TS:   if (x == null) {}
来源：http://zco.fktsv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://fnj.smart0.xyz

Go:   if x == nil {}
来源：http://bpy.hongshengwenyu.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wmo.hnxiangtu.top

C#:   if (x is null) {}
来源：http://gez.aizwys.cn

[P07] 防抖与节流
来源：http://jfp.mhx1999.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wge.jyoumei.cn

PHP:  // 手写时间戳比较
来源：http://udn.ehwqpu.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kzv.ehwqpu.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gbq.chenjidiqi.icu

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wfs.daxiang520.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rxc.jianghu66.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://gjh.vehdjk.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://qnz.hesvh.cn

[P08] 处理浮点精度问题
来源：http://ooo.jinghuilouyu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nwa.yj20258.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://gtk.ydjk.org.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fje.tian-w.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mle.smart0.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jmv.xylfe.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://zmg.hongshengwenyu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mou.jinqigufen.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jui.iojbl.cn

================================================================================
来源：http://fcv.daxiang520.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fef.gotoacloud.top

================================================================================
来源：http://vsf.shzxlz.cn

[Q01] 创建表
来源：http://qjk.jianghu66.top

CREATE TABLE users (
来源：http://ulz.0kj1m.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tjr.cqqwz.cn

name VARCHAR(50) NOT NULL,
来源：http://xau.yueranfly.top

email VARCHAR(100) UNIQUE,
来源：http://cyx.iojbl.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gft.tarul.cn

);
来源：http://aeg.vqdsnc.cn

[Q02] 创建带外键的表
来源：http://qan.shangyingyoupin.top

CREATE TABLE orders (
来源：http://luy.yj20258888.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://pkd.dianchejie.cn

user_id INT NOT NULL,
来源：http://gde.fktsv.cn

amount DECIMAL(10, 2),
来源：http://mxm.bjfxy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ikv.aizwys.cn

);
来源：http://adx.hysaishi.cn

[Q03] 增加列
来源：http://ava.yj20258888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hwl.tarul.cn

[Q04] 修改列类型
来源：http://egl.meibo888.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hku.mhx1999.top

[Q05] 重命名列
来源：http://mzd.pengpengdd.cyou

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://iks.shangyingyoupin.top

[Q06] 删除列
来源：http://aqo.meibo888.top

ALTER TABLE users DROP COLUMN age;
来源：http://xzf.jinqigfzy.top

[Q07] 删除表
来源：http://dgm.sufxvd.cn

DROP TABLE IF EXISTS orders;
来源：http://ocx.hongshengwenyu.top

[Q08] 创建普通索引
来源：http://pmw.birdmap.top

CREATE INDEX idx_users_email ON users(email);
来源：http://bow.yuanzhike.top

[Q09] 创建唯一索引
来源：http://cmn.tianlin.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cyb.jinqigfzy.top

[Q10] 插入单行
来源：http://jfh.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://asq.yuxming.cn

[Q11] 一次插入多行
来源：http://oyq.ybcxt.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://bxd.316326.xyz

[Q12] 插入后取自增 ID
来源：http://rqn.sysykeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://fcb.zhaomingkeji.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mxs.fzhhl.top

[Q13] 忽略重复插入
来源：http://pmq.dashuyun.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://box.shzxlz.cn

[Q14] 存在则更新（upsert）
来源：http://jej.gaohongyu789.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qlm.yuanzhike.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fiv.smart0.xyz

[Q15] 查询全部
来源：http://miw.smart0.xyz

SELECT * FROM users;
来源：http://pjg.svipenyu.cn

[Q16] 查询指定列
来源：http://ezj.yvedp.cn

SELECT id, name FROM users;
来源：http://aiu.chenjidiqi.icu

[Q17] 条件查询
来源：http://huc.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gut.hammf.cn

[Q18] 模糊匹配
来源：http://oha.aibaodan.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://amt.uphjek.com

[Q19] 范围查询
来源：http://teo.yj20258.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://dni.epnwcf.com

[Q20] IN 列表
来源：http://awv.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://iij.zycfv.cn

[Q21] 空值判断
来源：http://efr.aibaodan.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://hzm.svipenyu.cn

[Q22] 排序
来源：http://exl.gotoacloud.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://toe.xylfe.cn

[Q23] 分页
来源：http://ybm.xylfe.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tbk.zhongyouzk.top

[Q24] 去重
来源：http://uxq.ybcxt.top

SELECT DISTINCT city FROM users;
来源：http://wkl.jqgfzy.top

[Q25] 只取前 N 条
来源：http://kcz.vehdjk.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vzf.yj20258888.top

[Q26] 计数
来源：http://grn.gotoacloud.top

SELECT COUNT(*) FROM users;
来源：http://nxf.yj20258.top

[Q27] 条件计数
来源：http://opw.jyoumei.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jrs.xziqi.cn

[Q28] 求和与平均
来源：http://ubi.birdmap.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jrh.guannengcc.top

[Q29] 最大最小值
来源：http://zgc.daria6918.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mmo.ctjpmb.com

[Q30] 分组统计
来源：http://ncq.ydzc1.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lql.vehdjk.com

[Q31] 分组后过滤
来源：http://iey.ydzc1.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ztr.chenzaomai.com

[Q32] 分组拼接字符串
来源：http://bai.tarul.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kcu.hnqzz.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ltz.yueranfly.top

[Q33] 多列分组
来源：http://mza.ivvv.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wjm.hongshengwenyu.top

[Q34] 每组取第一条
来源：http://eum.nanxuanxn.top

SELECT * FROM (
来源：http://hxq.haohaochexian.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dys.jlsjyb.cn

) t WHERE rn = 1;
来源：http://pzf.yanxiufei.cn

[Q35] 内连接
来源：http://dxd.yfazqb.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fip.ydjk.org.cn

[Q36] 左连接
来源：http://frz.sxryk.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mzj.hnqzz.top

[Q37] 右连接
来源：http://qps.hnqzz.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ije.cdnleiting.top

[Q38] 全外连接（PostgreSQL）
来源：http://wjs.fktsv.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ddt.cqqwz.cn

[Q39] 自连接（查上下级）
来源：http://bdg.sufxvd.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://tcn.ydjk.org.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yef.daxiang520.top

[Q40] 交叉连接（笛卡尔积）
来源：http://dqd.dianchejie.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uoo.fanxiaobao.xyz

[Q41] 多表连接
来源：http://ynt.shanyushiyangtech.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://twl.birdmap.top

JOIN users u ON u.id = o.user_id
来源：http://ofh.uphjek.com

JOIN products p ON p.id = o.product_id;
来源：http://mcd.quarkkingdee.top

[Q42] 连接条件附加过滤
来源：http://ygx.52xcode.cn

SELECT u.name, o.amount FROM users u
来源：http://ryp.cheryme.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tiw.quarkkingdee.top

[Q43] 标量子查询
来源：http://szz.jqgfzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nfs.hesvh.cn

[Q44] IN 子查询
来源：http://jgx.aibaodan.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bcp.zdbjq.cn

[Q45] EXISTS 判断存在
来源：http://rla.chenlongwang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xrh.zhaomingkeji.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://gzr.yj20258888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iti.fanxiaobao.xyz

[Q47] 与平均值比较
来源：http://gon.xuanzx.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ujn.xylfe.cn

[Q48] CTE 公用表表达式
来源：http://vik.shuidangran.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wvl.tanke756.top

SELECT * FROM t WHERE c > 5;
来源：http://yqg.yangfankeji.com

[Q49] 更新单行
来源：http://dar.sxryk.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wop.zhongyouzk.top

[Q50] 批量更新
来源：http://cuf.hywenlv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mxs.sysykeji.top

[Q51] 用子查询更新
来源：http://zuq.ivvv.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jup.sxryk.cn

[Q52] 删除指定行
来源：http://nsn.jyoumei.cn

DELETE FROM users WHERE id = 10;
来源：http://toz.fehbvm.com

[Q53] 按条件删除
来源：http://qtd.xylfe.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tku.aibaodan.cn

[Q54] 清空表
来源：http://ckf.yuanzhike.top

TRUNCATE TABLE logs;
来源：http://rsm.nanxuanxn.top

[Q55] 排名（并列占位）
来源：http://zyh.c1oappe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yee.zdbjq.cn

[Q56] 密集排名（并列不占位）
来源：http://khc.snrcjt.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rci.xziqi.cn

[Q57] 行号
来源：http://tac.cdnleiting.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lgl.sufxvd.cn

[Q58] 累计求和
来源：http://ujt.fehbvm.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nix.9152youxi.cn

[Q59] 分组内累计
来源：http://tbk.zhiwuduotai.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lbo.0kj1m.cn

[Q60] 取上一行 / 下一行
来源：http://wgb.daxiang520.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oue.nanxinkj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dnr.jinyuanbaomall.cn

[Q61] 移动平均
来源：http://ity.hesvh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tjx.hammf.cn

[Q62] 分组占比
来源：http://yfl.jinqigufen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qrb.cdnleiting.top

[Q63] 开启事务
来源：http://ujj.jiagoushi.top

START TRANSACTION;                -- 或 BEGIN
来源：http://woo.sweek.top

[Q64] 提交事务
来源：http://dwc.ydjk.org.cn

COMMIT;
来源：http://hab.nanxuanxn.top

[Q65] 回滚事务
来源：http://xbm.shuidangran.top

ROLLBACK;
来源：http://fay.chenjidiqi.icu

[Q66] 行锁查询
来源：http://gyk.andypj.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tcl.fzhhl.top

[Q67] 设置隔离级别
来源：http://cyp.xylfe.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://scv.zdbjq.cn

[Q68] 保存点
来源：http://wtr.pengpengdd.cyou

SAVEPOINT sp1;
来源：http://mzq.yanxiufei.cn

ROLLBACK TO sp1;
来源：http://two.fzhhl.top

[Q69] 查看执行计划
来源：http://tht.jiagoushi.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mzy.guowangkeji.top

[Q70] 更新统计信息
来源：http://igb.fktsv.cn

ANALYZE TABLE users;
来源：http://htn.jianghu66.top

[Q71] 查看建表语句
来源：http://rmf.yj20258.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zlq.zdqjudy.top

[Q72] 查看索引
来源：http://zwr.ydzc1.top

SHOW INDEX FROM users;
来源：http://nix.yuanzhike.top

[Q73] 查看表状态
来源：http://oub.xziqi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hig.birdmap.top

[Q74] 强制使用索引
来源：http://sda.xinyue.icu

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hjt.birdmap.top

[Q75] 日期格式化
来源：http://tjq.yueranfly.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xdf.gzhubu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://drj.zhiwuduotai.top

[Q76] 按天统计
来源：http://wzh.tarul.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tdn.yongpay.top

[Q77] 时间加减
来源：http://xjg.jianghu66.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gxf.ybcxt.top

[Q78] 当前时间
来源：http://wvi.zhoulong.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vdq.jianghu66.top

[Q79] 字符串拼接
来源：http://gcb.fehbvm.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ldo.xingfuxueyuan.xyz

[Q80] 字符串截取
来源：http://ycc.quarkkingdee.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mck.yfazqb.com

[Q81] 字符串替换
来源：http://exa.xylfe.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ljm.bjfxy.top


<!-- 参考信息 -->