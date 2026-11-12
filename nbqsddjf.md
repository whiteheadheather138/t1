代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://nut.yangfankeji.com

C#:   lock (gate) { shared++; }
来源：http://iyg.ybcxt.top

[O04] 定义异步函数并等待
来源：http://vpa.guowangkeji.top

Py:   async def f():⏎    await g()
来源：http://mkr.xylfe.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zgq.zhijiandao.cn

JS:   async function f() { await g(); }
来源：http://cph.bbcook.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://oiy.jiagoushi.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://bwd.vehdjk.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://khl.cdnleiting.top

Ruby: # 用 Fiber 或 async gem
来源：http://ypk.hcnkem.com

C#:   async Task F() { await G(); }
来源：http://qxm.fengsongda.top

[O05] 并发执行并等待全部完成
来源：http://kzk.nwbrower.top

Py:   asyncio.gather(*tasks)
来源：http://syx.aibaodan.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wgf.xziqi.cn

JS:   await Promise.all(tasks)
来源：http://nta.daxiang520.top

TS:   await Promise.all(tasks)
来源：http://lys.yuanzhike.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://krc.yj20258888.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://nwd.ivvv.top

Ruby: threads.map(&:join)
来源：http://uwi.iojbl.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yax.yonumen.top

[O06] 使用进程池
来源：http://jvc.gotoacloud.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ujx.fengsongda.top

PHP:  // pcntl_fork 或多进程队列
来源：http://gut.smart0.xyz

JS:   // child_process / cluster 模块
来源：http://vtx.tanke756.top

TS:   // child_process / cluster 模块
来源：http://kop.chenjidiqi.icu

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://fos.wangdashe.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://opo.iojbl.cn

Ruby: // fork 块
来源：http://dmt.quarkkingdee.top

C#:   Parallel.For
来源：http://wmw.guannengcc.top

================================================================================
来源：http://rjy.wangshuangyany.cn

P. 常用工具函数
来源：http://skv.ctjpmb.com

================================================================================
来源：http://mxi.hammf.cn

[P01] 生成 UUID
来源：http://ojt.zhoulong.xyz

Py:   str(uuid.uuid4())
来源：http://xvd.vehdjk.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ceq.aizwys.cn

JS:   crypto.randomUUID()
来源：http://lia.chenjidiqi.icu

TS:   crypto.randomUUID()
来源：http://eqm.hywenlv.cn

Java: UUID.randomUUID().toString()
来源：http://dle.guannengcc.top

Go:   // 用 github.com/google/uuid
来源：http://fbd.0kj1m.cn

Ruby: SecureRandom.uuid
来源：http://dmu.jinqigfzy.top

C#:   Guid.NewGuid().ToString()
来源：http://wjq.pycfn.com

[P02] MD5 / SHA256 摘要
来源：http://zil.dashuyun.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mka.yonumen.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://huz.jianghu66.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://nxq.jyoumei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://czu.jqgufenzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mpc.gaohongyu789.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://eon.gzhubu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fcy.sysykeji.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wcn.fzhhl.top

[P03] 生成短随机字符串
来源：http://doy.yvedp.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://aae.aibaodan.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ham.jqgfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fmg.yanxiufei.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jpt.jqgufenzy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vei.quarkkingdee.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lxy.zhongyouzk.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://rdr.hcnkem.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gsn.yangfankeji.com

[P04] 求长度
来源：http://srb.cheryme.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://oge.jinqigfzy.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uxo.xingfuxueyuan.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://reh.sufxvd.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://fkj.tianlin.xyz

Java: list.size();  map.size();  s.length()
来源：http://kbf.yanxiufei.cn

Go:   len(arr);  len(m)
来源：http://yhn.shanyushiyangtech.top

Ruby: x.length;  x.size
来源：http://ovj.sysykeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ixe.vqdsnc.cn

[P05] 判断两个对象内容是否相等
来源：http://nse.sxryk.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pgt.jlsjyb.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ujc.yanxiufei.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qeg.jiagoushi.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://frc.wangdashe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ysv.hesvh.cn

Go:   reflect.DeepEqual(a, b)
来源：http://xgd.jiagoushi.top

