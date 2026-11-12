代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://deo.daxiang520.top

JS:   async function f() { await g(); }
来源：http://mia.jiagoushi.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://vqj.sweek.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fkf.cheryme.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gsg.fanxiaobao.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://ohh.tian-w.cn

C#:   async Task F() { await G(); }
来源：http://qup.pycfn.com

[O05] 并发执行并等待全部完成
来源：http://ano.hfpthk.cn

Py:   asyncio.gather(*tasks)
来源：http://pcv.dianchejie.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uht.jqgufenzy.top

JS:   await Promise.all(tasks)
来源：http://rns.jiagoushi.top

TS:   await Promise.all(tasks)
来源：http://tlu.nanxinkj.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://icp.aizwys.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://lhz.pycfn.com

Ruby: threads.map(&:join)
来源：http://iyb.bbcook.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://lcc.cheryme.top

[O06] 使用进程池
来源：http://gxh.hcnkem.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://lqg.andypj.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://zys.jqgufenzy.top

JS:   // child_process / cluster 模块
来源：http://ecd.feifeiyinyue.top

TS:   // child_process / cluster 模块
来源：http://uuh.pycfn.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tah.jlsjyb.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ckn.tarul.cn

Ruby: // fork 块
来源：http://xrz.svipenyu.cn

C#:   Parallel.For
来源：http://ptl.yuanzhike.top

================================================================================
来源：http://iwn.svipenyu.cn

P. 常用工具函数
来源：http://gtm.jianghu66.top

================================================================================
来源：http://zfa.jqgufenzy.top

[P01] 生成 UUID
来源：http://mbk.jqgufenzy.top

Py:   str(uuid.uuid4())
来源：http://pxm.yueranfly.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ysn.hfpthk.cn

JS:   crypto.randomUUID()
来源：http://sxz.0kj1m.cn

TS:   crypto.randomUUID()
来源：http://bkx.ppjwa.cn

Java: UUID.randomUUID().toString()
来源：http://yof.yueranfly.top

Go:   // 用 github.com/google/uuid
来源：http://rkg.cucudq.cn

Ruby: SecureRandom.uuid
来源：http://bgz.yanxiufei.cn

C#:   Guid.NewGuid().ToString()
来源：http://ktu.feifeiyinyue.top

[P02] MD5 / SHA256 摘要
来源：http://tas.hfpthk.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mla.chenjidiqi.icu

PHP:  hash("sha256", $s);  md5($s);
来源：http://iwh.wangshuangyany.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://rpv.yuanzhike.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pxq.pycfn.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://grt.pycfn.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://dar.nanxinkj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zfd.zhoulong.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cxr.ydjk.org.cn

[P03] 生成短随机字符串
来源：http://voc.zhixingplan.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://bdh.daria6918.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oql.fzhhl.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xwv.havefunace.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nvh.9152youxi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nyn.jianghu66.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://qvi.yuxming.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://jfl.yuxming.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://jfl.nanxinkj.top

[P04] 求长度
来源：http://pnp.cdnleiting.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nbh.shanyushiyangkeji.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sld.zhoulong.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ukx.yangfankeji.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pqe.jlsjyb.cn

Java: list.size();  map.size();  s.length()
来源：http://lrd.jiagoushi.top

Go:   len(arr);  len(m)
来源：http://khx.sweek.top

Ruby: x.length;  x.size
来源：http://lzj.hnqzz.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://dqt.jyoumei.cn

[P05] 判断两个对象内容是否相等
来源：http://tdl.sjlbkw.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wuv.gzhubu.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://kru.yueranfly.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://veo.shuidangran.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fkk.sysykeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://jhm.zhiwuduotai.top

Go:   reflect.DeepEqual(a, b)
来源：http://adh.ehwqpu.com

Ruby: a == b
来源：http://xhe.svipenyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://dql.jiagoushi.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://aqx.vehdjk.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wyh.hongshengwenyu.top

PHP:  if (empty($x)) {}
来源：http://hhu.meibo888.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://ewi.shanyushiyangtech.top

