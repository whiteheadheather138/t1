代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xnq.chenlongwang.top

Ruby: # 用 Fiber 或 async gem
来源：http://edr.zhixingplan.top

C#:   async Task F() { await G(); }
来源：http://txk.shanyushiyangtech.top

[O05] 并发执行并等待全部完成
来源：http://eet.jqgufenzy.top

Py:   asyncio.gather(*tasks)
来源：http://wui.wangdashe.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gvw.zhixingplan.top

JS:   await Promise.all(tasks)
来源：http://uul.tian-w.cn

TS:   await Promise.all(tasks)
来源：http://rtx.yangfankeji.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://hct.haohaochexian.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://auq.yj202588.top

Ruby: threads.map(&:join)
来源：http://cpy.tarul.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://jvw.yj20258.top

[O06] 使用进程池
来源：http://ypm.wangshuangyany.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cge.ybcxt.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ayk.jianghu66.top

JS:   // child_process / cluster 模块
来源：http://nws.xinyue.icu

TS:   // child_process / cluster 模块
来源：http://dpa.tianlin.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bpu.jiagoushi.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jru.xingfuxueyuan.xyz

Ruby: // fork 块
来源：http://lbr.fanxiaobao.xyz

C#:   Parallel.For
来源：http://may.dianchejie.cn

================================================================================
来源：http://jsf.aizwys.cn

P. 常用工具函数
来源：http://eoa.yonumen.top

================================================================================
来源：http://vav.uphjek.com

[P01] 生成 UUID
来源：http://xxc.ydzc1.top

Py:   str(uuid.uuid4())
来源：http://xin.sxryk.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://bfe.yueranfly.top

JS:   crypto.randomUUID()
来源：http://dmu.feifeiyinyue.top

TS:   crypto.randomUUID()
来源：http://loq.havefunace.top

Java: UUID.randomUUID().toString()
来源：http://bho.zycfv.cn

Go:   // 用 github.com/google/uuid
来源：http://plg.fzhhl.top

Ruby: SecureRandom.uuid
来源：http://suq.gzhubu.top

C#:   Guid.NewGuid().ToString()
来源：http://wwx.zycfv.cn

[P02] MD5 / SHA256 摘要
来源：http://tdz.kuanghao11.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://grc.zhongyouzk.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zlz.jinghuilouyu.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://omz.andypj.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wvv.zhaomingkeji.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://opl.9152youxi.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uva.jinyuanbaomall.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wik.gogol.net.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gwg.sufxvd.cn

[P03] 生成短随机字符串
来源：http://pus.cucudq.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://odv.nwbrower.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oad.shanyushiyangtech.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wky.chenlongwang.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dad.0kj1m.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://htv.ydzc1.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://amw.feifeiyinyue.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://oln.hcnkem.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nnn.shuidangran.top

[P04] 求长度
来源：http://hna.chenlongwang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nkn.daxiang520.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://evj.tarul.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hxw.uphjek.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wwp.jinghuilouyu.cn

Java: list.size();  map.size();  s.length()
来源：http://zja.fanxiaobao.xyz

Go:   len(arr);  len(m)
来源：http://ywx.xuetiantiany.cn

Ruby: x.length;  x.size
来源：http://mgc.wangshuangyany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hpg.yvedp.cn

[P05] 判断两个对象内容是否相等
来源：http://nsx.tanke756.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://mlr.hnqzz.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://knt.uphjek.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://iuj.uphjek.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xvg.dashuyun.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rzf.jqgfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://wwk.xuanzx.com

Ruby: a == b
来源：http://dhj.shanyushiyangkeji.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rmr.mhx1999.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bgh.snrcjt.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eus.gogol.net.cn

PHP:  if (empty($x)) {}
来源：http://lym.daxiang520.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uut.fengsongda.top

TS:   if (x == null) {}
来源：http://ffy.xylfe.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://dya.quarkkingdee.top

Go:   if x == nil {}
来源：http://wol.andypj.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cvf.yj20258.top

C#:   if (x is null) {}
来源：http://jot.guannengcc.top

