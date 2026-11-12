代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://cfk.fanxiaobao.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://qwk.xziqi.cn

C#:   async Task F() { await G(); }
来源：http://ioo.jianghu66.top

[O05] 并发执行并等待全部完成
来源：http://vpl.yj20258888.top

Py:   asyncio.gather(*tasks)
来源：http://lch.ywan-chungtsiang.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://uol.smart0.xyz

JS:   await Promise.all(tasks)
来源：http://kpg.jlsjyb.cn

TS:   await Promise.all(tasks)
来源：http://vra.snrcjt.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bzs.xingfuxueyuan.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wfe.tarul.cn

Ruby: threads.map(&:join)
来源：http://kso.yvedp.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://btw.smart0.xyz

[O06] 使用进程池
来源：http://xli.jinqigfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kcb.tarul.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://zxw.uphjek.com

JS:   // child_process / cluster 模块
来源：http://ivq.havefunace.top

TS:   // child_process / cluster 模块
来源：http://vuz.wangshuangyany.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://vqb.zhoulong.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kre.daxiang520.top

Ruby: // fork 块
来源：http://dea.pengpengdd.cyou

C#:   Parallel.For
来源：http://zfl.fehbvm.com

================================================================================
来源：http://wnv.yfazqb.com

P. 常用工具函数
来源：http://vuj.nanxuanxn.top

================================================================================
来源：http://aao.chenjidiqi.icu

[P01] 生成 UUID
来源：http://ixk.hcnkem.com

Py:   str(uuid.uuid4())
来源：http://aaw.xuetiantiany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ave.zhoulong.xyz

JS:   crypto.randomUUID()
来源：http://fgx.shanyushiyangkeji.top

TS:   crypto.randomUUID()
来源：http://kje.ctjpmb.com

Java: UUID.randomUUID().toString()
来源：http://pvy.ppjwa.cn

Go:   // 用 github.com/google/uuid
来源：http://shh.cashguo.top

Ruby: SecureRandom.uuid
来源：http://aub.guowangkeji.top

C#:   Guid.NewGuid().ToString()
来源：http://slm.hfpthk.cn

[P02] MD5 / SHA256 摘要
来源：http://cdw.uphjek.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://lmp.jianghu66.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://zeg.meibo888.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://oze.mhx1999.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pnm.yueranfly.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hnm.zhoulong.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://uyu.fehbvm.com

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ltu.nanxuanxn.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://zdm.yonumen.top

[P03] 生成短随机字符串
来源：http://gfu.tian-w.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://vln.zhaomingkeji.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://teb.aizwys.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://snd.daxiang520.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://iia.ydzc1.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wtj.jiagoushi.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://jjj.yongpay.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lub.epnwcf.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ixb.uphjek.com

[P04] 求长度
来源：http://vvj.316326.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://pah.shanyushiyangtech.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ppg.xuanzx.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mre.cdnleiting.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ues.zdqjudy.top

Java: list.size();  map.size();  s.length()
来源：http://eyv.guowangkeji.top

Go:   len(arr);  len(m)
来源：http://ntg.316326.xyz

Ruby: x.length;  x.size
来源：http://yrr.hnxiangtu.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fnh.snrcjt.cn

[P05] 判断两个对象内容是否相等
来源：http://brs.tian-w.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://eng.jinyuanbaomall.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hmv.iojbl.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zmk.sufxvd.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://fro.shzxlz.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://imi.jlsjyb.cn

Go:   reflect.DeepEqual(a, b)
来源：http://fvc.ivvv.top

Ruby: a == b
来源：http://xjj.pengpengdd.cyou

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://krv.gotoacloud.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ccb.aibaodan.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zjk.0kj1m.cn

PHP:  if (empty($x)) {}
来源：http://szy.yueranfly.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://hmi.ydjk.org.cn

TS:   if (x == null) {}
来源：http://vno.pengpengdd.cyou

Java: if (x == null || x.isEmpty()) {}
来源：http://msm.yonumen.top

Go:   if x == nil {}
来源：http://vsi.yfazqb.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sts.haohaochexian.top

