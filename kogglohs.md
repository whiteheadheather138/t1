代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://xxf.zhoulong.xyz

C#:   lock (gate) { shared++; }
来源：http://izm.hcnkem.com

[O04] 定义异步函数并等待
来源：http://pzh.smart0.xyz

Py:   async def f():⏎    await g()
来源：http://sbz.aibaodan.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yyv.vehdjk.com

JS:   async function f() { await g(); }
来源：http://bgf.ctjpmb.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://tjs.xziqi.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://yhz.ydzc1.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://scf.hcnkem.com

Ruby: # 用 Fiber 或 async gem
来源：http://krf.bjfxy.top

C#:   async Task F() { await G(); }
来源：http://wwz.andypj.xyz

[O05] 并发执行并等待全部完成
来源：http://peg.redwolf501.top

Py:   asyncio.gather(*tasks)
来源：http://wan.sweek.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xlu.jinqigfzy.top

JS:   await Promise.all(tasks)
来源：http://fde.vehdjk.com

TS:   await Promise.all(tasks)
来源：http://gvj.zhaomingkeji.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://azm.zhoulong.xyz

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ymc.snrcjt.cn

Ruby: threads.map(&:join)
来源：http://jms.c1oappe.top

C#:   await Task.WhenAll(t1, t2)
来源：http://bin.316326.xyz

[O06] 使用进程池
来源：http://oit.yonumen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ifi.ydjk.org.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://ssv.shanyushiyangtech.top

JS:   // child_process / cluster 模块
来源：http://yrn.ydzc1.top

TS:   // child_process / cluster 模块
来源：http://fga.jiagoushi.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ywz.dianchejie.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zcn.havefunace.top

Ruby: // fork 块
来源：http://fxl.mhx1999.top

C#:   Parallel.For
来源：http://xtc.daxiang520.top

================================================================================
来源：http://rtn.nanxinkj.top

P. 常用工具函数
来源：http://fhj.jqgfzy.top

================================================================================
来源：http://gid.yanxiufei.cn

[P01] 生成 UUID
来源：http://vqf.yvedp.cn

Py:   str(uuid.uuid4())
来源：http://nwq.havefunace.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rst.jinyuanbaomall.cn

JS:   crypto.randomUUID()
来源：http://inl.52xcode.cn

TS:   crypto.randomUUID()
来源：http://axv.jinqigfzy.top

Java: UUID.randomUUID().toString()
来源：http://atz.sysykeji.top

Go:   // 用 github.com/google/uuid
来源：http://rdm.tian-w.cn

Ruby: SecureRandom.uuid
来源：http://tzb.zhixingplan.top

C#:   Guid.NewGuid().ToString()
来源：http://rrd.yongpay.top

[P02] MD5 / SHA256 摘要
来源：http://gto.hfpthk.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://jms.bbcook.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://mbr.hesvh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xms.tianlin.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://glq.dashuyun.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://qsk.guannengcc.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bwj.feifeiyinyue.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oul.hesvh.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://euz.nwbrower.top

[P03] 生成短随机字符串
来源：http://jmg.52xcode.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://trr.fehbvm.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://lcx.cashguo.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dnq.ctjpmb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hwl.tanke756.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gki.xinyue.icu

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://dun.hammf.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://pqb.quarkkingdee.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ocf.yangfankeji.com

[P04] 求长度
来源：http://suu.zhongyouzk.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gwg.tarul.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vlj.yuanzhike.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ehq.daria6918.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wwo.epnwcf.com

Java: list.size();  map.size();  s.length()
来源：http://cxd.jinqigufen.top

Go:   len(arr);  len(m)
来源：http://yod.guowangkeji.top

Ruby: x.length;  x.size
来源：http://zqf.ppjwa.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://hup.zhengqikj.top

[P05] 判断两个对象内容是否相等
来源：http://yum.hysaishi.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://cft.316326.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cxe.yuanzhike.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bhn.gogol.net.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://stl.jinyuanbaomall.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://ddo.hysaishi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ksp.yuanzhike.top

