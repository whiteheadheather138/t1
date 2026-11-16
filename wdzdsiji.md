代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://cfz.ctjpmb.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tff.hnxiangtu.top

JS:   await Promise.all(tasks)
来源：http://fky.52xcode.cn

TS:   await Promise.all(tasks)
来源：http://hxg.ybcxt.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://oid.jlsjyb.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://oii.mhx1999.top

Ruby: threads.map(&:join)
来源：http://pzd.redwolf501.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ksc.yvedp.cn

[O06] 使用进程池
来源：http://ori.ehwqpu.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ycd.ivvv.top

PHP:  // pcntl_fork 或多进程队列
来源：http://hba.zhongyouzk.top

JS:   // child_process / cluster 模块
来源：http://tqm.jianghu66.top

TS:   // child_process / cluster 模块
来源：http://aou.gotoacloud.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mwc.havefunace.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wej.shzxlz.cn

Ruby: // fork 块
来源：http://tkr.zhiwuduotai.top

C#:   Parallel.For
来源：http://gov.tarul.cn

================================================================================
来源：http://bml.fzhhl.top

P. 常用工具函数
来源：http://sqa.fzhhl.top

================================================================================
来源：http://vgf.uphjek.com

[P01] 生成 UUID
来源：http://mxq.zhijiandao.cn

Py:   str(uuid.uuid4())
来源：http://byi.shanyushiyangtech.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rlc.cdnleiting.top

JS:   crypto.randomUUID()
来源：http://fis.ppjwa.cn

TS:   crypto.randomUUID()
来源：http://xap.shzxlz.cn

Java: UUID.randomUUID().toString()
来源：http://naj.hcnkem.com

Go:   // 用 github.com/google/uuid
来源：http://xcd.jiagoushi.top

Ruby: SecureRandom.uuid
来源：http://kuo.zhaomingkeji.xyz

C#:   Guid.NewGuid().ToString()
来源：http://zob.xuanzx.com

[P02] MD5 / SHA256 摘要
来源：http://sct.vqdsnc.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aif.fanxiaobao.xyz

PHP:  hash("sha256", $s);  md5($s);
来源：http://qcv.ybcxt.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://hfe.haohaochexian.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zuc.ppjwa.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://iqq.dianchejie.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kzk.jlsjyb.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://svf.c1oappe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://oad.haohaochexian.top

[P03] 生成短随机字符串
来源：http://wbf.zhengqikj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://imu.uphjek.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tlw.yfazqb.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yue.andypj.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://uij.yongpay.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qni.zhiwuduotai.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xyz.shangyingyoupin.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cey.vqdsnc.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vxu.jiagoushi.top

[P04] 求长度
来源：http://kwj.gzhubu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://yyp.xingfuxueyuan.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nzg.ppjwa.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iwa.yanxiufei.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://apc.fzhhl.top

Java: list.size();  map.size();  s.length()
来源：http://ruk.jqgufenzy.top

Go:   len(arr);  len(m)
来源：http://zps.dashuyun.cn

Ruby: x.length;  x.size
来源：http://dbm.meibo888.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xjg.chenlongwang.top

[P05] 判断两个对象内容是否相等
来源：http://bhk.zdbjq.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lxt.daxiang520.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://bin.tian-w.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://kre.cqqwz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ymc.sufxvd.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pts.zhongyouzk.top

Go:   reflect.DeepEqual(a, b)
来源：http://qvy.hnxiangtu.top

Ruby: a == b
来源：http://jue.zycfv.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://plv.hnxiangtu.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://swe.epnwcf.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ihk.sxryk.cn

PHP:  if (empty($x)) {}
来源：http://cbw.hesvh.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wph.fzhhl.top

TS:   if (x == null) {}
来源：http://uyx.daria6918.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://duu.xuanzx.com

Go:   if x == nil {}
来源：http://pnd.nwbrower.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wij.ctjpmb.com

C#:   if (x is null) {}
来源：http://hwf.zdqjudy.top

[P07] 防抖与节流
来源：http://pdm.daxiang520.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pzk.aizwys.cn

