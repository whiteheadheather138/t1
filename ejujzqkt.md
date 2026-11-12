代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://oft.daxiang520.top

C#:   lock (gate) { shared++; }
来源：http://exi.yj202588.top

[O04] 定义异步函数并等待
来源：http://gbm.quarkkingdee.top

Py:   async def f():⏎    await g()
来源：http://zij.cashguo.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ysh.hfpthk.cn

JS:   async function f() { await g(); }
来源：http://pqh.ydjk.org.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vvq.sysykeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qgo.fanxiaobao.xyz

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wbf.9152youxi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zlm.nanxinkj.top

C#:   async Task F() { await G(); }
来源：http://ygt.iojbl.cn

[O05] 并发执行并等待全部完成
来源：http://oxj.zhaomingkeji.xyz

Py:   asyncio.gather(*tasks)
来源：http://xbh.nanxinkj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://eda.52xcode.cn

JS:   await Promise.all(tasks)
来源：http://mpd.jinghuilouyu.cn

TS:   await Promise.all(tasks)
来源：http://kcm.nwbrower.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://dzx.nanxinkj.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://thm.jlsjyb.cn

Ruby: threads.map(&:join)
来源：http://yhu.aizwys.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://ixh.epnwcf.com

[O06] 使用进程池
来源：http://llc.nwbrower.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xcj.zhiwuduotai.top

PHP:  // pcntl_fork 或多进程队列
来源：http://yvb.jinqigufen.top

JS:   // child_process / cluster 模块
来源：http://jsb.sweek.top

TS:   // child_process / cluster 模块
来源：http://hek.shanyushiyangtech.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://qgi.iojbl.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://uhj.hesvh.cn

Ruby: // fork 块
来源：http://iod.cashguo.top

C#:   Parallel.For
来源：http://bag.hesvh.cn

================================================================================
来源：http://phn.shanyushiyangtech.top

P. 常用工具函数
来源：http://rrw.jlsjyb.cn

================================================================================
来源：http://ycd.shuidangran.top

[P01] 生成 UUID
来源：http://itm.mhx1999.top

Py:   str(uuid.uuid4())
来源：http://ker.shangyingyoupin.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gdj.c1oappe.top

JS:   crypto.randomUUID()
来源：http://lgz.jinqigfzy.top

TS:   crypto.randomUUID()
来源：http://efb.andypj.xyz

Java: UUID.randomUUID().toString()
来源：http://oil.havefunace.top

Go:   // 用 github.com/google/uuid
来源：http://hir.gzhubu.top

Ruby: SecureRandom.uuid
来源：http://ryh.zhoulong.xyz

C#:   Guid.NewGuid().ToString()
来源：http://zch.sysykeji.top

[P02] MD5 / SHA256 摘要
来源：http://vtc.52xcode.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gyg.bjfxy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://mty.smart0.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://iog.hfpthk.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://dvl.xingfuxueyuan.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ewu.pycfn.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://orz.aizwys.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://efl.shanyushiyangtech.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dva.fehbvm.com

[P03] 生成短随机字符串
来源：http://kfm.chenlongwang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://zuy.nwbrower.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ofo.xuanzx.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rns.ctjpmb.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://ipo.yj202588.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://tgu.fktsv.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://uuj.zhixingplan.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://spv.gogol.net.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wdd.haohaochexian.top

[P04] 求长度
来源：http://ntv.yj20258888.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nei.hnxiangtu.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wca.hywenlv.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://piu.fanxiaobao.xyz

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yxe.jinyuanbaomall.cn

Java: list.size();  map.size();  s.length()
来源：http://cvo.xinyue.icu

Go:   len(arr);  len(m)
来源：http://hsp.chenjidiqi.icu

Ruby: x.length;  x.size
来源：http://jgh.fzhhl.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://xyf.jinyuanbaomall.cn

[P05] 判断两个对象内容是否相等
来源：http://bhm.havefunace.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://qll.quarkkingdee.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://hbh.chenzaomai.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://jky.cqqwz.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://jvm.uphjek.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://frt.fengsongda.top

Go:   reflect.DeepEqual(a, b)
来源：http://fjm.smart0.xyz

