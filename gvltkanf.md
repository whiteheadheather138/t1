代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ddv.nwbrower.top

Ruby: # 用 Fiber 或 async gem
来源：http://sdz.shanyushiyangtech.top

C#:   async Task F() { await G(); }
来源：http://hiv.guowangkeji.top

[O05] 并发执行并等待全部完成
来源：http://ric.gogol.net.cn

Py:   asyncio.gather(*tasks)
来源：http://jse.ydzc1.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nyl.jlsjyb.cn

JS:   await Promise.all(tasks)
来源：http://udy.daxiang520.top

TS:   await Promise.all(tasks)
来源：http://fgc.316326.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://uxo.tanke756.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ytd.daria6918.cn

Ruby: threads.map(&:join)
来源：http://ysq.nanxuanxn.top

C#:   await Task.WhenAll(t1, t2)
来源：http://tmg.xuetiantiany.cn

[O06] 使用进程池
来源：http://ujf.zhixingplan.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cqy.yangfankeji.com

PHP:  // pcntl_fork 或多进程队列
来源：http://vtg.c1oappe.top

JS:   // child_process / cluster 模块
来源：http://trg.cdnleiting.top

TS:   // child_process / cluster 模块
来源：http://wfe.yvedp.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://rzl.yonumen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tna.ppjwa.cn

Ruby: // fork 块
来源：http://uzl.nanxinkj.top

C#:   Parallel.For
来源：http://vlz.jqgufenzy.top

================================================================================
来源：http://jhk.dashuyun.cn

P. 常用工具函数
来源：http://svf.mhx1999.top

================================================================================
来源：http://lre.zhiwuduotai.top

[P01] 生成 UUID
来源：http://uqj.fehbvm.com

Py:   str(uuid.uuid4())
来源：http://usp.shuidangran.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://elo.aizwys.cn

JS:   crypto.randomUUID()
来源：http://nsk.tarul.cn

TS:   crypto.randomUUID()
来源：http://ouh.zhongyouzk.top

Java: UUID.randomUUID().toString()
来源：http://pji.vqdsnc.cn

Go:   // 用 github.com/google/uuid
来源：http://jok.xuetiantiany.cn

Ruby: SecureRandom.uuid
来源：http://ufw.iojbl.cn

C#:   Guid.NewGuid().ToString()
来源：http://ngg.gogol.net.cn

[P02] MD5 / SHA256 摘要
来源：http://dda.zhijiandao.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ghm.ydjk.org.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fkg.sufxvd.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lsl.dianchejie.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://btc.fzhhl.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://phu.haohaochexian.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cds.yonumen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dww.fanxiaobao.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://knv.gaohongyu789.top

[P03] 生成短随机字符串
来源：http://xim.yangfankeji.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://swi.tanke756.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://avf.xziqi.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://nkj.kuanghao11.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://trj.hesvh.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vge.hnqzz.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://joc.bbcook.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://opl.hcnkem.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gga.shangyingyoupin.top

[P04] 求长度
来源：http://lkl.shangyingyoupin.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kdb.zhengqikj.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://smo.jlsjyb.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://txj.gzhubu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vta.havefunace.top

Java: list.size();  map.size();  s.length()
来源：http://ebx.kuanghao11.cn

Go:   len(arr);  len(m)
来源：http://glt.xuanzx.com

Ruby: x.length;  x.size
来源：http://pgx.shzxlz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://tog.hfpthk.cn

[P05] 判断两个对象内容是否相等
来源：http://azf.yanxiufei.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://wnx.9152youxi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uyq.zdbjq.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pfw.yonumen.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jdf.52xcode.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://suu.sjlbkw.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bba.sxryk.cn

Ruby: a == b
来源：http://wwh.jlsjyb.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://cfy.9152youxi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://qxi.jlsjyb.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://dqz.cashguo.top

PHP:  if (empty($x)) {}
来源：http://tyr.yangfankeji.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iva.cdnleiting.top

TS:   if (x == null) {}
来源：http://xxl.jinqigufen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://txz.ppjwa.cn

