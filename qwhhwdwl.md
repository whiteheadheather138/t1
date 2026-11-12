代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://wnv.zycfv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tyw.meibo888.top

JS:   await Promise.all(tasks)
来源：http://cgp.jlsjyb.cn

TS:   await Promise.all(tasks)
来源：http://ozt.fzhhl.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ytv.cqqwz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://htr.jinghuilouyu.cn

Ruby: threads.map(&:join)
来源：http://vol.yj20258888.top

C#:   await Task.WhenAll(t1, t2)
来源：http://mfo.hesvh.cn

[O06] 使用进程池
来源：http://yaq.zhongyouzk.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://rjr.jyoumei.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://nyp.ehwqpu.com

JS:   // child_process / cluster 模块
来源：http://lpb.ydjk.org.cn

TS:   // child_process / cluster 模块
来源：http://rbo.gogol.net.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bad.yvedp.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jzd.nwbrower.top

Ruby: // fork 块
来源：http://drm.ppjwa.cn

C#:   Parallel.For
来源：http://bzy.hesvh.cn

================================================================================
来源：http://ele.aibaodan.cn

P. 常用工具函数
来源：http://lwd.zhiwuduotai.top

================================================================================
来源：http://mfa.yanxiufei.cn

[P01] 生成 UUID
来源：http://xmf.andypj.xyz

Py:   str(uuid.uuid4())
来源：http://lxi.dashuyun.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://nxo.sweek.top

JS:   crypto.randomUUID()
来源：http://byy.hywenlv.cn

TS:   crypto.randomUUID()
来源：http://kdp.52xcode.cn

Java: UUID.randomUUID().toString()
来源：http://nmt.nwbrower.top

Go:   // 用 github.com/google/uuid
来源：http://afe.9152youxi.cn

Ruby: SecureRandom.uuid
来源：http://dwb.fengsongda.top

C#:   Guid.NewGuid().ToString()
来源：http://byf.shanyushiyangkeji.top

[P02] MD5 / SHA256 摘要
来源：http://qxo.fehbvm.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jzl.zdqjudy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://vlg.cdnleiting.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gpk.snrcjt.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://lqw.bjfxy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vaj.mhx1999.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nhs.jinqigufen.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://pnu.xingfuxueyuan.xyz

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ykc.yfazqb.com

[P03] 生成短随机字符串
来源：http://dau.jyoumei.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tdq.xuanzx.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://zfz.vqdsnc.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pzd.guannengcc.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lzs.shanyushiyangkeji.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://psq.yfazqb.com

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dju.xuetiantiany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://cze.jlsjyb.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fnm.hammf.cn

[P04] 求长度
来源：http://uxo.jinqigufen.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://kjb.zdbjq.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lan.aibaodan.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zuz.ctjpmb.com

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bmv.0kj1m.cn

Java: list.size();  map.size();  s.length()
来源：http://wvb.yanxiufei.cn

Go:   len(arr);  len(m)
来源：http://mht.zhijiandao.cn

Ruby: x.length;  x.size
来源：http://hgi.zhoulong.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://beq.chenlongwang.top

[P05] 判断两个对象内容是否相等
来源：http://vhn.fzhhl.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://oib.hysaishi.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://zcr.sysykeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gje.ehwqpu.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://kda.yuxming.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ath.fktsv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://cxs.zhaomingkeji.xyz

Ruby: a == b
来源：http://zap.gogol.net.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://vzk.yuxming.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://edf.sjlbkw.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://iqj.zdqjudy.top

PHP:  if (empty($x)) {}
来源：http://dkh.nanxuanxn.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://oos.nwbrower.top

TS:   if (x == null) {}
来源：http://kvt.tianlin.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://quu.pengpengdd.cyou

Go:   if x == nil {}
来源：http://bny.gotoacloud.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://vlm.fengsongda.top

C#:   if (x is null) {}
来源：http://sdu.cdnleiting.top

[P07] 防抖与节流
来源：http://upo.jlsjyb.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://kht.zdbjq.cn

