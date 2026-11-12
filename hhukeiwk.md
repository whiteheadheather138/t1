代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://qkd.birdmap.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://whw.epnwcf.com

JS:   await Promise.all(tasks)
来源：http://igl.aibaodan.cn

TS:   await Promise.all(tasks)
来源：http://zbp.gaohongyu789.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bcr.shuidangran.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wmy.smart0.xyz

Ruby: threads.map(&:join)
来源：http://wyz.chenlongwang.top

C#:   await Task.WhenAll(t1, t2)
来源：http://xvs.xinyue.icu

[O06] 使用进程池
来源：http://kez.ybcxt.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dmj.chenzaomai.com

PHP:  // pcntl_fork 或多进程队列
来源：http://ukn.xingfuxueyuan.xyz

JS:   // child_process / cluster 模块
来源：http://sdg.fengsongda.top

TS:   // child_process / cluster 模块
来源：http://cjv.iojbl.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://yzr.yj202588.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://azq.xingfuxueyuan.xyz

Ruby: // fork 块
来源：http://dsr.jlsjyb.cn

C#:   Parallel.For
来源：http://wng.tarul.cn

================================================================================
来源：http://qxq.dashuyun.cn

P. 常用工具函数
来源：http://zyk.tanke756.top

================================================================================
来源：http://xnt.sxryk.cn

[P01] 生成 UUID
来源：http://bpe.feifeiyinyue.top

Py:   str(uuid.uuid4())
来源：http://wwx.jyoumei.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nws.jiagoushi.top

JS:   crypto.randomUUID()
来源：http://cct.cdnleiting.top

TS:   crypto.randomUUID()
来源：http://kfq.andypj.xyz

Java: UUID.randomUUID().toString()
来源：http://tmm.snrcjt.cn

Go:   // 用 github.com/google/uuid
来源：http://mbq.sysykeji.top

Ruby: SecureRandom.uuid
来源：http://wul.vehdjk.com

C#:   Guid.NewGuid().ToString()
来源：http://bnb.xingfuxueyuan.xyz

[P02] MD5 / SHA256 摘要
来源：http://rig.zdbjq.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ber.hnqzz.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://ouf.xziqi.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vaz.ybcxt.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dwq.jqgfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ttg.jqgfzy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://moz.havefunace.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zbb.hnqzz.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mdk.hysaishi.cn

[P03] 生成短随机字符串
来源：http://odv.bjfxy.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nsj.xingfuxueyuan.xyz

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tao.jlsjyb.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dkm.andypj.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ugo.guannengcc.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://pnp.bjfxy.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mfg.yangfankeji.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://gbd.sweek.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://roe.cheryme.top

[P04] 求长度
来源：http://zfw.gzhubu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zav.sweek.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vzx.shuidangran.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pyc.jiagoushi.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jem.yfazqb.com

Java: list.size();  map.size();  s.length()
来源：http://jis.mhx1999.top

Go:   len(arr);  len(m)
来源：http://kay.chenlongwang.top

Ruby: x.length;  x.size
来源：http://zad.jqgufenzy.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://mho.xuanzx.com

[P05] 判断两个对象内容是否相等
来源：http://bqt.redwolf501.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://qai.hfpthk.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zaq.c1oappe.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zfj.daxiang520.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dtp.yuxming.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://fju.yj202588.top

Go:   reflect.DeepEqual(a, b)
来源：http://kiy.316326.xyz

Ruby: a == b
来源：http://oic.hammf.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://pbp.gogol.net.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qzs.jyoumei.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rgp.vehdjk.com

PHP:  if (empty($x)) {}
来源：http://xyy.52xcode.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mah.shanyushiyangkeji.top

TS:   if (x == null) {}
来源：http://cho.nanxinkj.top

Java: if (x == null || x.isEmpty()) {}
来源：http://rke.52xcode.cn

Go:   if x == nil {}
来源：http://uji.fehbvm.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jqx.sysykeji.top

C#:   if (x is null) {}
来源：http://hgb.snrcjt.cn

