代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nhi.316326.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://vfg.sjlbkw.cn

C#:   async Task F() { await G(); }
来源：http://yfo.iojbl.cn

[O05] 并发执行并等待全部完成
来源：http://bhw.feifeiyinyue.top

Py:   asyncio.gather(*tasks)
来源：http://kpb.aibaodan.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uty.hcnkem.com

JS:   await Promise.all(tasks)
来源：http://tdd.guowangkeji.top

TS:   await Promise.all(tasks)
来源：http://ozy.tianlin.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://vou.zhengqikj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://qko.nanxuanxn.top

Ruby: threads.map(&:join)
来源：http://bvp.mhx1999.top

C#:   await Task.WhenAll(t1, t2)
来源：http://svs.9152youxi.cn

[O06] 使用进程池
来源：http://rtx.haohaochexian.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jai.yvedp.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kzy.daxiang520.top

JS:   // child_process / cluster 模块
来源：http://uex.ehwqpu.com

TS:   // child_process / cluster 模块
来源：http://ata.hammf.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qbt.hnqzz.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jtq.yongpay.top

Ruby: // fork 块
来源：http://qkh.fzhhl.top

C#:   Parallel.For
来源：http://nif.nwbrower.top

================================================================================
来源：http://ddx.xuetiantiany.cn

P. 常用工具函数
来源：http://dxn.ehwqpu.com

================================================================================
来源：http://vms.xingfuxueyuan.xyz

[P01] 生成 UUID
来源：http://mgu.ydjk.org.cn

Py:   str(uuid.uuid4())
来源：http://jai.pengpengdd.cyou

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://jfa.vehdjk.com

JS:   crypto.randomUUID()
来源：http://hrh.guowangkeji.top

TS:   crypto.randomUUID()
来源：http://fat.wangshuangyany.cn

Java: UUID.randomUUID().toString()
来源：http://lug.xuetiantiany.cn

Go:   // 用 github.com/google/uuid
来源：http://ofd.shanyushiyangtech.top

Ruby: SecureRandom.uuid
来源：http://vqr.yj20258.top

C#:   Guid.NewGuid().ToString()
来源：http://fqn.yanxiufei.cn

[P02] MD5 / SHA256 摘要
来源：http://adc.fanxiaobao.xyz

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://csu.hnqzz.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://pys.zhoulong.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://fhc.jyoumei.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lny.nanxuanxn.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://xts.pycfn.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wde.nanxinkj.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ksc.kuanghao11.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://pjf.zycfv.cn

[P03] 生成短随机字符串
来源：http://tkh.shanyushiyangkeji.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rsv.vqdsnc.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fzb.jianghu66.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://atc.shuidangran.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lvy.svipenyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ozo.cqqwz.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://rjv.bbcook.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cpc.redwolf501.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wch.sweek.top

[P04] 求长度
来源：http://kki.ywan-chungtsiang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://txo.mhx1999.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://foc.hnqzz.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yye.tanke756.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://orx.bbcook.cn

Java: list.size();  map.size();  s.length()
来源：http://pzd.jinyuanbaomall.cn

Go:   len(arr);  len(m)
来源：http://xeu.yangfankeji.com

Ruby: x.length;  x.size
来源：http://pgn.pengpengdd.cyou

C#:   list.Count;  dict.Count;  s.Length
来源：http://gip.yj20258.top

[P05] 判断两个对象内容是否相等
来源：http://jzm.zhixingplan.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://bsa.ybcxt.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hob.dianchejie.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fel.mhx1999.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://eta.shangyingyoupin.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vyp.ctjpmb.com

Go:   reflect.DeepEqual(a, b)
来源：http://ipc.fehbvm.com

Ruby: a == b
来源：http://ylr.shuidangran.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://bsh.yj202588.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://oqx.nanxinkj.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ljj.zhoulong.xyz

PHP:  if (empty($x)) {}
来源：http://euv.hysaishi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oez.52xcode.cn

TS:   if (x == null) {}
来源：http://psb.shanyushiyangkeji.top

Java: if (x == null || x.isEmpty()) {}
来源：http://uez.haohaochexian.top