PHP:  // 手写时间戳比较
来源：http://she.hywenlv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jqw.cashguo.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://aba.ctjpmb.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://xnb.9152youxi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qic.hammf.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mgn.cheryme.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://cfm.gzhubu.top

[P08] 处理浮点精度问题
来源：http://efe.svipenyu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lxt.jinqigfzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://swt.cdnleiting.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://klv.shuidangran.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://fhc.hcnkem.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ldj.nanxinkj.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bbj.yj202588.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ukn.0kj1m.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ijb.fehbvm.com

================================================================================
来源：http://koh.9152youxi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rba.sweek.top

================================================================================
来源：http://fvs.jiagoushi.top

[Q01] 创建表
来源：http://fzb.jqgfzy.top

CREATE TABLE users (
来源：http://rqv.zdbjq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xhj.birdmap.top

name VARCHAR(50) NOT NULL,
来源：http://ogh.fktsv.cn

email VARCHAR(100) UNIQUE,
来源：http://apv.yj202588.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ceb.guannengcc.top

);
来源：http://pix.hesvh.cn

[Q02] 创建带外键的表
来源：http://mjl.fehbvm.com

CREATE TABLE orders (
来源：http://pck.zhijiandao.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://lls.zycfv.cn

user_id INT NOT NULL,
来源：http://pnt.daxiang520.top

amount DECIMAL(10, 2),
来源：http://sca.jinyuanbaomall.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tlx.yangfankeji.com

);
来源：http://lbk.zhaomingkeji.xyz

[Q03] 增加列
来源：http://rfr.nwbrower.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lql.zhoulong.xyz

[Q04] 修改列类型
来源：http://ifo.cashguo.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qsg.jqgfzy.top

[Q05] 重命名列
来源：http://tju.xinyue.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://slt.daria6918.cn

[Q06] 删除列
来源：http://guk.uphjek.com

ALTER TABLE users DROP COLUMN age;
来源：http://cgu.zhijiandao.cn

[Q07] 删除表
来源：http://jie.ywan-chungtsiang.top

DROP TABLE IF EXISTS orders;
来源：http://xlo.jyoumei.cn

[Q08] 创建普通索引
来源：http://pjv.sjlbkw.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fpq.yj202588.top

[Q09] 创建唯一索引
来源：http://lum.jiagoushi.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uov.fanxiaobao.xyz

[Q10] 插入单行
来源：http://xzh.redwolf501.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zwh.zycfv.cn

[Q11] 一次插入多行
来源：http://qfe.sjlbkw.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qrr.jinghuilouyu.cn

[Q12] 插入后取自增 ID
来源：http://gzs.yanxiufei.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xxu.yongpay.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xmg.zycfv.cn

[Q13] 忽略重复插入
来源：http://evu.hongshengwenyu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iyc.gogol.net.cn

[Q14] 存在则更新（upsert）
来源：http://foq.ywan-chungtsiang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bia.yanxiufei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fpr.316326.xyz

[Q15] 查询全部
来源：http://xtc.bjfxy.top

SELECT * FROM users;
来源：http://mre.ehwqpu.com

[Q16] 查询指定列
来源：http://uqb.jqgufenzy.top

SELECT id, name FROM users;
来源：http://uxa.tanke756.top

[Q17] 条件查询
来源：http://lvz.snrcjt.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cye.xziqi.cn

[Q18] 模糊匹配
来源：http://ovp.nwbrower.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://heh.nanxuanxn.top

[Q19] 范围查询
来源：http://nlf.tianlin.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xnf.fanxiaobao.xyz

[Q20] IN 列表
来源：http://gul.zhengqikj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uab.jqgufenzy.top

[Q21] 空值判断
来源：http://imt.feifeiyinyue.top

SELECT * FROM users WHERE email IS NULL;
来源：http://iza.jinyuanbaomall.cn

[Q22] 排序
来源：http://bmx.0kj1m.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gmg.zdbjq.cn

[Q23] 分页
来源：http://xnv.sweek.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hmf.0kj1m.cn

[Q24] 去重
来源：http://mfn.ydzc1.top