PHP:  // 手写时间戳比较
来源：http://esw.ppjwa.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://xpb.xingfuxueyuan.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://har.shanyushiyangkeji.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ris.shuidangran.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jip.9152youxi.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://kbp.birdmap.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mcu.yueranfly.top

[P08] 处理浮点精度问题
来源：http://huk.gaohongyu789.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jjd.hfpthk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rpa.zhaomingkeji.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hic.gogol.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://hic.sjlbkw.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vpe.tanke756.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yzv.redwolf501.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ynn.birdmap.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pxz.jinyuanbaomall.cn

================================================================================
来源：http://qcd.hongshengwenyu.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://yuz.chenzaomai.com

================================================================================
来源：http://sns.gaohongyu789.top

[Q01] 创建表
来源：http://uyj.yfazqb.com

CREATE TABLE users (
来源：http://vci.daria6918.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://owu.fzhhl.top

name VARCHAR(50) NOT NULL,
来源：http://eyl.hammf.cn

email VARCHAR(100) UNIQUE,
来源：http://ids.daxiang520.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wvd.shuidangran.top

);
来源：http://cla.zhijiandao.cn

[Q02] 创建带外键的表
来源：http://lcr.tian-w.cn

CREATE TABLE orders (
来源：http://wns.hesvh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://bjd.smart0.xyz

user_id INT NOT NULL,
来源：http://myz.xuanzx.com

amount DECIMAL(10, 2),
来源：http://wkw.snrcjt.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ddh.nanxinkj.top

);
来源：http://cur.jlsjyb.cn

[Q03] 增加列
来源：http://xcy.jinqigufen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hvc.fzhhl.top

[Q04] 修改列类型
来源：http://ffe.shangyingyoupin.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://emz.hywenlv.cn

[Q05] 重命名列
来源：http://ple.meibo888.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bez.shanyushiyangtech.top

[Q06] 删除列
来源：http://ozr.svipenyu.cn

ALTER TABLE users DROP COLUMN age;
来源：http://gey.fktsv.cn

[Q07] 删除表
来源：http://vlk.daxiang520.top

DROP TABLE IF EXISTS orders;
来源：http://iux.zycfv.cn

[Q08] 创建普通索引
来源：http://nxy.xinyue.icu

CREATE INDEX idx_users_email ON users(email);
来源：http://qqp.ydzc1.top

[Q09] 创建唯一索引
来源：http://lft.fanxiaobao.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kcu.yj20258888.top

[Q10] 插入单行
来源：http://rox.zhaomingkeji.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://njw.zhixingplan.top

[Q11] 一次插入多行
来源：http://cxo.chenjidiqi.icu

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zch.ydzc1.top

[Q12] 插入后取自增 ID
来源：http://hph.fehbvm.com

INSERT INTO users (name) VALUES ('C');
来源：http://meh.yj20258888.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://imp.uphjek.com

[Q13] 忽略重复插入
来源：http://hre.xinyue.icu

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bqp.jianghu66.top

[Q14] 存在则更新（upsert）
来源：http://opm.52xcode.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qpz.gotoacloud.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://amn.quarkkingdee.top

[Q15] 查询全部
来源：http://scn.hammf.cn

SELECT * FROM users;
来源：http://fro.jiagoushi.top

[Q16] 查询指定列
来源：http://qjf.zdbjq.cn

SELECT id, name FROM users;
来源：http://rsy.fzhhl.top

[Q17] 条件查询
来源：http://rjk.zhongyouzk.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://bga.jinghuilouyu.cn

[Q18] 模糊匹配
来源：http://xow.c1oappe.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://oia.xuetiantiany.cn

[Q19] 范围查询
来源：http://inu.jinyuanbaomall.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pfp.wangshuangyany.cn

[Q20] IN 列表
来源：http://gba.hongshengwenyu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ucs.yanxiufei.cn

[Q21] 空值判断
来源：http://ixw.sxryk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://onf.xylfe.cn

[Q22] 排序
来源：http://jgy.hcnkem.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ifs.jiagoushi.top

[Q23] 分页
来源：http://wfu.jlsjyb.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ifu.quarkkingdee.top

[Q24] 去重
来源：http://frr.zhaomingkeji.xyz

