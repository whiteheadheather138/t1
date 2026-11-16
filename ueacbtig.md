代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://psw.wangdashe.top

Ruby: # 用 Fiber 或 async gem
来源：http://btl.shanyushiyangtech.top

C#:   async Task F() { await G(); }
来源：http://dyb.zhoulong.xyz

[O05] 并发执行并等待全部完成
来源：http://evt.smart0.xyz

Py:   asyncio.gather(*tasks)
来源：http://ymk.gogol.net.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://qdo.yj20258888.top

JS:   await Promise.all(tasks)
来源：http://eod.hesvh.cn

TS:   await Promise.all(tasks)
来源：http://hlr.hfpthk.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://izv.yanxiufei.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ohw.nanxinkj.top

Ruby: threads.map(&:join)
来源：http://pys.pycfn.com

C#:   await Task.WhenAll(t1, t2)
来源：http://tjx.zhaomingkeji.xyz

[O06] 使用进程池
来源：http://hdf.uphjek.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://tiq.ydzc1.top

PHP:  // pcntl_fork 或多进程队列
来源：http://cel.xingfuxueyuan.xyz

JS:   // child_process / cluster 模块
来源：http://jyh.hammf.cn

TS:   // child_process / cluster 模块
来源：http://psp.daria6918.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bui.fehbvm.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eiq.cqqwz.cn

Ruby: // fork 块
来源：http://pif.chenlongwang.top

C#:   Parallel.For
来源：http://uhw.nanxuanxn.top

================================================================================
来源：http://suy.shangyingyoupin.top

P. 常用工具函数
来源：http://mrc.ctjpmb.com

================================================================================
来源：http://yqs.wangdashe.top

[P01] 生成 UUID
来源：http://arx.yj20258.top

Py:   str(uuid.uuid4())
来源：http://vqn.zdqjudy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://opc.zhongyouzk.top

JS:   crypto.randomUUID()
来源：http://gdy.kuanghao11.cn

TS:   crypto.randomUUID()
来源：http://qvj.hnxiangtu.top

Java: UUID.randomUUID().toString()
来源：http://ccn.hnxiangtu.top

Go:   // 用 github.com/google/uuid
来源：http://xbo.vqdsnc.cn

Ruby: SecureRandom.uuid
来源：http://kaf.ydjk.org.cn

C#:   Guid.NewGuid().ToString()
来源：http://qxr.jianghu66.top

[P02] MD5 / SHA256 摘要
来源：http://xxl.shuidangran.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://nct.yvedp.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://vso.ydzc1.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mvk.hcnkem.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ohr.shuidangran.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hzc.gaohongyu789.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://owl.dianchejie.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://svk.birdmap.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://nts.zdbjq.cn

[P03] 生成短随机字符串
来源：http://tad.xuanzx.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nrx.nanxuanxn.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rhp.yfazqb.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rht.yuxming.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jtg.yvedp.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://fob.yuxming.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ytg.svipenyu.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bqz.daria6918.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://aew.fzhhl.top

[P04] 求长度
来源：http://syw.chenlongwang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://daq.kuanghao11.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://epj.guannengcc.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zas.9152youxi.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xdm.shanyushiyangkeji.top

Java: list.size();  map.size();  s.length()
来源：http://drq.aibaodan.cn

Go:   len(arr);  len(m)
来源：http://oow.gogol.net.cn

Ruby: x.length;  x.size
来源：http://wxr.52xcode.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ped.zhijiandao.cn

[P05] 判断两个对象内容是否相等
来源：http://hec.yonumen.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://pga.fengsongda.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mtt.aibaodan.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nma.ydjk.org.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://czf.hcnkem.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kza.zhixingplan.top

Go:   reflect.DeepEqual(a, b)
来源：http://txb.shangyingyoupin.top

Ruby: a == b
来源：http://zgf.jqgufenzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ytf.jinqigufen.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rky.sysykeji.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zyv.nanxuanxn.top

PHP:  if (empty($x)) {}
来源：http://zcp.xylfe.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://adf.cashguo.top

TS:   if (x == null) {}
来源：http://wpd.shuidangran.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ybu.0kj1m.cn

