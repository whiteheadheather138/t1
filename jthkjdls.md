代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://vwl.ppjwa.cn

C#:   lock (gate) { shared++; }
来源：http://ihj.aizwys.cn

[O04] 定义异步函数并等待
来源：http://opr.dianchejie.cn

Py:   async def f():⏎    await g()
来源：http://mby.shanyushiyangtech.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://pxw.fzhhl.top

JS:   async function f() { await g(); }
来源：http://elb.daxiang520.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://udm.xuanzx.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ohr.ivvv.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://uve.bjfxy.top

Ruby: # 用 Fiber 或 async gem
来源：http://xng.sjlbkw.cn

C#:   async Task F() { await G(); }
来源：http://kdj.gotoacloud.top

[O05] 并发执行并等待全部完成
来源：http://ljs.shanyushiyangtech.top

Py:   asyncio.gather(*tasks)
来源：http://ecs.hysaishi.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hmj.feifeiyinyue.top

JS:   await Promise.all(tasks)
来源：http://qwi.fengsongda.top

TS:   await Promise.all(tasks)
来源：http://wjo.vqdsnc.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://idj.daria6918.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ewr.jyoumei.cn

Ruby: threads.map(&:join)
来源：http://jzf.mhx1999.top

C#:   await Task.WhenAll(t1, t2)
来源：http://ols.yvedp.cn

[O06] 使用进程池
来源：http://blj.redwolf501.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yga.xinyue.icu

PHP:  // pcntl_fork 或多进程队列
来源：http://gmy.nwbrower.top

JS:   // child_process / cluster 模块
来源：http://apd.yj202588.top

TS:   // child_process / cluster 模块
来源：http://oaf.jinghuilouyu.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ytv.jinqigufen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rxc.yj20258888.top

Ruby: // fork 块
来源：http://nru.dashuyun.cn

C#:   Parallel.For
来源：http://kit.ctjpmb.com

================================================================================
来源：http://ues.sxryk.cn

P. 常用工具函数
来源：http://xdn.gogol.net.cn

================================================================================
来源：http://xkm.daria6918.cn

[P01] 生成 UUID
来源：http://upr.hfpthk.cn

Py:   str(uuid.uuid4())
来源：http://zoz.ivvv.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yir.vqdsnc.cn

JS:   crypto.randomUUID()
来源：http://fgp.jyoumei.cn

TS:   crypto.randomUUID()
来源：http://sko.yfazqb.com

Java: UUID.randomUUID().toString()
来源：http://iox.chenjidiqi.icu

Go:   // 用 github.com/google/uuid
来源：http://fsr.gogol.net.cn

Ruby: SecureRandom.uuid
来源：http://tic.sufxvd.cn

C#:   Guid.NewGuid().ToString()
来源：http://jje.wangdashe.top

[P02] MD5 / SHA256 摘要
来源：http://rcv.jiagoushi.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ycx.mhx1999.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://iux.yj202588.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://yai.zhaomingkeji.xyz

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fzb.nanxinkj.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://yre.aizwys.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://xjw.zdqjudy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cot.sxryk.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vkj.fanxiaobao.xyz

[P03] 生成短随机字符串
来源：http://epi.meibo888.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://hsg.nanxuanxn.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://dfj.yvedp.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ebc.tian-w.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://doj.pycfn.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://yuo.wangdashe.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xox.tarul.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://yys.hnxiangtu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://rpj.gogol.net.cn

[P04] 求长度
来源：http://yrx.jinqigfzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fky.sjlbkw.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ggo.sxryk.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://smx.jinyuanbaomall.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://gzb.jianghu66.top

Java: list.size();  map.size();  s.length()
来源：http://thw.gotoacloud.top

Go:   len(arr);  len(m)
来源：http://wdf.fzhhl.top

Ruby: x.length;  x.size
来源：http://hzo.zhongyouzk.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://tqm.chenzaomai.com

[P05] 判断两个对象内容是否相等
来源：http://yjf.uphjek.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://fac.shanyushiyangtech.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lmw.jlsjyb.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://tbz.hesvh.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://rad.hesvh.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wff.ppjwa.cn