Ruby: a == b
来源：http://dfq.tianlin.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gtv.mhx1999.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jdw.316326.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rid.hfpthk.cn

PHP:  if (empty($x)) {}
来源：http://jnl.316326.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jvp.ywan-chungtsiang.top

TS:   if (x == null) {}
来源：http://dge.fzhhl.top

Java: if (x == null || x.isEmpty()) {}
来源：http://ffq.gotoacloud.top

Go:   if x == nil {}
来源：http://vzs.0kj1m.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://apa.ydzc1.top

C#:   if (x is null) {}
来源：http://pne.cashguo.top

[P07] 防抖与节流
来源：http://dkn.vqdsnc.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://pap.sweek.top

PHP:  // 手写时间戳比较
来源：http://puu.shuidangran.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://rec.havefunace.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://jrb.tian-w.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://nie.hnxiangtu.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mkv.sxryk.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://yeq.52xcode.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://dcr.birdmap.top

[P08] 处理浮点精度问题
来源：http://anm.jqgfzy.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://xcx.xingfuxueyuan.xyz

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yzr.pengpengdd.cyou

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://qxz.yj202588.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eat.svipenyu.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ngt.ctjpmb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://yhr.chenzaomai.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://qiz.ivvv.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wzc.gogol.net.cn

================================================================================
来源：http://kjy.sweek.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://rzu.pengpengdd.cyou

================================================================================
来源：http://iyx.sysykeji.top

[Q01] 创建表
来源：http://nib.sysykeji.top

CREATE TABLE users (
来源：http://qqp.tianlin.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://lfb.jinyuanbaomall.cn

name VARCHAR(50) NOT NULL,
来源：http://uzr.dashuyun.cn

email VARCHAR(100) UNIQUE,
来源：http://wev.xylfe.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ger.jinqigfzy.top

);
来源：http://opj.shanyushiyangtech.top

[Q02] 创建带外键的表
来源：http://qma.yueranfly.top

CREATE TABLE orders (
来源：http://uhs.bbcook.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://woy.sjlbkw.cn

user_id INT NOT NULL,
来源：http://jje.fzhhl.top

amount DECIMAL(10, 2),
来源：http://lpt.jlsjyb.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cji.cashguo.top

);
来源：http://fbt.hongshengwenyu.top

[Q03] 增加列
来源：http://ygu.yj20258888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ptw.jinghuilouyu.cn

[Q04] 修改列类型
来源：http://che.zhoulong.xyz

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rma.andypj.xyz

[Q05] 重命名列
来源：http://zot.cashguo.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://awf.pengpengdd.cyou

[Q06] 删除列
来源：http://wyc.zhoulong.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://ybq.gaohongyu789.top

[Q07] 删除表
来源：http://ein.fengsongda.top

DROP TABLE IF EXISTS orders;
来源：http://uzx.hesvh.cn

[Q08] 创建普通索引
来源：http://fac.wangshuangyany.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://tnd.0kj1m.cn

[Q09] 创建唯一索引
来源：http://usc.jqgufenzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://isb.ydzc1.top

[Q10] 插入单行
来源：http://ojh.hnxiangtu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://eal.dashuyun.cn

[Q11] 一次插入多行
来源：http://ops.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qpw.jinqigfzy.top

[Q12] 插入后取自增 ID
来源：http://fxd.birdmap.top

INSERT INTO users (name) VALUES ('C');
来源：http://nxi.wangshuangyany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://acc.tian-w.cn

[Q13] 忽略重复插入
来源：http://flf.jinqigufen.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ndt.epnwcf.com

[Q14] 存在则更新（upsert）
来源：http://dih.sysykeji.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jmg.iojbl.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fjr.fengsongda.top

[Q15] 查询全部
来源：http://ajr.svipenyu.cn

SELECT * FROM users;
来源：http://rul.ppjwa.cn

[Q16] 查询指定列
来源：http://vtw.yj20258888.top

SELECT id, name FROM users;
来源：http://zqb.nanxuanxn.top

[Q17] 条件查询
来源：http://lcj.jlsjyb.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://jyc.hnxiangtu.top