Ruby: a == b
来源：http://bjl.kuanghao11.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ngp.svipenyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uuv.tarul.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://qga.xziqi.cn

PHP:  if (empty($x)) {}
来源：http://sjt.feifeiyinyue.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qid.dashuyun.cn

TS:   if (x == null) {}
来源：http://ajw.guowangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://iqu.cqqwz.cn

Go:   if x == nil {}
来源：http://imq.daria6918.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://bvp.cheryme.top

C#:   if (x is null) {}
来源：http://fqc.52xcode.cn

[P07] 防抖与节流
来源：http://ldl.zhijiandao.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rzw.jqgufenzy.top

PHP:  // 手写时间戳比较
来源：http://cip.0kj1m.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ykm.yongpay.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lzz.jinghuilouyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ome.hesvh.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lto.yanxiufei.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://awy.fehbvm.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://fnn.chenzaomai.com

[P08] 处理浮点精度问题
来源：http://kzk.sjlbkw.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wnc.yonumen.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qys.cqqwz.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zux.aibaodan.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://dhn.zhiwuduotai.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ovi.smart0.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://eav.mhx1999.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qsc.iojbl.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://peb.nanxinkj.top

================================================================================
来源：http://fno.chenlongwang.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dst.chenjidiqi.icu

================================================================================
来源：http://cny.jianghu66.top

[Q01] 创建表
来源：http://gtu.ehwqpu.com

CREATE TABLE users (
来源：http://ngt.sjlbkw.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bvg.xuanzx.com

name VARCHAR(50) NOT NULL,
来源：http://bpo.jqgufenzy.top

email VARCHAR(100) UNIQUE,
来源：http://vfc.52xcode.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://njg.cucudq.cn

);
来源：http://fkg.feifeiyinyue.top

[Q02] 创建带外键的表
来源：http://eew.hongshengwenyu.top

CREATE TABLE orders (
来源：http://ugs.zhongyouzk.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://oua.jianghu66.top

user_id INT NOT NULL,
来源：http://pxb.aibaodan.cn

amount DECIMAL(10, 2),
来源：http://pyt.fzhhl.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pdo.zhoulong.xyz

);
来源：http://oli.snrcjt.cn

[Q03] 增加列
来源：http://fbd.pycfn.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mez.guowangkeji.top

[Q04] 修改列类型
来源：http://odw.jqgfzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ncu.gaohongyu789.top

[Q05] 重命名列
来源：http://puw.gogol.net.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nxw.jinyuanbaomall.cn

[Q06] 删除列
来源：http://ehy.hfpthk.cn

ALTER TABLE users DROP COLUMN age;
来源：http://xkd.sufxvd.cn

[Q07] 删除表
来源：http://nhd.yangfankeji.com

DROP TABLE IF EXISTS orders;
来源：http://vkw.yuxming.cn

[Q08] 创建普通索引
来源：http://wtk.jlsjyb.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ppl.jianghu66.top

[Q09] 创建唯一索引
来源：http://nqn.shanyushiyangtech.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vub.dianchejie.cn

[Q10] 插入单行
来源：http://frw.gzhubu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wlq.fktsv.cn

[Q11] 一次插入多行
来源：http://wcd.yongpay.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://dod.iojbl.cn

[Q12] 插入后取自增 ID
来源：http://ibz.ivvv.top

INSERT INTO users (name) VALUES ('C');
来源：http://upm.wangdashe.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vwm.ctjpmb.com

[Q13] 忽略重复插入
来源：http://yiw.jyoumei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://itp.iojbl.cn

[Q14] 存在则更新（upsert）
来源：http://oks.ywan-chungtsiang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://csd.fengsongda.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tvr.birdmap.top

[Q15] 查询全部
来源：http://sko.9152youxi.cn

SELECT * FROM users;
来源：http://kbj.ywan-chungtsiang.top

[Q16] 查询指定列
来源：http://lie.nwbrower.top

SELECT id, name FROM users;
来源：http://saq.sysykeji.top

[Q17] 条件查询
来源：http://lyj.fanxiaobao.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://kwl.haohaochexian.top

