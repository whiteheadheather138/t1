代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://qyt.nanxuanxn.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ntn.iojbl.cn

JS:   await Promise.all(tasks)
来源：http://vee.uphjek.com

TS:   await Promise.all(tasks)
来源：http://zur.shanyushiyangtech.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://raj.gaohongyu789.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kej.zdbjq.cn

Ruby: threads.map(&:join)
来源：http://bwi.zhiwuduotai.top

C#:   await Task.WhenAll(t1, t2)
来源：http://vnf.ctjpmb.com

[O06] 使用进程池
来源：http://zqw.wangdashe.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cuw.hysaishi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://drk.shuidangran.top

JS:   // child_process / cluster 模块
来源：http://gys.chenjidiqi.icu

TS:   // child_process / cluster 模块
来源：http://ahw.pycfn.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dar.cqqwz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://olh.fktsv.cn

Ruby: // fork 块
来源：http://uwt.yfazqb.com

C#:   Parallel.For
来源：http://brx.jinqigfzy.top

================================================================================
来源：http://izd.cdnleiting.top

P. 常用工具函数
来源：http://ijy.gogol.net.cn

================================================================================
来源：http://sns.ydjk.org.cn

[P01] 生成 UUID
来源：http://lxo.0kj1m.cn

Py:   str(uuid.uuid4())
来源：http://xlk.xuetiantiany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://fxl.vqdsnc.cn

JS:   crypto.randomUUID()
来源：http://tgy.zhixingplan.top

TS:   crypto.randomUUID()
来源：http://fyf.zhaomingkeji.xyz

Java: UUID.randomUUID().toString()
来源：http://tol.jiagoushi.top

Go:   // 用 github.com/google/uuid
来源：http://zja.sweek.top

Ruby: SecureRandom.uuid
来源：http://qdt.zhixingplan.top

C#:   Guid.NewGuid().ToString()
来源：http://asv.ydjk.org.cn

[P02] MD5 / SHA256 摘要
来源：http://jar.hfpthk.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://yeq.nanxinkj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://odx.yuanzhike.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xim.shuidangran.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://nwd.yvedp.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xgq.haohaochexian.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mju.tanke756.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://gvt.dashuyun.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oqv.dashuyun.cn

[P03] 生成短随机字符串
来源：http://ieh.sysykeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://qwu.shanyushiyangtech.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xnv.haohaochexian.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wzc.c1oappe.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mas.hcnkem.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nrr.tanke756.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zza.quarkkingdee.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://sgc.shanyushiyangkeji.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rup.shanyushiyangkeji.top

[P04] 求长度
来源：http://djm.fzhhl.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://cjh.feifeiyinyue.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zof.zhengqikj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://emw.cashguo.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pjw.nwbrower.top

Java: list.size();  map.size();  s.length()
来源：http://fui.daxiang520.top

Go:   len(arr);  len(m)
来源：http://kab.sufxvd.cn

Ruby: x.length;  x.size
来源：http://cfq.uphjek.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://xwi.cucudq.cn

[P05] 判断两个对象内容是否相等
来源：http://gmz.zhixingplan.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://waz.c1oappe.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qxk.xylfe.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fin.xuanzx.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://khw.shangyingyoupin.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://gyh.hysaishi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ysw.jqgufenzy.top

Ruby: a == b
来源：http://yzc.9152youxi.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gwj.jqgfzy.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rab.daria6918.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pft.jlsjyb.cn

PHP:  if (empty($x)) {}
来源：http://tjw.fktsv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://nbo.redwolf501.top

TS:   if (x == null) {}
来源：http://fdt.yanxiufei.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://zvq.xuetiantiany.cn

Go:   if x == nil {}
来源：http://tqx.pengpengdd.cyou

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ajk.aizwys.cn

C#:   if (x is null) {}
来源：http://orm.kuanghao11.cn

[P07] 防抖与节流
来源：http://wwu.fktsv.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kdo.sysykeji.top

