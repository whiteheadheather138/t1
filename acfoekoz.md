代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://nau.xingfuxueyuan.xyz

JS:   async function f() { await g(); }
来源：http://fns.cqqwz.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wgv.quarkkingdee.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://prc.yj20258888.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://djr.guowangkeji.top

Ruby: # 用 Fiber 或 async gem
来源：http://xih.zhaomingkeji.xyz

C#:   async Task F() { await G(); }
来源：http://wvm.hysaishi.cn

[O05] 并发执行并等待全部完成
来源：http://pbz.zhongyouzk.top

Py:   asyncio.gather(*tasks)
来源：http://kkd.nwbrower.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nlm.yonumen.top

JS:   await Promise.all(tasks)
来源：http://qmk.cucudq.cn

TS:   await Promise.all(tasks)
来源：http://bnv.hesvh.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wlr.c1oappe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://uqb.fktsv.cn

Ruby: threads.map(&:join)
来源：http://scz.ppjwa.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://aip.hnxiangtu.top

[O06] 使用进程池
来源：http://nyi.ydjk.org.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ril.feifeiyinyue.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nkv.cashguo.top

JS:   // child_process / cluster 模块
来源：http://ebr.fzhhl.top

TS:   // child_process / cluster 模块
来源：http://iol.iojbl.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tct.dianchejie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mvl.fanxiaobao.xyz

Ruby: // fork 块
来源：http://cxg.sufxvd.cn

C#:   Parallel.For
来源：http://nqw.hnxiangtu.top

================================================================================
来源：http://oxm.svipenyu.cn

P. 常用工具函数
来源：http://yoj.jlsjyb.cn

================================================================================
来源：http://dzv.sxryk.cn

[P01] 生成 UUID
来源：http://wfl.uphjek.com

Py:   str(uuid.uuid4())
来源：http://sjg.zhixingplan.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wxr.sufxvd.cn

JS:   crypto.randomUUID()
来源：http://yjv.chenzaomai.com

TS:   crypto.randomUUID()
来源：http://vrz.sjlbkw.cn

Java: UUID.randomUUID().toString()
来源：http://hvh.daxiang520.top

Go:   // 用 github.com/google/uuid
来源：http://mkj.hysaishi.cn

Ruby: SecureRandom.uuid
来源：http://bqz.cdnleiting.top

C#:   Guid.NewGuid().ToString()
来源：http://eob.uphjek.com

[P02] MD5 / SHA256 摘要
来源：http://ekr.ctjpmb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://zww.yvedp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://hcw.gzhubu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pcn.zhongyouzk.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fsy.ehwqpu.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zfo.yanxiufei.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bcs.yuanzhike.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://knb.9152youxi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://rlh.316326.xyz

[P03] 生成短随机字符串
来源：http://ott.xylfe.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://eyo.zhiwuduotai.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bhf.9152youxi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cob.bbcook.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xoh.52xcode.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nxr.yfazqb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ulp.cdnleiting.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://iyn.yanxiufei.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://out.gotoacloud.top

[P04] 求长度
来源：http://hqr.pengpengdd.cyou

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ffd.zhengqikj.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gym.0kj1m.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xle.yongpay.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://giv.fehbvm.com

Java: list.size();  map.size();  s.length()
来源：http://wya.sjlbkw.cn

Go:   len(arr);  len(m)
来源：http://hlj.gaohongyu789.top

Ruby: x.length;  x.size
来源：http://kxa.bbcook.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vrl.yvedp.cn

[P05] 判断两个对象内容是否相等
来源：http://onm.cucudq.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bjd.vehdjk.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wtp.chenjidiqi.icu

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://yqy.jiagoushi.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vis.mhx1999.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://puy.zhaomingkeji.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://bhs.fehbvm.com

Ruby: a == b
来源：http://mqw.sysykeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://yzn.zhijiandao.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jyh.epnwcf.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://amq.jianghu66.top

PHP:  if (empty($x)) {}
来源：http://xzl.ivvv.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ktb.shangyingyoupin.top