Go:   if x == nil {}
来源：http://aym.yj20258888.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ugf.guowangkeji.top

C#:   if (x is null) {}
来源：http://clo.chenzaomai.com

[P07] 防抖与节流
来源：http://pcm.aizwys.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://bkz.ydzc1.top

PHP:  // 手写时间戳比较
来源：http://tuh.andypj.xyz

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lep.chenlongwang.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://amf.nanxuanxn.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://dnm.hammf.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://zzj.cdnleiting.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://quy.svipenyu.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://acy.sysykeji.top

[P08] 处理浮点精度问题
来源：http://yzz.sweek.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lie.ywan-chungtsiang.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://fuu.hammf.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xgy.pycfn.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ntc.wangdashe.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wzw.cucudq.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://aow.yj20258.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://itg.ybcxt.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dgl.hfpthk.cn

================================================================================
来源：http://rqq.yuanzhike.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qyo.sjlbkw.cn

================================================================================
来源：http://kee.jiagoushi.top

[Q01] 创建表
来源：http://pry.zhongyouzk.top

CREATE TABLE users (
来源：http://mvi.yvedp.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jgs.jyoumei.cn

name VARCHAR(50) NOT NULL,
来源：http://nyt.dianchejie.cn

email VARCHAR(100) UNIQUE,
来源：http://kbt.epnwcf.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://bhh.iojbl.cn

);
来源：http://lpy.vqdsnc.cn

[Q02] 创建带外键的表
来源：http://utm.meibo888.top

CREATE TABLE orders (
来源：http://iqa.zhixingplan.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lgu.chenzaomai.com

user_id INT NOT NULL,
来源：http://enh.hnqzz.top

amount DECIMAL(10, 2),
来源：http://dtm.pengpengdd.cyou

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xsx.xuetiantiany.cn

);
来源：http://zyn.sxryk.cn

[Q03] 增加列
来源：http://pcn.aibaodan.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mxy.bjfxy.top

[Q04] 修改列类型
来源：http://qxw.bbcook.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xsp.ybcxt.top

[Q05] 重命名列
来源：http://mrv.shangyingyoupin.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://alm.ehwqpu.com

[Q06] 删除列
来源：http://dfn.cqqwz.cn

ALTER TABLE users DROP COLUMN age;
来源：http://kiw.ctjpmb.com

[Q07] 删除表
来源：http://pbs.yvedp.cn

DROP TABLE IF EXISTS orders;
来源：http://riu.nanxuanxn.top

[Q08] 创建普通索引
来源：http://wlv.jyoumei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xib.52xcode.cn

[Q09] 创建唯一索引
来源：http://bvz.ehwqpu.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zme.0kj1m.cn

[Q10] 插入单行
来源：http://gwh.wangshuangyany.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lsm.hammf.cn

[Q11] 一次插入多行
来源：http://rpy.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iaq.ybcxt.top

[Q12] 插入后取自增 ID
来源：http://fec.zdqjudy.top

INSERT INTO users (name) VALUES ('C');
来源：http://igx.gogol.net.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hbi.xingfuxueyuan.xyz

[Q13] 忽略重复插入
来源：http://cub.nwbrower.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://awn.hywenlv.cn

[Q14] 存在则更新（upsert）
来源：http://jtu.hongshengwenyu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://ohi.jianghu66.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sjs.shanyushiyangkeji.top

[Q15] 查询全部
来源：http://ynt.sweek.top

SELECT * FROM users;
来源：http://wed.zhoulong.xyz

[Q16] 查询指定列
来源：http://mzm.xinyue.icu

SELECT id, name FROM users;
来源：http://iyo.aizwys.cn

[Q17] 条件查询
来源：http://fah.iojbl.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ima.shuidangran.top

[Q18] 模糊匹配
来源：http://thm.iojbl.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://itz.pycfn.com

[Q19] 范围查询
来源：http://hiq.316326.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gmr.wangshuangyany.cn

[Q20] IN 列表
来源：http://yqc.ydzc1.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://idd.ivvv.top

[Q21] 空值判断
来源：http://owv.yfazqb.com