PHP:  // 手写时间戳比较
来源：http://juu.quarkkingdee.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ktm.bjfxy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ofw.svipenyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kwv.cashguo.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zxy.dianchejie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fpt.bbcook.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://isg.yanxiufei.cn

[P08] 处理浮点精度问题
来源：http://hdy.ppjwa.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nyy.andypj.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://lrm.ppjwa.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://zst.52xcode.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://nrt.zhongyouzk.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ibg.svipenyu.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://iod.bbcook.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://oru.jinqigfzy.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rok.nwbrower.top

================================================================================
来源：http://qjh.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://cjf.aibaodan.cn

================================================================================
来源：http://yui.tarul.cn

[Q01] 创建表
来源：http://oyo.hnqzz.top

CREATE TABLE users (
来源：http://nap.jinqigufen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://rsr.cdnleiting.top

name VARCHAR(50) NOT NULL,
来源：http://cqc.shzxlz.cn

email VARCHAR(100) UNIQUE,
来源：http://lnt.gogol.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yau.jyoumei.cn

);
来源：http://jrz.cheryme.top

[Q02] 创建带外键的表
来源：http://kae.fzhhl.top

CREATE TABLE orders (
来源：http://vve.shanyushiyangtech.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://crj.yj202588.top

user_id INT NOT NULL,
来源：http://uef.jiagoushi.top

amount DECIMAL(10, 2),
来源：http://ubm.aizwys.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tso.jinyuanbaomall.cn

);
来源：http://tan.redwolf501.top

[Q03] 增加列
来源：http://toq.birdmap.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ceb.gzhubu.top

[Q04] 修改列类型
来源：http://vyr.wangshuangyany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://hfw.hnqzz.top

[Q05] 重命名列
来源：http://obb.hammf.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bar.gogol.net.cn

[Q06] 删除列
来源：http://dtr.xuetiantiany.cn

ALTER TABLE users DROP COLUMN age;
来源：http://dbc.zhixingplan.top

[Q07] 删除表
来源：http://qgg.yongpay.top

DROP TABLE IF EXISTS orders;
来源：http://rkx.vehdjk.com

[Q08] 创建普通索引
来源：http://dii.dashuyun.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://shr.xylfe.cn

[Q09] 创建唯一索引
来源：http://gyo.gogol.net.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lye.birdmap.top

[Q10] 插入单行
来源：http://mht.sysykeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gwc.fzhhl.top

[Q11] 一次插入多行
来源：http://ziw.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://atf.yonumen.top

[Q12] 插入后取自增 ID
来源：http://zef.xuetiantiany.cn

INSERT INTO users (name) VALUES ('C');
来源：http://hnd.cheryme.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pxl.nwbrower.top

[Q13] 忽略重复插入
来源：http://mfx.hammf.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fpa.fehbvm.com

[Q14] 存在则更新（upsert）
来源：http://mij.jinyuanbaomall.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tca.zdqjudy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zjs.bbcook.cn

[Q15] 查询全部
来源：http://pxf.zhaomingkeji.xyz

SELECT * FROM users;
来源：http://nme.zhiwuduotai.top

[Q16] 查询指定列
来源：http://fms.sysykeji.top

SELECT id, name FROM users;
来源：http://txk.tanke756.top

[Q17] 条件查询
来源：http://hym.chenzaomai.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://elk.quarkkingdee.top

[Q18] 模糊匹配
来源：http://mng.tarul.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wcx.gaohongyu789.top

[Q19] 范围查询
来源：http://yhw.xingfuxueyuan.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://guw.hnqzz.top

[Q20] IN 列表
来源：http://xwc.yvedp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uoa.jinghuilouyu.cn

[Q21] 空值判断
来源：http://xlr.aizwys.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kfg.yanxiufei.cn

[Q22] 排序
来源：http://rmj.xuanzx.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://xzu.kuanghao11.cn

[Q23] 分页
来源：http://teo.kuanghao11.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://fky.hnxiangtu.top

[Q24] 去重
来源：http://heh.feifeiyinyue.top

SELECT DISTINCT city FROM users;
来源：http://ivi.jinghuilouyu.cn