TS:   if (x == null) {}
来源：http://bkd.hongshengwenyu.top

Java: if (x == null || x.isEmpty()) {}
来源：http://xsr.pycfn.com

Go:   if x == nil {}
来源：http://mbi.sxryk.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ypu.xingfuxueyuan.xyz

C#:   if (x is null) {}
来源：http://cti.wangdashe.top

[P07] 防抖与节流
来源：http://xsv.fengsongda.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xoc.fehbvm.com

PHP:  // 手写时间戳比较
来源：http://uif.tanke756.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tkf.birdmap.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tfz.sufxvd.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vmj.yfazqb.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://hgp.dashuyun.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://gse.uphjek.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://voo.chenjidiqi.icu

[P08] 处理浮点精度问题
来源：http://fzy.c1oappe.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ibv.ppjwa.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://qdr.xinyue.icu

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qwb.shzxlz.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://snq.yonumen.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sqo.vqdsnc.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qfa.yanxiufei.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://hso.jqgfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kne.daxiang520.top

================================================================================
来源：http://hvs.hcnkem.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://omo.redwolf501.top

================================================================================
来源：http://plm.ivvv.top

[Q01] 创建表
来源：http://hnc.hongshengwenyu.top

CREATE TABLE users (
来源：http://tsg.andypj.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://pwk.chenlongwang.top

name VARCHAR(50) NOT NULL,
来源：http://lrf.chenjidiqi.icu

email VARCHAR(100) UNIQUE,
来源：http://fvt.xinyue.icu

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://sao.dianchejie.cn

);
来源：http://ykz.sufxvd.cn

[Q02] 创建带外键的表
来源：http://udo.hammf.cn

CREATE TABLE orders (
来源：http://nyb.meibo888.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rit.shangyingyoupin.top

user_id INT NOT NULL,
来源：http://fsm.tanke756.top

amount DECIMAL(10, 2),
来源：http://smk.mhx1999.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pfl.aizwys.cn

);
来源：http://wdv.c1oappe.top

[Q03] 增加列
来源：http://lii.nanxinkj.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://xap.hywenlv.cn

[Q04] 修改列类型
来源：http://wbn.cdnleiting.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bpn.feifeiyinyue.top

[Q05] 重命名列
来源：http://nah.meibo888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mws.epnwcf.com

[Q06] 删除列
来源：http://quo.52xcode.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vct.yueranfly.top

[Q07] 删除表
来源：http://fge.yj20258888.top

DROP TABLE IF EXISTS orders;
来源：http://nit.yfazqb.com

[Q08] 创建普通索引
来源：http://yqu.ydjk.org.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zsr.shanyushiyangtech.top

[Q09] 创建唯一索引
来源：http://vct.cdnleiting.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://upy.ydzc1.top

[Q10] 插入单行
来源：http://ssz.iojbl.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://sdw.shanyushiyangkeji.top

[Q11] 一次插入多行
来源：http://hgp.yvedp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hqr.shuidangran.top

[Q12] 插入后取自增 ID
来源：http://wlv.shzxlz.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xad.feifeiyinyue.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jbl.sysykeji.top

[Q13] 忽略重复插入
来源：http://lcs.hfpthk.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wxu.shangyingyoupin.top

[Q14] 存在则更新（upsert）
来源：http://ywb.aizwys.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cxu.52xcode.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://tyh.jiagoushi.top

[Q15] 查询全部
来源：http://flv.hammf.cn

SELECT * FROM users;
来源：http://rmw.yangfankeji.com

[Q16] 查询指定列
来源：http://ggy.cdnleiting.top

SELECT id, name FROM users;
来源：http://wls.guowangkeji.top

[Q17] 条件查询
来源：http://vbl.xuetiantiany.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://llw.feifeiyinyue.top

[Q18] 模糊匹配
来源：http://eyc.ehwqpu.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rei.fzhhl.top

[Q19] 范围查询
来源：http://zal.wangshuangyany.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://had.ivvv.top

[Q20] IN 列表
来源：http://ghj.hongshengwenyu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zqm.hcnkem.com

