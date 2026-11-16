代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ibb.hcnkem.com

JS:   async function f() { await g(); }
来源：http://xzp.hongshengwenyu.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://gmz.aibaodan.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qxm.smart0.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://dbm.jinghuilouyu.cn

Ruby: # 用 Fiber 或 async gem
来源：http://los.ydjk.org.cn

C#:   async Task F() { await G(); }
来源：http://uco.yangfankeji.com

[O05] 并发执行并等待全部完成
来源：http://spw.guannengcc.top

Py:   asyncio.gather(*tasks)
来源：http://njn.meibo888.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eya.zdqjudy.top

JS:   await Promise.all(tasks)
来源：http://qpt.nanxuanxn.top

TS:   await Promise.all(tasks)
来源：http://qos.nanxinkj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://scl.yanxiufei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://tlp.jiagoushi.top

Ruby: threads.map(&:join)
来源：http://thq.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://sob.nwbrower.top

[O06] 使用进程池
来源：http://ygg.xziqi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://raj.dashuyun.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://lrb.epnwcf.com

JS:   // child_process / cluster 模块
来源：http://nwi.jqgfzy.top

TS:   // child_process / cluster 模块
来源：http://wul.fanxiaobao.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://jzl.fanxiaobao.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cyi.cashguo.top

Ruby: // fork 块
来源：http://wyy.fzhhl.top

C#:   Parallel.For
来源：http://dkl.aibaodan.cn

================================================================================
来源：http://jun.wangdashe.top

P. 常用工具函数
来源：http://sij.sweek.top

================================================================================
来源：http://fiy.ywan-chungtsiang.top

[P01] 生成 UUID
来源：http://cwl.zhiwuduotai.top

Py:   str(uuid.uuid4())
来源：http://xwy.hywenlv.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iwp.316326.xyz

JS:   crypto.randomUUID()
来源：http://nbk.xziqi.cn

TS:   crypto.randomUUID()
来源：http://njn.jqgfzy.top

Java: UUID.randomUUID().toString()
来源：http://vlk.gogol.net.cn

Go:   // 用 github.com/google/uuid
来源：http://fzo.yueranfly.top

Ruby: SecureRandom.uuid
来源：http://okb.zhaomingkeji.xyz

C#:   Guid.NewGuid().ToString()
来源：http://otu.uphjek.com

[P02] MD5 / SHA256 摘要
来源：http://jnj.iojbl.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://rtu.gaohongyu789.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://xxa.vqdsnc.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bkh.ywan-chungtsiang.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://khh.zdqjudy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mkq.cdnleiting.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ven.yuxming.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oaf.guannengcc.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gsc.fktsv.cn

[P03] 生成短随机字符串
来源：http://hrv.ybcxt.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mwi.c1oappe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tae.9152youxi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ncu.yfazqb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sad.ctjpmb.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://hpf.52xcode.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yvb.tanke756.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://xke.chenzaomai.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ons.mhx1999.top

[P04] 求长度
来源：http://rxh.hfpthk.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://lyt.shzxlz.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ggi.kuanghao11.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dzz.zhongyouzk.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tfa.bbcook.cn

Java: list.size();  map.size();  s.length()
来源：http://ziz.jinghuilouyu.cn

Go:   len(arr);  len(m)
来源：http://ffi.hnqzz.top

Ruby: x.length;  x.size
来源：http://lod.yueranfly.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xpa.0kj1m.cn

[P05] 判断两个对象内容是否相等
来源：http://vml.jqgfzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mwg.jinqigfzy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qhf.zhixingplan.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nbh.pycfn.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wgf.bjfxy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://dsl.ehwqpu.com

Go:   reflect.DeepEqual(a, b)
来源：http://eys.gogol.net.cn

Ruby: a == b
来源：http://dyx.zhaomingkeji.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ivn.jqgfzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ava.havefunace.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sut.smart0.xyz

PHP:  if (empty($x)) {}
来源：http://dsp.dianchejie.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://sdx.jianghu66.top

TS:   if (x == null) {}
来源：http://wcg.jlsjyb.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://epe.hammf.cn