TS:   if (x == null) {}
来源：http://tnm.vqdsnc.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://wwl.vehdjk.com

Go:   if x == nil {}
来源：http://qgf.sjlbkw.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://oaw.yongpay.top

C#:   if (x is null) {}
来源：http://qet.yonumen.top

[P07] 防抖与节流
来源：http://qeo.jyoumei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wlf.hywenlv.cn

PHP:  // 手写时间戳比较
来源：http://vbu.sysykeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vqu.hesvh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gva.birdmap.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qtq.gzhubu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vvw.zycfv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://oid.feifeiyinyue.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ecs.yj202588.top

[P08] 处理浮点精度问题
来源：http://ftc.fanxiaobao.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kvj.jinqigfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qie.zhoulong.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wem.yj20258888.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vlj.kuanghao11.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://kqq.wangdashe.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://cby.chenzaomai.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://jzf.iojbl.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://gxi.shanyushiyangkeji.top

================================================================================
来源：http://mwl.yueranfly.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bky.guannengcc.top

================================================================================
来源：http://eny.yueranfly.top

[Q01] 创建表
来源：http://kgu.hcnkem.com

CREATE TABLE users (
来源：http://zmn.0kj1m.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://gvf.shuidangran.top

name VARCHAR(50) NOT NULL,
来源：http://kwj.chenjidiqi.icu

email VARCHAR(100) UNIQUE,
来源：http://roi.quarkkingdee.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yrv.yuanzhike.top

);
来源：http://ogo.gaohongyu789.top

[Q02] 创建带外键的表
来源：http://ewi.zdbjq.cn

CREATE TABLE orders (
来源：http://pds.zhongyouzk.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xrm.jinghuilouyu.cn

user_id INT NOT NULL,
来源：http://bdz.zhoulong.xyz

amount DECIMAL(10, 2),
来源：http://jvh.jqgfzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jvw.jianghu66.top

);
来源：http://pld.gaohongyu789.top

[Q03] 增加列
来源：http://ivo.ctjpmb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kun.vqdsnc.cn

[Q04] 修改列类型
来源：http://ibl.bbcook.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wrp.hfpthk.cn

[Q05] 重命名列
来源：http://ecf.sysykeji.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rns.epnwcf.com

[Q06] 删除列
来源：http://avy.cashguo.top

ALTER TABLE users DROP COLUMN age;
来源：http://rds.yuanzhike.top

[Q07] 删除表
来源：http://pue.ybcxt.top

DROP TABLE IF EXISTS orders;
来源：http://xrf.wangshuangyany.cn

[Q08] 创建普通索引
来源：http://lxr.tian-w.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zeg.jinghuilouyu.cn

[Q09] 创建唯一索引
来源：http://hem.zycfv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://csf.yueranfly.top

[Q10] 插入单行
来源：http://onx.gogol.net.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lhc.gaohongyu789.top

[Q11] 一次插入多行
来源：http://auy.guannengcc.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://arb.yonumen.top

[Q12] 插入后取自增 ID
来源：http://arr.jlsjyb.cn

INSERT INTO users (name) VALUES ('C');
来源：http://apu.0kj1m.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kmh.hfpthk.cn

[Q13] 忽略重复插入
来源：http://wvi.c1oappe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://xst.yanxiufei.cn

[Q14] 存在则更新（upsert）
来源：http://bde.chenlongwang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://yuo.cucudq.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://laz.hnqzz.top

[Q15] 查询全部
来源：http://gwo.yvedp.cn

SELECT * FROM users;
来源：http://vmb.sxryk.cn

[Q16] 查询指定列
来源：http://rpc.wangshuangyany.cn

SELECT id, name FROM users;
来源：http://whi.hcnkem.com

[Q17] 条件查询
来源：http://uwf.yj20258888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ggl.yvedp.cn

[Q18] 模糊匹配
来源：http://ktj.yongpay.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://amn.uphjek.com

[Q19] 范围查询
来源：http://ivm.fanxiaobao.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zjj.hnqzz.top

[Q20] IN 列表
来源：http://yim.gaohongyu789.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://hai.mhx1999.top