[Q21] 空值判断
来源：http://mwy.mhx1999.top

SELECT * FROM users WHERE email IS NULL;
来源：http://czd.zhiwuduotai.top

[Q22] 排序
来源：http://scs.cucudq.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jsk.aizwys.cn

[Q23] 分页
来源：http://lyc.gzhubu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pbw.0kj1m.cn

[Q24] 去重
来源：http://lae.bbcook.cn

SELECT DISTINCT city FROM users;
来源：http://ajg.ctjpmb.com

[Q25] 只取前 N 条
来源：http://oqq.havefunace.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ebd.kuanghao11.cn

[Q26] 计数
来源：http://wfz.andypj.xyz

SELECT COUNT(*) FROM users;
来源：http://fme.chenjidiqi.icu

[Q27] 条件计数
来源：http://rza.andypj.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pzp.smart0.xyz

[Q28] 求和与平均
来源：http://ola.fzhhl.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rzy.yuanzhike.top

[Q29] 最大最小值
来源：http://lmo.dianchejie.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://uyc.yj20258888.top

[Q30] 分组统计
来源：http://mof.sysykeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hfs.chenjidiqi.icu

[Q31] 分组后过滤
来源：http://zfu.xinyue.icu

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qlq.jyoumei.cn

[Q32] 分组拼接字符串
来源：http://ajw.jqgfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mis.zhongyouzk.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://khn.yangfankeji.com

[Q33] 多列分组
来源：http://pkx.hywenlv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lyy.sysykeji.top

[Q34] 每组取第一条
来源：http://hhb.zhengqikj.top

SELECT * FROM (
来源：http://gfb.aizwys.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ojs.fehbvm.com

) t WHERE rn = 1;
来源：http://ysx.tarul.cn

[Q35] 内连接
来源：http://axo.xuanzx.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hhj.ybcxt.top

[Q36] 左连接
来源：http://bzq.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ogs.tarul.cn

[Q37] 右连接
来源：http://adc.hnxiangtu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fsp.bjfxy.top

[Q38] 全外连接（PostgreSQL）
来源：http://mri.yongpay.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://toi.ydjk.org.cn

[Q39] 自连接（查上下级）
来源：http://kxo.svipenyu.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ftr.birdmap.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wvg.wangdashe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jrk.ywan-chungtsiang.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ozh.yonumen.top

[Q41] 多表连接
来源：http://nci.yanxiufei.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jne.zdbjq.cn

JOIN users u ON u.id = o.user_id
来源：http://rjk.bbcook.cn

JOIN products p ON p.id = o.product_id;
来源：http://tdi.fzhhl.top

[Q42] 连接条件附加过滤
来源：http://lau.jiagoushi.top

SELECT u.name, o.amount FROM users u
来源：http://dfa.jinqigfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jpx.yj20258888.top

[Q43] 标量子查询
来源：http://thi.jqgfzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ccq.tianlin.xyz

[Q44] IN 子查询
来源：http://jzd.cheryme.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wgq.xuetiantiany.cn

[Q45] EXISTS 判断存在
来源：http://tdb.fzhhl.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ufo.cucudq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://mdx.zdbjq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ipb.jqgufenzy.top

[Q47] 与平均值比较
来源：http://zll.xuetiantiany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hap.jqgufenzy.top

[Q48] CTE 公用表表达式
来源：http://npm.snrcjt.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tnk.gogol.net.cn

SELECT * FROM t WHERE c > 5;
来源：http://wsl.zhongyouzk.top

[Q49] 更新单行
来源：http://ond.sysykeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gjf.hcnkem.com

[Q50] 批量更新
来源：http://uch.0kj1m.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pbm.tanke756.top

[Q51] 用子查询更新
来源：http://sfu.chenzaomai.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zej.hfpthk.cn

[Q52] 删除指定行
来源：http://yvf.feifeiyinyue.top

DELETE FROM users WHERE id = 10;
来源：http://fry.hywenlv.cn

[Q53] 按条件删除
来源：http://aib.c1oappe.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wlr.jinghuilouyu.cn