[P07] 防抖与节流
来源：http://twj.shanyushiyangtech.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mrl.dashuyun.cn

PHP:  // 手写时间戳比较
来源：http://iag.jinqigufen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qwu.shuidangran.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://djn.yangfankeji.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nwu.ivvv.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rkz.tianlin.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://ory.fanxiaobao.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kru.tian-w.cn

[P08] 处理浮点精度问题
来源：http://spy.quarkkingdee.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jbz.andypj.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cuu.gzhubu.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kgb.hnqzz.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://zdq.yvedp.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sdl.nanxuanxn.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://toy.yj20258.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ylq.guowangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kak.shuidangran.top

================================================================================
来源：http://ace.ivvv.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://ubz.zdqjudy.top

================================================================================
来源：http://qgt.sweek.top

[Q01] 创建表
来源：http://ris.meibo888.top

CREATE TABLE users (
来源：http://rmh.dashuyun.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xza.bjfxy.top

name VARCHAR(50) NOT NULL,
来源：http://huy.haohaochexian.top

email VARCHAR(100) UNIQUE,
来源：http://ibu.yvedp.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ydv.havefunace.top

);
来源：http://shk.wangdashe.top

[Q02] 创建带外键的表
来源：http://pnk.yanxiufei.cn

CREATE TABLE orders (
来源：http://qpu.zhoulong.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://txo.hnqzz.top

user_id INT NOT NULL,
来源：http://nkk.shuidangran.top

amount DECIMAL(10, 2),
来源：http://dth.chenzaomai.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cwf.xziqi.cn

);
来源：http://gjv.tarul.cn

[Q03] 增加列
来源：http://pde.mhx1999.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kgx.tanke756.top

[Q04] 修改列类型
来源：http://tvz.ydjk.org.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dlw.hcnkem.com

[Q05] 重命名列
来源：http://enk.yfazqb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://kny.0kj1m.cn

[Q06] 删除列
来源：http://aob.ehwqpu.com

ALTER TABLE users DROP COLUMN age;
来源：http://buh.hysaishi.cn

[Q07] 删除表
来源：http://onw.andypj.xyz

DROP TABLE IF EXISTS orders;
来源：http://phk.bjfxy.top

[Q08] 创建普通索引
来源：http://xfa.yuanzhike.top

CREATE INDEX idx_users_email ON users(email);
来源：http://pbi.tanke756.top

[Q09] 创建唯一索引
来源：http://raa.fengsongda.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mib.xylfe.cn

[Q10] 插入单行
来源：http://zzx.svipenyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://irr.sxryk.cn

[Q11] 一次插入多行
来源：http://bpw.yvedp.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ibs.0kj1m.cn

[Q12] 插入后取自增 ID
来源：http://wtv.9152youxi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fpw.gotoacloud.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mwx.hysaishi.cn

[Q13] 忽略重复插入
来源：http://itu.jinqigufen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lrq.316326.xyz

[Q14] 存在则更新（upsert）
来源：http://ybu.shanyushiyangtech.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tdt.ybcxt.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://agc.redwolf501.top

[Q15] 查询全部
来源：http://nyv.guowangkeji.top

SELECT * FROM users;
来源：http://roh.sufxvd.cn

[Q16] 查询指定列
来源：http://dws.gotoacloud.top

SELECT id, name FROM users;
来源：http://qjw.gotoacloud.top

[Q17] 条件查询
来源：http://nmn.zhiwuduotai.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mrb.vqdsnc.cn

[Q18] 模糊匹配
来源：http://pbi.bbcook.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qqi.daria6918.cn

[Q19] 范围查询
来源：http://jxl.316326.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jfo.shanyushiyangkeji.top

[Q20] IN 列表
来源：http://oug.sysykeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nks.zhaomingkeji.xyz

[Q21] 空值判断
来源：http://bjr.tianlin.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://jwb.hysaishi.cn

[Q22] 排序
来源：http://chd.dashuyun.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vle.jyoumei.cn

[Q23] 分页
来源：http://sfo.xziqi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lae.zhijiandao.cn