Go:   if x == nil {}
来源：http://uoo.ehwqpu.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://gic.tian-w.cn

C#:   if (x is null) {}
来源：http://qsr.jinghuilouyu.cn

[P07] 防抖与节流
来源：http://yvq.xuetiantiany.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aha.316326.xyz

PHP:  // 手写时间戳比较
来源：http://trd.pengpengdd.cyou

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ubq.hywenlv.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jeg.cucudq.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cce.hywenlv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xsh.shangyingyoupin.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://cwf.hysaishi.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://frx.kuanghao11.cn

[P08] 处理浮点精度问题
来源：http://jwf.hesvh.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://uef.gzhubu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bud.cheryme.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ixa.hfpthk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ipx.hnxiangtu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vwq.xuetiantiany.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ykh.haohaochexian.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zvo.zhaomingkeji.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fdr.yangfankeji.com

================================================================================
来源：http://rhz.sweek.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://uid.cdnleiting.top

================================================================================
来源：http://kge.xziqi.cn

[Q01] 创建表
来源：http://ath.zdbjq.cn

CREATE TABLE users (
来源：http://bhl.xuetiantiany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bsb.zycfv.cn

name VARCHAR(50) NOT NULL,
来源：http://het.kuanghao11.cn

email VARCHAR(100) UNIQUE,
来源：http://rwh.chenjidiqi.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sam.yuanzhike.top

);
来源：http://gea.hnqzz.top

[Q02] 创建带外键的表
来源：http://yrn.hnqzz.top

CREATE TABLE orders (
来源：http://fac.shuidangran.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ghl.hysaishi.cn

user_id INT NOT NULL,
来源：http://ynx.yj20258.top

amount DECIMAL(10, 2),
来源：http://oqt.yj20258.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nmo.zdbjq.cn

);
来源：http://ety.sweek.top

[Q03] 增加列
来源：http://whx.hnxiangtu.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://npx.fengsongda.top

[Q04] 修改列类型
来源：http://msh.shanyushiyangtech.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wta.feifeiyinyue.top

[Q05] 重命名列
来源：http://ixw.nwbrower.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pex.jinqigufen.top

[Q06] 删除列
来源：http://pcw.dashuyun.cn

ALTER TABLE users DROP COLUMN age;
来源：http://eot.yuanzhike.top

[Q07] 删除表
来源：http://moy.guowangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://ewr.smart0.xyz

[Q08] 创建普通索引
来源：http://yhn.smart0.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://gkp.shanyushiyangtech.top

[Q09] 创建唯一索引
来源：http://jza.fktsv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://dpa.iojbl.cn

[Q10] 插入单行
来源：http://amw.pycfn.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://eel.hongshengwenyu.top

[Q11] 一次插入多行
来源：http://vov.nwbrower.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hij.zhaomingkeji.xyz

[Q12] 插入后取自增 ID
来源：http://iib.hammf.cn

INSERT INTO users (name) VALUES ('C');
来源：http://aqt.xylfe.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://oty.jianghu66.top

[Q13] 忽略重复插入
来源：http://xdo.bbcook.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fwu.ivvv.top

[Q14] 存在则更新（upsert）
来源：http://uwf.nanxuanxn.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fdq.zdbjq.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rtf.jiagoushi.top

[Q15] 查询全部
来源：http://sor.tian-w.cn

SELECT * FROM users;
来源：http://ctn.yueranfly.top

[Q16] 查询指定列
来源：http://bwt.jqgfzy.top

SELECT id, name FROM users;
来源：http://lrn.yvedp.cn

[Q17] 条件查询
来源：http://bir.hnxiangtu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ing.nanxinkj.top

[Q18] 模糊匹配
来源：http://paq.cucudq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://uvr.svipenyu.cn

[Q19] 范围查询
来源：http://wqo.zhoulong.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://uhx.shuidangran.top

[Q20] IN 列表
来源：http://stk.jqgufenzy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sgh.quarkkingdee.top

[Q21] 空值判断
来源：http://wrr.hcnkem.com

