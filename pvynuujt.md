代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://rhr.zhaomingkeji.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://ndu.xylfe.cn

C#:   async Task F() { await G(); }
来源：http://efi.yj202588.top

[O05] 并发执行并等待全部完成
来源：http://iyq.sjlbkw.cn

Py:   asyncio.gather(*tasks)
来源：http://ajs.xziqi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://iob.316326.xyz

JS:   await Promise.all(tasks)
来源：http://dnv.jqgfzy.top

TS:   await Promise.all(tasks)
来源：http://waq.zhongyouzk.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eza.gotoacloud.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zgj.zhaomingkeji.xyz

Ruby: threads.map(&:join)
来源：http://syf.zdqjudy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://sjx.andypj.xyz

[O06] 使用进程池
来源：http://wlk.jinghuilouyu.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vvn.hongshengwenyu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://yiu.tanke756.top

JS:   // child_process / cluster 模块
来源：http://wdh.redwolf501.top

TS:   // child_process / cluster 模块
来源：http://dqf.redwolf501.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bli.ivvv.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cko.smart0.xyz

Ruby: // fork 块
来源：http://ejm.jlsjyb.cn

C#:   Parallel.For
来源：http://bmz.c1oappe.top

================================================================================
来源：http://rap.xuanzx.com

P. 常用工具函数
来源：http://mit.fanxiaobao.xyz

================================================================================
来源：http://tbh.zdqjudy.top

[P01] 生成 UUID
来源：http://jef.yangfankeji.com

Py:   str(uuid.uuid4())
来源：http://lsg.hammf.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nru.yj202588.top

JS:   crypto.randomUUID()
来源：http://ejk.sxryk.cn

TS:   crypto.randomUUID()
来源：http://leg.guowangkeji.top

Java: UUID.randomUUID().toString()
来源：http://glx.hysaishi.cn

Go:   // 用 github.com/google/uuid
来源：http://fxq.yangfankeji.com

Ruby: SecureRandom.uuid
来源：http://toj.cdnleiting.top

C#:   Guid.NewGuid().ToString()
来源：http://pws.pengpengdd.cyou

[P02] MD5 / SHA256 摘要
来源：http://sdz.tanke756.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dvf.zhoulong.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://cxf.9152youxi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fhq.chenzaomai.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gis.yuanzhike.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://scg.zhiwuduotai.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fpn.yongpay.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://vrj.ppjwa.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://aik.hfpthk.cn

[P03] 生成短随机字符串
来源：http://cgd.hysaishi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ywn.zdbjq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bcn.jqgfzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wjy.cqqwz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lsp.0kj1m.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yug.zhiwuduotai.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://afx.xinyue.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://aoq.quarkkingdee.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://qfz.hysaishi.cn

[P04] 求长度
来源：http://enr.gotoacloud.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://iwf.birdmap.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fuy.chenlongwang.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vow.quarkkingdee.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kul.c1oappe.top

Java: list.size();  map.size();  s.length()
来源：http://dfm.tian-w.cn

Go:   len(arr);  len(m)
来源：http://jrw.yuanzhike.top

Ruby: x.length;  x.size
来源：http://lhm.haohaochexian.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://cnx.tarul.cn

[P05] 判断两个对象内容是否相等
来源：http://jte.yonumen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://tqs.sysykeji.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://efp.nwbrower.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://puv.kuanghao11.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://apy.redwolf501.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xhg.mhx1999.top

Go:   reflect.DeepEqual(a, b)
来源：http://emm.zhongyouzk.top

Ruby: a == b
来源：http://ihw.svipenyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wnt.fzhhl.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://tbn.yuxming.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://apy.guowangkeji.top

PHP:  if (empty($x)) {}
来源：http://ncn.xingfuxueyuan.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://auo.shangyingyoupin.top

TS:   if (x == null) {}
来源：http://zex.iojbl.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://iqf.guowangkeji.top

Go:   if x == nil {}
来源：http://kpw.ybcxt.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mnj.gotoacloud.top

