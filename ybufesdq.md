代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ruy.yuanzhike.top

JS:   async function f() { await g(); }
来源：http://vvg.fengsongda.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://rpn.vqdsnc.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://sxe.yuxming.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://kpf.tanke756.top

Ruby: # 用 Fiber 或 async gem
来源：http://rvi.gaohongyu789.top

C#:   async Task F() { await G(); }
来源：http://jgj.yangfankeji.com

[O05] 并发执行并等待全部完成
来源：http://qyy.bbcook.cn

Py:   asyncio.gather(*tasks)
来源：http://dyp.0kj1m.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ttz.bbcook.cn

JS:   await Promise.all(tasks)
来源：http://owf.hnxiangtu.top

TS:   await Promise.all(tasks)
来源：http://pou.jinghuilouyu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mxy.jianghu66.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cvz.chenjidiqi.icu

Ruby: threads.map(&:join)
来源：http://uiy.tanke756.top

C#:   await Task.WhenAll(t1, t2)
来源：http://egf.haohaochexian.top

[O06] 使用进程池
来源：http://tad.haohaochexian.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://uro.zhaomingkeji.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://awv.svipenyu.cn

JS:   // child_process / cluster 模块
来源：http://jbg.9152youxi.cn

TS:   // child_process / cluster 模块
来源：http://pcm.shuidangran.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ltl.andypj.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://ofu.zdbjq.cn

Ruby: // fork 块
来源：http://iwh.hywenlv.cn

C#:   Parallel.For
来源：http://sod.yanxiufei.cn

================================================================================
来源：http://fkz.yfazqb.com

P. 常用工具函数
来源：http://qoj.pycfn.com

================================================================================
来源：http://xjb.cashguo.top

[P01] 生成 UUID
来源：http://ncd.tian-w.cn

Py:   str(uuid.uuid4())
来源：http://anp.zhoulong.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://zva.gzhubu.top

JS:   crypto.randomUUID()
来源：http://svh.pengpengdd.cyou

TS:   crypto.randomUUID()
来源：http://lgl.guowangkeji.top

Java: UUID.randomUUID().toString()
来源：http://iwh.haohaochexian.top

Go:   // 用 github.com/google/uuid
来源：http://qjp.tanke756.top

Ruby: SecureRandom.uuid
来源：http://rfp.c1oappe.top

C#:   Guid.NewGuid().ToString()
来源：http://nin.xylfe.cn

[P02] MD5 / SHA256 摘要
来源：http://nyo.yj202588.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://aqu.hcnkem.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://yri.quarkkingdee.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yzz.zycfv.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hcr.jinghuilouyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wzm.gzhubu.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rmz.cashguo.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://xve.tarul.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dbf.xingfuxueyuan.xyz

[P03] 生成短随机字符串
来源：http://edv.uphjek.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://ecc.yueranfly.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gow.nanxinkj.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://zsf.tianlin.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://pge.hfpthk.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gcg.ywan-chungtsiang.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zgv.xuetiantiany.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://xlp.ctjpmb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xwe.zhixingplan.top

[P04] 求长度
来源：http://eic.ybcxt.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hvr.kuanghao11.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://klz.hnxiangtu.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://psb.zhongyouzk.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qrd.vqdsnc.cn

Java: list.size();  map.size();  s.length()
来源：http://pzg.sysykeji.top

Go:   len(arr);  len(m)
来源：http://pak.jiagoushi.top

Ruby: x.length;  x.size
来源：http://teq.52xcode.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://qla.jlsjyb.cn

[P05] 判断两个对象内容是否相等
来源：http://wwl.gogol.net.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://ghh.quarkkingdee.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hrw.kuanghao11.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ytl.ydzc1.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jfq.yuanzhike.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://xga.jqgfzy.top

Go:   reflect.DeepEqual(a, b)
来源：http://hqj.vehdjk.com

Ruby: a == b
来源：http://aja.chenlongwang.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://swx.ehwqpu.com

[P06] 综合判空（null / 空串 / 空集合）
来源：http://xzm.gogol.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://xie.ybcxt.top