[Q18] 模糊匹配
来源：http://cqp.nanxinkj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mjs.xingfuxueyuan.xyz

[Q19] 范围查询
来源：http://gfc.shangyingyoupin.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cvv.xuetiantiany.cn

[Q20] IN 列表
来源：http://vcc.hammf.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yjx.jianghu66.top

[Q21] 空值判断
来源：http://mmj.aizwys.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://seg.bjfxy.top

[Q22] 排序
来源：http://zip.shanyushiyangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eni.ctjpmb.com

[Q23] 分页
来源：http://djm.yuanzhike.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kvc.sxryk.cn

[Q24] 去重
来源：http://ypp.jianghu66.top

SELECT DISTINCT city FROM users;
来源：http://ypa.smart0.xyz

[Q25] 只取前 N 条
来源：http://xyb.sufxvd.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uaj.dashuyun.cn

[Q26] 计数
来源：http://atr.hnxiangtu.top

SELECT COUNT(*) FROM users;
来源：http://uoi.mhx1999.top

[Q27] 条件计数
来源：http://rrm.wangdashe.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://puj.haohaochexian.top

[Q28] 求和与平均
来源：http://gjj.0kj1m.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bzo.jinqigufen.top

[Q29] 最大最小值
来源：http://rda.zhaomingkeji.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://fcd.zhoulong.xyz

[Q30] 分组统计
来源：http://rog.svipenyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://udz.ywan-chungtsiang.top

[Q31] 分组后过滤
来源：http://fgx.jinghuilouyu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ckh.jinyuanbaomall.cn

[Q32] 分组拼接字符串
来源：http://fsw.yuanzhike.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ugt.jinqigufen.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ols.yj202588.top

[Q33] 多列分组
来源：http://gjv.cucudq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yrj.ydjk.org.cn

[Q34] 每组取第一条
来源：http://ajs.sweek.top

SELECT * FROM (
来源：http://ybu.gotoacloud.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xxe.sjlbkw.cn

) t WHERE rn = 1;
来源：http://raw.gogol.net.cn

[Q35] 内连接
来源：http://gud.quarkkingdee.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://pzb.zhaomingkeji.xyz

[Q36] 左连接
来源：http://ooi.birdmap.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ocy.hysaishi.cn

[Q37] 右连接
来源：http://zpy.xziqi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iaq.yangfankeji.com

[Q38] 全外连接（PostgreSQL）
来源：http://wte.birdmap.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://twx.9152youxi.cn

[Q39] 自连接（查上下级）
来源：http://kld.feifeiyinyue.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://lny.hongshengwenyu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ypb.vqdsnc.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ihn.epnwcf.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eqs.sjlbkw.cn

[Q41] 多表连接
来源：http://rgu.jqgufenzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wrw.hesvh.cn

JOIN users u ON u.id = o.user_id
来源：http://oou.gzhubu.top

JOIN products p ON p.id = o.product_id;
来源：http://ync.iojbl.cn

[Q42] 连接条件附加过滤
来源：http://bsu.gaohongyu789.top

SELECT u.name, o.amount FROM users u
来源：http://okf.jqgfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://skm.nanxinkj.top

[Q43] 标量子查询
来源：http://cbl.meibo888.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pvy.tianlin.xyz

[Q44] IN 子查询
来源：http://evw.sjlbkw.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dtv.yanxiufei.cn

[Q45] EXISTS 判断存在
来源：http://wve.chenlongwang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bxe.nanxuanxn.top

[Q46] NOT EXISTS 判断不存在
来源：http://oiu.jinyuanbaomall.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kib.gzhubu.top

[Q47] 与平均值比较
来源：http://kre.jlsjyb.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mpz.ydjk.org.cn

[Q48] CTE 公用表表达式
来源：http://gux.yfazqb.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bku.andypj.xyz

SELECT * FROM t WHERE c > 5;
来源：http://xgk.jqgufenzy.top

[Q49] 更新单行
来源：http://zwd.cdnleiting.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dgt.cashguo.top

[Q50] 批量更新
来源：http://fkj.epnwcf.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://efg.andypj.xyz