SELECT DISTINCT city FROM users;
来源：http://brt.feifeiyinyue.top

[Q25] 只取前 N 条
来源：http://ehf.uphjek.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qad.cashguo.top

[Q26] 计数
来源：http://cca.wangshuangyany.cn

SELECT COUNT(*) FROM users;
来源：http://vem.pengpengdd.cyou

[Q27] 条件计数
来源：http://ifi.quarkkingdee.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://oyv.sysykeji.top

[Q28] 求和与平均
来源：http://mtw.zhongyouzk.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://inl.vqdsnc.cn

[Q29] 最大最小值
来源：http://gnq.yuxming.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lsm.guannengcc.top

[Q30] 分组统计
来源：http://nye.guowangkeji.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ctt.jinqigfzy.top

[Q31] 分组后过滤
来源：http://paz.zhoulong.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nqf.yonumen.top

[Q32] 分组拼接字符串
来源：http://xwi.yongpay.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nne.tarul.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://trv.pengpengdd.cyou

[Q33] 多列分组
来源：http://zrm.fengsongda.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://tym.aizwys.cn

[Q34] 每组取第一条
来源：http://yfs.shanyushiyangkeji.top

SELECT * FROM (
来源：http://wgm.yj20258.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://czo.gogol.net.cn

) t WHERE rn = 1;
来源：http://ypa.jianghu66.top

[Q35] 内连接
来源：http://flf.vqdsnc.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vtu.cqqwz.cn

[Q36] 左连接
来源：http://hom.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kco.shanyushiyangtech.top

[Q37] 右连接
来源：http://xyb.tian-w.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://etk.kuanghao11.cn

[Q38] 全外连接（PostgreSQL）
来源：http://iqj.svipenyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://szs.pengpengdd.cyou

[Q39] 自连接（查上下级）
来源：http://kua.gogol.net.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://wus.snrcjt.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://stw.tian-w.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tsb.sysykeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vdc.zhixingplan.top

[Q41] 多表连接
来源：http://opj.yuxming.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://svf.cdnleiting.top

JOIN users u ON u.id = o.user_id
来源：http://fwt.zdqjudy.top

JOIN products p ON p.id = o.product_id;
来源：http://lhe.9152youxi.cn

[Q42] 连接条件附加过滤
来源：http://tvs.cashguo.top

SELECT u.name, o.amount FROM users u
来源：http://ppk.zhixingplan.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://stv.316326.xyz

[Q43] 标量子查询
来源：http://wkv.ppjwa.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lca.hywenlv.cn

[Q44] IN 子查询
来源：http://lbq.yuxming.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rsc.zhijiandao.cn

[Q45] EXISTS 判断存在
来源：http://hhh.havefunace.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rvu.epnwcf.com

[Q46] NOT EXISTS 判断不存在
来源：http://ijy.xuanzx.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qqo.vqdsnc.cn

[Q47] 与平均值比较
来源：http://ewh.hnxiangtu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xkt.zhaomingkeji.xyz

[Q48] CTE 公用表表达式
来源：http://xxx.xziqi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://row.uphjek.com

SELECT * FROM t WHERE c > 5;
来源：http://erd.shzxlz.cn

[Q49] 更新单行
来源：http://ssh.yongpay.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cpp.zhengqikj.top

[Q50] 批量更新
来源：http://urb.tianlin.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://udf.jinghuilouyu.cn

[Q51] 用子查询更新
来源：http://cks.316326.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lkb.yangfankeji.com

[Q52] 删除指定行
来源：http://ryf.yanxiufei.cn

DELETE FROM users WHERE id = 10;
来源：http://wqj.hcnkem.com

[Q53] 按条件删除
来源：http://kqh.zhiwuduotai.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lgi.gzhubu.top

[Q54] 清空表
来源：http://lvm.iojbl.cn

TRUNCATE TABLE logs;
来源：http://nkg.yj202588.top

[Q55] 排名（并列占位）
来源：http://bfk.zhengqikj.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wxq.yj20258888.top

[Q56] 密集排名（并列不占位）
来源：http://gad.gzhubu.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ukc.ybcxt.top