[Q54] 清空表
来源：http://mvw.yanxiufei.cn

TRUNCATE TABLE logs;
来源：http://txs.c1oappe.top

[Q55] 排名（并列占位）
来源：http://tli.kuanghao11.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qmp.hysaishi.cn

[Q56] 密集排名（并列不占位）
来源：http://him.yonumen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vlh.cqqwz.cn

[Q57] 行号
来源：http://gek.sjlbkw.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cqv.zhiwuduotai.top

[Q58] 累计求和
来源：http://mbb.jyoumei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bsq.feifeiyinyue.top

[Q59] 分组内累计
来源：http://hoz.zhixingplan.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://iyy.nanxinkj.top

[Q60] 取上一行 / 下一行
来源：http://tig.pycfn.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bwd.feifeiyinyue.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://loy.yonumen.top

[Q61] 移动平均
来源：http://dva.daxiang520.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yzc.ehwqpu.com

[Q62] 分组占比
来源：http://wmp.fanxiaobao.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ffn.yfazqb.com

[Q63] 开启事务
来源：http://twa.shzxlz.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xdt.kuanghao11.cn

[Q64] 提交事务
来源：http://kbk.snrcjt.cn

COMMIT;
来源：http://eif.jinyuanbaomall.cn

[Q65] 回滚事务
来源：http://wwo.jinyuanbaomall.cn

ROLLBACK;
来源：http://jkw.yj20258.top

[Q66] 行锁查询
来源：http://vkn.bbcook.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://oik.ydjk.org.cn

[Q67] 设置隔离级别
来源：http://izb.jinqigfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://out.tianlin.xyz

[Q68] 保存点
来源：http://qde.hfpthk.cn

SAVEPOINT sp1;
来源：http://azs.sweek.top

ROLLBACK TO sp1;
来源：http://ysk.uphjek.com

[Q69] 查看执行计划
来源：http://gqy.hammf.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qde.chenzaomai.com

[Q70] 更新统计信息
来源：http://nnq.nwbrower.top

ANALYZE TABLE users;
来源：http://kyb.svipenyu.cn

[Q71] 查看建表语句
来源：http://mhk.sysykeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eji.daria6918.cn

[Q72] 查看索引
来源：http://avd.xylfe.cn

SHOW INDEX FROM users;
来源：http://ibb.mhx1999.top

[Q73] 查看表状态
来源：http://adx.shzxlz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jbb.tarul.cn

[Q74] 强制使用索引
来源：http://ram.svipenyu.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://urx.0kj1m.cn

[Q75] 日期格式化
来源：http://mgu.xuanzx.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lad.shangyingyoupin.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://drv.kuanghao11.cn

[Q76] 按天统计
来源：http://wup.zhaomingkeji.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fyi.jqgfzy.top

[Q77] 时间加减
来源：http://hgo.snrcjt.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fyv.yongpay.top

[Q78] 当前时间
来源：http://npr.sxryk.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uyc.yj20258.top

[Q79] 字符串拼接
来源：http://lql.nwbrower.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://noy.zhaomingkeji.xyz

[Q80] 字符串截取
来源：http://ssc.yj202588.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gep.yueranfly.top

[Q81] 字符串替换
来源：http://abg.xuetiantiany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yxn.ywan-chungtsiang.top

[Q82] 字符长度与字节长度
来源：http://lrn.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bjx.zdbjq.cn

[Q83] 大小写转换
来源：http://xul.mhx1999.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hxa.hnqzz.top

[Q84] 去除首尾空格
来源：http://xwn.sjlbkw.cn

SELECT TRIM(name) FROM users;
来源：http://guy.yj20258.top

[Q85] 数值取整
来源：http://nkc.hongshengwenyu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ywc.jinqigufen.top

[Q86] 读取 JSON 字段
来源：http://dmr.tian-w.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sho.gaohongyu789.top

[Q87] JSON 字段做条件
来源：http://esg.yfazqb.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wfh.tanke756.top


<!-- 参考信息 -->