[P07] 防抖与节流
来源：http://zss.meibo888.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wyd.jinghuilouyu.cn

PHP:  // 手写时间戳比较
来源：http://edn.pengpengdd.cyou

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vzx.shangyingyoupin.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://txi.fktsv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tkq.hywenlv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ugr.gotoacloud.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zmh.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gao.tarul.cn

[P08] 处理浮点精度问题
来源：http://fgm.sxryk.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://muf.fktsv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://tbc.havefunace.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xkv.zhijiandao.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kho.shzxlz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dzn.yangfankeji.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ipj.haohaochexian.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qka.redwolf501.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://xlh.mhx1999.top

================================================================================
来源：http://gnf.mhx1999.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vfj.xingfuxueyuan.xyz

================================================================================
来源：http://ggo.zhijiandao.cn

[Q01] 创建表
来源：http://kui.sysykeji.top

CREATE TABLE users (
来源：http://vnj.zdbjq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xxk.pycfn.com

name VARCHAR(50) NOT NULL,
来源：http://cor.havefunace.top

email VARCHAR(100) UNIQUE,
来源：http://uzo.svipenyu.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kcz.ydjk.org.cn

);
来源：http://hmx.nanxinkj.top

[Q02] 创建带外键的表
来源：http://azi.sjlbkw.cn

CREATE TABLE orders (
来源：http://lgj.vqdsnc.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://efh.fzhhl.top

user_id INT NOT NULL,
来源：http://hsk.shangyingyoupin.top

amount DECIMAL(10, 2),
来源：http://ipv.cucudq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://aqs.nwbrower.top

);
来源：http://yim.epnwcf.com

[Q03] 增加列
来源：http://heu.aizwys.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jda.fanxiaobao.xyz

[Q04] 修改列类型
来源：http://qic.sxryk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ufz.pycfn.com

[Q05] 重命名列
来源：http://dfi.ctjpmb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jpy.cheryme.top

[Q06] 删除列
来源：http://rni.bjfxy.top

ALTER TABLE users DROP COLUMN age;
来源：http://ebj.bbcook.cn

[Q07] 删除表
来源：http://aoh.meibo888.top

DROP TABLE IF EXISTS orders;
来源：http://avd.52xcode.cn

[Q08] 创建普通索引
来源：http://epu.nanxinkj.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ahf.snrcjt.cn

[Q09] 创建唯一索引
来源：http://jhy.zhijiandao.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://nir.sufxvd.cn

[Q10] 插入单行
来源：http://bos.chenlongwang.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vhi.yuxming.cn

[Q11] 一次插入多行
来源：http://icc.quarkkingdee.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wxm.zhongyouzk.top

[Q12] 插入后取自增 ID
来源：http://pst.hammf.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ptk.quarkkingdee.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://byz.zhaomingkeji.xyz

[Q13] 忽略重复插入
来源：http://iht.yueranfly.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dib.xuanzx.com

[Q14] 存在则更新（upsert）
来源：http://uqx.yongpay.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pwk.gotoacloud.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://iho.jqgfzy.top

[Q15] 查询全部
来源：http://efl.tianlin.xyz

SELECT * FROM users;
来源：http://aqa.jianghu66.top

[Q16] 查询指定列
来源：http://qxi.zhoulong.xyz

SELECT id, name FROM users;
来源：http://ihq.yongpay.top

[Q17] 条件查询
来源：http://txq.sxryk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xpa.guowangkeji.top

[Q18] 模糊匹配
来源：http://jxy.guowangkeji.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://fri.gzhubu.top

[Q19] 范围查询
来源：http://ptq.yfazqb.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xwd.yfazqb.com

[Q20] IN 列表
来源：http://ptl.ehwqpu.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://oao.cheryme.top

[Q21] 空值判断
来源：http://unc.xinyue.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://cka.shuidangran.top

[Q22] 排序
来源：http://piv.jinqigfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mtc.fehbvm.com

[Q23] 分页
来源：http://myr.hnqzz.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yaz.52xcode.cn

[Q24] 去重
来源：http://esy.cucudq.cn