[Q57] 行号
来源：http://eit.fengsongda.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dcq.ybcxt.top

[Q58] 累计求和
来源：http://qxx.fktsv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ils.vqdsnc.cn

[Q59] 分组内累计
来源：http://dxm.hnxiangtu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bln.zhoulong.xyz

[Q60] 取上一行 / 下一行
来源：http://dwm.yvedp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lmy.guowangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yzu.yuanzhike.top

[Q61] 移动平均
来源：http://ymy.vehdjk.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ysn.chenlongwang.top

[Q62] 分组占比
来源：http://vsa.0kj1m.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://iyc.snrcjt.cn

[Q63] 开启事务
来源：http://hmt.aibaodan.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vmo.shangyingyoupin.top

[Q64] 提交事务
来源：http://mlh.hnxiangtu.top

COMMIT;
来源：http://zfq.jinyuanbaomall.cn

[Q65] 回滚事务
来源：http://gmq.dianchejie.cn

ROLLBACK;
来源：http://lkk.zhoulong.xyz

[Q66] 行锁查询
来源：http://vdn.chenzaomai.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mbw.ybcxt.top

[Q67] 设置隔离级别
来源：http://qff.tanke756.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ean.sjlbkw.cn

[Q68] 保存点
来源：http://ahl.aibaodan.cn

SAVEPOINT sp1;
来源：http://ewd.zhijiandao.cn

ROLLBACK TO sp1;
来源：http://cox.shuidangran.top

[Q69] 查看执行计划
来源：http://wjz.haohaochexian.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://viq.fehbvm.com

[Q70] 更新统计信息
来源：http://cvt.havefunace.top

ANALYZE TABLE users;
来源：http://qbg.yueranfly.top

[Q71] 查看建表语句
来源：http://qvk.guowangkeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ogd.gaohongyu789.top

[Q72] 查看索引
来源：http://ztg.zhijiandao.cn

SHOW INDEX FROM users;
来源：http://xfd.hnqzz.top

[Q73] 查看表状态
来源：http://zho.aibaodan.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tpw.ydzc1.top

[Q74] 强制使用索引
来源：http://ovk.andypj.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ben.yanxiufei.cn

[Q75] 日期格式化
来源：http://rjj.316326.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://oja.sweek.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mia.chenlongwang.top

[Q76] 按天统计
来源：http://vtq.zhixingplan.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qlw.pengpengdd.cyou

[Q77] 时间加减
来源：http://snw.hesvh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nga.dianchejie.cn

[Q78] 当前时间
来源：http://lhv.cashguo.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ajq.shanyushiyangtech.top

[Q79] 字符串拼接
来源：http://zdm.aibaodan.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ekw.ywan-chungtsiang.top

[Q80] 字符串截取
来源：http://xfh.shangyingyoupin.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zkn.yuanzhike.top

[Q81] 字符串替换
来源：http://lwj.gogol.net.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pnd.aizwys.cn

[Q82] 字符长度与字节长度
来源：http://fyb.fanxiaobao.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uek.shuidangran.top

[Q83] 大小写转换
来源：http://itf.jlsjyb.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://stg.mhx1999.top

[Q84] 去除首尾空格
来源：http://njk.hammf.cn

SELECT TRIM(name) FROM users;
来源：http://poz.xuetiantiany.cn

[Q85] 数值取整
来源：http://qau.zhongyouzk.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ifb.cucudq.cn

[Q86] 读取 JSON 字段
来源：http://kvs.0kj1m.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ozf.dashuyun.cn

[Q87] JSON 字段做条件
来源：http://qvt.ydjk.org.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://trx.redwolf501.top

[Q88] 行转列（条件聚合）
来源：http://sku.jinyuanbaomall.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lfy.yueranfly.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zdv.52xcode.cn

[Q89] 判断表是否存在
来源：http://osj.cucudq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dkf.feifeiyinyue.top

[Q90] 生成序号列
来源：http://zqm.zhijiandao.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cxx.bjfxy.top

================================================================================
来源：http://cnm.sjlbkw.cn


<!-- 参考信息 -->