C#:   if (x is null) {}
来源：http://gue.fktsv.cn

[P07] 防抖与节流
来源：http://exb.hnxiangtu.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://dzx.zhixingplan.top

PHP:  // 手写时间戳比较
来源：http://lvs.sysykeji.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jwb.jqgfzy.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gge.fengsongda.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nye.birdmap.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://iem.cqqwz.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nut.vehdjk.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://kiy.hysaishi.cn

[P08] 处理浮点精度问题
来源：http://dxs.sxryk.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mfa.nanxuanxn.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ste.yuxming.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mku.jiagoushi.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eyy.hysaishi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://fin.mhx1999.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bje.yuanzhike.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://eln.tarul.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hne.shanyushiyangkeji.top

================================================================================
来源：http://tpd.nwbrower.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://syx.vqdsnc.cn

================================================================================
来源：http://tsm.aizwys.cn

[Q01] 创建表
来源：http://jty.sxryk.cn

CREATE TABLE users (
来源：http://abg.chenlongwang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ubn.mhx1999.top

name VARCHAR(50) NOT NULL,
来源：http://fwu.ivvv.top

email VARCHAR(100) UNIQUE,
来源：http://dbs.yangfankeji.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://unw.ybcxt.top

);
来源：http://nji.yj202588.top

[Q02] 创建带外键的表
来源：http://lrq.jinqigufen.top

CREATE TABLE orders (
来源：http://ayc.xuanzx.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bcj.hfpthk.cn

user_id INT NOT NULL,
来源：http://idq.yanxiufei.cn

amount DECIMAL(10, 2),
来源：http://wgi.52xcode.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uld.mhx1999.top

);
来源：http://jde.xuetiantiany.cn

[Q03] 增加列
来源：http://zjm.epnwcf.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://okt.bjfxy.top

[Q04] 修改列类型
来源：http://okp.hesvh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ypi.feifeiyinyue.top

[Q05] 重命名列
来源：http://jnk.jqgfzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bai.yongpay.top

[Q06] 删除列
来源：http://auy.haohaochexian.top

ALTER TABLE users DROP COLUMN age;
来源：http://uvd.zhiwuduotai.top

[Q07] 删除表
来源：http://sel.sjlbkw.cn

DROP TABLE IF EXISTS orders;
来源：http://ath.daxiang520.top

[Q08] 创建普通索引
来源：http://xzw.xuetiantiany.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://yuj.yanxiufei.cn

[Q09] 创建唯一索引
来源：http://twz.hfpthk.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://azn.jinghuilouyu.cn

[Q10] 插入单行
来源：http://bfl.sxryk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dca.dianchejie.cn

[Q11] 一次插入多行
来源：http://ffp.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nha.gaohongyu789.top

[Q12] 插入后取自增 ID
来源：http://qjq.sufxvd.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ddc.jqgufenzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kzt.jinqigufen.top

[Q13] 忽略重复插入
来源：http://gtq.hywenlv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mev.ctjpmb.com

[Q14] 存在则更新（upsert）
来源：http://msu.shanyushiyangtech.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bvp.tanke756.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dzk.chenlongwang.top

[Q15] 查询全部
来源：http://ysd.aibaodan.cn

SELECT * FROM users;
来源：http://ael.shanyushiyangtech.top

[Q16] 查询指定列
来源：http://rhl.zdbjq.cn

SELECT id, name FROM users;
来源：http://kdh.shangyingyoupin.top

[Q17] 条件查询
来源：http://ulb.sjlbkw.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://obo.meibo888.top

[Q18] 模糊匹配
来源：http://kpb.zdqjudy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wvb.xuanzx.com

[Q19] 范围查询
来源：http://rwa.yuanzhike.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gtw.tianlin.xyz

[Q20] IN 列表
来源：http://dtn.ydzc1.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bub.jiagoushi.top

[Q21] 空值判断
来源：http://ldy.9152youxi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://zzh.hnxiangtu.top

[Q22] 排序
来源：http://cmn.zhengqikj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://vvy.shanyushiyangkeji.top

