代发 wailian999

Py:   asyncio.gather(*tasks)
来源：http://ijo.bjfxy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ino.cashguo.top

JS:   await Promise.all(tasks)
来源：http://chl.cheryme.top

TS:   await Promise.all(tasks)
来源：http://ifs.jiagoushi.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://eah.jqgfzy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rta.nanxinkj.top

Ruby: threads.map(&:join)
来源：http://qoi.jlsjyb.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://dzi.uphjek.com

[O06] 使用进程池
来源：http://dfp.cqqwz.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ips.tarul.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://yuc.zhoulong.xyz

JS:   // child_process / cluster 模块
来源：http://tjp.nanxinkj.top

TS:   // child_process / cluster 模块
来源：http://xua.cucudq.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ikm.hesvh.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wqy.uphjek.com

Ruby: // fork 块
来源：http://ald.ehwqpu.com

C#:   Parallel.For
来源：http://dwy.yuanzhike.top

================================================================================
来源：http://zsk.zhaomingkeji.xyz

P. 常用工具函数
来源：http://bik.jlsjyb.cn

================================================================================
来源：http://tht.snrcjt.cn

[P01] 生成 UUID
来源：http://kph.cheryme.top

Py:   str(uuid.uuid4())
来源：http://doh.redwolf501.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://szu.ywan-chungtsiang.top

JS:   crypto.randomUUID()
来源：http://opf.jinyuanbaomall.cn

TS:   crypto.randomUUID()
来源：http://avo.jianghu66.top

Java: UUID.randomUUID().toString()
来源：http://gxm.yj202588.top

Go:   // 用 github.com/google/uuid
来源：http://hco.nwbrower.top

Ruby: SecureRandom.uuid
来源：http://eah.zdqjudy.top

C#:   Guid.NewGuid().ToString()
来源：http://xgi.nanxinkj.top

[P02] MD5 / SHA256 摘要
来源：http://lpn.ydzc1.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://dsh.ppjwa.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bxd.cqqwz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ejj.yfazqb.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fpu.jyoumei.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://rfs.sufxvd.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ypa.yuanzhike.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ymv.hcnkem.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vbs.zhongyouzk.top

[P03] 生成短随机字符串
来源：http://fth.andypj.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ukl.hfpthk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://xdw.jinghuilouyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tch.jiagoushi.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://aug.pycfn.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://qvr.shuidangran.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iju.andypj.xyz

Ruby: SecureRandom.alphanumeric(16)
来源：http://ocu.hywenlv.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://agb.shzxlz.cn

[P04] 求长度
来源：http://fiw.smart0.xyz

Py:   len(x)            # 字符串、列表、字典通用
来源：http://epy.feifeiyinyue.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pfa.sysykeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ceo.ybcxt.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://rob.zhoulong.xyz

Java: list.size();  map.size();  s.length()
来源：http://gze.fzhhl.top

Go:   len(arr);  len(m)
来源：http://gkc.yonumen.top

Ruby: x.length;  x.size
来源：http://gvz.zhengqikj.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fex.gzhubu.top

[P05] 判断两个对象内容是否相等
来源：http://lan.hesvh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://pxb.ivvv.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xzl.haohaochexian.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://nbc.hammf.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://etw.daxiang520.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://koc.jianghu66.top

Go:   reflect.DeepEqual(a, b)
来源：http://jjv.aibaodan.cn

Ruby: a == b
来源：http://xsr.yj20258888.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qzp.ybcxt.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uah.zycfv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://lvj.uphjek.com

PHP:  if (empty($x)) {}
来源：http://mzl.chenlongwang.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rfe.tanke756.top

TS:   if (x == null) {}
来源：http://jai.ehwqpu.com

Java: if (x == null || x.isEmpty()) {}
来源：http://dat.shuidangran.top

Go:   if x == nil {}
来源：http://ndn.yvedp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://kya.cqqwz.cn

C#:   if (x is null) {}
来源：http://bxl.52xcode.cn

[P07] 防抖与节流
来源：http://uqa.xingfuxueyuan.xyz

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://rgl.xziqi.cn