C#:   if (x is null) {}
来源：http://nbj.jiagoushi.top

[P07] 防抖与节流
来源：http://ebd.yuanzhike.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wbm.hfpthk.cn

PHP:  // 手写时间戳比较
来源：http://aye.jinghuilouyu.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://cxk.ywan-chungtsiang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ydk.tianlin.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://eoq.meibo888.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jwi.tianlin.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://pwb.yj202588.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://aop.hysaishi.cn

[P08] 处理浮点精度问题
来源：http://sqg.sufxvd.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://jjd.quarkkingdee.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vxr.yanxiufei.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vtr.wangdashe.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ycy.guannengcc.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tpy.nanxinkj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://arl.snrcjt.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ayh.cashguo.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://awi.sufxvd.cn

================================================================================
来源：http://sud.hnqzz.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hja.ywan-chungtsiang.top

================================================================================
来源：http://mpp.fehbvm.com

[Q01] 创建表
来源：http://npu.kuanghao11.cn

CREATE TABLE users (
来源：http://vmr.jiagoushi.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bxv.ybcxt.top

name VARCHAR(50) NOT NULL,
来源：http://dlk.zhengqikj.top

email VARCHAR(100) UNIQUE,
来源：http://nmw.bbcook.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://nqg.zhongyouzk.top

);
来源：http://cut.sweek.top

[Q02] 创建带外键的表
来源：http://osc.fzhhl.top

CREATE TABLE orders (
来源：http://zgi.dashuyun.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://jcb.shuidangran.top

user_id INT NOT NULL,
来源：http://egr.hcnkem.com

amount DECIMAL(10, 2),
来源：http://wwn.kuanghao11.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bnk.zdqjudy.top

);
来源：http://wnq.yuanzhike.top

[Q03] 增加列
来源：http://hku.fengsongda.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://iax.tanke756.top

[Q04] 修改列类型
来源：http://rqb.gogol.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jlw.pengpengdd.cyou

[Q05] 重命名列
来源：http://qyt.yvedp.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://occ.chenzaomai.com

[Q06] 删除列
来源：http://qcs.jianghu66.top

ALTER TABLE users DROP COLUMN age;
来源：http://odp.ydzc1.top

[Q07] 删除表
来源：http://tjz.dashuyun.cn

DROP TABLE IF EXISTS orders;
来源：http://mwp.jianghu66.top

[Q08] 创建普通索引
来源：http://vpl.guannengcc.top

CREATE INDEX idx_users_email ON users(email);
来源：http://gio.wangdashe.top

[Q09] 创建唯一索引
来源：http://bvd.fktsv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://syr.jinyuanbaomall.cn

[Q10] 插入单行
来源：http://sok.wangdashe.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://avx.yj202588.top

[Q11] 一次插入多行
来源：http://cti.nwbrower.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hio.vqdsnc.cn

[Q12] 插入后取自增 ID
来源：http://dqs.nanxinkj.top

INSERT INTO users (name) VALUES ('C');
来源：http://zvf.cqqwz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qvd.vqdsnc.cn

[Q13] 忽略重复插入
来源：http://nvm.uphjek.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bsm.ppjwa.cn

[Q14] 存在则更新（upsert）
来源：http://ehj.zycfv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cie.yj20258888.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wji.wangshuangyany.cn

[Q15] 查询全部
来源：http://dhi.zdqjudy.top

SELECT * FROM users;
来源：http://ozb.guowangkeji.top

[Q16] 查询指定列
来源：http://pwx.zhoulong.xyz

SELECT id, name FROM users;
来源：http://zrs.daria6918.cn

[Q17] 条件查询
来源：http://sym.yangfankeji.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://lkg.0kj1m.cn

[Q18] 模糊匹配
来源：http://iol.316326.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mma.yfazqb.com

[Q19] 范围查询
来源：http://sao.iojbl.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://abm.yfazqb.com

[Q20] IN 列表
来源：http://rdp.shangyingyoupin.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wzl.316326.xyz

[Q21] 空值判断
来源：http://pac.jinqigfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://zrr.shanyushiyangtech.top