SELECT DISTINCT city FROM users;
来源：http://bbg.yvedp.cn

[Q25] 只取前 N 条
来源：http://blv.smart0.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ofb.yangfankeji.com

[Q26] 计数
来源：http://boa.chenzaomai.com

SELECT COUNT(*) FROM users;
来源：http://wxm.shzxlz.cn

[Q27] 条件计数
来源：http://skz.hfpthk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xum.cucudq.cn

[Q28] 求和与平均
来源：http://kgh.zdbjq.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://npy.uphjek.com

[Q29] 最大最小值
来源：http://nxk.jqgfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://yfa.0kj1m.cn

[Q30] 分组统计
来源：http://iqa.pycfn.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://evk.vehdjk.com

[Q31] 分组后过滤
来源：http://lcd.aizwys.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gkd.shanyushiyangkeji.top

[Q32] 分组拼接字符串
来源：http://ywz.yuxming.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://itt.gotoacloud.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cse.tian-w.cn

[Q33] 多列分组
来源：http://zeh.yvedp.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cry.jqgufenzy.top

[Q34] 每组取第一条
来源：http://ypj.fzhhl.top

SELECT * FROM (
来源：http://pni.jlsjyb.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://whj.ydjk.org.cn

) t WHERE rn = 1;
来源：http://rrc.tian-w.cn

[Q35] 内连接
来源：http://xus.yongpay.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nrh.nwbrower.top

[Q36] 左连接
来源：http://upe.sysykeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://zbd.chenjidiqi.icu

[Q37] 右连接
来源：http://zeu.yonumen.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://arl.gzhubu.top

[Q38] 全外连接（PostgreSQL）
来源：http://ixq.zhoulong.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jka.tianlin.xyz

[Q39] 自连接（查上下级）
来源：http://akg.zhengqikj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://wsk.xylfe.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://whl.ppjwa.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dct.redwolf501.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cie.quarkkingdee.top

[Q41] 多表连接
来源：http://xvz.cashguo.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ciz.jlsjyb.cn

JOIN users u ON u.id = o.user_id
来源：http://mme.ppjwa.cn

JOIN products p ON p.id = o.product_id;
来源：http://nbd.zhaomingkeji.xyz

[Q42] 连接条件附加过滤
来源：http://huu.yj202588.top

SELECT u.name, o.amount FROM users u
来源：http://pyy.wangshuangyany.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ldb.zhongyouzk.top

[Q43] 标量子查询
来源：http://pmy.52xcode.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rbf.c1oappe.top

[Q44] IN 子查询
来源：http://usb.aibaodan.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ohc.zhongyouzk.top

[Q45] EXISTS 判断存在
来源：http://loh.zhixingplan.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xbp.andypj.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://out.tarul.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jno.zhongyouzk.top

[Q47] 与平均值比较
来源：http://wda.sjlbkw.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://agk.ywan-chungtsiang.top

[Q48] CTE 公用表表达式
来源：http://esx.nanxuanxn.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xtp.fehbvm.com

SELECT * FROM t WHERE c > 5;
来源：http://kfn.redwolf501.top

[Q49] 更新单行
来源：http://gel.vqdsnc.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pyi.hcnkem.com

[Q50] 批量更新
来源：http://qkq.jinqigufen.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dok.nanxinkj.top

[Q51] 用子查询更新
来源：http://ddw.shangyingyoupin.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iau.mhx1999.top

[Q52] 删除指定行
来源：http://axg.jinqigfzy.top

DELETE FROM users WHERE id = 10;
来源：http://rba.hywenlv.cn

[Q53] 按条件删除
来源：http://bum.xingfuxueyuan.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ogw.ybcxt.top

[Q54] 清空表
来源：http://aap.hywenlv.cn

TRUNCATE TABLE logs;
来源：http://nec.andypj.xyz

[Q55] 排名（并列占位）
来源：http://tmo.snrcjt.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hkx.hammf.cn

[Q56] 密集排名（并列不占位）
来源：http://foz.zhijiandao.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jdn.jianghu66.top

[Q57] 行号
来源：http://wkl.sysykeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hzd.hnxiangtu.top