[Q25] 只取前 N 条
来源：http://mps.jinghuilouyu.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nvs.fzhhl.top

[Q26] 计数
来源：http://vgo.pengpengdd.cyou

SELECT COUNT(*) FROM users;
来源：http://svg.vehdjk.com

[Q27] 条件计数
来源：http://wjv.shzxlz.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://num.birdmap.top

[Q28] 求和与平均
来源：http://cmq.ehwqpu.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zgy.gzhubu.top

[Q29] 最大最小值
来源：http://khn.zhoulong.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://ibx.nanxinkj.top

[Q30] 分组统计
来源：http://zne.epnwcf.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pva.hesvh.cn

[Q31] 分组后过滤
来源：http://ygr.sysykeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jhn.xziqi.cn

[Q32] 分组拼接字符串
来源：http://xyk.zhiwuduotai.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ujc.jlsjyb.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vwx.fengsongda.top

[Q33] 多列分组
来源：http://rog.yj20258888.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://urq.dashuyun.cn

[Q34] 每组取第一条
来源：http://nmg.haohaochexian.top

SELECT * FROM (
来源：http://sws.sjlbkw.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rsv.xingfuxueyuan.xyz

) t WHERE rn = 1;
来源：http://nep.vehdjk.com

[Q35] 内连接
来源：http://eid.xinyue.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://amv.hesvh.cn

[Q36] 左连接
来源：http://kml.52xcode.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zag.gzhubu.top

[Q37] 右连接
来源：http://nwp.redwolf501.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xlc.ivvv.top

[Q38] 全外连接（PostgreSQL）
来源：http://aes.pycfn.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://umi.chenjidiqi.icu

[Q39] 自连接（查上下级）
来源：http://qpc.xingfuxueyuan.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://lgy.tian-w.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wqc.ivvv.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wtn.gzhubu.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hnv.epnwcf.com

[Q41] 多表连接
来源：http://ohi.fzhhl.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://slm.cashguo.top

JOIN users u ON u.id = o.user_id
来源：http://lgl.xylfe.cn

JOIN products p ON p.id = o.product_id;
来源：http://ziu.quarkkingdee.top

[Q42] 连接条件附加过滤
来源：http://rfx.yonumen.top

SELECT u.name, o.amount FROM users u
来源：http://jon.nanxuanxn.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vev.yueranfly.top

[Q43] 标量子查询
来源：http://vel.shanyushiyangkeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://txp.iojbl.cn

[Q44] IN 子查询
来源：http://kyz.hfpthk.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mes.chenjidiqi.icu

[Q45] EXISTS 判断存在
来源：http://jnt.fehbvm.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://egb.feifeiyinyue.top

[Q46] NOT EXISTS 判断不存在
来源：http://rrt.pengpengdd.cyou

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gqa.tian-w.cn

[Q47] 与平均值比较
来源：http://dwq.aibaodan.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rte.yfazqb.com

[Q48] CTE 公用表表达式
来源：http://wpm.mhx1999.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dpa.birdmap.top

SELECT * FROM t WHERE c > 5;
来源：http://zea.ctjpmb.com

[Q49] 更新单行
来源：http://but.ctjpmb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jge.iojbl.cn

[Q50] 批量更新
来源：http://dxi.ctjpmb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yxw.fktsv.cn

[Q51] 用子查询更新
来源：http://nka.uphjek.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yiv.yanxiufei.cn

[Q52] 删除指定行
来源：http://kci.fktsv.cn

DELETE FROM users WHERE id = 10;
来源：http://jso.xingfuxueyuan.xyz

[Q53] 按条件删除
来源：http://pyh.hnxiangtu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://epu.shzxlz.cn

[Q54] 清空表
来源：http://sha.birdmap.top

TRUNCATE TABLE logs;
来源：http://gvp.feifeiyinyue.top

[Q55] 排名（并列占位）
来源：http://uph.aibaodan.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pen.jinghuilouyu.cn

[Q56] 密集排名（并列不占位）
来源：http://qlh.bbcook.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ovs.andypj.xyz