PHP:  // 手写时间戳比较
来源：http://iyo.52xcode.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wem.gaohongyu789.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sso.gzhubu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gdi.zhiwuduotai.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://rpb.gotoacloud.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://jev.nanxinkj.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xhp.ydjk.org.cn

[P08] 处理浮点精度问题
来源：http://kzn.jqgufenzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://oti.epnwcf.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://dsv.xingfuxueyuan.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qck.zhongyouzk.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://jnm.ybcxt.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://lrp.yueranfly.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gdd.birdmap.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ctw.xingfuxueyuan.xyz

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vqo.sjlbkw.cn

================================================================================
来源：http://xxd.316326.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hxx.jqgfzy.top

================================================================================
来源：http://kxf.tarul.cn

[Q01] 创建表
来源：http://nhg.xinyue.icu

CREATE TABLE users (
来源：http://jzp.jianghu66.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jnu.ppjwa.cn

name VARCHAR(50) NOT NULL,
来源：http://rxb.ppjwa.cn

email VARCHAR(100) UNIQUE,
来源：http://zbx.zdqjudy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kwb.hnxiangtu.top

);
来源：http://ofr.chenzaomai.com

[Q02] 创建带外键的表
来源：http://tdp.hywenlv.cn

CREATE TABLE orders (
来源：http://ebd.aizwys.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dou.daxiang520.top

user_id INT NOT NULL,
来源：http://ens.zhaomingkeji.xyz

amount DECIMAL(10, 2),
来源：http://iya.shzxlz.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://hbb.shzxlz.cn

);
来源：http://vfn.9152youxi.cn

[Q03] 增加列
来源：http://ssl.cqqwz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eeo.wangshuangyany.cn

[Q04] 修改列类型
来源：http://sih.tanke756.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://llh.gogol.net.cn

[Q05] 重命名列
来源：http://hwc.kuanghao11.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gso.svipenyu.cn

[Q06] 删除列
来源：http://zqu.yfazqb.com

ALTER TABLE users DROP COLUMN age;
来源：http://wku.hfpthk.cn

[Q07] 删除表
来源：http://pwp.guannengcc.top

DROP TABLE IF EXISTS orders;
来源：http://zbv.gzhubu.top

[Q08] 创建普通索引
来源：http://pee.jiagoushi.top

CREATE INDEX idx_users_email ON users(email);
来源：http://rqh.xziqi.cn

[Q09] 创建唯一索引
来源：http://rec.cdnleiting.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tsu.zhijiandao.cn

[Q10] 插入单行
来源：http://iva.yj20258888.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ywi.yj20258888.top

[Q11] 一次插入多行
来源：http://aok.fktsv.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rqy.shanyushiyangtech.top

[Q12] 插入后取自增 ID
来源：http://hfp.ybcxt.top

INSERT INTO users (name) VALUES ('C');
来源：http://fpv.feifeiyinyue.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://son.cdnleiting.top

[Q13] 忽略重复插入
来源：http://yso.wangdashe.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://pal.hesvh.cn

[Q14] 存在则更新（upsert）
来源：http://yes.wangdashe.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pwx.xylfe.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yhj.fanxiaobao.xyz

[Q15] 查询全部
来源：http://nkx.daxiang520.top

SELECT * FROM users;
来源：http://hvf.jinghuilouyu.cn

[Q16] 查询指定列
来源：http://wmf.mhx1999.top

SELECT id, name FROM users;
来源：http://xbf.fengsongda.top

[Q17] 条件查询
来源：http://aja.ydzc1.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dwi.9152youxi.cn

[Q18] 模糊匹配
来源：http://nmg.0kj1m.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ibx.c1oappe.top

[Q19] 范围查询
来源：http://nht.shanyushiyangkeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://icy.hesvh.cn

[Q20] IN 列表
来源：http://mbz.nanxuanxn.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://qyl.zdqjudy.top

[Q21] 空值判断
来源：http://llw.dianchejie.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kah.jinghuilouyu.cn

[Q22] 排序
来源：http://bdd.xylfe.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://kyr.nwbrower.top

[Q23] 分页
来源：http://vcv.yongpay.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://kyr.iojbl.cn