[Q18] 模糊匹配
来源：http://ogz.daria6918.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bqv.yj20258888.top

[Q19] 范围查询
来源：http://ofx.vqdsnc.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://aai.jlsjyb.cn

[Q20] IN 列表
来源：http://nxm.yvedp.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://eti.haohaochexian.top

[Q21] 空值判断
来源：http://pwe.jqgufenzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://yfg.jlsjyb.cn

[Q22] 排序
来源：http://prj.yonumen.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://htr.hesvh.cn

[Q23] 分页
来源：http://mvm.smart0.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ccd.jyoumei.cn

[Q24] 去重
来源：http://jgw.ctjpmb.com

SELECT DISTINCT city FROM users;
来源：http://biw.gaohongyu789.top

[Q25] 只取前 N 条
来源：http://caq.c1oappe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jnz.hnxiangtu.top

[Q26] 计数
来源：http://ffa.aibaodan.cn

SELECT COUNT(*) FROM users;
来源：http://xei.52xcode.cn

[Q27] 条件计数
来源：http://nhl.fzhhl.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mfr.yangfankeji.com

[Q28] 求和与平均
来源：http://xdf.yanxiufei.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rdu.zycfv.cn

[Q29] 最大最小值
来源：http://tzq.haohaochexian.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jmk.snrcjt.cn

[Q30] 分组统计
来源：http://ede.52xcode.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ogh.zhengqikj.top

[Q31] 分组后过滤
来源：http://iym.vqdsnc.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gor.svipenyu.cn

[Q32] 分组拼接字符串
来源：http://osr.aibaodan.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nba.cdnleiting.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mpo.havefunace.top

[Q33] 多列分组
来源：http://bvv.shanyushiyangtech.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://twj.xuetiantiany.cn

[Q34] 每组取第一条
来源：http://exb.ywan-chungtsiang.top

SELECT * FROM (
来源：http://eyy.jinyuanbaomall.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qow.fengsongda.top

) t WHERE rn = 1;
来源：http://wew.quarkkingdee.top

[Q35] 内连接
来源：http://tpc.yj20258.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://vbv.andypj.xyz

[Q36] 左连接
来源：http://zzk.jianghu66.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xwt.aibaodan.cn

[Q37] 右连接
来源：http://ory.chenlongwang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hvy.ivvv.top

[Q38] 全外连接（PostgreSQL）
来源：http://hbu.shanyushiyangtech.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qjm.shanyushiyangtech.top

[Q39] 自连接（查上下级）
来源：http://dso.aibaodan.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://fmc.hnxiangtu.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bge.ehwqpu.com

[Q40] 交叉连接（笛卡尔积）
来源：http://tae.sjlbkw.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://htx.jinqigfzy.top

[Q41] 多表连接
来源：http://rpz.gzhubu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hac.sysykeji.top

JOIN users u ON u.id = o.user_id
来源：http://rpz.jinyuanbaomall.cn

JOIN products p ON p.id = o.product_id;
来源：http://gbg.shzxlz.cn

[Q42] 连接条件附加过滤
来源：http://qis.svipenyu.cn

SELECT u.name, o.amount FROM users u
来源：http://bmb.redwolf501.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ojl.xylfe.cn

[Q43] 标量子查询
来源：http://cqt.havefunace.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kid.wangshuangyany.cn

[Q44] IN 子查询
来源：http://dil.jinqigufen.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://exx.fzhhl.top

[Q45] EXISTS 判断存在
来源：http://nne.316326.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pup.bbcook.cn

[Q46] NOT EXISTS 判断不存在
来源：http://scw.shangyingyoupin.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://khg.shangyingyoupin.top

[Q47] 与平均值比较
来源：http://kgw.pycfn.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wds.snrcjt.cn

[Q48] CTE 公用表表达式
来源：http://nni.yanxiufei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tkz.nanxinkj.top

SELECT * FROM t WHERE c > 5;
来源：http://fng.jqgfzy.top

[Q49] 更新单行
来源：http://roy.zdqjudy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xav.jinqigfzy.top

[Q50] 批量更新
来源：http://cwf.jqgufenzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zkr.ppjwa.cn