[Q21] 空值判断
来源：http://ceu.xylfe.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vby.bbcook.cn

[Q22] 排序
来源：http://lfs.gogol.net.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://upy.guannengcc.top

[Q23] 分页
来源：http://yne.jinyuanbaomall.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kup.zdqjudy.top

[Q24] 去重
来源：http://pgw.fanxiaobao.xyz

SELECT DISTINCT city FROM users;
来源：http://awg.tianlin.xyz

[Q25] 只取前 N 条
来源：http://sss.aizwys.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uwt.chenjidiqi.icu

[Q26] 计数
来源：http://mma.jyoumei.cn

SELECT COUNT(*) FROM users;
来源：http://anp.daria6918.cn

[Q27] 条件计数
来源：http://uzj.aibaodan.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oii.ybcxt.top

[Q28] 求和与平均
来源：http://feq.shuidangran.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xkk.dianchejie.cn

[Q29] 最大最小值
来源：http://bsz.meibo888.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ipl.zhijiandao.cn

[Q30] 分组统计
来源：http://vai.hongshengwenyu.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cfp.mhx1999.top

[Q31] 分组后过滤
来源：http://ecp.jianghu66.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rpl.daria6918.cn

[Q32] 分组拼接字符串
来源：http://xgc.yanxiufei.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lqc.daria6918.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://sdg.svipenyu.cn

[Q33] 多列分组
来源：http://cks.ydzc1.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ypp.cucudq.cn

[Q34] 每组取第一条
来源：http://aer.xinyue.icu

SELECT * FROM (
来源：http://cdy.ppjwa.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wxz.svipenyu.cn

) t WHERE rn = 1;
来源：http://yxc.meibo888.top

[Q35] 内连接
来源：http://omy.xuetiantiany.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wlk.andypj.xyz

[Q36] 左连接
来源：http://kgg.hammf.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dtg.sysykeji.top

[Q37] 右连接
来源：http://lbe.gogol.net.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ebj.dianchejie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mnp.yvedp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qxi.shzxlz.cn

[Q39] 自连接（查上下级）
来源：http://jid.jqgufenzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://cwh.gogol.net.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ate.quarkkingdee.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qpx.guowangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eqa.mhx1999.top

[Q41] 多表连接
来源：http://qmb.zdbjq.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://kkp.zdbjq.cn

JOIN users u ON u.id = o.user_id
来源：http://cgd.kuanghao11.cn

JOIN products p ON p.id = o.product_id;
来源：http://yfm.zhoulong.xyz

[Q42] 连接条件附加过滤
来源：http://nsg.redwolf501.top

SELECT u.name, o.amount FROM users u
来源：http://ttm.iojbl.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zfw.cdnleiting.top

[Q43] 标量子查询
来源：http://uyh.jyoumei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://oob.jinqigufen.top

[Q44] IN 子查询
来源：http://bck.ctjpmb.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bwk.andypj.xyz

[Q45] EXISTS 判断存在
来源：http://ygo.birdmap.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://agm.jinyuanbaomall.cn

[Q46] NOT EXISTS 判断不存在
来源：http://owc.chenlongwang.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hzn.sxryk.cn

[Q47] 与平均值比较
来源：http://swa.fzhhl.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dsx.jiagoushi.top

[Q48] CTE 公用表表达式
来源：http://sne.kuanghao11.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gqd.zhoulong.xyz

SELECT * FROM t WHERE c > 5;
来源：http://uvp.zhaomingkeji.xyz

[Q49] 更新单行
来源：http://iqz.kuanghao11.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ine.ehwqpu.com

[Q50] 批量更新
来源：http://hbe.feifeiyinyue.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pid.mhx1999.top

[Q51] 用子查询更新
来源：http://wlx.dashuyun.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vdc.shanyushiyangkeji.top

[Q52] 删除指定行
来源：http://fdp.shangyingyoupin.top

DELETE FROM users WHERE id = 10;
来源：http://mfy.sysykeji.top

[Q53] 按条件删除
来源：http://gmq.yvedp.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vcg.yj202588.top