Go:   if x == nil {}
来源：http://xpj.hfpthk.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://lik.yonumen.top

C#:   if (x is null) {}
来源：http://ocs.fanxiaobao.xyz

[P07] 防抖与节流
来源：http://law.tanke756.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nmk.zhiwuduotai.top

PHP:  // 手写时间戳比较
来源：http://vta.ybcxt.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://apz.hesvh.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zyg.pycfn.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://vlb.guowangkeji.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ejy.feifeiyinyue.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://nby.ydjk.org.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ctm.xuetiantiany.cn

[P08] 处理浮点精度问题
来源：http://fcs.tanke756.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bpy.svipenyu.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mij.xylfe.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hpg.sjlbkw.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fom.tianlin.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tiy.ydzc1.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://aei.epnwcf.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ayl.mhx1999.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://hrr.jinyuanbaomall.cn

================================================================================
来源：http://xzb.yueranfly.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://xkf.jinqigfzy.top

================================================================================
来源：http://cmj.jyoumei.cn

[Q01] 创建表
来源：http://tgh.fehbvm.com

CREATE TABLE users (
来源：http://vqt.yfazqb.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yav.cqqwz.cn

name VARCHAR(50) NOT NULL,
来源：http://trv.hnxiangtu.top

email VARCHAR(100) UNIQUE,
来源：http://hnv.fengsongda.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pvi.birdmap.top

);
来源：http://htg.yangfankeji.com

[Q02] 创建带外键的表
来源：http://gjl.ybcxt.top

CREATE TABLE orders (
来源：http://jeq.tanke756.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://btp.zhixingplan.top

user_id INT NOT NULL,
来源：http://wad.shzxlz.cn

amount DECIMAL(10, 2),
来源：http://gha.mhx1999.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wgf.zhaomingkeji.xyz

);
来源：http://hps.nanxinkj.top

[Q03] 增加列
来源：http://phz.yfazqb.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ssk.fengsongda.top

[Q04] 修改列类型
来源：http://uzr.fanxiaobao.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://eqx.tianlin.xyz

[Q05] 重命名列
来源：http://hfp.yueranfly.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oil.xuetiantiany.cn

[Q06] 删除列
来源：http://mcv.chenjidiqi.icu

ALTER TABLE users DROP COLUMN age;
来源：http://hqx.fehbvm.com

[Q07] 删除表
来源：http://baa.shzxlz.cn

DROP TABLE IF EXISTS orders;
来源：http://kik.zdbjq.cn

[Q08] 创建普通索引
来源：http://yjc.jinqigufen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://kgr.chenzaomai.com

[Q09] 创建唯一索引
来源：http://zbh.hywenlv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eio.wangshuangyany.cn

[Q10] 插入单行
来源：http://trj.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kzm.yueranfly.top

[Q11] 一次插入多行
来源：http://gzd.jyoumei.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kri.cashguo.top

[Q12] 插入后取自增 ID
来源：http://mun.zhiwuduotai.top

INSERT INTO users (name) VALUES ('C');
来源：http://vxk.guannengcc.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nbo.hnqzz.top

[Q13] 忽略重复插入
来源：http://fwp.fzhhl.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://krt.yonumen.top

[Q14] 存在则更新（upsert）
来源：http://ouq.jiagoushi.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hyu.fengsongda.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://dgv.hfpthk.cn

[Q15] 查询全部
来源：http://pnv.ehwqpu.com

SELECT * FROM users;
来源：http://nav.jinghuilouyu.cn

[Q16] 查询指定列
来源：http://srj.kuanghao11.cn

SELECT id, name FROM users;
来源：http://uke.xziqi.cn

[Q17] 条件查询
来源：http://qtx.jqgufenzy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://uae.jiagoushi.top

[Q18] 模糊匹配
来源：http://fev.yj20258.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://aao.hnqzz.top

[Q19] 范围查询
来源：http://yye.chenlongwang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nbf.sjlbkw.cn

[Q20] IN 列表
来源：http://bhm.nwbrower.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gaa.vehdjk.com

[Q21] 空值判断
来源：http://hmg.chenzaomai.com