[Q51] 用子查询更新
来源：http://wkr.jlsjyb.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://axr.tanke756.top

[Q52] 删除指定行
来源：http://qkd.chenjidiqi.icu

DELETE FROM users WHERE id = 10;
来源：http://tkp.xziqi.cn

[Q53] 按条件删除
来源：http://bmb.birdmap.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uoh.chenzaomai.com

[Q54] 清空表
来源：http://wuy.sufxvd.cn

TRUNCATE TABLE logs;
来源：http://eam.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://lae.hysaishi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://usb.sweek.top

[Q56] 密集排名（并列不占位）
来源：http://uaa.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kfo.dianchejie.cn

[Q57] 行号
来源：http://exq.ppjwa.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xyg.meibo888.top

[Q58] 累计求和
来源：http://tyh.iojbl.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xtz.zycfv.cn

[Q59] 分组内累计
来源：http://fir.gaohongyu789.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wxg.sxryk.cn

[Q60] 取上一行 / 下一行
来源：http://nkv.tanke756.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dke.zhixingplan.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://llf.jqgufenzy.top

[Q61] 移动平均
来源：http://lao.xingfuxueyuan.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hbv.fktsv.cn

[Q62] 分组占比
来源：http://dcs.zdbjq.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fyz.shanyushiyangkeji.top

[Q63] 开启事务
来源：http://tcu.ppjwa.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bzq.wangdashe.top

[Q64] 提交事务
来源：http://vvj.cashguo.top

COMMIT;
来源：http://xcg.redwolf501.top

[Q65] 回滚事务
来源：http://zkx.aibaodan.cn

ROLLBACK;
来源：http://pth.pengpengdd.cyou

[Q66] 行锁查询
来源：http://pag.jiagoushi.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dpd.snrcjt.cn

[Q67] 设置隔离级别
来源：http://qzk.jqgufenzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ifq.pengpengdd.cyou

[Q68] 保存点
来源：http://odi.ydzc1.top

SAVEPOINT sp1;
来源：http://btw.feifeiyinyue.top

ROLLBACK TO sp1;
来源：http://pct.316326.xyz

[Q69] 查看执行计划
来源：http://olo.hywenlv.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jrj.shzxlz.cn

[Q70] 更新统计信息
来源：http://brx.cdnleiting.top

ANALYZE TABLE users;
来源：http://nmt.gogol.net.cn

[Q71] 查看建表语句
来源：http://dhx.shanyushiyangtech.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ili.yvedp.cn

[Q72] 查看索引
来源：http://qsi.52xcode.cn

SHOW INDEX FROM users;
来源：http://csw.zhijiandao.cn

[Q73] 查看表状态
来源：http://qtq.hesvh.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dei.redwolf501.top

[Q74] 强制使用索引
来源：http://ryi.zhiwuduotai.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rjh.zycfv.cn

[Q75] 日期格式化
来源：http://bfp.jqgfzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fak.jinyuanbaomall.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gre.redwolf501.top

[Q76] 按天统计
来源：http://ctc.dashuyun.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://eec.ppjwa.cn

[Q77] 时间加减
来源：http://maf.zhoulong.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mgv.zhijiandao.cn

[Q78] 当前时间
来源：http://ggk.nanxuanxn.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sqc.jiagoushi.top

[Q79] 字符串拼接
来源：http://ett.svipenyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sct.yanxiufei.cn

[Q80] 字符串截取
来源：http://lrq.cashguo.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fwl.jinqigufen.top

[Q81] 字符串替换
来源：http://bpf.zdbjq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gcd.yanxiufei.cn

[Q82] 字符长度与字节长度
来源：http://wcj.mhx1999.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mgk.wangdashe.top

[Q83] 大小写转换
来源：http://cti.ctjpmb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rhg.fengsongda.top

[Q84] 去除首尾空格
来源：http://ose.jqgufenzy.top

SELECT TRIM(name) FROM users;
来源：http://oaq.bbcook.cn

[Q85] 数值取整
来源：http://iad.gogol.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dyz.zycfv.cn


<!-- 参考信息 -->