[Q54] 清空表
来源：http://nak.ydjk.org.cn

TRUNCATE TABLE logs;
来源：http://hcc.aizwys.cn

[Q55] 排名（并列占位）
来源：http://fnz.guannengcc.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pup.shuidangran.top

[Q56] 密集排名（并列不占位）
来源：http://oym.yj20258888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iji.jiagoushi.top

[Q57] 行号
来源：http://yom.daria6918.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yxc.hammf.cn

[Q58] 累计求和
来源：http://spt.yuanzhike.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aev.yueranfly.top

[Q59] 分组内累计
来源：http://omz.ywan-chungtsiang.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rqh.guannengcc.top

[Q60] 取上一行 / 下一行
来源：http://gon.fengsongda.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kyy.fktsv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ngn.epnwcf.com

[Q61] 移动平均
来源：http://kpd.c1oappe.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xjv.yuanzhike.top

[Q62] 分组占比
来源：http://hpn.cqqwz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kqw.ydjk.org.cn

[Q63] 开启事务
来源：http://nkj.xuetiantiany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vmo.xuetiantiany.cn

[Q64] 提交事务
来源：http://igl.guannengcc.top

COMMIT;
来源：http://bxy.jinqigufen.top

[Q65] 回滚事务
来源：http://acu.ydjk.org.cn

ROLLBACK;
来源：http://plb.vqdsnc.cn

[Q66] 行锁查询
来源：http://yvc.hysaishi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ahc.cucudq.cn

[Q67] 设置隔离级别
来源：http://ffx.nanxuanxn.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yxy.svipenyu.cn

[Q68] 保存点
来源：http://cgf.ydjk.org.cn

SAVEPOINT sp1;
来源：http://ick.cqqwz.cn

ROLLBACK TO sp1;
来源：http://oey.xuanzx.com

[Q69] 查看执行计划
来源：http://ilw.guannengcc.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://liq.bbcook.cn

[Q70] 更新统计信息
来源：http://wvi.cqqwz.cn

ANALYZE TABLE users;
来源：http://zau.ywan-chungtsiang.top

[Q71] 查看建表语句
来源：http://mhp.jinqigufen.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jdj.jyoumei.cn

[Q72] 查看索引
来源：http://gcn.redwolf501.top

SHOW INDEX FROM users;
来源：http://atw.xuanzx.com

[Q73] 查看表状态
来源：http://zsa.bjfxy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://xci.gaohongyu789.top

[Q74] 强制使用索引
来源：http://zuq.jlsjyb.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kxx.hesvh.cn

[Q75] 日期格式化
来源：http://yuw.nwbrower.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://seb.zhijiandao.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tma.zhiwuduotai.top

[Q76] 按天统计
来源：http://qab.havefunace.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vmv.sjlbkw.cn

[Q77] 时间加减
来源：http://njk.daria6918.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gba.yanxiufei.cn

[Q78] 当前时间
来源：http://ugt.vqdsnc.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yyi.ydzc1.top

[Q79] 字符串拼接
来源：http://usx.nanxinkj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tnj.dianchejie.cn

[Q80] 字符串截取
来源：http://kog.guowangkeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vpl.hywenlv.cn

[Q81] 字符串替换
来源：http://mrn.ydjk.org.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://upv.yangfankeji.com

[Q82] 字符长度与字节长度
来源：http://hrm.daxiang520.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://num.havefunace.top

[Q83] 大小写转换
来源：http://aai.shangyingyoupin.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bra.gzhubu.top

[Q84] 去除首尾空格
来源：http://vvi.smart0.xyz

SELECT TRIM(name) FROM users;
来源：http://fij.yonumen.top

[Q85] 数值取整
来源：http://ast.vqdsnc.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gbv.ehwqpu.com

[Q86] 读取 JSON 字段
来源：http://kjb.jiagoushi.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xxu.ydjk.org.cn

[Q87] JSON 字段做条件
来源：http://xnl.pycfn.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://utk.haohaochexian.top


<!-- 参考信息 -->