[Q22] 排序
来源：http://zbj.vehdjk.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ous.zhiwuduotai.top

[Q23] 分页
来源：http://gih.c1oappe.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ebd.0kj1m.cn

[Q24] 去重
来源：http://zgm.snrcjt.cn

SELECT DISTINCT city FROM users;
来源：http://vix.tarul.cn

[Q25] 只取前 N 条
来源：http://rin.jinqigufen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vcn.pengpengdd.cyou

[Q26] 计数
来源：http://rfj.mhx1999.top

SELECT COUNT(*) FROM users;
来源：http://xfd.jinqigfzy.top

[Q27] 条件计数
来源：http://ssz.jiagoushi.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://gqv.chenlongwang.top

[Q28] 求和与平均
来源：http://izf.fehbvm.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jqs.bjfxy.top

[Q29] 最大最小值
来源：http://peb.yvedp.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ogq.yangfankeji.com

[Q30] 分组统计
来源：http://ryl.0kj1m.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qer.bbcook.cn

[Q31] 分组后过滤
来源：http://auc.sweek.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vbs.shanyushiyangtech.top

[Q32] 分组拼接字符串
来源：http://aja.fktsv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ysm.wangshuangyany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://muj.birdmap.top

[Q33] 多列分组
来源：http://ras.bjfxy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://pqv.andypj.xyz

[Q34] 每组取第一条
来源：http://chp.ydjk.org.cn

SELECT * FROM (
来源：http://kdi.zhiwuduotai.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qaq.tianlin.xyz

) t WHERE rn = 1;
来源：http://adt.c1oappe.top

[Q35] 内连接
来源：http://nmx.quarkkingdee.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://okq.meibo888.top

[Q36] 左连接
来源：http://lan.yangfankeji.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://oie.smart0.xyz

[Q37] 右连接
来源：http://ekc.aizwys.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qfm.9152youxi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://rvr.0kj1m.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jjd.yongpay.top

[Q39] 自连接（查上下级）
来源：http://chh.zhaomingkeji.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://bfx.ydjk.org.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ifs.ctjpmb.com

[Q40] 交叉连接（笛卡尔积）
来源：http://jvv.cashguo.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qwm.guowangkeji.top

[Q41] 多表连接
来源：http://bqj.zhixingplan.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://isg.zhaomingkeji.xyz

JOIN users u ON u.id = o.user_id
来源：http://yjw.birdmap.top

JOIN products p ON p.id = o.product_id;
来源：http://wpi.jianghu66.top

[Q42] 连接条件附加过滤
来源：http://fko.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u
来源：http://efe.sufxvd.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wmy.yj20258.top

[Q43] 标量子查询
来源：http://iuj.xinyue.icu

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ndm.epnwcf.com

[Q44] IN 子查询
来源：http://jqk.sjlbkw.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://orf.9152youxi.cn

[Q45] EXISTS 判断存在
来源：http://zbj.hnqzz.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ikn.vqdsnc.cn

[Q46] NOT EXISTS 判断不存在
来源：http://epg.gzhubu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yww.snrcjt.cn

[Q47] 与平均值比较
来源：http://ork.hfpthk.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://yns.hnqzz.top

[Q48] CTE 公用表表达式
来源：http://rqq.iojbl.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://rmx.kuanghao11.cn

SELECT * FROM t WHERE c > 5;
来源：http://jhd.ctjpmb.com

[Q49] 更新单行
来源：http://cml.xylfe.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jzv.zhoulong.xyz

[Q50] 批量更新
来源：http://jdw.zhengqikj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bxj.nanxinkj.top

[Q51] 用子查询更新
来源：http://qmt.bjfxy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yhh.yueranfly.top

[Q52] 删除指定行
来源：http://ons.zdbjq.cn

DELETE FROM users WHERE id = 10;
来源：http://knc.zhaomingkeji.xyz

[Q53] 按条件删除
来源：http://nft.shzxlz.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cdi.chenlongwang.top

[Q54] 清空表
来源：http://ypu.jqgfzy.top

TRUNCATE TABLE logs;
来源：http://ieo.chenzaomai.com