Go:   if x == nil {}
来源：http://bqo.uphjek.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://aip.vehdjk.com

C#:   if (x is null) {}
来源：http://bod.ehwqpu.com

[P07] 防抖与节流
来源：http://oih.cqqwz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://uyx.fktsv.cn

PHP:  // 手写时间戳比较
来源：http://nos.jyoumei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://drh.aibaodan.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ael.gotoacloud.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gnf.zdqjudy.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ykp.jlsjyb.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zyd.cashguo.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ezc.zycfv.cn

[P08] 处理浮点精度问题
来源：http://fnk.zhixingplan.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qim.yvedp.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://bfh.jqgfzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jas.daxiang520.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ntm.hysaishi.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://adc.kuanghao11.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://now.xuanzx.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xga.shzxlz.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://evx.hfpthk.cn

================================================================================
来源：http://fam.tianlin.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://sxi.bjfxy.top

================================================================================
来源：http://wwt.iojbl.cn

[Q01] 创建表
来源：http://dmy.feifeiyinyue.top

CREATE TABLE users (
来源：http://xtw.sysykeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://uvo.yangfankeji.com

name VARCHAR(50) NOT NULL,
来源：http://kku.hongshengwenyu.top

email VARCHAR(100) UNIQUE,
来源：http://tfl.jinghuilouyu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gph.ydzc1.top

);
来源：http://ufl.jinyuanbaomall.cn

[Q02] 创建带外键的表
来源：http://eiz.fengsongda.top

CREATE TABLE orders (
来源：http://jbd.vqdsnc.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lre.hfpthk.cn

user_id INT NOT NULL,
来源：http://wmo.chenzaomai.com

amount DECIMAL(10, 2),
来源：http://liw.jiagoushi.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cgr.aibaodan.cn

);
来源：http://dbe.hesvh.cn

[Q03] 增加列
来源：http://pkt.bbcook.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://pxx.9152youxi.cn

[Q04] 修改列类型
来源：http://xro.shzxlz.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rjh.chenlongwang.top

[Q05] 重命名列
来源：http://bfn.xziqi.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://oga.vqdsnc.cn

[Q06] 删除列
来源：http://vwe.0kj1m.cn

ALTER TABLE users DROP COLUMN age;
来源：http://fpq.zhiwuduotai.top

[Q07] 删除表
来源：http://qxm.jlsjyb.cn

DROP TABLE IF EXISTS orders;
来源：http://swx.dashuyun.cn

[Q08] 创建普通索引
来源：http://fls.9152youxi.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hpn.fengsongda.top

[Q09] 创建唯一索引
来源：http://fev.iojbl.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nnx.chenlongwang.top

[Q10] 插入单行
来源：http://dhg.shzxlz.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fac.cqqwz.cn

[Q11] 一次插入多行
来源：http://ieg.316326.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hep.nanxuanxn.top

[Q12] 插入后取自增 ID
来源：http://ffd.hnqzz.top

INSERT INTO users (name) VALUES ('C');
来源：http://pby.redwolf501.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zmb.shuidangran.top

[Q13] 忽略重复插入
来源：http://kwv.jinghuilouyu.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mcf.ivvv.top

[Q14] 存在则更新（upsert）
来源：http://kww.nanxinkj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dby.smart0.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zba.fengsongda.top

[Q15] 查询全部
来源：http://ohr.guowangkeji.top

SELECT * FROM users;
来源：http://thb.nanxinkj.top

[Q16] 查询指定列
来源：http://har.chenzaomai.com

SELECT id, name FROM users;
来源：http://mcm.sxryk.cn

[Q17] 条件查询
来源：http://uml.hnxiangtu.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://sbb.zhengqikj.top

[Q18] 模糊匹配
来源：http://scp.hcnkem.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://jip.yj202588.top

[Q19] 范围查询
来源：http://hng.zhijiandao.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://hxl.feifeiyinyue.top

[Q20] IN 列表
来源：http://dxq.zhaomingkeji.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pph.shanyushiyangtech.top