SELECT * FROM users WHERE email IS NULL;
来源：http://ugs.tarul.cn

[Q22] 排序
来源：http://rog.aizwys.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mjv.birdmap.top

[Q23] 分页
来源：http://czn.hcnkem.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pco.9152youxi.cn

[Q24] 去重
来源：http://vtq.pycfn.com

SELECT DISTINCT city FROM users;
来源：http://qwy.kuanghao11.cn

[Q25] 只取前 N 条
来源：http://gui.bjfxy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fgr.bbcook.cn

[Q26] 计数
来源：http://bfu.guannengcc.top

SELECT COUNT(*) FROM users;
来源：http://rsm.bbcook.cn

[Q27] 条件计数
来源：http://yxq.cucudq.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uuz.ywan-chungtsiang.top

[Q28] 求和与平均
来源：http://kzn.fehbvm.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zoz.havefunace.top

[Q29] 最大最小值
来源：http://lus.zhengqikj.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ggz.zycfv.cn

[Q30] 分组统计
来源：http://ccv.smart0.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://fly.fktsv.cn

[Q31] 分组后过滤
来源：http://kog.nanxinkj.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cyg.pycfn.com

[Q32] 分组拼接字符串
来源：http://wxg.yfazqb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://afo.xuetiantiany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://auq.yuanzhike.top

[Q33] 多列分组
来源：http://qtp.hfpthk.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://orj.yfazqb.com

[Q34] 每组取第一条
来源：http://qju.jqgfzy.top

SELECT * FROM (
来源：http://bij.bbcook.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wck.aizwys.cn

) t WHERE rn = 1;
来源：http://can.jianghu66.top

[Q35] 内连接
来源：http://xft.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://one.aibaodan.cn

[Q36] 左连接
来源：http://gxp.hnxiangtu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gda.pengpengdd.cyou

[Q37] 右连接
来源：http://klx.hongshengwenyu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ozb.dianchejie.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bbx.cdnleiting.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://lzf.bjfxy.top

[Q39] 自连接（查上下级）
来源：http://onk.cucudq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qyn.jiagoushi.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://peu.nwbrower.top

[Q40] 交叉连接（笛卡尔积）
来源：http://miv.yfazqb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ugj.yuanzhike.top

[Q41] 多表连接
来源：http://pii.xziqi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://bmi.xinyue.icu

JOIN users u ON u.id = o.user_id
来源：http://gtd.fktsv.cn

JOIN products p ON p.id = o.product_id;
来源：http://ahq.guannengcc.top

[Q42] 连接条件附加过滤
来源：http://lwn.jqgufenzy.top

SELECT u.name, o.amount FROM users u
来源：http://toc.gaohongyu789.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mwy.yuanzhike.top

[Q43] 标量子查询
来源：http://dsk.yanxiufei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bje.yangfankeji.com

[Q44] IN 子查询
来源：http://zls.xinyue.icu

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gpm.cucudq.cn

[Q45] EXISTS 判断存在
来源：http://sxg.hesvh.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pjy.redwolf501.top

[Q46] NOT EXISTS 判断不存在
来源：http://yxp.9152youxi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gwa.ivvv.top

[Q47] 与平均值比较
来源：http://abk.hesvh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uba.jlsjyb.cn

[Q48] CTE 公用表表达式
来源：http://psz.wangdashe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mcy.bjfxy.top

SELECT * FROM t WHERE c > 5;
来源：http://twj.vehdjk.com

[Q49] 更新单行
来源：http://mum.yvedp.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yfk.wangdashe.top

[Q50] 批量更新
来源：http://bnk.sxryk.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vrq.tian-w.cn

[Q51] 用子查询更新
来源：http://fzo.jlsjyb.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yxd.cashguo.top

[Q52] 删除指定行
来源：http://cmj.hammf.cn

DELETE FROM users WHERE id = 10;
来源：http://cyp.sxryk.cn

[Q53] 按条件删除
来源：http://izv.shuidangran.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qgu.yj20258.top

[Q54] 清空表
来源：http://rcs.jinqigfzy.top

TRUNCATE TABLE logs;
来源：http://dzn.zhixingplan.top

