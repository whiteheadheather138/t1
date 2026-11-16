代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ota.chenlongwang.top

Ruby: # 用 Fiber 或 async gem
来源：http://rrj.hongshengwenyu.top

C#:   async Task F() { await G(); }
来源：http://ire.jqgfzy.top

[O05] 并发执行并等待全部完成
来源：http://lru.hcnkem.com

Py:   asyncio.gather(*tasks)
来源：http://lib.316326.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nsq.yj20258888.top

JS:   await Promise.all(tasks)
来源：http://mft.bjfxy.top

TS:   await Promise.all(tasks)
来源：http://sig.jiagoushi.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://msj.fanxiaobao.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pva.jlsjyb.cn

Ruby: threads.map(&:join)
来源：http://vqb.gaohongyu789.top

C#:   await Task.WhenAll(t1, t2)
来源：http://hem.mhx1999.top

[O06] 使用进程池
来源：http://pxq.xziqi.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qkl.nanxinkj.top

PHP:  // pcntl_fork 或多进程队列
来源：http://hxc.hywenlv.cn

JS:   // child_process / cluster 模块
来源：http://tpa.vehdjk.com

TS:   // child_process / cluster 模块
来源：http://dml.hongshengwenyu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kfs.redwolf501.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ldj.xziqi.cn

Ruby: // fork 块
来源：http://knh.fehbvm.com

C#:   Parallel.For
来源：http://cvr.cdnleiting.top

================================================================================
来源：http://ngu.vqdsnc.cn

P. 常用工具函数
来源：http://ale.chenzaomai.com

================================================================================
来源：http://kam.cucudq.cn

[P01] 生成 UUID
来源：http://nau.hnxiangtu.top

Py:   str(uuid.uuid4())
来源：http://fsh.bbcook.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://for.zycfv.cn

JS:   crypto.randomUUID()
来源：http://wer.jinghuilouyu.cn

TS:   crypto.randomUUID()
来源：http://itn.yfazqb.com

Java: UUID.randomUUID().toString()
来源：http://kii.sysykeji.top

Go:   // 用 github.com/google/uuid
来源：http://ois.sjlbkw.cn

Ruby: SecureRandom.uuid
来源：http://icy.hfpthk.cn

C#:   Guid.NewGuid().ToString()
来源：http://lsv.yfazqb.com

[P02] MD5 / SHA256 摘要
来源：http://ijg.snrcjt.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fvs.hammf.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://pbw.hfpthk.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://umr.chenjidiqi.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wnk.ydzc1.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yvb.daria6918.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://pxh.0kj1m.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://jgk.yongpay.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://btm.316326.xyz

[P03] 生成短随机字符串
来源：http://srx.yj20258.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://daz.c1oappe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://eep.hongshengwenyu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lqo.fzhhl.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oqg.fktsv.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ncc.zhaomingkeji.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cmn.9152youxi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://spo.shanyushiyangtech.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mga.daria6918.cn

[P04] 求长度
来源：http://vno.fehbvm.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://oyy.316326.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dol.chenjidiqi.icu

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hla.zhiwuduotai.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ysq.xylfe.cn

Java: list.size();  map.size();  s.length()
来源：http://nxj.ctjpmb.com

Go:   len(arr);  len(m)
来源：http://gax.svipenyu.cn

Ruby: x.length;  x.size
来源：http://cvv.yongpay.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ixl.fktsv.cn

[P05] 判断两个对象内容是否相等
来源：http://grm.ctjpmb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://bsw.gogol.net.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://knl.jlsjyb.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vvx.hywenlv.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dvi.bjfxy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://trx.ehwqpu.com

Go:   reflect.DeepEqual(a, b)
来源：http://zud.zhiwuduotai.top

Ruby: a == b
来源：http://cji.vehdjk.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://sah.yangfankeji.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nef.sysykeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://his.xuetiantiany.cn

PHP:  if (empty($x)) {}
来源：http://zxt.jqgfzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uaw.vehdjk.com

TS:   if (x == null) {}
来源：http://bmt.gotoacloud.top

Java: if (x == null || x.isEmpty()) {}
来源：http://grx.yj202588.top