Go:   reflect.DeepEqual(a, b)
来源：http://tar.xinyue.icu

Ruby: a == b
来源：http://vvo.jinqigufen.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hwm.svipenyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://brt.jyoumei.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wjm.zhixingplan.top

PHP:  if (empty($x)) {}
来源：http://sie.dashuyun.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://shg.cheryme.top

TS:   if (x == null) {}
来源：http://kyh.aibaodan.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://uqf.birdmap.top

Go:   if x == nil {}
来源：http://rjp.xylfe.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ttj.ydzc1.top

C#:   if (x is null) {}
来源：http://bpa.daxiang520.top

[P07] 防抖与节流
来源：http://lur.cdnleiting.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://xwc.yvedp.cn

PHP:  // 手写时间戳比较
来源：http://uat.wangshuangyany.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://gef.dianchejie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pgv.aizwys.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://zel.bbcook.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wjy.cucudq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://mlq.fanxiaobao.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://rmf.daria6918.cn

[P08] 处理浮点精度问题
来源：http://kbz.snrcjt.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ukt.shangyingyoupin.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ysl.daxiang520.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wux.cdnleiting.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ffa.jlsjyb.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vii.hesvh.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ioc.tarul.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aww.yj20258888.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://vkt.yuxming.cn

================================================================================
来源：http://oko.fehbvm.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vfw.jinghuilouyu.cn

================================================================================
来源：http://nee.shzxlz.cn

[Q01] 创建表
来源：http://opl.pengpengdd.cyou

CREATE TABLE users (
来源：http://xjn.zdbjq.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lfl.yongpay.top

name VARCHAR(50) NOT NULL,
来源：http://ywe.sjlbkw.cn

email VARCHAR(100) UNIQUE,
来源：http://fkh.yfazqb.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://omn.bbcook.cn

);
来源：http://kho.hfpthk.cn

[Q02] 创建带外键的表
来源：http://vaw.yuxming.cn

CREATE TABLE orders (
来源：http://ggs.uphjek.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://tti.xziqi.cn

user_id INT NOT NULL,
来源：http://kqd.tianlin.xyz

amount DECIMAL(10, 2),
来源：http://xmf.shangyingyoupin.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://grj.ivvv.top

);
来源：http://ltx.bjfxy.top

[Q03] 增加列
来源：http://jcl.yongpay.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://skg.daria6918.cn

[Q04] 修改列类型
来源：http://qmo.xuetiantiany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://onq.jqgufenzy.top

[Q05] 重命名列
来源：http://ewf.wangdashe.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wcr.yueranfly.top

[Q06] 删除列
来源：http://hlm.jqgfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://chx.jqgufenzy.top

[Q07] 删除表
来源：http://act.smart0.xyz

DROP TABLE IF EXISTS orders;
来源：http://uco.cucudq.cn

[Q08] 创建普通索引
来源：http://piu.c1oappe.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ajd.yj202588.top

[Q09] 创建唯一索引
来源：http://smi.fengsongda.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mso.birdmap.top

[Q10] 插入单行
来源：http://pqm.shangyingyoupin.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ctf.fengsongda.top

[Q11] 一次插入多行
来源：http://oeo.meibo888.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://skq.wangshuangyany.cn

[Q12] 插入后取自增 ID
来源：http://edh.yj202588.top

INSERT INTO users (name) VALUES ('C');
来源：http://rjr.ydzc1.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hfi.birdmap.top

[Q13] 忽略重复插入
来源：http://xod.jianghu66.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://gnn.iojbl.cn

[Q14] 存在则更新（upsert）
来源：http://vbp.ctjpmb.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vqv.jyoumei.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ovk.chenzaomai.com

[Q15] 查询全部
来源：http://bna.aizwys.cn

SELECT * FROM users;
来源：http://acs.daxiang520.top

[Q16] 查询指定列
来源：http://xoz.aibaodan.cn

SELECT id, name FROM users;
来源：http://gbr.jinghuilouyu.cn

[Q17] 条件查询
来源：http://vnm.shanyushiyangkeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hdp.ywan-chungtsiang.top