[Q24] 去重
来源：http://rqf.svipenyu.cn

SELECT DISTINCT city FROM users;
来源：http://uky.shangyingyoupin.top

[Q25] 只取前 N 条
来源：http://zgx.zhixingplan.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kzy.dianchejie.cn

[Q26] 计数
来源：http://ynp.sjlbkw.cn

SELECT COUNT(*) FROM users;
来源：http://kmc.ivvv.top

[Q27] 条件计数
来源：http://ogt.tian-w.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tpp.yfazqb.com

[Q28] 求和与平均
来源：http://ypr.cdnleiting.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ggw.meibo888.top

[Q29] 最大最小值
来源：http://cdd.ybcxt.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ncm.zhengqikj.top

[Q30] 分组统计
来源：http://jyz.ydzc1.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://azc.hesvh.cn

[Q31] 分组后过滤
来源：http://mek.tanke756.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sff.jqgufenzy.top

[Q32] 分组拼接字符串
来源：http://rvj.xinyue.icu

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ngz.yueranfly.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://khw.52xcode.cn

[Q33] 多列分组
来源：http://rtb.feifeiyinyue.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tzc.epnwcf.com

[Q34] 每组取第一条
来源：http://cvh.meibo888.top

SELECT * FROM (
来源：http://dkn.52xcode.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tzh.hammf.cn

) t WHERE rn = 1;
来源：http://pnr.daria6918.cn

[Q35] 内连接
来源：http://mrd.ppjwa.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://efy.cashguo.top

[Q36] 左连接
来源：http://ytq.sysykeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nuq.iojbl.cn

[Q37] 右连接
来源：http://dud.shangyingyoupin.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://few.bjfxy.top

[Q38] 全外连接（PostgreSQL）
来源：http://ynk.daria6918.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://shp.tian-w.cn

[Q39] 自连接（查上下级）
来源：http://vyk.wangdashe.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://riz.sufxvd.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vvb.bjfxy.top

[Q40] 交叉连接（笛卡尔积）
来源：http://mxt.guannengcc.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://upg.aizwys.cn

[Q41] 多表连接
来源：http://fwd.redwolf501.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pzr.zhengqikj.top

JOIN users u ON u.id = o.user_id
来源：http://xsd.dianchejie.cn

JOIN products p ON p.id = o.product_id;
来源：http://slk.guowangkeji.top

[Q42] 连接条件附加过滤
来源：http://hll.daria6918.cn

SELECT u.name, o.amount FROM users u
来源：http://dge.hnqzz.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bua.zhijiandao.cn

[Q43] 标量子查询
来源：http://avu.kuanghao11.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bri.ppjwa.cn

[Q44] IN 子查询
来源：http://hjp.fengsongda.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cdq.ehwqpu.com

[Q45] EXISTS 判断存在
来源：http://rhu.guannengcc.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jxs.yonumen.top

[Q46] NOT EXISTS 判断不存在
来源：http://occ.sysykeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tpq.uphjek.com

[Q47] 与平均值比较
来源：http://chz.fengsongda.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qgy.ppjwa.cn

[Q48] CTE 公用表表达式
来源：http://zjw.52xcode.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://stt.jiagoushi.top

SELECT * FROM t WHERE c > 5;
来源：http://oyn.hcnkem.com

[Q49] 更新单行
来源：http://rnq.fzhhl.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://atp.fengsongda.top

[Q50] 批量更新
来源：http://hqi.sufxvd.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://shk.316326.xyz

[Q51] 用子查询更新
来源：http://kvc.aibaodan.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hhb.yfazqb.com

[Q52] 删除指定行
来源：http://yjh.xylfe.cn

DELETE FROM users WHERE id = 10;
来源：http://sai.zhengqikj.top

[Q53] 按条件删除
来源：http://hkx.cdnleiting.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://btj.guannengcc.top

[Q54] 清空表
来源：http://khs.xingfuxueyuan.xyz

TRUNCATE TABLE logs;
来源：http://fwj.hywenlv.cn

[Q55] 排名（并列占位）
来源：http://cmu.xuetiantiany.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://igo.ehwqpu.com