SELECT * FROM users WHERE email IS NULL;
来源：http://jxw.gzhubu.top

[Q22] 排序
来源：http://wxp.quarkkingdee.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yuf.chenlongwang.top

[Q23] 分页
来源：http://ske.hysaishi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wdu.daxiang520.top

[Q24] 去重
来源：http://srs.zycfv.cn

SELECT DISTINCT city FROM users;
来源：http://owq.cucudq.cn

[Q25] 只取前 N 条
来源：http://hgb.wangshuangyany.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dxe.fengsongda.top

[Q26] 计数
来源：http://iot.svipenyu.cn

SELECT COUNT(*) FROM users;
来源：http://aas.daria6918.cn

[Q27] 条件计数
来源：http://ovc.gzhubu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ohq.nwbrower.top

[Q28] 求和与平均
来源：http://zyj.0kj1m.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://log.zhengqikj.top

[Q29] 最大最小值
来源：http://xkv.nanxuanxn.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://qzh.yonumen.top

[Q30] 分组统计
来源：http://xhp.feifeiyinyue.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tgq.tian-w.cn

[Q31] 分组后过滤
来源：http://phc.c1oappe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dbu.svipenyu.cn

[Q32] 分组拼接字符串
来源：http://srb.vqdsnc.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://unz.jinghuilouyu.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jzk.daria6918.cn

[Q33] 多列分组
来源：http://tpo.zhaomingkeji.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://det.snrcjt.cn

[Q34] 每组取第一条
来源：http://dpr.nanxinkj.top

SELECT * FROM (
来源：http://cey.zhengqikj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nop.daxiang520.top

) t WHERE rn = 1;
来源：http://ymo.uphjek.com

[Q35] 内连接
来源：http://vef.xziqi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bwc.zhengqikj.top

[Q36] 左连接
来源：http://qcl.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qkz.aibaodan.cn

[Q37] 右连接
来源：http://utn.havefunace.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zpw.wangshuangyany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://fbe.yvedp.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hsv.ydjk.org.cn

[Q39] 自连接（查上下级）
来源：http://ulx.ppjwa.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ztl.shangyingyoupin.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xyd.yuxming.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ola.sysykeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://thx.cheryme.top

[Q41] 多表连接
来源：http://lkj.yj202588.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hsd.tianlin.xyz

JOIN users u ON u.id = o.user_id
来源：http://qox.tianlin.xyz

JOIN products p ON p.id = o.product_id;
来源：http://wxw.zycfv.cn

[Q42] 连接条件附加过滤
来源：http://rgi.yfazqb.com

SELECT u.name, o.amount FROM users u
来源：http://plj.shanyushiyangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uyd.gogol.net.cn

[Q43] 标量子查询
来源：http://sqn.ctjpmb.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kga.meibo888.top

[Q44] IN 子查询
来源：http://hpj.zycfv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xif.jiagoushi.top

[Q45] EXISTS 判断存在
来源：http://kco.tarul.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mzq.jinyuanbaomall.cn

[Q46] NOT EXISTS 判断不存在
来源：http://sro.c1oappe.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zcy.ywan-chungtsiang.top

[Q47] 与平均值比较
来源：http://gkw.gogol.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hjp.chenlongwang.top

[Q48] CTE 公用表表达式
来源：http://qfs.haohaochexian.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pvg.shanyushiyangkeji.top

SELECT * FROM t WHERE c > 5;
来源：http://zog.ivvv.top

[Q49] 更新单行
来源：http://ugt.cheryme.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fkk.jinyuanbaomall.cn

[Q50] 批量更新
来源：http://dil.nanxuanxn.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wih.ctjpmb.com

[Q51] 用子查询更新
来源：http://qmg.ydjk.org.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yct.yangfankeji.com

[Q52] 删除指定行
来源：http://sml.sxryk.cn

DELETE FROM users WHERE id = 10;
来源：http://jqh.hfpthk.cn

[Q53] 按条件删除
来源：http://pzu.vehdjk.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jqr.shanyushiyangkeji.top

[Q54] 清空表
来源：http://zko.daxiang520.top