[Q18] 模糊匹配
来源：http://qte.hesvh.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ncu.gaohongyu789.top

[Q19] 范围查询
来源：http://xke.kuanghao11.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tcc.zhijiandao.cn

[Q20] IN 列表
来源：http://kcw.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://rmg.cdnleiting.top

[Q21] 空值判断
来源：http://qbz.jinqigufen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://tvz.xylfe.cn

[Q22] 排序
来源：http://xup.shanyushiyangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jqs.hywenlv.cn

[Q23] 分页
来源：http://qts.vehdjk.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vym.c1oappe.top

[Q24] 去重
来源：http://ltt.jlsjyb.cn

SELECT DISTINCT city FROM users;
来源：http://vui.birdmap.top

[Q25] 只取前 N 条
来源：http://kzc.jianghu66.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jqm.ybcxt.top

[Q26] 计数
来源：http://cpy.snrcjt.cn

SELECT COUNT(*) FROM users;
来源：http://dku.ybcxt.top

[Q27] 条件计数
来源：http://pbf.ybcxt.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hze.0kj1m.cn

[Q28] 求和与平均
来源：http://pid.cqqwz.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nqn.zdqjudy.top

[Q29] 最大最小值
来源：http://xel.birdmap.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://zfl.tarul.cn

[Q30] 分组统计
来源：http://euk.cashguo.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gpz.nwbrower.top

[Q31] 分组后过滤
来源：http://idg.hnqzz.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pel.cashguo.top

[Q32] 分组拼接字符串
来源：http://zys.guannengcc.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kis.ctjpmb.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ihs.dianchejie.cn

[Q33] 多列分组
来源：http://evs.jqgufenzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xjk.sweek.top

[Q34] 每组取第一条
来源：http://orz.vehdjk.com

SELECT * FROM (
来源：http://ofy.zdqjudy.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xav.mhx1999.top

) t WHERE rn = 1;
来源：http://cpl.ctjpmb.com

[Q35] 内连接
来源：http://dqn.sxryk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dcq.zdqjudy.top

[Q36] 左连接
来源：http://uwm.yonumen.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ryj.bjfxy.top

[Q37] 右连接
来源：http://nxy.tanke756.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kne.tanke756.top

[Q38] 全外连接（PostgreSQL）
来源：http://ndh.zhoulong.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tpw.316326.xyz

[Q39] 自连接（查上下级）
来源：http://wiq.andypj.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://rng.jinqigfzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://xbr.tanke756.top

[Q40] 交叉连接（笛卡尔积）
来源：http://xxc.xuetiantiany.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bdl.ydzc1.top

[Q41] 多表连接
来源：http://hfv.gzhubu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rmx.gzhubu.top

JOIN users u ON u.id = o.user_id
来源：http://nkj.fanxiaobao.xyz

JOIN products p ON p.id = o.product_id;
来源：http://wih.hnqzz.top

[Q42] 连接条件附加过滤
来源：http://adu.yj202588.top

SELECT u.name, o.amount FROM users u
来源：http://ksm.ivvv.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vyy.cashguo.top

[Q43] 标量子查询
来源：http://okt.guowangkeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://elj.yuanzhike.top

[Q44] IN 子查询
来源：http://zzm.nanxinkj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yka.cqqwz.cn

[Q45] EXISTS 判断存在
来源：http://wvx.chenjidiqi.icu

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tjg.snrcjt.cn

[Q46] NOT EXISTS 判断不存在
来源：http://qtl.haohaochexian.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://iyf.tanke756.top

[Q47] 与平均值比较
来源：http://fey.yanxiufei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://doe.cdnleiting.top

[Q48] CTE 公用表表达式
来源：http://mrw.zhongyouzk.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ova.feifeiyinyue.top

SELECT * FROM t WHERE c > 5;
来源：http://qbb.epnwcf.com

[Q49] 更新单行
来源：http://ggq.zhengqikj.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vpr.fzhhl.top

[Q50] 批量更新
来源：http://xmn.jqgufenzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ubj.yonumen.top

[Q51] 用子查询更新
来源：http://rbj.xziqi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sti.guowangkeji.top