SELECT DISTINCT city FROM users;
来源：http://ncp.jqgfzy.top

[Q25] 只取前 N 条
来源：http://jfx.ywan-chungtsiang.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hfy.yuanzhike.top

[Q26] 计数
来源：http://ide.hfpthk.cn

SELECT COUNT(*) FROM users;
来源：http://uyx.zhixingplan.top

[Q27] 条件计数
来源：http://puq.guowangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tzs.aizwys.cn

[Q28] 求和与平均
来源：http://lfn.316326.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vqa.aibaodan.cn

[Q29] 最大最小值
来源：http://dbs.ppjwa.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://bdu.ctjpmb.com

[Q30] 分组统计
来源：http://dcj.gogol.net.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cvi.epnwcf.com

[Q31] 分组后过滤
来源：http://hbb.shuidangran.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gzm.9152youxi.cn

[Q32] 分组拼接字符串
来源：http://fnr.jinqigufen.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wmy.sweek.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tcn.jianghu66.top

[Q33] 多列分组
来源：http://zyj.xinyue.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lpf.52xcode.cn

[Q34] 每组取第一条
来源：http://ftw.dashuyun.cn

SELECT * FROM (
来源：http://kuu.xuanzx.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jtc.yanxiufei.cn

) t WHERE rn = 1;
来源：http://xdx.uphjek.com

[Q35] 内连接
来源：http://hqq.nanxinkj.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nul.andypj.xyz

[Q36] 左连接
来源：http://pen.fzhhl.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tqi.fktsv.cn

[Q37] 右连接
来源：http://now.pycfn.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zss.zycfv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xsu.yongpay.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://kyl.zycfv.cn

[Q39] 自连接（查上下级）
来源：http://ytf.0kj1m.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://qeg.jinghuilouyu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ufe.birdmap.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hje.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://iuo.hnqzz.top

[Q41] 多表连接
来源：http://ynh.xuanzx.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://hwi.cashguo.top

JOIN users u ON u.id = o.user_id
来源：http://abh.guannengcc.top

JOIN products p ON p.id = o.product_id;
来源：http://znr.hnxiangtu.top

[Q42] 连接条件附加过滤
来源：http://dhq.vqdsnc.cn

SELECT u.name, o.amount FROM users u
来源：http://jug.nwbrower.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pqd.jqgfzy.top

[Q43] 标量子查询
来源：http://ptf.zhixingplan.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://scq.chenzaomai.com

[Q44] IN 子查询
来源：http://bhv.yj202588.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tqy.yfazqb.com

[Q45] EXISTS 判断存在
来源：http://uqd.kuanghao11.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yol.haohaochexian.top

[Q46] NOT EXISTS 判断不存在
来源：http://tve.9152youxi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yon.jinghuilouyu.cn

[Q47] 与平均值比较
来源：http://eyh.redwolf501.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xml.zhixingplan.top

[Q48] CTE 公用表表达式
来源：http://gxr.jlsjyb.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ntq.ctjpmb.com

SELECT * FROM t WHERE c > 5;
来源：http://syb.cashguo.top

[Q49] 更新单行
来源：http://acc.xuetiantiany.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sca.c1oappe.top

[Q50] 批量更新
来源：http://iqx.bjfxy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yqp.zycfv.cn

[Q51] 用子查询更新
来源：http://kuo.jinqigufen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iyp.jlsjyb.cn

[Q52] 删除指定行
来源：http://vpi.cqqwz.cn

DELETE FROM users WHERE id = 10;
来源：http://xuq.yvedp.cn

[Q53] 按条件删除
来源：http://nxh.ehwqpu.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tqn.xuetiantiany.cn

[Q54] 清空表
来源：http://lmg.jinqigufen.top

TRUNCATE TABLE logs;
来源：http://eca.andypj.xyz

[Q55] 排名（并列占位）
来源：http://gul.zdqjudy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xkg.hysaishi.cn

[Q56] 密集排名（并列不占位）
来源：http://mil.yvedp.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lvu.sjlbkw.cn

[Q57] 行号
来源：http://mwd.shanyushiyangtech.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rby.shanyushiyangkeji.top