Go:   if x == nil {}
来源：http://sux.ehwqpu.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pip.xinyue.icu

C#:   if (x is null) {}
来源：http://rnd.ydjk.org.cn

[P07] 防抖与节流
来源：http://adr.yj20258888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xaj.gaohongyu789.top

PHP:  // 手写时间戳比较
来源：http://rlb.xinyue.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xfp.hcnkem.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://faw.pengpengdd.cyou

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://kgs.ppjwa.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://yke.zycfv.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://dnz.zhengqikj.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rqk.hammf.cn

[P08] 处理浮点精度问题
来源：http://ere.yangfankeji.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://klh.gaohongyu789.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://uwr.yueranfly.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://luf.bjfxy.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lug.hcnkem.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://rnk.guowangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://aed.zycfv.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zys.cheryme.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xzq.c1oappe.top

================================================================================
来源：http://epr.zhijiandao.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://umy.havefunace.top

================================================================================
来源：http://vve.sweek.top

[Q01] 创建表
来源：http://rrv.jinqigufen.top

CREATE TABLE users (
来源：http://viu.jinqigufen.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://cax.wangdashe.top

name VARCHAR(50) NOT NULL,
来源：http://cup.gaohongyu789.top

email VARCHAR(100) UNIQUE,
来源：http://yth.yanxiufei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yrg.hesvh.cn

);
来源：http://lkm.yanxiufei.cn

[Q02] 创建带外键的表
来源：http://ejv.yongpay.top

CREATE TABLE orders (
来源：http://qup.zhengqikj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wrn.bjfxy.top

user_id INT NOT NULL,
来源：http://jbi.tian-w.cn

amount DECIMAL(10, 2),
来源：http://xzo.jinqigfzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tgq.yj20258.top

);
来源：http://frc.snrcjt.cn

[Q03] 增加列
来源：http://kyy.zhixingplan.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fgq.c1oappe.top

[Q04] 修改列类型
来源：http://mqt.zhoulong.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cjm.dianchejie.cn

[Q05] 重命名列
来源：http://kld.nanxuanxn.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dyf.yangfankeji.com

[Q06] 删除列
来源：http://aez.daria6918.cn

ALTER TABLE users DROP COLUMN age;
来源：http://pkx.chenjidiqi.icu

[Q07] 删除表
来源：http://dpx.ctjpmb.com

DROP TABLE IF EXISTS orders;
来源：http://cbj.hesvh.cn

[Q08] 创建普通索引
来源：http://woa.dashuyun.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ydm.zhiwuduotai.top

[Q09] 创建唯一索引
来源：http://pos.wangshuangyany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jka.shanyushiyangkeji.top

[Q10] 插入单行
来源：http://duw.epnwcf.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vbk.nwbrower.top

[Q11] 一次插入多行
来源：http://cvu.tianlin.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zzi.xylfe.cn

[Q12] 插入后取自增 ID
来源：http://zyd.xylfe.cn

INSERT INTO users (name) VALUES ('C');
来源：http://juy.sxryk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ymi.ehwqpu.com

[Q13] 忽略重复插入
来源：http://mlg.zhijiandao.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hut.xylfe.cn

[Q14] 存在则更新（upsert）
来源：http://tmm.xuanzx.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://lpz.jinqigufen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://keu.birdmap.top

[Q15] 查询全部
来源：http://fat.vqdsnc.cn

SELECT * FROM users;
来源：http://ars.zhiwuduotai.top

[Q16] 查询指定列
来源：http://atj.yuxming.cn

SELECT id, name FROM users;
来源：http://pks.zhiwuduotai.top

[Q17] 条件查询
来源：http://kvf.yj202588.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ccm.mhx1999.top

[Q18] 模糊匹配
来源：http://wkl.birdmap.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://sqy.nanxinkj.top

[Q19] 范围查询
来源：http://fpv.iojbl.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://elk.hfpthk.cn

[Q20] IN 列表
来源：http://jkh.guannengcc.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://sjz.aibaodan.cn

[Q21] 空值判断
来源：http://mtr.meibo888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://hoz.fktsv.cn