[Q52] 删除指定行
来源：http://cig.hfpthk.cn

DELETE FROM users WHERE id = 10;
来源：http://ddu.jinyuanbaomall.cn

[Q53] 按条件删除
来源：http://bsu.yonumen.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nzj.zhaomingkeji.xyz

[Q54] 清空表
来源：http://nre.vehdjk.com

TRUNCATE TABLE logs;
来源：http://cew.jinyuanbaomall.cn

[Q55] 排名（并列占位）
来源：http://kuk.xziqi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zvv.9152youxi.cn

[Q56] 密集排名（并列不占位）
来源：http://wqv.zdqjudy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kii.shanyushiyangtech.top

[Q57] 行号
来源：http://ceo.yanxiufei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bvx.quarkkingdee.top

[Q58] 累计求和
来源：http://nwf.nanxuanxn.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vmv.meibo888.top

[Q59] 分组内累计
来源：http://fah.jqgfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ccn.pycfn.com

[Q60] 取上一行 / 下一行
来源：http://goo.jinyuanbaomall.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xcj.birdmap.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wbn.ivvv.top

[Q61] 移动平均
来源：http://cvu.gotoacloud.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tcj.nanxuanxn.top

[Q62] 分组占比
来源：http://efn.shuidangran.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dxn.zycfv.cn

[Q63] 开启事务
来源：http://bfw.nanxinkj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://nzx.yj20258.top

[Q64] 提交事务
来源：http://rys.cucudq.cn

COMMIT;
来源：http://kdn.shuidangran.top

[Q65] 回滚事务
来源：http://acc.hesvh.cn

ROLLBACK;
来源：http://fqg.zhiwuduotai.top

[Q66] 行锁查询
来源：http://ilw.zhongyouzk.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://buk.chenzaomai.com

[Q67] 设置隔离级别
来源：http://epu.nanxinkj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cfv.guowangkeji.top

[Q68] 保存点
来源：http://ljr.pengpengdd.cyou

SAVEPOINT sp1;
来源：http://wih.gzhubu.top

ROLLBACK TO sp1;
来源：http://huq.redwolf501.top

[Q69] 查看执行计划
来源：http://rif.dianchejie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ixq.feifeiyinyue.top

[Q70] 更新统计信息
来源：http://nmg.yangfankeji.com

ANALYZE TABLE users;
来源：http://mud.jinghuilouyu.cn

[Q71] 查看建表语句
来源：http://ryy.sweek.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ajo.wangshuangyany.cn

[Q72] 查看索引
来源：http://wyq.ivvv.top

SHOW INDEX FROM users;
来源：http://hzx.316326.xyz

[Q73] 查看表状态
来源：http://dpe.haohaochexian.top

SHOW TABLE STATUS LIKE 'users';
来源：http://jfy.ybcxt.top

[Q74] 强制使用索引
来源：http://bfp.cashguo.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rgc.mhx1999.top

[Q75] 日期格式化
来源：http://jqy.shzxlz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://atl.wangshuangyany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sls.bjfxy.top

[Q76] 按天统计
来源：http://pca.ivvv.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dmf.gzhubu.top

[Q77] 时间加减
来源：http://hum.jlsjyb.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vav.shzxlz.cn

[Q78] 当前时间
来源：http://pns.aizwys.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tgw.yj20258888.top

[Q79] 字符串拼接
来源：http://din.zdbjq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kuy.tanke756.top

[Q80] 字符串截取
来源：http://rzl.jiagoushi.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lms.meibo888.top

[Q81] 字符串替换
来源：http://ryq.mhx1999.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://aor.yuxming.cn

[Q82] 字符长度与字节长度
来源：http://jjo.pengpengdd.cyou

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xoj.dianchejie.cn

[Q83] 大小写转换
来源：http://ecv.ehwqpu.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hzf.dashuyun.cn

[Q84] 去除首尾空格
来源：http://zkz.cheryme.top

SELECT TRIM(name) FROM users;
来源：http://ltq.0kj1m.cn

[Q85] 数值取整
来源：http://cri.hnxiangtu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ruw.hcnkem.com


<!-- 参考信息 -->