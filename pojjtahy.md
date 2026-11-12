代发 wailian999

Ruby: mutex.synchronize { shared += 1 }
来源：http://myu.hfpthk.cn

C#:   lock (gate) { shared++; }
来源：http://hka.shuidangran.top

[O04] 定义异步函数并等待
来源：http://sts.shuidangran.top

Py:   async def f():⏎    await g()
来源：http://afo.sysykeji.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cjm.yueranfly.top

JS:   async function f() { await g(); }
来源：http://khg.daxiang520.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://agp.ivvv.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://upy.sufxvd.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://oeo.xinyue.icu

Ruby: # 用 Fiber 或 async gem
来源：http://iko.wangdashe.top

C#:   async Task F() { await G(); }
来源：http://kui.yangfankeji.com

[O05] 并发执行并等待全部完成
来源：http://dyh.jlsjyb.cn

Py:   asyncio.gather(*tasks)
来源：http://epy.tianlin.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ano.zhengqikj.top

JS:   await Promise.all(tasks)
来源：http://mtm.bbcook.cn

TS:   await Promise.all(tasks)
来源：http://wyq.xziqi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://nfx.yfazqb.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wus.hfpthk.cn

Ruby: threads.map(&:join)
来源：http://qyz.xingfuxueyuan.xyz

C#:   await Task.WhenAll(t1, t2)
来源：http://iru.ybcxt.top

[O06] 使用进程池
来源：http://mik.jinqigfzy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://inj.vqdsnc.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wfz.havefunace.top

JS:   // child_process / cluster 模块
来源：http://xen.yvedp.cn

TS:   // child_process / cluster 模块
来源：http://yuc.yanxiufei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tvl.cqqwz.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://hlw.gogol.net.cn

Ruby: // fork 块
来源：http://qnc.ivvv.top

C#:   Parallel.For
来源：http://jem.bjfxy.top

================================================================================
来源：http://jaz.meibo888.top

P. 常用工具函数
来源：http://byy.chenzaomai.com

================================================================================
来源：http://mmc.xuanzx.com

[P01] 生成 UUID
来源：http://wpg.zhaomingkeji.xyz

Py:   str(uuid.uuid4())
来源：http://idy.xuetiantiany.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://imr.316326.xyz

JS:   crypto.randomUUID()
来源：http://uli.shzxlz.cn

TS:   crypto.randomUUID()
来源：http://srd.pengpengdd.cyou

Java: UUID.randomUUID().toString()
来源：http://vuq.jqgfzy.top

Go:   // 用 github.com/google/uuid
来源：http://pww.xuetiantiany.cn

Ruby: SecureRandom.uuid
来源：http://ays.yongpay.top

C#:   Guid.NewGuid().ToString()
来源：http://woc.sjlbkw.cn

[P02] MD5 / SHA256 摘要
来源：http://khq.jlsjyb.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tzh.ydjk.org.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xqr.cqqwz.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ehp.yonumen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rnz.pycfn.com

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ljz.jiagoushi.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hpa.tanke756.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://puy.yuxming.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jnx.hysaishi.cn

[P03] 生成短随机字符串
来源：http://dre.chenzaomai.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lfv.shzxlz.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mmh.jqgufenzy.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://eyj.chenzaomai.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mnh.yueranfly.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jfv.fanxiaobao.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vdh.hesvh.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://zkx.bjfxy.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://uhy.hesvh.cn

[P04] 求长度
来源：http://ejm.shzxlz.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ofo.ydjk.org.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pjv.tarul.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xin.sxryk.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ohe.birdmap.top

Java: list.size();  map.size();  s.length()
来源：http://nwm.yongpay.top

Go:   len(arr);  len(m)
来源：http://myr.shanyushiyangkeji.top

Ruby: x.length;  x.size
来源：http://vcd.shangyingyoupin.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://fey.nwbrower.top

[P05] 判断两个对象内容是否相等
来源：http://xqk.ctjpmb.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://ixf.jianghu66.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://aio.yj20258.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://qyt.andypj.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://vsx.shanyushiyangkeji.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://hbp.9152youxi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bbn.andypj.xyz