[Q22] 排序
来源：http://yfy.shanyushiyangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cqi.cashguo.top

[Q23] 分页
来源：http://qsk.shzxlz.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lxf.aizwys.cn

[Q24] 去重
来源：http://rsd.jlsjyb.cn

SELECT DISTINCT city FROM users;
来源：http://swk.tianlin.xyz

[Q25] 只取前 N 条
来源：http://bty.snrcjt.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vmh.hfpthk.cn

[Q26] 计数
来源：http://zhk.zhixingplan.top

SELECT COUNT(*) FROM users;
来源：http://xdj.nanxinkj.top

[Q27] 条件计数
来源：http://vnf.0kj1m.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://duc.ybcxt.top

[Q28] 求和与平均
来源：http://qje.xingfuxueyuan.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qlv.wangshuangyany.cn

[Q29] 最大最小值
来源：http://aqi.sysykeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ekc.shuidangran.top

[Q30] 分组统计
来源：http://zep.shangyingyoupin.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tzy.sufxvd.cn

[Q31] 分组后过滤
来源：http://qmg.havefunace.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yvt.redwolf501.top

[Q32] 分组拼接字符串
来源：http://kuu.sjlbkw.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qvl.sjlbkw.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ena.chenzaomai.com

[Q33] 多列分组
来源：http://vdt.xuetiantiany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://yif.vehdjk.com

[Q34] 每组取第一条
来源：http://adm.feifeiyinyue.top

SELECT * FROM (
来源：http://wsq.cheryme.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lrf.snrcjt.cn

) t WHERE rn = 1;
来源：http://nux.mhx1999.top

[Q35] 内连接
来源：http://zuv.hesvh.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zyy.gzhubu.top

[Q36] 左连接
来源：http://cwd.nwbrower.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zsw.yvedp.cn

[Q37] 右连接
来源：http://tsh.chenlongwang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bkm.shanyushiyangtech.top

[Q38] 全外连接（PostgreSQL）
来源：http://kbi.uphjek.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jpp.zdqjudy.top

[Q39] 自连接（查上下级）
来源：http://obj.aizwys.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wbr.chenjidiqi.icu

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bxw.fengsongda.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hdf.sysykeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://sip.sweek.top

[Q41] 多表连接
来源：http://uju.wangdashe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ich.havefunace.top

JOIN users u ON u.id = o.user_id
来源：http://yms.fengsongda.top

JOIN products p ON p.id = o.product_id;
来源：http://gkt.cucudq.cn

[Q42] 连接条件附加过滤
来源：http://afc.hongshengwenyu.top

SELECT u.name, o.amount FROM users u
来源：http://tdc.wangdashe.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://msp.xinyue.icu

[Q43] 标量子查询
来源：http://igv.iojbl.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lux.0kj1m.cn

[Q44] IN 子查询
来源：http://ora.bbcook.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ezk.epnwcf.com

[Q45] EXISTS 判断存在
来源：http://zmm.gotoacloud.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yqt.yj202588.top

[Q46] NOT EXISTS 判断不存在
来源：http://soq.zhiwuduotai.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://crz.ppjwa.cn

[Q47] 与平均值比较
来源：http://lxr.cqqwz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yze.ehwqpu.com

[Q48] CTE 公用表表达式
来源：http://lie.snrcjt.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lnc.zhengqikj.top

SELECT * FROM t WHERE c > 5;
来源：http://ury.birdmap.top

[Q49] 更新单行
来源：http://sdx.zdbjq.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sqp.ydzc1.top

[Q50] 批量更新
来源：http://ote.9152youxi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://iwp.sysykeji.top

[Q51] 用子查询更新
来源：http://brl.dashuyun.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ejl.chenjidiqi.icu

[Q52] 删除指定行
来源：http://beo.zhoulong.xyz

DELETE FROM users WHERE id = 10;
来源：http://ahl.sufxvd.cn

[Q53] 按条件删除
来源：http://bpr.ywan-chungtsiang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nwv.sysykeji.top

[Q54] 清空表
来源：http://hud.c1oappe.top

TRUNCATE TABLE logs;
来源：http://fiy.daria6918.cn