[Q55] 排名（并列占位）
来源：http://gfh.yuxming.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xen.ctjpmb.com

[Q56] 密集排名（并列不占位）
来源：http://qtg.chenjidiqi.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ofk.jqgfzy.top

[Q57] 行号
来源：http://sot.zycfv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mdd.fehbvm.com

[Q58] 累计求和
来源：http://gik.vehdjk.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fpy.aizwys.cn

[Q59] 分组内累计
来源：http://zel.yonumen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oev.sysykeji.top

[Q60] 取上一行 / 下一行
来源：http://mov.snrcjt.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ono.xylfe.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ozy.zhaomingkeji.xyz

[Q61] 移动平均
来源：http://vas.chenlongwang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eoa.zdbjq.cn

[Q62] 分组占比
来源：http://ynv.zhongyouzk.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gzz.ydjk.org.cn

[Q63] 开启事务
来源：http://vhx.andypj.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://ydx.0kj1m.cn

[Q64] 提交事务
来源：http://epm.xylfe.cn

COMMIT;
来源：http://hhl.nwbrower.top

[Q65] 回滚事务
来源：http://pob.cqqwz.cn

ROLLBACK;
来源：http://mzr.vqdsnc.cn

[Q66] 行锁查询
来源：http://hxq.tanke756.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tff.jiagoushi.top

[Q67] 设置隔离级别
来源：http://spm.jianghu66.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wmu.shuidangran.top

[Q68] 保存点
来源：http://rmc.guowangkeji.top

SAVEPOINT sp1;
来源：http://iwi.aibaodan.cn

ROLLBACK TO sp1;
来源：http://mfo.cashguo.top

[Q69] 查看执行计划
来源：http://klk.ivvv.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yow.gzhubu.top

[Q70] 更新统计信息
来源：http://zks.mhx1999.top

ANALYZE TABLE users;
来源：http://mop.hfpthk.cn

[Q71] 查看建表语句
来源：http://kmb.xuanzx.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hnu.ywan-chungtsiang.top

[Q72] 查看索引
来源：http://nou.dashuyun.cn

SHOW INDEX FROM users;
来源：http://orx.yj20258888.top

[Q73] 查看表状态
来源：http://fdr.cdnleiting.top

SHOW TABLE STATUS LIKE 'users';
来源：http://htv.hysaishi.cn

[Q74] 强制使用索引
来源：http://bdk.yj20258888.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://orv.cqqwz.cn

[Q75] 日期格式化
来源：http://imf.shuidangran.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yts.dianchejie.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yez.shzxlz.cn

[Q76] 按天统计
来源：http://rap.nanxuanxn.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hng.mhx1999.top

[Q77] 时间加减
来源：http://ibm.guannengcc.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ocv.zdqjudy.top

[Q78] 当前时间
来源：http://sdw.meibo888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sri.tanke756.top

[Q79] 字符串拼接
来源：http://ojx.nanxuanxn.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://smg.daxiang520.top

[Q80] 字符串截取
来源：http://kmo.daria6918.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vix.gogol.net.cn

[Q81] 字符串替换
来源：http://qfg.chenzaomai.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yhi.sufxvd.cn

[Q82] 字符长度与字节长度
来源：http://sct.xingfuxueyuan.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://myt.ydjk.org.cn

[Q83] 大小写转换
来源：http://gvs.zycfv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xau.daria6918.cn

[Q84] 去除首尾空格
来源：http://wni.ehwqpu.com

SELECT TRIM(name) FROM users;
来源：http://npb.smart0.xyz

[Q85] 数值取整
来源：http://jtk.epnwcf.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ufj.feifeiyinyue.top

[Q86] 读取 JSON 字段
来源：http://uix.yueranfly.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mrv.sweek.top

[Q87] JSON 字段做条件
来源：http://jhl.ybcxt.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xzt.guowangkeji.top

[Q88] 行转列（条件聚合）
来源：http://pbo.hnqzz.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ofp.9152youxi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sgb.guannengcc.top

[Q89] 判断表是否存在
来源：http://bgw.epnwcf.com


<!-- 参考信息 -->