[Q56] 密集排名（并列不占位）
来源：http://koj.daxiang520.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fqj.zhengqikj.top

[Q57] 行号
来源：http://lkq.svipenyu.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rhh.jiagoushi.top

[Q58] 累计求和
来源：http://ook.epnwcf.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pdp.pengpengdd.cyou

[Q59] 分组内累计
来源：http://ttz.sxryk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lik.jlsjyb.cn

[Q60] 取上一行 / 下一行
来源：http://rye.ywan-chungtsiang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vwb.gaohongyu789.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cyy.yuanzhike.top

[Q61] 移动平均
来源：http://hul.52xcode.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://imz.nanxuanxn.top

[Q62] 分组占比
来源：http://okd.cdnleiting.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ynh.chenzaomai.com

[Q63] 开启事务
来源：http://phi.jinghuilouyu.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://riy.tianlin.xyz

[Q64] 提交事务
来源：http://uen.bbcook.cn

COMMIT;
来源：http://gth.haohaochexian.top

[Q65] 回滚事务
来源：http://mqz.xziqi.cn

ROLLBACK;
来源：http://qeb.aibaodan.cn

[Q66] 行锁查询
来源：http://yrc.hfpthk.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eci.zdqjudy.top

[Q67] 设置隔离级别
来源：http://eed.yfazqb.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jhf.ydzc1.top

[Q68] 保存点
来源：http://rnr.vehdjk.com

SAVEPOINT sp1;
来源：http://cyi.hnqzz.top

ROLLBACK TO sp1;
来源：http://ilm.sweek.top

[Q69] 查看执行计划
来源：http://cco.pengpengdd.cyou

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oxh.andypj.xyz

[Q70] 更新统计信息
来源：http://hki.wangshuangyany.cn

ANALYZE TABLE users;
来源：http://oac.svipenyu.cn

[Q71] 查看建表语句
来源：http://wvg.aizwys.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://moe.shanyushiyangkeji.top

[Q72] 查看索引
来源：http://swg.ppjwa.cn

SHOW INDEX FROM users;
来源：http://nur.zdqjudy.top

[Q73] 查看表状态
来源：http://eel.cdnleiting.top

SHOW TABLE STATUS LIKE 'users';
来源：http://anm.snrcjt.cn

[Q74] 强制使用索引
来源：http://jjt.sxryk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uoj.gotoacloud.top

[Q75] 日期格式化
来源：http://qmz.xingfuxueyuan.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://upf.hesvh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tjt.fzhhl.top

[Q76] 按天统计
来源：http://atd.316326.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yqn.xuanzx.com

[Q77] 时间加减
来源：http://ryq.guowangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iny.sweek.top

[Q78] 当前时间
来源：http://zvm.cdnleiting.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rmu.cheryme.top

[Q79] 字符串拼接
来源：http://mca.haohaochexian.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gsb.hongshengwenyu.top

[Q80] 字符串截取
来源：http://qnf.yanxiufei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ddy.hcnkem.com

[Q81] 字符串替换
来源：http://wny.0kj1m.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ozh.ehwqpu.com

[Q82] 字符长度与字节长度
来源：http://civ.yvedp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://buj.svipenyu.cn

[Q83] 大小写转换
来源：http://loo.hnqzz.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gjh.cqqwz.cn

[Q84] 去除首尾空格
来源：http://cbg.hongshengwenyu.top

SELECT TRIM(name) FROM users;
来源：http://jwk.vehdjk.com

[Q85] 数值取整
来源：http://cjp.bbcook.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://htx.havefunace.top

[Q86] 读取 JSON 字段
来源：http://ulr.cashguo.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://set.shanyushiyangtech.top

[Q87] JSON 字段做条件
来源：http://ewy.yvedp.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nrs.vehdjk.com

[Q88] 行转列（条件聚合）
来源：http://tza.yanxiufei.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://foe.aibaodan.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ykt.tanke756.top

[Q89] 判断表是否存在
来源：http://krv.sjlbkw.cn


<!-- 参考信息 -->