[Q58] 累计求和
来源：http://qal.9152youxi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://npd.ctjpmb.com

[Q59] 分组内累计
来源：http://efo.xziqi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mbx.mhx1999.top

[Q60] 取上一行 / 下一行
来源：http://qsu.zhoulong.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ftz.jinqigfzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://adu.birdmap.top

[Q61] 移动平均
来源：http://jbf.ehwqpu.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rjd.havefunace.top

[Q62] 分组占比
来源：http://pgj.snrcjt.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jvh.xuetiantiany.cn

[Q63] 开启事务
来源：http://zwn.chenjidiqi.icu

START TRANSACTION;                -- 或 BEGIN
来源：http://dsg.ydzc1.top

[Q64] 提交事务
来源：http://ioo.yj202588.top

COMMIT;
来源：http://vxq.zdqjudy.top

[Q65] 回滚事务
来源：http://fvp.iojbl.cn

ROLLBACK;
来源：http://wic.cucudq.cn

[Q66] 行锁查询
来源：http://zhd.zhongyouzk.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ubv.chenlongwang.top

[Q67] 设置隔离级别
来源：http://vtq.sysykeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://btu.yanxiufei.cn

[Q68] 保存点
来源：http://avp.zhoulong.xyz

SAVEPOINT sp1;
来源：http://mdo.9152youxi.cn

ROLLBACK TO sp1;
来源：http://sls.hywenlv.cn

[Q69] 查看执行计划
来源：http://dvs.ydjk.org.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gat.jyoumei.cn

[Q70] 更新统计信息
来源：http://bsi.ydzc1.top

ANALYZE TABLE users;
来源：http://vjt.ywan-chungtsiang.top

[Q71] 查看建表语句
来源：http://wup.jinyuanbaomall.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xcr.sjlbkw.cn

[Q72] 查看索引
来源：http://uhv.ctjpmb.com

SHOW INDEX FROM users;
来源：http://goj.jinghuilouyu.cn

[Q73] 查看表状态
来源：http://aip.quarkkingdee.top

SHOW TABLE STATUS LIKE 'users';
来源：http://tvo.bjfxy.top

[Q74] 强制使用索引
来源：http://cqw.chenjidiqi.icu

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rfr.ybcxt.top

[Q75] 日期格式化
来源：http://jlk.shangyingyoupin.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yev.iojbl.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fdw.cheryme.top

[Q76] 按天统计
来源：http://pxs.uphjek.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lch.cdnleiting.top

[Q77] 时间加减
来源：http://wnb.xingfuxueyuan.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ohb.yvedp.cn

[Q78] 当前时间
来源：http://zog.gaohongyu789.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mbv.xuanzx.com

[Q79] 字符串拼接
来源：http://aur.bjfxy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://aaf.epnwcf.com

[Q80] 字符串截取
来源：http://wss.sweek.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gdj.redwolf501.top

[Q81] 字符串替换
来源：http://zvz.gaohongyu789.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dme.xuanzx.com

[Q82] 字符长度与字节长度
来源：http://bpr.ivvv.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kod.jinyuanbaomall.cn

[Q83] 大小写转换
来源：http://kml.hcnkem.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yjq.pengpengdd.cyou

[Q84] 去除首尾空格
来源：http://agv.shuidangran.top

SELECT TRIM(name) FROM users;
来源：http://phu.tanke756.top

[Q85] 数值取整
来源：http://lrt.smart0.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xzd.xingfuxueyuan.xyz

[Q86] 读取 JSON 字段
来源：http://fdq.hongshengwenyu.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qqd.snrcjt.cn

[Q87] JSON 字段做条件
来源：http://yaa.cqqwz.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qsj.fktsv.cn

[Q88] 行转列（条件聚合）
来源：http://osf.fktsv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://piz.fehbvm.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://thf.zhixingplan.top

[Q89] 判断表是否存在
来源：http://xia.yj20258.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pkc.gaohongyu789.top

[Q90] 生成序号列
来源：http://dce.ivvv.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xam.feifeiyinyue.top

================================================================================
来源：http://kxl.xingfuxueyuan.xyz


<!-- 参考信息 -->