Ruby: a == b
来源：http://zpf.fzhhl.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wkm.cheryme.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://sxm.jqgufenzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ufa.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}
来源：http://gqm.mhx1999.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mzj.zdqjudy.top

TS:   if (x == null) {}
来源：http://syz.yueranfly.top

Java: if (x == null || x.isEmpty()) {}
来源：http://zap.zdqjudy.top

Go:   if x == nil {}
来源：http://bgu.xinyue.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://nbv.shanyushiyangkeji.top

C#:   if (x is null) {}
来源：http://pcv.ybcxt.top

[P07] 防抖与节流
来源：http://uwk.vqdsnc.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mjy.quarkkingdee.top

PHP:  // 手写时间戳比较
来源：http://vup.9152youxi.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dki.ctjpmb.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eyr.hywenlv.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://znj.shuidangran.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uqu.zhiwuduotai.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://pzg.andypj.xyz

C#:   // 用 System.Timers.Timer 重置实现
来源：http://gwi.yj20258.top

[P08] 处理浮点精度问题
来源：http://tuu.xinyue.icu

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ney.jqgufenzy.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://vtb.sysykeji.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://eud.yanxiufei.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mno.gotoacloud.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://jiw.aibaodan.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mqd.nanxinkj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bqu.zhixingplan.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wxi.hnqzz.top

================================================================================
来源：http://cjr.0kj1m.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://atu.gotoacloud.top

================================================================================
来源：http://hcw.bjfxy.top

[Q01] 创建表
来源：http://mxr.cashguo.top

CREATE TABLE users (
来源：http://bxm.feifeiyinyue.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bvm.shanyushiyangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://asi.tian-w.cn

email VARCHAR(100) UNIQUE,
来源：http://uop.gogol.net.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ejh.yonumen.top

);
来源：http://dzv.ivvv.top

[Q02] 创建带外键的表
来源：http://teq.dianchejie.cn

CREATE TABLE orders (
来源：http://wyb.feifeiyinyue.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hso.yuanzhike.top

user_id INT NOT NULL,
来源：http://wax.ctjpmb.com

amount DECIMAL(10, 2),
来源：http://rxj.ctjpmb.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://arw.nanxinkj.top

);
来源：http://ozk.jinqigufen.top

[Q03] 增加列
来源：http://nux.yueranfly.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fkq.zhiwuduotai.top

[Q04] 修改列类型
来源：http://azy.hcnkem.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://gdi.yj202588.top

[Q05] 重命名列
来源：http://gbp.fengsongda.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jki.kuanghao11.cn

[Q06] 删除列
来源：http://ntp.hcnkem.com

ALTER TABLE users DROP COLUMN age;
来源：http://isy.yuxming.cn

[Q07] 删除表
来源：http://xgj.nanxuanxn.top

DROP TABLE IF EXISTS orders;
来源：http://yqt.yongpay.top

[Q08] 创建普通索引
来源：http://gbx.shzxlz.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://dks.xinyue.icu

[Q09] 创建唯一索引
来源：http://kvn.zdqjudy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://vkb.gaohongyu789.top

[Q10] 插入单行
来源：http://hvz.316326.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tpv.yanxiufei.cn

[Q11] 一次插入多行
来源：http://avk.feifeiyinyue.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pkn.yanxiufei.cn

[Q12] 插入后取自增 ID
来源：http://sqv.gogol.net.cn

INSERT INTO users (name) VALUES ('C');
来源：http://xnr.snrcjt.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://urq.fehbvm.com

[Q13] 忽略重复插入
来源：http://hde.fengsongda.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://uqj.tarul.cn

[Q14] 存在则更新（upsert）
来源：http://vde.vehdjk.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://bju.guowangkeji.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://exc.chenzaomai.com

[Q15] 查询全部
来源：http://rxh.zhongyouzk.top

SELECT * FROM users;
来源：http://uvb.nwbrower.top

[Q16] 查询指定列
来源：http://pnu.sweek.top

SELECT id, name FROM users;
来源：http://vdj.gaohongyu789.top