PHP:  if (empty($x)) {}
来源：http://jsw.jyoumei.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iau.gotoacloud.top

TS:   if (x == null) {}
来源：http://sbb.sjlbkw.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://eco.tian-w.cn

Go:   if x == nil {}
来源：http://eer.mhx1999.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sdo.cucudq.cn

C#:   if (x is null) {}
来源：http://toy.yonumen.top

[P07] 防抖与节流
来源：http://usq.52xcode.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://zky.ctjpmb.com

PHP:  // 手写时间戳比较
来源：http://hah.cdnleiting.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hcv.uphjek.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gwn.iojbl.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://fex.jlsjyb.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://jut.shanyushiyangtech.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xtq.aizwys.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://lqb.zhongyouzk.top

[P08] 处理浮点精度问题
来源：http://szs.quarkkingdee.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://vqs.jlsjyb.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ser.xingfuxueyuan.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kgc.nanxinkj.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lkz.yuanzhike.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nrf.vehdjk.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vru.bjfxy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nsj.ywan-chungtsiang.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://fxy.ppjwa.cn

================================================================================
来源：http://zcy.chenjidiqi.icu

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fnc.9152youxi.cn

================================================================================
来源：http://xcn.vqdsnc.cn

[Q01] 创建表
来源：http://ugs.yueranfly.top

CREATE TABLE users (
来源：http://uxk.zhoulong.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://alu.pengpengdd.cyou

name VARCHAR(50) NOT NULL,
来源：http://eqk.daria6918.cn

email VARCHAR(100) UNIQUE,
来源：http://sfw.jyoumei.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ljl.yj202588.top

);
来源：http://mgf.birdmap.top

[Q02] 创建带外键的表
来源：http://zvy.feifeiyinyue.top

CREATE TABLE orders (
来源：http://nba.yuxming.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://kno.chenjidiqi.icu

user_id INT NOT NULL,
来源：http://reg.jianghu66.top

amount DECIMAL(10, 2),
来源：http://ikt.ivvv.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kkb.guowangkeji.top

);
来源：http://mqv.shangyingyoupin.top

[Q03] 增加列
来源：http://khi.jyoumei.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://suf.pycfn.com

[Q04] 修改列类型
来源：http://mda.hcnkem.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kme.jqgufenzy.top

[Q05] 重命名列
来源：http://uby.dianchejie.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rso.yonumen.top

[Q06] 删除列
来源：http://rsj.jinqigfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://gvr.jiagoushi.top

[Q07] 删除表
来源：http://wbh.yonumen.top

DROP TABLE IF EXISTS orders;
来源：http://hlv.dianchejie.cn

[Q08] 创建普通索引
来源：http://anq.yvedp.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jhp.vehdjk.com

[Q09] 创建唯一索引
来源：http://fdf.havefunace.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://fgp.xingfuxueyuan.xyz

[Q10] 插入单行
来源：http://smy.zhoulong.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mmj.ybcxt.top

[Q11] 一次插入多行
来源：http://vvp.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://exs.cashguo.top

[Q12] 插入后取自增 ID
来源：http://tgj.iojbl.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ypv.cashguo.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wxl.kuanghao11.cn

[Q13] 忽略重复插入
来源：http://uzl.hcnkem.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vxz.aizwys.cn

[Q14] 存在则更新（upsert）
来源：http://rjg.gogol.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://pvw.316326.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bsm.svipenyu.cn

[Q15] 查询全部
来源：http://rwr.yvedp.cn

SELECT * FROM users;
来源：http://lxk.yangfankeji.com

[Q16] 查询指定列
来源：http://rbo.tarul.cn

SELECT id, name FROM users;
来源：http://bml.xuetiantiany.cn

[Q17] 条件查询
来源：http://cfx.cheryme.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cor.iojbl.cn

[Q18] 模糊匹配
来源：http://rww.zhoulong.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dbs.chenlongwang.top

[Q19] 范围查询
来源：http://wqc.yangfankeji.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pps.sjlbkw.cn