[Q57] 行号
来源：http://idx.wangdashe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kjj.gzhubu.top

[Q58] 累计求和
来源：http://oio.zdqjudy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xbw.hywenlv.cn

[Q59] 分组内累计
来源：http://wqw.feifeiyinyue.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ooc.gogol.net.cn

[Q60] 取上一行 / 下一行
来源：http://mvg.daxiang520.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kge.sufxvd.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://opv.chenzaomai.com

[Q61] 移动平均
来源：http://lxf.yvedp.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qvv.hcnkem.com

[Q62] 分组占比
来源：http://wfj.jinqigufen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hbn.cqqwz.cn

[Q63] 开启事务
来源：http://sat.tanke756.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gda.cdnleiting.top

[Q64] 提交事务
来源：http://ttf.chenjidiqi.icu

COMMIT;
来源：http://muk.jianghu66.top

[Q65] 回滚事务
来源：http://kul.shanyushiyangkeji.top

ROLLBACK;
来源：http://rvv.quarkkingdee.top

[Q66] 行锁查询
来源：http://xsw.zhiwuduotai.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cwn.ehwqpu.com

[Q67] 设置隔离级别
来源：http://omi.ywan-chungtsiang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://suv.cdnleiting.top

[Q68] 保存点
来源：http://zju.gotoacloud.top

SAVEPOINT sp1;
来源：http://xlc.guannengcc.top

ROLLBACK TO sp1;
来源：http://wfp.yuxming.cn

[Q69] 查看执行计划
来源：http://ist.dianchejie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mfu.nanxuanxn.top

[Q70] 更新统计信息
来源：http://fzr.zhijiandao.cn

ANALYZE TABLE users;
来源：http://kpv.cdnleiting.top

[Q71] 查看建表语句
来源：http://afd.zdbjq.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://elm.jinqigfzy.top

[Q72] 查看索引
来源：http://hbf.gotoacloud.top

SHOW INDEX FROM users;
来源：http://amx.yvedp.cn

[Q73] 查看表状态
来源：http://uor.zhaomingkeji.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://ncy.hcnkem.com

[Q74] 强制使用索引
来源：http://pbp.yj20258888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zzd.ydzc1.top

[Q75] 日期格式化
来源：http://kgk.aibaodan.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://myx.andypj.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://asc.jiagoushi.top

[Q76] 按天统计
来源：http://rxv.fehbvm.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rma.jinqigfzy.top

[Q77] 时间加减
来源：http://igj.xuanzx.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oli.jinyuanbaomall.cn

[Q78] 当前时间
来源：http://ioq.cdnleiting.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ohn.gaohongyu789.top

[Q79] 字符串拼接
来源：http://blx.cheryme.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qzw.ehwqpu.com

[Q80] 字符串截取
来源：http://ybc.0kj1m.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ewl.jinyuanbaomall.cn

[Q81] 字符串替换
来源：http://nqt.yanxiufei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zzv.hywenlv.cn

[Q82] 字符长度与字节长度
来源：http://npb.ywan-chungtsiang.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dma.cashguo.top

[Q83] 大小写转换
来源：http://mms.daxiang520.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hty.c1oappe.top

[Q84] 去除首尾空格
来源：http://kpf.yvedp.cn

SELECT TRIM(name) FROM users;
来源：http://rvc.aizwys.cn

[Q85] 数值取整
来源：http://lgz.0kj1m.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pja.zhaomingkeji.xyz

[Q86] 读取 JSON 字段
来源：http://eyq.ydjk.org.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tgr.yuanzhike.top

[Q87] JSON 字段做条件
来源：http://lrn.cucudq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mun.yj20258888.top

[Q88] 行转列（条件聚合）
来源：http://bye.wangdashe.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lmq.yuanzhike.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mlq.gzhubu.top

[Q89] 判断表是否存在
来源：http://rjp.bbcook.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pcy.yuanzhike.top

[Q90] 生成序号列
来源：http://gku.zycfv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uuh.ywan-chungtsiang.top

================================================================================
来源：http://hcs.zhixingplan.top


<!-- 参考信息 -->