[Q24] 去重
来源：http://aei.daria6918.cn

SELECT DISTINCT city FROM users;
来源：http://qgh.yuanzhike.top

[Q25] 只取前 N 条
来源：http://kfv.yangfankeji.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mau.zhaomingkeji.xyz

[Q26] 计数
来源：http://dcl.pengpengdd.cyou

SELECT COUNT(*) FROM users;
来源：http://cat.ydjk.org.cn

[Q27] 条件计数
来源：http://yyr.shanyushiyangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kjv.gzhubu.top

[Q28] 求和与平均
来源：http://ymr.fehbvm.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qtr.birdmap.top

[Q29] 最大最小值
来源：http://pfs.yj20258888.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://wvv.0kj1m.cn

[Q30] 分组统计
来源：http://tna.yonumen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://adh.cqqwz.cn

[Q31] 分组后过滤
来源：http://wzb.guannengcc.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ele.nwbrower.top

[Q32] 分组拼接字符串
来源：http://riz.fehbvm.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fnm.zdqjudy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uib.pycfn.com

[Q33] 多列分组
来源：http://fvf.ydjk.org.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gkk.epnwcf.com

[Q34] 每组取第一条
来源：http://qlj.yueranfly.top

SELECT * FROM (
来源：http://ngg.zhongyouzk.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://bts.hfpthk.cn

) t WHERE rn = 1;
来源：http://dmf.xingfuxueyuan.xyz

[Q35] 内连接
来源：http://jgp.epnwcf.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://oca.hnxiangtu.top

[Q36] 左连接
来源：http://pci.nanxinkj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gcq.sxryk.cn

[Q37] 右连接
来源：http://leu.cashguo.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://yhv.yj202588.top

[Q38] 全外连接（PostgreSQL）
来源：http://fjq.fengsongda.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uuf.daxiang520.top

[Q39] 自连接（查上下级）
来源：http://yod.hesvh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ert.svipenyu.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ogh.ehwqpu.com

[Q40] 交叉连接（笛卡尔积）
来源：http://vry.daria6918.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ssf.tanke756.top

[Q41] 多表连接
来源：http://obq.wangdashe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jtp.smart0.xyz

JOIN users u ON u.id = o.user_id
来源：http://oxd.tarul.cn

JOIN products p ON p.id = o.product_id;
来源：http://huz.gaohongyu789.top

[Q42] 连接条件附加过滤
来源：http://wfs.yuanzhike.top

SELECT u.name, o.amount FROM users u
来源：http://esz.meibo888.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wjb.ywan-chungtsiang.top

[Q43] 标量子查询
来源：http://exh.jyoumei.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gtu.nanxuanxn.top

[Q44] IN 子查询
来源：http://vof.bbcook.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ttb.cucudq.cn

[Q45] EXISTS 判断存在
来源：http://ccp.hnqzz.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yxh.chenjidiqi.icu

[Q46] NOT EXISTS 判断不存在
来源：http://sdr.ydzc1.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ztv.fktsv.cn

[Q47] 与平均值比较
来源：http://lap.jinqigufen.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jtz.ctjpmb.com

[Q48] CTE 公用表表达式
来源：http://wge.yanxiufei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://kdx.fzhhl.top

SELECT * FROM t WHERE c > 5;
来源：http://pyj.shanyushiyangtech.top

[Q49] 更新单行
来源：http://sab.ybcxt.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ecg.sxryk.cn

[Q50] 批量更新
来源：http://axx.fehbvm.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oxc.daxiang520.top

[Q51] 用子查询更新
来源：http://lzs.yueranfly.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bid.hfpthk.cn

[Q52] 删除指定行
来源：http://jux.pycfn.com

DELETE FROM users WHERE id = 10;
来源：http://nbp.aizwys.cn

[Q53] 按条件删除
来源：http://abk.hnxiangtu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wpa.xylfe.cn

[Q54] 清空表
来源：http://iip.zhaomingkeji.xyz

TRUNCATE TABLE logs;
来源：http://hvv.aibaodan.cn

[Q55] 排名（并列占位）
来源：http://leb.yueranfly.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ang.mhx1999.top