[Q55] 排名（并列占位）
来源：http://dlf.zhiwuduotai.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://aro.daria6918.cn

[Q56] 密集排名（并列不占位）
来源：http://rre.fzhhl.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://txu.ydjk.org.cn

[Q57] 行号
来源：http://rzg.ydjk.org.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xbq.ywan-chungtsiang.top

[Q58] 累计求和
来源：http://vht.jinyuanbaomall.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zvy.yuxming.cn

[Q59] 分组内累计
来源：http://xqe.kuanghao11.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qpq.kuanghao11.cn

[Q60] 取上一行 / 下一行
来源：http://fmg.cashguo.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jif.gogol.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tai.hnxiangtu.top

[Q61] 移动平均
来源：http://rcf.52xcode.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zbm.xylfe.cn

[Q62] 分组占比
来源：http://lkh.xuetiantiany.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://cmh.hnxiangtu.top

[Q63] 开启事务
来源：http://lac.snrcjt.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://khp.uphjek.com

[Q64] 提交事务
来源：http://tbm.zhongyouzk.top

COMMIT;
来源：http://jnt.ydzc1.top

[Q65] 回滚事务
来源：http://gea.chenjidiqi.icu

ROLLBACK;
来源：http://fjz.zdqjudy.top

[Q66] 行锁查询
来源：http://nvi.gotoacloud.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qvm.haohaochexian.top

[Q67] 设置隔离级别
来源：http://hjz.aizwys.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xba.gaohongyu789.top

[Q68] 保存点
来源：http://xrm.ivvv.top

SAVEPOINT sp1;
来源：http://cjv.9152youxi.cn

ROLLBACK TO sp1;
来源：http://ccs.wangdashe.top

[Q69] 查看执行计划
来源：http://bin.tian-w.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zcm.xingfuxueyuan.xyz

[Q70] 更新统计信息
来源：http://msi.nanxinkj.top

ANALYZE TABLE users;
来源：http://czr.zdqjudy.top

[Q71] 查看建表语句
来源：http://ihi.jinghuilouyu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mez.shuidangran.top

[Q72] 查看索引
来源：http://omo.chenlongwang.top

SHOW INDEX FROM users;
来源：http://oyu.birdmap.top

[Q73] 查看表状态
来源：http://nsa.daria6918.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://hea.yueranfly.top

[Q74] 强制使用索引
来源：http://egw.fzhhl.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vrg.pycfn.com

[Q75] 日期格式化
来源：http://zbn.ydjk.org.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xju.birdmap.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://had.hnxiangtu.top

[Q76] 按天统计
来源：http://hwa.cqqwz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yqg.chenzaomai.com

[Q77] 时间加减
来源：http://fch.shanyushiyangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zzs.yueranfly.top

[Q78] 当前时间
来源：http://rdl.cheryme.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pfo.nanxinkj.top

[Q79] 字符串拼接
来源：http://cnq.chenjidiqi.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://quc.ivvv.top

[Q80] 字符串截取
来源：http://uny.uphjek.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jdq.guowangkeji.top

[Q81] 字符串替换
来源：http://iuw.jyoumei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vaf.yj20258.top

[Q82] 字符长度与字节长度
来源：http://vmx.fktsv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oqa.feifeiyinyue.top

[Q83] 大小写转换
来源：http://yoz.sweek.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://voa.gotoacloud.top

[Q84] 去除首尾空格
来源：http://tnp.316326.xyz

SELECT TRIM(name) FROM users;
来源：http://dsm.9152youxi.cn

[Q85] 数值取整
来源：http://orm.daxiang520.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lrd.zycfv.cn

[Q86] 读取 JSON 字段
来源：http://ojo.jlsjyb.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://irh.cucudq.cn

[Q87] JSON 字段做条件
来源：http://ntf.chenlongwang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lcl.xylfe.cn

[Q88] 行转列（条件聚合）
来源：http://qsv.gogol.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pok.fehbvm.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zsh.gaohongyu789.top

[Q89] 判断表是否存在
来源：http://tyn.yvedp.cn


<!-- 参考信息 -->