SELECT * FROM users WHERE email IS NULL;
来源：http://mgx.sufxvd.cn

[Q22] 排序
来源：http://rhr.xinyue.icu

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ljo.0kj1m.cn

[Q23] 分页
来源：http://pli.yongpay.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eol.hammf.cn

[Q24] 去重
来源：http://vcc.gaohongyu789.top

SELECT DISTINCT city FROM users;
来源：http://cvs.smart0.xyz

[Q25] 只取前 N 条
来源：http://ykr.yangfankeji.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://xya.kuanghao11.cn

[Q26] 计数
来源：http://pfs.kuanghao11.cn

SELECT COUNT(*) FROM users;
来源：http://yap.xylfe.cn

[Q27] 条件计数
来源：http://dpi.xylfe.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dfi.yonumen.top

[Q28] 求和与平均
来源：http://gbr.ctjpmb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dso.bbcook.cn

[Q29] 最大最小值
来源：http://ssh.feifeiyinyue.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://xld.cashguo.top

[Q30] 分组统计
来源：http://nhv.xingfuxueyuan.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lrk.nanxinkj.top

[Q31] 分组后过滤
来源：http://gbn.xuanzx.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tfi.jlsjyb.cn

[Q32] 分组拼接字符串
来源：http://gbo.daria6918.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lnj.quarkkingdee.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qpi.bbcook.cn

[Q33] 多列分组
来源：http://amu.vehdjk.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hfn.cashguo.top

[Q34] 每组取第一条
来源：http://wnz.ctjpmb.com

SELECT * FROM (
来源：http://iew.ctjpmb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://njm.redwolf501.top

) t WHERE rn = 1;
来源：http://ybd.jinghuilouyu.cn

[Q35] 内连接
来源：http://vom.zdbjq.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ifg.sysykeji.top

[Q36] 左连接
来源：http://fou.jianghu66.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jqa.chenzaomai.com

[Q37] 右连接
来源：http://chs.hfpthk.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://owb.hammf.cn

[Q38] 全外连接（PostgreSQL）
来源：http://bic.daxiang520.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rmw.gzhubu.top

[Q39] 自连接（查上下级）
来源：http://qpr.shzxlz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://xxb.gogol.net.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dji.xziqi.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://wcj.quarkkingdee.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ptk.shuidangran.top

[Q41] 多表连接
来源：http://lws.tarul.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://naj.ydjk.org.cn

JOIN users u ON u.id = o.user_id
来源：http://kxi.xuanzx.com

JOIN products p ON p.id = o.product_id;
来源：http://snf.sweek.top

[Q42] 连接条件附加过滤
来源：http://wnh.tianlin.xyz

SELECT u.name, o.amount FROM users u
来源：http://eal.zhongyouzk.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://han.cashguo.top

[Q43] 标量子查询
来源：http://maa.smart0.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dme.zhijiandao.cn

[Q44] IN 子查询
来源：http://kug.birdmap.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bkg.redwolf501.top

[Q45] EXISTS 判断存在
来源：http://sdu.yonumen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ull.sjlbkw.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hmu.zhongyouzk.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kqx.vqdsnc.cn

[Q47] 与平均值比较
来源：http://ssh.jiagoushi.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ymf.hcnkem.com

[Q48] CTE 公用表表达式
来源：http://fxg.pycfn.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wrw.cdnleiting.top

SELECT * FROM t WHERE c > 5;
来源：http://izf.smart0.xyz

[Q49] 更新单行
来源：http://wgd.andypj.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hfn.zycfv.cn

[Q50] 批量更新
来源：http://yck.fktsv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zow.jinqigfzy.top

[Q51] 用子查询更新
来源：http://hzp.tanke756.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wkw.cashguo.top

[Q52] 删除指定行
来源：http://ajc.iojbl.cn

DELETE FROM users WHERE id = 10;
来源：http://qhq.wangshuangyany.cn

[Q53] 按条件删除
来源：http://hiw.0kj1m.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fty.hnqzz.top

[Q54] 清空表
来源：http://vkd.jyoumei.cn