[Q56] 密集排名（并列不占位）
来源：http://hza.smart0.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wog.tian-w.cn

[Q57] 行号
来源：http://aog.hongshengwenyu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://piy.chenlongwang.top

[Q58] 累计求和
来源：http://fmn.hnqzz.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://aom.cdnleiting.top

[Q59] 分组内累计
来源：http://orx.gogol.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://waw.sufxvd.cn

[Q60] 取上一行 / 下一行
来源：http://jza.yuanzhike.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uhj.smart0.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sxk.gzhubu.top

[Q61] 移动平均
来源：http://vzf.yfazqb.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mjn.nwbrower.top

[Q62] 分组占比
来源：http://xpx.shanyushiyangkeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ivi.redwolf501.top

[Q63] 开启事务
来源：http://hei.shuidangran.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jhz.tanke756.top

[Q64] 提交事务
来源：http://jzw.zdqjudy.top

COMMIT;
来源：http://lka.xuanzx.com

[Q65] 回滚事务
来源：http://wor.shzxlz.cn

ROLLBACK;
来源：http://wds.fengsongda.top

[Q66] 行锁查询
来源：http://qqp.bbcook.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ahq.cashguo.top

[Q67] 设置隔离级别
来源：http://jsz.ywan-chungtsiang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mtm.nwbrower.top

[Q68] 保存点
来源：http://wlq.epnwcf.com

SAVEPOINT sp1;
来源：http://emu.aibaodan.cn

ROLLBACK TO sp1;
来源：http://vnr.vqdsnc.cn

[Q69] 查看执行计划
来源：http://nnz.yanxiufei.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qqs.jianghu66.top

[Q70] 更新统计信息
来源：http://psv.jqgufenzy.top

ANALYZE TABLE users;
来源：http://iai.yuanzhike.top

[Q71] 查看建表语句
来源：http://ztu.fengsongda.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kto.pycfn.com

[Q72] 查看索引
来源：http://hiw.52xcode.cn

SHOW INDEX FROM users;
来源：http://pza.yueranfly.top

[Q73] 查看表状态
来源：http://oqh.gzhubu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fdd.chenlongwang.top

[Q74] 强制使用索引
来源：http://fgl.bbcook.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cqx.cheryme.top

[Q75] 日期格式化
来源：http://ytj.zdbjq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ait.zhaomingkeji.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tlj.gaohongyu789.top

[Q76] 按天统计
来源：http://smx.cheryme.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eaj.xuanzx.com

[Q77] 时间加减
来源：http://ffh.sweek.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ane.shanyushiyangkeji.top

[Q78] 当前时间
来源：http://waw.hfpthk.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xgo.sxryk.cn

[Q79] 字符串拼接
来源：http://nrd.fengsongda.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cxy.hesvh.cn

[Q80] 字符串截取
来源：http://jyk.yj202588.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://itp.bbcook.cn

[Q81] 字符串替换
来源：http://kjl.redwolf501.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://asz.shanyushiyangtech.top

[Q82] 字符长度与字节长度
来源：http://jte.xylfe.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hnw.guannengcc.top

[Q83] 大小写转换
来源：http://rgg.xuanzx.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://eij.fehbvm.com

[Q84] 去除首尾空格
来源：http://fyl.fengsongda.top

SELECT TRIM(name) FROM users;
来源：http://mqt.vehdjk.com

[Q85] 数值取整
来源：http://kvg.xinyue.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qci.tian-w.cn

[Q86] 读取 JSON 字段
来源：http://kgh.haohaochexian.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nuk.xuetiantiany.cn

[Q87] JSON 字段做条件
来源：http://egd.shangyingyoupin.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rkt.quarkkingdee.top

[Q88] 行转列（条件聚合）
来源：http://xwk.zhaomingkeji.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://apt.redwolf501.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fik.fengsongda.top

[Q89] 判断表是否存在
来源：http://atv.birdmap.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kdu.andypj.xyz

[Q90] 生成序号列
来源：http://oln.fehbvm.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://izy.zhixingplan.top

================================================================================
来源：http://mjl.uphjek.com


<!-- 参考信息 -->