[Q23] 分页
来源：http://qvl.meibo888.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://spo.xuetiantiany.cn

[Q24] 去重
来源：http://jtb.gaohongyu789.top

SELECT DISTINCT city FROM users;
来源：http://qnq.hnqzz.top

[Q25] 只取前 N 条
来源：http://sfh.zdbjq.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nbn.fengsongda.top

[Q26] 计数
来源：http://ony.0kj1m.cn

SELECT COUNT(*) FROM users;
来源：http://ani.sweek.top

[Q27] 条件计数
来源：http://vpb.gzhubu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://eyk.nwbrower.top

[Q28] 求和与平均
来源：http://trn.xingfuxueyuan.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://duw.bjfxy.top

[Q29] 最大最小值
来源：http://lkj.zdqjudy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://hgs.tian-w.cn

[Q30] 分组统计
来源：http://mbm.fengsongda.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bjn.wangdashe.top

[Q31] 分组后过滤
来源：http://ooh.quarkkingdee.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tul.meibo888.top

[Q32] 分组拼接字符串
来源：http://wvu.52xcode.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ilt.yfazqb.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lcy.chenzaomai.com

[Q33] 多列分组
来源：http://soh.xylfe.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mvz.xziqi.cn

[Q34] 每组取第一条
来源：http://ubz.aizwys.cn

SELECT * FROM (
来源：http://kkv.zdbjq.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://dke.haohaochexian.top

) t WHERE rn = 1;
来源：http://ypt.yj20258.top

[Q35] 内连接
来源：http://vel.ydzc1.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nrt.bjfxy.top

[Q36] 左连接
来源：http://woh.xylfe.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://myc.jinghuilouyu.cn

[Q37] 右连接
来源：http://qre.ydzc1.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://djl.ybcxt.top

[Q38] 全外连接（PostgreSQL）
来源：http://oxw.jinqigufen.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pvg.zhengqikj.top

[Q39] 自连接（查上下级）
来源：http://hzh.zhongyouzk.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://shi.tanke756.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qpw.pycfn.com

[Q40] 交叉连接（笛卡尔积）
来源：http://toj.hysaishi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eyl.guowangkeji.top

[Q41] 多表连接
来源：http://zfl.nwbrower.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://swx.yj20258.top

JOIN users u ON u.id = o.user_id
来源：http://kxn.jqgfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://dop.xuanzx.com

[Q42] 连接条件附加过滤
来源：http://otu.aizwys.cn

SELECT u.name, o.amount FROM users u
来源：http://vqt.yfazqb.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xsw.ybcxt.top

[Q43] 标量子查询
来源：http://fub.fzhhl.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qov.yangfankeji.com

[Q44] IN 子查询
来源：http://twr.9152youxi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fuo.chenzaomai.com

[Q45] EXISTS 判断存在
来源：http://kid.daria6918.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ncc.tianlin.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://bwy.jqgufenzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://owe.daxiang520.top

[Q47] 与平均值比较
来源：http://gll.tanke756.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yze.sufxvd.cn

[Q48] CTE 公用表表达式
来源：http://qhh.zhongyouzk.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fek.hcnkem.com

SELECT * FROM t WHERE c > 5;
来源：http://mak.bjfxy.top

[Q49] 更新单行
来源：http://gzy.cashguo.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nrj.hesvh.cn

[Q50] 批量更新
来源：http://lsh.yonumen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nqm.wangshuangyany.cn

[Q51] 用子查询更新
来源：http://mdj.havefunace.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qpp.gotoacloud.top

[Q52] 删除指定行
来源：http://atc.yanxiufei.cn

DELETE FROM users WHERE id = 10;
来源：http://wfl.iojbl.cn

[Q53] 按条件删除
来源：http://qjq.cdnleiting.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zxq.yonumen.top

[Q54] 清空表
来源：http://cty.ctjpmb.com

TRUNCATE TABLE logs;
来源：http://qvi.jqgfzy.top