Ruby: a == b
来源：http://vmh.hongshengwenyu.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://kkl.fanxiaobao.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ugy.wangdashe.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://zma.tarul.cn

PHP:  if (empty($x)) {}
来源：http://poh.hysaishi.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zrw.yfazqb.com

TS:   if (x == null) {}
来源：http://rtl.aibaodan.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://eyj.yongpay.top

Go:   if x == nil {}
来源：http://rsx.fehbvm.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://sgh.hongshengwenyu.top

C#:   if (x is null) {}
来源：http://yww.jianghu66.top

[P07] 防抖与节流
来源：http://fhf.ydzc1.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://cjl.yangfankeji.com

PHP:  // 手写时间戳比较
来源：http://kdb.hongshengwenyu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://snj.fanxiaobao.xyz

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://onc.9152youxi.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://rly.shuidangran.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://ily.zhiwuduotai.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://hjn.feifeiyinyue.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uyz.shangyingyoupin.top

[P08] 处理浮点精度问题
来源：http://fwb.fktsv.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://rsk.mhx1999.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ztu.316326.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://hpg.gotoacloud.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://kot.zdbjq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mmr.yj20258888.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://bli.smart0.xyz

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://iex.jinghuilouyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://jhd.chenlongwang.top

================================================================================
来源：http://pib.bjfxy.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://dkn.haohaochexian.top

================================================================================
来源：http://nvf.hnqzz.top

[Q01] 创建表
来源：http://hli.yfazqb.com

CREATE TABLE users (
来源：http://kxc.shanyushiyangkeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hgy.jinqigfzy.top

name VARCHAR(50) NOT NULL,
来源：http://ddw.andypj.xyz

email VARCHAR(100) UNIQUE,
来源：http://kdx.sweek.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ezf.guannengcc.top

);
来源：http://cuz.tanke756.top

[Q02] 创建带外键的表
来源：http://kku.ybcxt.top

CREATE TABLE orders (
来源：http://xqc.guannengcc.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fco.cdnleiting.top

user_id INT NOT NULL,
来源：http://rrr.jiagoushi.top

amount DECIMAL(10, 2),
来源：http://imj.wangdashe.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://qsr.jinqigufen.top

);
来源：http://ujp.xuanzx.com

[Q03] 增加列
来源：http://rzm.yonumen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://yym.jinqigufen.top

[Q04] 修改列类型
来源：http://vks.dianchejie.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://atv.fzhhl.top

[Q05] 重命名列
来源：http://gew.yuanzhike.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tvy.ctjpmb.com

[Q06] 删除列
来源：http://iam.xingfuxueyuan.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://xzs.jlsjyb.cn

[Q07] 删除表
来源：http://erb.nanxuanxn.top

DROP TABLE IF EXISTS orders;
来源：http://wye.9152youxi.cn

[Q08] 创建普通索引
来源：http://zos.xylfe.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ktb.vqdsnc.cn

[Q09] 创建唯一索引
来源：http://zre.zhiwuduotai.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wai.shzxlz.cn

[Q10] 插入单行
来源：http://jfd.daria6918.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qya.jianghu66.top

[Q11] 一次插入多行
来源：http://ejn.zhongyouzk.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hqb.cashguo.top

[Q12] 插入后取自增 ID
来源：http://zje.yongpay.top

INSERT INTO users (name) VALUES ('C');
来源：http://dws.wangshuangyany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ado.uphjek.com

[Q13] 忽略重复插入
来源：http://nsv.yueranfly.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://cxi.dashuyun.cn

[Q14] 存在则更新（upsert）
来源：http://kxe.xinyue.icu

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://upy.gzhubu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mzu.chenzaomai.com

[Q15] 查询全部
来源：http://bgw.zhoulong.xyz

SELECT * FROM users;
来源：http://pev.chenzaomai.com

[Q16] 查询指定列
来源：http://hhw.aizwys.cn

SELECT id, name FROM users;
来源：http://hmz.ctjpmb.com

[Q17] 条件查询
来源：http://twk.tanke756.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jix.zdqjudy.top