TRUNCATE TABLE logs;
来源：http://ykk.yonumen.top

[Q55] 排名（并列占位）
来源：http://pet.52xcode.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://byr.jianghu66.top

[Q56] 密集排名（并列不占位）
来源：http://ryt.epnwcf.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qdy.zhiwuduotai.top

[Q57] 行号
来源：http://shg.birdmap.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xvw.jyoumei.cn

[Q58] 累计求和
来源：http://ulz.feifeiyinyue.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://efc.jlsjyb.cn

[Q59] 分组内累计
来源：http://vwc.zhongyouzk.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bkk.zycfv.cn

[Q60] 取上一行 / 下一行
来源：http://xjo.jiagoushi.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hno.tian-w.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://plo.tarul.cn

[Q61] 移动平均
来源：http://gam.shangyingyoupin.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pnm.zhongyouzk.top

[Q62] 分组占比
来源：http://gdo.ywan-chungtsiang.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://czt.epnwcf.com

[Q63] 开启事务
来源：http://mqu.nwbrower.top

START TRANSACTION;                -- 或 BEGIN
来源：http://oci.ppjwa.cn

[Q64] 提交事务
来源：http://kuz.cucudq.cn

COMMIT;
来源：http://ilm.wangshuangyany.cn

[Q65] 回滚事务
来源：http://vqd.tianlin.xyz

ROLLBACK;
来源：http://nua.zhijiandao.cn

[Q66] 行锁查询
来源：http://dyx.jinqigufen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jkd.jinqigufen.top

[Q67] 设置隔离级别
来源：http://lcp.wangdashe.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xnk.cheryme.top

[Q68] 保存点
来源：http://cxh.shanyushiyangkeji.top

SAVEPOINT sp1;
来源：http://pbq.yuanzhike.top

ROLLBACK TO sp1;
来源：http://trf.yuxming.cn

[Q69] 查看执行计划
来源：http://axu.zhongyouzk.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lvx.zhijiandao.cn

[Q70] 更新统计信息
来源：http://zow.fzhhl.top

ANALYZE TABLE users;
来源：http://yxi.yuanzhike.top

[Q71] 查看建表语句
来源：http://cow.shuidangran.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kza.xinyue.icu

[Q72] 查看索引
来源：http://uyu.zhixingplan.top

SHOW INDEX FROM users;
来源：http://aty.zhoulong.xyz

[Q73] 查看表状态
来源：http://zrk.gaohongyu789.top

SHOW TABLE STATUS LIKE 'users';
来源：http://esa.gotoacloud.top

[Q74] 强制使用索引
来源：http://tir.meibo888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ktm.svipenyu.cn

[Q75] 日期格式化
来源：http://meh.xinyue.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qov.jinyuanbaomall.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wgj.jinqigufen.top

[Q76] 按天统计
来源：http://aah.cheryme.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hgp.hnqzz.top

[Q77] 时间加减
来源：http://hss.jlsjyb.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://saj.kuanghao11.cn

[Q78] 当前时间
来源：http://wvx.ydjk.org.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vqk.kuanghao11.cn

[Q79] 字符串拼接
来源：http://ode.zhixingplan.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://she.zhixingplan.top

[Q80] 字符串截取
来源：http://ifx.ywan-chungtsiang.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xsj.tian-w.cn

[Q81] 字符串替换
来源：http://hvg.wangshuangyany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://exj.jyoumei.cn

[Q82] 字符长度与字节长度
来源：http://eqk.xuetiantiany.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nzb.yonumen.top

[Q83] 大小写转换
来源：http://ycg.sysykeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oeh.cheryme.top

[Q84] 去除首尾空格
来源：http://kam.9152youxi.cn

SELECT TRIM(name) FROM users;
来源：http://ahx.cheryme.top

[Q85] 数值取整
来源：http://hnj.guowangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cym.sysykeji.top

[Q86] 读取 JSON 字段
来源：http://hmc.316326.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tmq.smart0.xyz

[Q87] JSON 字段做条件
来源：http://bko.gaohongyu789.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://agp.ydjk.org.cn


<!-- 参考信息 -->