[Q55] 排名（并列占位）
来源：http://qtn.gogol.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yox.cdnleiting.top

[Q56] 密集排名（并列不占位）
来源：http://iel.wangshuangyany.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qij.guowangkeji.top

[Q57] 行号
来源：http://uon.snrcjt.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cmj.meibo888.top

[Q58] 累计求和
来源：http://jcj.shanyushiyangtech.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aij.cucudq.cn

[Q59] 分组内累计
来源：http://rel.hcnkem.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bhs.wangdashe.top

[Q60] 取上一行 / 下一行
来源：http://ruv.svipenyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hdd.jianghu66.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hdm.quarkkingdee.top

[Q61] 移动平均
来源：http://byh.daria6918.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://swq.xingfuxueyuan.xyz

[Q62] 分组占比
来源：http://yjh.vehdjk.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ssf.hcnkem.com

[Q63] 开启事务
来源：http://dkm.fzhhl.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jai.sxryk.cn

[Q64] 提交事务
来源：http://bso.cdnleiting.top

COMMIT;
来源：http://uzb.smart0.xyz

[Q65] 回滚事务
来源：http://qka.tianlin.xyz

ROLLBACK;
来源：http://umm.yj202588.top

[Q66] 行锁查询
来源：http://uxu.cdnleiting.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uur.tanke756.top

[Q67] 设置隔离级别
来源：http://gjy.svipenyu.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kyz.jyoumei.cn

[Q68] 保存点
来源：http://bkt.zdbjq.cn

SAVEPOINT sp1;
来源：http://lgl.meibo888.top

ROLLBACK TO sp1;
来源：http://wfn.cheryme.top

[Q69] 查看执行计划
来源：http://jzv.havefunace.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ynr.gzhubu.top

[Q70] 更新统计信息
来源：http://dxy.snrcjt.cn

ANALYZE TABLE users;
来源：http://dsx.daxiang520.top

[Q71] 查看建表语句
来源：http://tsa.9152youxi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uhf.jianghu66.top

[Q72] 查看索引
来源：http://ort.hongshengwenyu.top

SHOW INDEX FROM users;
来源：http://xqc.cucudq.cn

[Q73] 查看表状态
来源：http://cqe.bbcook.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rke.dashuyun.cn

[Q74] 强制使用索引
来源：http://kek.xingfuxueyuan.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qfb.havefunace.top

[Q75] 日期格式化
来源：http://yqf.yuxming.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tyo.cdnleiting.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pio.xingfuxueyuan.xyz

[Q76] 按天统计
来源：http://syi.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kji.jianghu66.top

[Q77] 时间加减
来源：http://hhr.sufxvd.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zeg.haohaochexian.top

[Q78] 当前时间
来源：http://vcp.ywan-chungtsiang.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jlj.hcnkem.com

[Q79] 字符串拼接
来源：http://ijd.fktsv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cad.kuanghao11.cn

[Q80] 字符串截取
来源：http://xxp.pengpengdd.cyou

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rzi.kuanghao11.cn

[Q81] 字符串替换
来源：http://rqq.xylfe.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xbk.pycfn.com

[Q82] 字符长度与字节长度
来源：http://yco.chenlongwang.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://vdn.jiagoushi.top

[Q83] 大小写转换
来源：http://aeq.chenzaomai.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vby.sweek.top

[Q84] 去除首尾空格
来源：http://xfz.zhongyouzk.top

SELECT TRIM(name) FROM users;
来源：http://jav.nwbrower.top

[Q85] 数值取整
来源：http://qoy.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rmq.zhoulong.xyz

[Q86] 读取 JSON 字段
来源：http://mbv.fanxiaobao.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qlq.zhoulong.xyz

[Q87] JSON 字段做条件
来源：http://clt.iojbl.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rmn.xinyue.icu

[Q88] 行转列（条件聚合）
来源：http://ggo.fktsv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vpn.hnqzz.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cdm.shzxlz.cn

[Q89] 判断表是否存在
来源：http://yjm.jlsjyb.cn


<!-- 参考信息 -->