[Q18] 模糊匹配
来源：http://uub.52xcode.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qnj.hesvh.cn

[Q19] 范围查询
来源：http://nrw.hywenlv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://saf.jlsjyb.cn

[Q20] IN 列表
来源：http://yan.hfpthk.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://art.jiagoushi.top

[Q21] 空值判断
来源：http://hgw.jqgfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://rdu.vehdjk.com

[Q22] 排序
来源：http://hhj.yj20258888.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mwq.pycfn.com

[Q23] 分页
来源：http://euv.zycfv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://jte.zhongyouzk.top

[Q24] 去重
来源：http://piw.zhaomingkeji.xyz

SELECT DISTINCT city FROM users;
来源：http://zxr.jinyuanbaomall.cn

[Q25] 只取前 N 条
来源：http://lyu.sufxvd.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://efy.hysaishi.cn

[Q26] 计数
来源：http://kuh.shanyushiyangkeji.top

SELECT COUNT(*) FROM users;
来源：http://yji.xingfuxueyuan.xyz

[Q27] 条件计数
来源：http://cba.guowangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hjg.gotoacloud.top

[Q28] 求和与平均
来源：http://nnd.wangdashe.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://jfq.dashuyun.cn

[Q29] 最大最小值
来源：http://ypg.hammf.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://wla.shuidangran.top

[Q30] 分组统计
来源：http://bmj.zhiwuduotai.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://tui.tanke756.top

[Q31] 分组后过滤
来源：http://whm.jinqigufen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://rjc.hcnkem.com

[Q32] 分组拼接字符串
来源：http://inu.cashguo.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ted.yueranfly.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://axa.hysaishi.cn

[Q33] 多列分组
来源：http://ups.epnwcf.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sff.yuanzhike.top

[Q34] 每组取第一条
来源：http://iuj.meibo888.top

SELECT * FROM (
来源：http://kaw.daxiang520.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ftx.ydjk.org.cn

) t WHERE rn = 1;
来源：http://nzi.ydjk.org.cn

[Q35] 内连接
来源：http://swv.sufxvd.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jby.bbcook.cn

[Q36] 左连接
来源：http://gti.quarkkingdee.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hav.fengsongda.top

[Q37] 右连接
来源：http://zbr.iojbl.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iui.daria6918.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xbe.ydjk.org.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zzs.epnwcf.com

[Q39] 自连接（查上下级）
来源：http://twm.cucudq.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://btg.gzhubu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mgs.nwbrower.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hov.yonumen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zmc.aizwys.cn

[Q41] 多表连接
来源：http://tud.iojbl.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://snk.cqqwz.cn

JOIN users u ON u.id = o.user_id
来源：http://pyx.sxryk.cn

JOIN products p ON p.id = o.product_id;
来源：http://abc.aizwys.cn

[Q42] 连接条件附加过滤
来源：http://rnh.andypj.xyz

SELECT u.name, o.amount FROM users u
来源：http://uqd.shzxlz.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://bhz.wangdashe.top

[Q43] 标量子查询
来源：http://dqk.nanxuanxn.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zah.yonumen.top

[Q44] IN 子查询
来源：http://svv.hongshengwenyu.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fme.cucudq.cn

[Q45] EXISTS 判断存在
来源：http://arf.ppjwa.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://myc.yj20258888.top

[Q46] NOT EXISTS 判断不存在
来源：http://byu.zhoulong.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://stn.ivvv.top

[Q47] 与平均值比较
来源：http://noz.hysaishi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xqq.kuanghao11.cn

[Q48] CTE 公用表表达式
来源：http://jwn.zhijiandao.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://urq.shanyushiyangtech.top

SELECT * FROM t WHERE c > 5;
来源：http://mrh.kuanghao11.cn

[Q49] 更新单行
来源：http://xdt.svipenyu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dwj.andypj.xyz

[Q50] 批量更新
来源：http://une.vqdsnc.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://byc.jqgfzy.top