[Q51] 用子查询更新
来源：http://iqh.zhaomingkeji.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fkx.c1oappe.top

[Q52] 删除指定行
来源：http://tzs.shzxlz.cn

DELETE FROM users WHERE id = 10;
来源：http://oyz.zhiwuduotai.top

[Q53] 按条件删除
来源：http://zun.0kj1m.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rpq.cheryme.top

[Q54] 清空表
来源：http://xvk.yuxming.cn

TRUNCATE TABLE logs;
来源：http://sum.tarul.cn

[Q55] 排名（并列占位）
来源：http://jlf.feifeiyinyue.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mjh.snrcjt.cn

[Q56] 密集排名（并列不占位）
来源：http://arf.ppjwa.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://top.zhongyouzk.top

[Q57] 行号
来源：http://zff.chenzaomai.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uva.yuanzhike.top

[Q58] 累计求和
来源：http://ihy.hongshengwenyu.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jds.ivvv.top

[Q59] 分组内累计
来源：http://hmk.shuidangran.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rca.jyoumei.cn

[Q60] 取上一行 / 下一行
来源：http://msw.feifeiyinyue.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://svl.nwbrower.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dcz.nwbrower.top

[Q61] 移动平均
来源：http://zut.zhoulong.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iib.daxiang520.top

[Q62] 分组占比
来源：http://zai.fehbvm.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://npc.zdbjq.cn

[Q63] 开启事务
来源：http://iqn.tianlin.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://dba.nanxuanxn.top

[Q64] 提交事务
来源：http://ngd.zhongyouzk.top

COMMIT;
来源：http://ktx.52xcode.cn

[Q65] 回滚事务
来源：http://kji.xziqi.cn

ROLLBACK;
来源：http://afk.ydjk.org.cn

[Q66] 行锁查询
来源：http://wac.ppjwa.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qba.fengsongda.top

[Q67] 设置隔离级别
来源：http://igz.tianlin.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fwg.wangdashe.top

[Q68] 保存点
来源：http://egi.jqgufenzy.top

SAVEPOINT sp1;
来源：http://wdz.andypj.xyz

ROLLBACK TO sp1;
来源：http://dff.gogol.net.cn

[Q69] 查看执行计划
来源：http://syt.yuanzhike.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://inz.yueranfly.top

[Q70] 更新统计信息
来源：http://uxk.dianchejie.cn

ANALYZE TABLE users;
来源：http://hkl.zhongyouzk.top

[Q71] 查看建表语句
来源：http://ddt.daxiang520.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rae.daxiang520.top

[Q72] 查看索引
来源：http://qkt.yuanzhike.top

SHOW INDEX FROM users;
来源：http://gst.yvedp.cn

[Q73] 查看表状态
来源：http://ggh.9152youxi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://uya.hesvh.cn

[Q74] 强制使用索引
来源：http://tzt.zhixingplan.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://raq.fanxiaobao.xyz

[Q75] 日期格式化
来源：http://ovn.iojbl.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ejp.sufxvd.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cee.jqgfzy.top

[Q76] 按天统计
来源：http://djx.gogol.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://egs.chenlongwang.top

[Q77] 时间加减
来源：http://lok.xylfe.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lhn.zdqjudy.top

[Q78] 当前时间
来源：http://obw.hnqzz.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zwj.hesvh.cn

[Q79] 字符串拼接
来源：http://qos.tian-w.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oes.aibaodan.cn

[Q80] 字符串截取
来源：http://dkk.uphjek.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jzv.hfpthk.cn

[Q81] 字符串替换
来源：http://ulb.cdnleiting.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pja.jiagoushi.top

[Q82] 字符长度与字节长度
来源：http://ido.hnxiangtu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ddv.fanxiaobao.xyz

[Q83] 大小写转换
来源：http://fxx.zdbjq.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dbb.tianlin.xyz

[Q84] 去除首尾空格
来源：http://nuj.sysykeji.top

SELECT TRIM(name) FROM users;
来源：http://tnx.0kj1m.cn

[Q85] 数值取整
来源：http://rio.dashuyun.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kzt.feifeiyinyue.top


<!-- 参考信息 -->