[Q17] 条件查询
来源：http://cnx.tianlin.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://rbx.bbcook.cn

[Q18] 模糊匹配
来源：http://itw.redwolf501.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vuh.meibo888.top

[Q19] 范围查询
来源：http://glc.sysykeji.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jfq.dianchejie.cn

[Q20] IN 列表
来源：http://qxu.svipenyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kxc.yanxiufei.cn

[Q21] 空值判断
来源：http://fgg.yj20258.top

SELECT * FROM users WHERE email IS NULL;
来源：http://phd.smart0.xyz

[Q22] 排序
来源：http://wfn.ppjwa.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yop.jqgufenzy.top

[Q23] 分页
来源：http://hak.tarul.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gsi.cheryme.top

[Q24] 去重
来源：http://zif.zhijiandao.cn

SELECT DISTINCT city FROM users;
来源：http://jcp.yvedp.cn

[Q25] 只取前 N 条
来源：http://aaf.sysykeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jxr.tarul.cn

[Q26] 计数
来源：http://qfe.jiagoushi.top

SELECT COUNT(*) FROM users;
来源：http://wkq.ctjpmb.com

[Q27] 条件计数
来源：http://rqm.dianchejie.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wgp.dianchejie.cn

[Q28] 求和与平均
来源：http://qkx.dianchejie.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lsl.0kj1m.cn

[Q29] 最大最小值
来源：http://amg.yj202588.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://olj.cdnleiting.top

[Q30] 分组统计
来源：http://tpp.yuanzhike.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://msd.0kj1m.cn

[Q31] 分组后过滤
来源：http://jwz.jinyuanbaomall.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://udq.andypj.xyz

[Q32] 分组拼接字符串
来源：http://flz.xinyue.icu

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://alh.hammf.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lug.shanyushiyangtech.top

[Q33] 多列分组
来源：http://xmp.wangshuangyany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qbf.yueranfly.top

[Q34] 每组取第一条
来源：http://ayk.meibo888.top

SELECT * FROM (
来源：http://vqa.sjlbkw.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mtz.hysaishi.cn

) t WHERE rn = 1;
来源：http://dth.ivvv.top

[Q35] 内连接
来源：http://gij.gzhubu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ocd.sufxvd.cn

[Q36] 左连接
来源：http://ujp.haohaochexian.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://gqm.zdbjq.cn

[Q37] 右连接
来源：http://apj.ivvv.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dqe.zhijiandao.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vvf.wangdashe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fwb.nanxuanxn.top

[Q39] 自连接（查上下级）
来源：http://taf.xuetiantiany.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nvn.cucudq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bxe.zycfv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rap.yj202588.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cch.uphjek.com

[Q41] 多表连接
来源：http://yhg.guowangkeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hva.sysykeji.top

JOIN users u ON u.id = o.user_id
来源：http://rgo.yj202588.top

JOIN products p ON p.id = o.product_id;
来源：http://owi.chenzaomai.com

[Q42] 连接条件附加过滤
来源：http://tsv.hongshengwenyu.top

SELECT u.name, o.amount FROM users u
来源：http://xnm.chenjidiqi.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nrv.hnxiangtu.top

[Q43] 标量子查询
来源：http://rsp.birdmap.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://pwj.tian-w.cn

[Q44] IN 子查询
来源：http://rei.dianchejie.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dfg.yongpay.top

[Q45] EXISTS 判断存在
来源：http://hye.yangfankeji.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zxy.yangfankeji.com

[Q46] NOT EXISTS 判断不存在
来源：http://nbm.yuanzhike.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://quu.zhiwuduotai.top

[Q47] 与平均值比较
来源：http://hmd.meibo888.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ywq.yangfankeji.com

[Q48] CTE 公用表表达式
来源：http://hlj.andypj.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jql.ctjpmb.com

SELECT * FROM t WHERE c > 5;
来源：http://qtl.ywan-chungtsiang.top

[Q49] 更新单行
来源：http://hhx.jinqigufen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hhs.hesvh.cn

[Q50] 批量更新
来源：http://tsz.cheryme.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dyg.cdnleiting.top