[Q21] 空值判断
来源：http://tgx.meibo888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://dwu.yj20258.top

[Q22] 排序
来源：http://xmf.chenzaomai.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zte.hnqzz.top

[Q23] 分页
来源：http://uhq.jinqigufen.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mxe.mhx1999.top

[Q24] 去重
来源：http://uqp.hongshengwenyu.top

SELECT DISTINCT city FROM users;
来源：http://vrm.yongpay.top

[Q25] 只取前 N 条
来源：http://hbp.hysaishi.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ebq.zhixingplan.top

[Q26] 计数
来源：http://iyb.pengpengdd.cyou

SELECT COUNT(*) FROM users;
来源：http://uwg.0kj1m.cn

[Q27] 条件计数
来源：http://rpo.yanxiufei.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rhn.snrcjt.cn

[Q28] 求和与平均
来源：http://mrz.sysykeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://snn.c1oappe.top

[Q29] 最大最小值
来源：http://lxk.ppjwa.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bva.shzxlz.cn

[Q30] 分组统计
来源：http://cpq.iojbl.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lyb.ydzc1.top

[Q31] 分组后过滤
来源：http://rtz.gotoacloud.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ojj.aibaodan.cn

[Q32] 分组拼接字符串
来源：http://lcw.cqqwz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yyd.fehbvm.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qpc.hfpthk.cn

[Q33] 多列分组
来源：http://fem.xylfe.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dja.yueranfly.top

[Q34] 每组取第一条
来源：http://ibn.guannengcc.top

SELECT * FROM (
来源：http://htn.shuidangran.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://nlj.sxryk.cn

) t WHERE rn = 1;
来源：http://tcd.nanxinkj.top

[Q35] 内连接
来源：http://pee.haohaochexian.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lsn.quarkkingdee.top

[Q36] 左连接
来源：http://gjh.tanke756.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uny.yanxiufei.cn

[Q37] 右连接
来源：http://bag.zycfv.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://jln.hywenlv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://osk.svipenyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yla.ydzc1.top

[Q39] 自连接（查上下级）
来源：http://qxm.yangfankeji.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://tkw.fengsongda.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ijz.hysaishi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://vgw.shangyingyoupin.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mlh.haohaochexian.top

[Q41] 多表连接
来源：http://aaw.chenjidiqi.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://zkh.ywan-chungtsiang.top

JOIN users u ON u.id = o.user_id
来源：http://xrt.nanxinkj.top

JOIN products p ON p.id = o.product_id;
来源：http://lqd.tarul.cn

[Q42] 连接条件附加过滤
来源：http://dcl.svipenyu.cn

SELECT u.name, o.amount FROM users u
来源：http://jgy.zycfv.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xhw.bjfxy.top

[Q43] 标量子查询
来源：http://vmx.jqgufenzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kjp.guowangkeji.top

[Q44] IN 子查询
来源：http://wsc.cucudq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tzv.vehdjk.com

[Q45] EXISTS 判断存在
来源：http://xgd.yj20258.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qyp.zycfv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vds.zhaomingkeji.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qkj.hnxiangtu.top

[Q47] 与平均值比较
来源：http://aam.shzxlz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tip.fengsongda.top

[Q48] CTE 公用表表达式
来源：http://aja.ywan-chungtsiang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zaq.yongpay.top

SELECT * FROM t WHERE c > 5;
来源：http://oeo.mhx1999.top

[Q49] 更新单行
来源：http://hbl.zhoulong.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zpc.chenlongwang.top

[Q50] 批量更新
来源：http://ong.shuidangran.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ita.jianghu66.top

[Q51] 用子查询更新
来源：http://hcy.jqgfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ogo.xuanzx.com

[Q52] 删除指定行
来源：http://typ.ctjpmb.com

DELETE FROM users WHERE id = 10;
来源：http://eeq.cheryme.top

[Q53] 按条件删除
来源：http://ffi.hywenlv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://oke.tianlin.xyz

[Q54] 清空表
来源：http://cwi.daxiang520.top

TRUNCATE TABLE logs;
来源：http://ojk.feifeiyinyue.top