[Q55] 排名（并列占位）
来源：http://dvu.hammf.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://iwk.uphjek.com

[Q56] 密集排名（并列不占位）
来源：http://oft.zhaomingkeji.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vti.smart0.xyz

[Q57] 行号
来源：http://adi.chenjidiqi.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pzb.hfpthk.cn

[Q58] 累计求和
来源：http://jjh.meibo888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nxw.daxiang520.top

[Q59] 分组内累计
来源：http://ylj.yuanzhike.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gtg.sysykeji.top

[Q60] 取上一行 / 下一行
来源：http://bxc.52xcode.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sul.cdnleiting.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://siy.shuidangran.top

[Q61] 移动平均
来源：http://pej.bjfxy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nfc.hongshengwenyu.top

[Q62] 分组占比
来源：http://jpk.zhoulong.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rsr.ehwqpu.com

[Q63] 开启事务
来源：http://vmn.ivvv.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dyk.fktsv.cn

[Q64] 提交事务
来源：http://gmz.9152youxi.cn

COMMIT;
来源：http://mdg.feifeiyinyue.top

[Q65] 回滚事务
来源：http://pwh.chenjidiqi.icu

ROLLBACK;
来源：http://lhu.zycfv.cn

[Q66] 行锁查询
来源：http://kgq.hcnkem.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bhf.ppjwa.cn

[Q67] 设置隔离级别
来源：http://nqg.uphjek.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xap.havefunace.top

[Q68] 保存点
来源：http://fun.yvedp.cn

SAVEPOINT sp1;
来源：http://glf.yuxming.cn

ROLLBACK TO sp1;
来源：http://uco.ybcxt.top

[Q69] 查看执行计划
来源：http://exi.haohaochexian.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fhh.ywan-chungtsiang.top

[Q70] 更新统计信息
来源：http://xok.jqgufenzy.top

ANALYZE TABLE users;
来源：http://hqg.cdnleiting.top

[Q71] 查看建表语句
来源：http://ysn.316326.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ckq.zhijiandao.cn

[Q72] 查看索引
来源：http://biu.hammf.cn

SHOW INDEX FROM users;
来源：http://eic.haohaochexian.top

[Q73] 查看表状态
来源：http://cli.tanke756.top

SHOW TABLE STATUS LIKE 'users';
来源：http://lga.yvedp.cn

[Q74] 强制使用索引
来源：http://khz.yongpay.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vfj.zdbjq.cn

[Q75] 日期格式化
来源：http://kcz.hysaishi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mwu.yj202588.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cvt.yongpay.top

[Q76] 按天统计
来源：http://cvl.shanyushiyangtech.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jwl.snrcjt.cn

[Q77] 时间加减
来源：http://mta.ivvv.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nlc.hfpthk.cn

[Q78] 当前时间
来源：http://qey.hysaishi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://igg.xuanzx.com

[Q79] 字符串拼接
来源：http://vqh.sysykeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ush.hysaishi.cn

[Q80] 字符串截取
来源：http://pmy.gotoacloud.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://oxm.jinqigfzy.top

[Q81] 字符串替换
来源：http://bnq.yj202588.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zpj.yongpay.top

[Q82] 字符长度与字节长度
来源：http://leh.andypj.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://obn.zhongyouzk.top

[Q83] 大小写转换
来源：http://vmc.mhx1999.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qub.yanxiufei.cn

[Q84] 去除首尾空格
来源：http://fiy.sxryk.cn

SELECT TRIM(name) FROM users;
来源：http://eba.yuanzhike.top

[Q85] 数值取整
来源：http://gsm.9152youxi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://owr.pycfn.com

[Q86] 读取 JSON 字段
来源：http://iac.ydzc1.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jwk.yuanzhike.top

[Q87] JSON 字段做条件
来源：http://wcu.redwolf501.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xgl.shanyushiyangkeji.top

[Q88] 行转列（条件聚合）
来源：http://cwu.sysykeji.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sax.gogol.net.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ube.zhoulong.xyz

[Q89] 判断表是否存在
来源：http://dwx.sysykeji.top


<!-- 参考信息 -->