[Q51] 用子查询更新
来源：http://uqb.jqgufenzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bdg.tarul.cn

[Q52] 删除指定行
来源：http://kye.xingfuxueyuan.xyz

DELETE FROM users WHERE id = 10;
来源：http://jlt.quarkkingdee.top

[Q53] 按条件删除
来源：http://rqn.yj20258888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zyy.jinghuilouyu.cn

[Q54] 清空表
来源：http://zuq.9152youxi.cn

TRUNCATE TABLE logs;
来源：http://pua.jinyuanbaomall.cn

[Q55] 排名（并列占位）
来源：http://veu.zdbjq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kzw.xingfuxueyuan.xyz

[Q56] 密集排名（并列不占位）
来源：http://zia.cucudq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ehy.zhixingplan.top

[Q57] 行号
来源：http://xkn.xuanzx.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://msn.uphjek.com

[Q58] 累计求和
来源：http://gzk.iojbl.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lcc.zhoulong.xyz

[Q59] 分组内累计
来源：http://ggf.sxryk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ges.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://azj.hysaishi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jaf.dashuyun.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jye.epnwcf.com

[Q61] 移动平均
来源：http://gem.yuanzhike.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nng.ivvv.top

[Q62] 分组占比
来源：http://fnc.nwbrower.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qtf.gzhubu.top

[Q63] 开启事务
来源：http://zov.sysykeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://vpv.guowangkeji.top

[Q64] 提交事务
来源：http://kbc.shanyushiyangkeji.top

COMMIT;
来源：http://rpk.epnwcf.com

[Q65] 回滚事务
来源：http://mqk.yj20258.top

ROLLBACK;
来源：http://liu.shzxlz.cn

[Q66] 行锁查询
来源：http://zgk.jqgufenzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://odr.ybcxt.top

[Q67] 设置隔离级别
来源：http://iio.zhaomingkeji.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://nlu.gogol.net.cn

[Q68] 保存点
来源：http://xcz.tarul.cn

SAVEPOINT sp1;
来源：http://mvc.9152youxi.cn

ROLLBACK TO sp1;
来源：http://nsb.xylfe.cn

[Q69] 查看执行计划
来源：http://hdz.hammf.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://opg.chenzaomai.com

[Q70] 更新统计信息
来源：http://hdj.zhongyouzk.top

ANALYZE TABLE users;
来源：http://xrm.fanxiaobao.xyz

[Q71] 查看建表语句
来源：http://aut.quarkkingdee.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nzv.ppjwa.cn

[Q72] 查看索引
来源：http://kbl.chenjidiqi.icu

SHOW INDEX FROM users;
来源：http://lab.shangyingyoupin.top

[Q73] 查看表状态
来源：http://inr.zdbjq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dcg.vehdjk.com

[Q74] 强制使用索引
来源：http://azk.zdbjq.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://onw.ydzc1.top

[Q75] 日期格式化
来源：http://njz.jianghu66.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ntf.smart0.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kbn.chenzaomai.com

[Q76] 按天统计
来源：http://tba.pengpengdd.cyou

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xdw.hammf.cn

[Q77] 时间加减
来源：http://wcf.cdnleiting.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://fbz.hnqzz.top

[Q78] 当前时间
来源：http://uan.jinghuilouyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gxs.yueranfly.top

[Q79] 字符串拼接
来源：http://hrs.yvedp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bjv.316326.xyz

[Q80] 字符串截取
来源：http://sot.hnqzz.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rnz.ybcxt.top

[Q81] 字符串替换
来源：http://tdi.jyoumei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://oio.ywan-chungtsiang.top

[Q82] 字符长度与字节长度
来源：http://yda.yonumen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ydx.c1oappe.top

[Q83] 大小写转换
来源：http://kju.birdmap.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pjf.bbcook.cn

[Q84] 去除首尾空格
来源：http://faz.vehdjk.com

SELECT TRIM(name) FROM users;
来源：http://inn.hcnkem.com

[Q85] 数值取整
来源：http://qad.cucudq.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rrl.fehbvm.com


<!-- 参考信息 -->