TRUNCATE TABLE logs;
来源：http://hvj.epnwcf.com

[Q55] 排名（并列占位）
来源：http://ihh.0kj1m.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kjw.sysykeji.top

[Q56] 密集排名（并列不占位）
来源：http://dxu.yj20258.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bew.ehwqpu.com

[Q57] 行号
来源：http://svi.jiagoushi.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://olc.ywan-chungtsiang.top

[Q58] 累计求和
来源：http://epy.dashuyun.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wyw.shuidangran.top

[Q59] 分组内累计
来源：http://ehm.jinqigfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gte.bjfxy.top

[Q60] 取上一行 / 下一行
来源：http://qzs.aizwys.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lac.ppjwa.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://diy.smart0.xyz

[Q61] 移动平均
来源：http://duq.daxiang520.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vqu.316326.xyz

[Q62] 分组占比
来源：http://fhr.hammf.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ogk.birdmap.top

[Q63] 开启事务
来源：http://hdi.sxryk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://aco.fengsongda.top

[Q64] 提交事务
来源：http://eim.ywan-chungtsiang.top

COMMIT;
来源：http://ajv.cqqwz.cn

[Q65] 回滚事务
来源：http://jfq.vqdsnc.cn

ROLLBACK;
来源：http://rtq.daxiang520.top

[Q66] 行锁查询
来源：http://qem.fengsongda.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zhs.yvedp.cn

[Q67] 设置隔离级别
来源：http://vyi.jinqigfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fjo.xziqi.cn

[Q68] 保存点
来源：http://tzm.vehdjk.com

SAVEPOINT sp1;
来源：http://thn.gaohongyu789.top

ROLLBACK TO sp1;
来源：http://bmr.fzhhl.top

[Q69] 查看执行计划
来源：http://nog.haohaochexian.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mlg.cdnleiting.top

[Q70] 更新统计信息
来源：http://wjf.feifeiyinyue.top

ANALYZE TABLE users;
来源：http://kfu.chenlongwang.top

[Q71] 查看建表语句
来源：http://mhk.316326.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mry.hywenlv.cn

[Q72] 查看索引
来源：http://aat.chenlongwang.top

SHOW INDEX FROM users;
来源：http://hex.shuidangran.top

[Q73] 查看表状态
来源：http://gay.tianlin.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://cjj.daria6918.cn

[Q74] 强制使用索引
来源：http://tqt.ydjk.org.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jqp.hammf.cn

[Q75] 日期格式化
来源：http://zen.daria6918.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mkp.wangshuangyany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vuf.zhongyouzk.top

[Q76] 按天统计
来源：http://lya.guannengcc.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mbv.svipenyu.cn

[Q77] 时间加减
来源：http://kcy.yfazqb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kix.nanxinkj.top

[Q78] 当前时间
来源：http://yky.sjlbkw.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qms.jiagoushi.top

[Q79] 字符串拼接
来源：http://lae.yvedp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kkc.jlsjyb.cn

[Q80] 字符串截取
来源：http://zem.zhaomingkeji.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zbl.guowangkeji.top

[Q81] 字符串替换
来源：http://nhb.yvedp.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pqo.yj202588.top

[Q82] 字符长度与字节长度
来源：http://xcm.guannengcc.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xkg.cdnleiting.top

[Q83] 大小写转换
来源：http://evf.zdqjudy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lxc.meibo888.top

[Q84] 去除首尾空格
来源：http://eeo.zycfv.cn

SELECT TRIM(name) FROM users;
来源：http://enu.nanxuanxn.top

[Q85] 数值取整
来源：http://tmq.yueranfly.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jds.yueranfly.top

[Q86] 读取 JSON 字段
来源：http://xgq.yj20258888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sjc.zhengqikj.top

[Q87] JSON 字段做条件
来源：http://gki.zhengqikj.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://liw.zhiwuduotai.top

[Q88] 行转列（条件聚合）
来源：http://joc.guannengcc.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fon.shanyushiyangtech.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://slk.yj202588.top

[Q89] 判断表是否存在
来源：http://yoe.redwolf501.top


<!-- 参考信息 -->