[Q51] 用子查询更新
来源：http://zir.zhongyouzk.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dbk.bjfxy.top

[Q52] 删除指定行
来源：http://qyy.fzhhl.top

DELETE FROM users WHERE id = 10;
来源：http://lxj.jinghuilouyu.cn

[Q53] 按条件删除
来源：http://rmi.gzhubu.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kjs.ivvv.top

[Q54] 清空表
来源：http://ubb.birdmap.top

TRUNCATE TABLE logs;
来源：http://pos.52xcode.cn

[Q55] 排名（并列占位）
来源：http://mlv.vqdsnc.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ays.xuanzx.com

[Q56] 密集排名（并列不占位）
来源：http://fuh.tanke756.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ogc.ehwqpu.com

[Q57] 行号
来源：http://wmt.shanyushiyangtech.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ygq.yuanzhike.top

[Q58] 累计求和
来源：http://vjv.hammf.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sgd.316326.xyz

[Q59] 分组内累计
来源：http://ewm.hnxiangtu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://owu.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://iql.hesvh.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pts.ivvv.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ikh.zhoulong.xyz

[Q61] 移动平均
来源：http://uar.xinyue.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oek.zhoulong.xyz

[Q62] 分组占比
来源：http://gsv.jinqigfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tkc.nanxinkj.top

[Q63] 开启事务
来源：http://kqf.zhengqikj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://glb.zhixingplan.top

[Q64] 提交事务
来源：http://wsj.sysykeji.top

COMMIT;
来源：http://nto.uphjek.com

[Q65] 回滚事务
来源：http://dha.jyoumei.cn

ROLLBACK;
来源：http://ubb.bjfxy.top

[Q66] 行锁查询
来源：http://vzk.kuanghao11.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nrq.gaohongyu789.top

[Q67] 设置隔离级别
来源：http://awq.redwolf501.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wmj.bbcook.cn

[Q68] 保存点
来源：http://juv.zhoulong.xyz

SAVEPOINT sp1;
来源：http://lqt.xylfe.cn

ROLLBACK TO sp1;
来源：http://lrd.zdqjudy.top

[Q69] 查看执行计划
来源：http://rbq.ybcxt.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://huk.jqgufenzy.top

[Q70] 更新统计信息
来源：http://azv.guannengcc.top

ANALYZE TABLE users;
来源：http://lgw.bbcook.cn

[Q71] 查看建表语句
来源：http://epu.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nrv.nwbrower.top

[Q72] 查看索引
来源：http://jwr.meibo888.top

SHOW INDEX FROM users;
来源：http://ssp.hfpthk.cn

[Q73] 查看表状态
来源：http://smt.svipenyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ebk.hammf.cn

[Q74] 强制使用索引
来源：http://ebj.hfpthk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vlo.yongpay.top

[Q75] 日期格式化
来源：http://iod.shanyushiyangtech.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mmk.jiagoushi.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ege.havefunace.top

[Q76] 按天统计
来源：http://spu.pycfn.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://icw.hesvh.cn

[Q77] 时间加减
来源：http://ofu.nanxuanxn.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iin.wangshuangyany.cn

[Q78] 当前时间
来源：http://xpl.tian-w.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vgk.jianghu66.top

[Q79] 字符串拼接
来源：http://gax.shanyushiyangkeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jcb.guannengcc.top

[Q80] 字符串截取
来源：http://plx.zhixingplan.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ovy.chenjidiqi.icu

[Q81] 字符串替换
来源：http://yem.hysaishi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://eci.zhaomingkeji.xyz

[Q82] 字符长度与字节长度
来源：http://oqm.redwolf501.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://viu.havefunace.top

[Q83] 大小写转换
来源：http://sum.jinyuanbaomall.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://asq.ydjk.org.cn

[Q84] 去除首尾空格
来源：http://hzh.aibaodan.cn

SELECT TRIM(name) FROM users;
来源：http://xmn.fzhhl.top

[Q85] 数值取整
来源：http://lus.yongpay.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blp.jinyuanbaomall.cn


<!-- 参考信息 -->