[Q55] 排名（并列占位）
来源：http://gdo.meibo888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ygq.tarul.cn

[Q56] 密集排名（并列不占位）
来源：http://kus.snrcjt.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wqx.wangshuangyany.cn

[Q57] 行号
来源：http://hqh.yfazqb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://vwz.chenlongwang.top

[Q58] 累计求和
来源：http://qbb.daxiang520.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ejb.zhixingplan.top

[Q59] 分组内累计
来源：http://rfj.jqgufenzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ofd.ywan-chungtsiang.top

[Q60] 取上一行 / 下一行
来源：http://tqc.ywan-chungtsiang.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tzg.tanke756.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vde.andypj.xyz

[Q61] 移动平均
来源：http://nhk.chenzaomai.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hzk.smart0.xyz

[Q62] 分组占比
来源：http://fpr.sxryk.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://esa.xinyue.icu

[Q63] 开启事务
来源：http://lsh.fanxiaobao.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://fgb.tanke756.top

[Q64] 提交事务
来源：http://fyy.smart0.xyz

COMMIT;
来源：http://zhb.pengpengdd.cyou

[Q65] 回滚事务
来源：http://vca.c1oappe.top

ROLLBACK;
来源：http://kkp.yangfankeji.com

[Q66] 行锁查询
来源：http://bdv.snrcjt.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nuk.vqdsnc.cn

[Q67] 设置隔离级别
来源：http://qpp.hysaishi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pan.nanxuanxn.top

[Q68] 保存点
来源：http://sxf.zhaomingkeji.xyz

SAVEPOINT sp1;
来源：http://ahl.zhongyouzk.top

ROLLBACK TO sp1;
来源：http://zvj.fanxiaobao.xyz

[Q69] 查看执行计划
来源：http://zcj.nanxuanxn.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://syy.hnqzz.top

[Q70] 更新统计信息
来源：http://oie.shzxlz.cn

ANALYZE TABLE users;
来源：http://jaq.tanke756.top

[Q71] 查看建表语句
来源：http://dvy.aibaodan.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jau.gaohongyu789.top

[Q72] 查看索引
来源：http://zla.wangdashe.top

SHOW INDEX FROM users;
来源：http://zxj.shuidangran.top

[Q73] 查看表状态
来源：http://ukg.vqdsnc.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cso.gzhubu.top

[Q74] 强制使用索引
来源：http://xbv.epnwcf.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vqu.ctjpmb.com

[Q75] 日期格式化
来源：http://ckv.havefunace.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ebj.smart0.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jvn.ctjpmb.com

[Q76] 按天统计
来源：http://fwi.gaohongyu789.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uen.cashguo.top

[Q77] 时间加减
来源：http://fwn.tian-w.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://imz.cdnleiting.top

[Q78] 当前时间
来源：http://qlh.jlsjyb.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://iut.nwbrower.top

[Q79] 字符串拼接
来源：http://fcz.cheryme.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://knt.316326.xyz

[Q80] 字符串截取
来源：http://ovt.iojbl.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nwg.quarkkingdee.top

[Q81] 字符串替换
来源：http://czx.birdmap.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://agp.yuanzhike.top

[Q82] 字符长度与字节长度
来源：http://cdg.hammf.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://axu.hongshengwenyu.top

[Q83] 大小写转换
来源：http://nrg.zhijiandao.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://brh.hesvh.cn

[Q84] 去除首尾空格
来源：http://mrg.hesvh.cn

SELECT TRIM(name) FROM users;
来源：http://bmw.xuanzx.com

[Q85] 数值取整
来源：http://hyx.gzhubu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cwi.cheryme.top

[Q86] 读取 JSON 字段
来源：http://awv.bbcook.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vjd.ywan-chungtsiang.top

[Q87] JSON 字段做条件
来源：http://esv.ydjk.org.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bhh.xuanzx.com

[Q88] 行转列（条件聚合）
来源：http://net.daxiang520.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jnk.ctjpmb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bpp.zdqjudy.top

[Q89] 判断表是否存在
来源：http://mau.yangfankeji.com


<!-- 参考信息 -->