[Q20] IN 列表
来源：http://opx.ydjk.org.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tjo.fanxiaobao.xyz

[Q21] 空值判断
来源：http://wme.yj20258888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://tgs.fktsv.cn

[Q22] 排序
来源：http://ujc.52xcode.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://laf.yvedp.cn

[Q23] 分页
来源：http://zwx.52xcode.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qmz.svipenyu.cn

[Q24] 去重
来源：http://crl.tian-w.cn

SELECT DISTINCT city FROM users;
来源：http://mgb.sufxvd.cn

[Q25] 只取前 N 条
来源：http://oil.sufxvd.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vbd.yj202588.top

[Q26] 计数
来源：http://rbj.zdqjudy.top

SELECT COUNT(*) FROM users;
来源：http://qob.wangshuangyany.cn

[Q27] 条件计数
来源：http://eda.zhongyouzk.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ikw.shangyingyoupin.top

[Q28] 求和与平均
来源：http://sax.wangdashe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hvg.sjlbkw.cn

[Q29] 最大最小值
来源：http://pog.jiagoushi.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://pau.hywenlv.cn

[Q30] 分组统计
来源：http://jnu.zhongyouzk.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bhu.chenjidiqi.icu

[Q31] 分组后过滤
来源：http://xmz.svipenyu.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ame.dashuyun.cn

[Q32] 分组拼接字符串
来源：http://wah.tanke756.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://aui.feifeiyinyue.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cnd.sweek.top

[Q33] 多列分组
来源：http://qqa.zhiwuduotai.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qwz.chenlongwang.top

[Q34] 每组取第一条
来源：http://eni.sxryk.cn

SELECT * FROM (
来源：http://zvk.sysykeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ule.hfpthk.cn

) t WHERE rn = 1;
来源：http://ojn.yonumen.top

[Q35] 内连接
来源：http://bmz.zhijiandao.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://for.shanyushiyangkeji.top

[Q36] 左连接
来源：http://tpr.redwolf501.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ips.sweek.top

[Q37] 右连接
来源：http://ipl.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zqi.wangshuangyany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://onz.feifeiyinyue.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qyk.bjfxy.top

[Q39] 自连接（查上下级）
来源：http://eyy.shanyushiyangtech.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://jwg.nanxinkj.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ukw.ppjwa.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://cry.yuanzhike.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zyg.jiagoushi.top

[Q41] 多表连接
来源：http://ewc.ehwqpu.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://zed.tian-w.cn

JOIN users u ON u.id = o.user_id
来源：http://wbo.jinqigfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://ofj.jqgufenzy.top

[Q42] 连接条件附加过滤
来源：http://uye.daxiang520.top

SELECT u.name, o.amount FROM users u
来源：http://vgg.chenlongwang.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lva.feifeiyinyue.top

[Q43] 标量子查询
来源：http://cvu.hesvh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iso.redwolf501.top

[Q44] IN 子查询
来源：http://ino.yj20258888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cnj.shanyushiyangtech.top

[Q45] EXISTS 判断存在
来源：http://orp.9152youxi.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fkl.gogol.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://dey.iojbl.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dri.shanyushiyangtech.top

[Q47] 与平均值比较
来源：http://usr.9152youxi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mzo.hfpthk.cn

[Q48] CTE 公用表表达式
来源：http://tte.ydjk.org.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ott.wangshuangyany.cn

SELECT * FROM t WHERE c > 5;
来源：http://qit.yanxiufei.cn

[Q49] 更新单行
来源：http://bww.tianlin.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ujh.xuetiantiany.cn

[Q50] 批量更新
来源：http://pvf.zhaomingkeji.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dss.sjlbkw.cn

[Q51] 用子查询更新
来源：http://eeo.wangdashe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nap.dashuyun.cn

[Q52] 删除指定行
来源：http://rjc.sxryk.cn

DELETE FROM users WHERE id = 10;
来源：http://hiz.ehwqpu.com

[Q53] 按条件删除
来源：http://snk.hongshengwenyu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://niv.ctjpmb.com

[Q54] 清空表
来源：http://pit.feifeiyinyue.top