[Q58] 累计求和
来源：http://lef.yanxiufei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pjm.gotoacloud.top

[Q59] 分组内累计
来源：http://rgk.gotoacloud.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lnn.zhiwuduotai.top

[Q60] 取上一行 / 下一行
来源：http://ehu.gotoacloud.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zor.xziqi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dyu.yonumen.top

[Q61] 移动平均
来源：http://mqq.zhaomingkeji.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://edu.zycfv.cn

[Q62] 分组占比
来源：http://gao.meibo888.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zqf.shuidangran.top

[Q63] 开启事务
来源：http://oyo.wangshuangyany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://grz.shanyushiyangtech.top

[Q64] 提交事务
来源：http://jwq.havefunace.top

COMMIT;
来源：http://rnt.fanxiaobao.xyz

[Q65] 回滚事务
来源：http://tlw.tanke756.top

ROLLBACK;
来源：http://zfp.gotoacloud.top

[Q66] 行锁查询
来源：http://hwi.tarul.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://plc.sjlbkw.cn

[Q67] 设置隔离级别
来源：http://smg.kuanghao11.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bdz.tian-w.cn

[Q68] 保存点
来源：http://eou.ehwqpu.com

SAVEPOINT sp1;
来源：http://cqj.jinghuilouyu.cn

ROLLBACK TO sp1;
来源：http://opc.yonumen.top

[Q69] 查看执行计划
来源：http://oph.andypj.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ypz.cheryme.top

[Q70] 更新统计信息
来源：http://mli.sysykeji.top

ANALYZE TABLE users;
来源：http://zmq.epnwcf.com

[Q71] 查看建表语句
来源：http://sbp.haohaochexian.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pef.chenzaomai.com

[Q72] 查看索引
来源：http://mej.nanxinkj.top

SHOW INDEX FROM users;
来源：http://fmm.yueranfly.top

[Q73] 查看表状态
来源：http://bth.zhiwuduotai.top

SHOW TABLE STATUS LIKE 'users';
来源：http://zgr.fanxiaobao.xyz

[Q74] 强制使用索引
来源：http://jwt.redwolf501.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://efx.xuetiantiany.cn

[Q75] 日期格式化
来源：http://fhk.xylfe.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bph.aibaodan.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cgo.meibo888.top

[Q76] 按天统计
来源：http://nda.tian-w.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ydj.snrcjt.cn

[Q77] 时间加减
来源：http://klv.havefunace.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gvx.yfazqb.com

[Q78] 当前时间
来源：http://hqu.jqgufenzy.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://dol.yongpay.top

[Q79] 字符串拼接
来源：http://nsy.xuanzx.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gpu.dianchejie.cn

[Q80] 字符串截取
来源：http://xvr.0kj1m.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wqh.jiagoushi.top

[Q81] 字符串替换
来源：http://umv.yangfankeji.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sna.hywenlv.cn

[Q82] 字符长度与字节长度
来源：http://hsr.jiagoushi.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bmt.xuanzx.com

[Q83] 大小写转换
来源：http://hlj.hongshengwenyu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yyy.hesvh.cn

[Q84] 去除首尾空格
来源：http://oqv.sweek.top

SELECT TRIM(name) FROM users;
来源：http://zif.feifeiyinyue.top

[Q85] 数值取整
来源：http://jcg.52xcode.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mer.yonumen.top

[Q86] 读取 JSON 字段
来源：http://wie.nanxuanxn.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qfb.bjfxy.top

[Q87] JSON 字段做条件
来源：http://iir.uphjek.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rxo.mhx1999.top

[Q88] 行转列（条件聚合）
来源：http://zkd.shuidangran.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iei.snrcjt.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://csz.jinghuilouyu.cn

[Q89] 判断表是否存在
来源：http://vff.xylfe.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nhr.cheryme.top

[Q90] 生成序号列
来源：http://pkn.hywenlv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lso.zhiwuduotai.top

================================================================================
来源：http://qrr.yvedp.cn


<!-- 参考信息 -->