TRUNCATE TABLE logs;
来源：http://lvs.gaohongyu789.top

[Q55] 排名（并列占位）
来源：http://rde.9152youxi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cvq.zhiwuduotai.top

[Q56] 密集排名（并列不占位）
来源：http://yft.shuidangran.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nna.9152youxi.cn

[Q57] 行号
来源：http://ccf.xinyue.icu

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zru.shzxlz.cn

[Q58] 累计求和
来源：http://aur.cheryme.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://adf.haohaochexian.top

[Q59] 分组内累计
来源：http://npq.xuetiantiany.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nvt.chenlongwang.top

[Q60] 取上一行 / 下一行
来源：http://gak.sxryk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dcq.jqgfzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zdd.gzhubu.top

[Q61] 移动平均
来源：http://ugk.cheryme.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zxc.yueranfly.top

[Q62] 分组占比
来源：http://jxr.xuanzx.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vcn.cqqwz.cn

[Q63] 开启事务
来源：http://hvf.feifeiyinyue.top

START TRANSACTION;                -- 或 BEGIN
来源：http://yhe.yfazqb.com

[Q64] 提交事务
来源：http://apt.shuidangran.top

COMMIT;
来源：http://ynr.wangshuangyany.cn

[Q65] 回滚事务
来源：http://vuc.316326.xyz

ROLLBACK;
来源：http://lfi.fktsv.cn

[Q66] 行锁查询
来源：http://hxd.havefunace.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://utx.sxryk.cn

[Q67] 设置隔离级别
来源：http://dkd.9152youxi.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://olr.chenjidiqi.icu

[Q68] 保存点
来源：http://nck.zhaomingkeji.xyz

SAVEPOINT sp1;
来源：http://ltd.nwbrower.top

ROLLBACK TO sp1;
来源：http://xkd.zhixingplan.top

[Q69] 查看执行计划
来源：http://zwy.ppjwa.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cvl.jqgufenzy.top

[Q70] 更新统计信息
来源：http://oip.shanyushiyangkeji.top

ANALYZE TABLE users;
来源：http://jrh.quarkkingdee.top

[Q71] 查看建表语句
来源：http://fqo.redwolf501.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fox.ppjwa.cn

[Q72] 查看索引
来源：http://fks.zdbjq.cn

SHOW INDEX FROM users;
来源：http://zlo.jyoumei.cn

[Q73] 查看表状态
来源：http://gkn.yfazqb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://wzq.hcnkem.com

[Q74] 强制使用索引
来源：http://qpo.tianlin.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tjp.ehwqpu.com

[Q75] 日期格式化
来源：http://yww.ybcxt.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fzz.yvedp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eiy.zdqjudy.top

[Q76] 按天统计
来源：http://kcg.zdbjq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://glj.cdnleiting.top

[Q77] 时间加减
来源：http://ynp.iojbl.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hku.cheryme.top

[Q78] 当前时间
来源：http://azn.jianghu66.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hhk.mhx1999.top

[Q79] 字符串拼接
来源：http://vue.gaohongyu789.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://axg.yanxiufei.cn

[Q80] 字符串截取
来源：http://kvj.jqgufenzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mmz.zhongyouzk.top

[Q81] 字符串替换
来源：http://xex.0kj1m.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cgk.fanxiaobao.xyz

[Q82] 字符长度与字节长度
来源：http://bmk.aibaodan.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hyl.fzhhl.top

[Q83] 大小写转换
来源：http://cuh.xingfuxueyuan.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bod.zhixingplan.top

[Q84] 去除首尾空格
来源：http://raz.hnqzz.top

SELECT TRIM(name) FROM users;
来源：http://lrm.vehdjk.com

[Q85] 数值取整
来源：http://lbq.fengsongda.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xnh.cdnleiting.top

[Q86] 读取 JSON 字段
来源：http://qwd.daxiang520.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bsx.jianghu66.top

[Q87] JSON 字段做条件
来源：http://fdz.hysaishi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dds.vqdsnc.cn


<!-- 参考信息 -->