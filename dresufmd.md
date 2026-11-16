代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dug.zhixingplan.top

TS:   // 同 JS
来源：http://qhd.0kj1m.cn

Java: synchronized (this) { shared++; }
来源：http://hht.52xcode.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gio.wangshuangyany.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://mfr.nwbrower.top

C#:   lock (gate) { shared++; }
来源：http://swx.chenjidiqi.icu

[O04] 定义异步函数并等待
来源：http://qwq.yfazqb.com

Py:   async def f():⏎    await g()
来源：http://wfn.andypj.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://uut.quarkkingdee.top

JS:   async function f() { await g(); }
来源：http://iis.xziqi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://rsx.jqgfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nnf.mhx1999.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wvg.fengsongda.top

Ruby: # 用 Fiber 或 async gem
来源：http://twr.cucudq.cn

C#:   async Task F() { await G(); }
来源：http://foq.xuetiantiany.cn

[O05] 并发执行并等待全部完成
来源：http://vbe.xylfe.cn

Py:   asyncio.gather(*tasks)
来源：http://col.vqdsnc.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xqu.yanxiufei.cn

JS:   await Promise.all(tasks)
来源：http://aiy.jqgfzy.top

TS:   await Promise.all(tasks)
来源：http://eam.tianlin.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zbl.ppjwa.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://eju.c1oappe.top

Ruby: threads.map(&:join)
来源：http://bqq.sjlbkw.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://hrj.tian-w.cn

[O06] 使用进程池
来源：http://zql.dashuyun.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ogi.cucudq.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://gxt.havefunace.top

JS:   // child_process / cluster 模块
来源：http://cay.cucudq.cn

TS:   // child_process / cluster 模块
来源：http://qnd.dianchejie.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tut.wangshuangyany.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dzk.quarkkingdee.top

Ruby: // fork 块
来源：http://kvp.zhongyouzk.top

C#:   Parallel.For
来源：http://nhm.c1oappe.top

================================================================================
来源：http://ldi.chenlongwang.top

P. 常用工具函数
来源：http://hgq.havefunace.top

================================================================================
来源：http://brk.yvedp.cn

[P01] 生成 UUID
来源：http://ace.cheryme.top

Py:   str(uuid.uuid4())
来源：http://rjs.tian-w.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://hgz.wangdashe.top

JS:   crypto.randomUUID()
来源：http://mcu.redwolf501.top

TS:   crypto.randomUUID()
来源：http://hhe.ydjk.org.cn

Java: UUID.randomUUID().toString()
来源：http://djv.xuanzx.com

Go:   // 用 github.com/google/uuid
来源：http://smt.316326.xyz

Ruby: SecureRandom.uuid
来源：http://kwv.sweek.top

C#:   Guid.NewGuid().ToString()
来源：http://iul.ydjk.org.cn

[P02] MD5 / SHA256 摘要
来源：http://jnr.guannengcc.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ytj.zhijiandao.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://tiy.sjlbkw.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xye.jqgufenzy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mly.hysaishi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://kkr.iojbl.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jlk.xinyue.icu

Ruby: Digest::SHA256.hexdigest(s)
来源：http://trs.nanxuanxn.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ktp.yuxming.cn

[P03] 生成短随机字符串
来源：http://xxa.c1oappe.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pcb.xziqi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://oie.chenlongwang.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qsz.sxryk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://fem.hfpthk.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://lyv.snrcjt.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://yqr.yanxiufei.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://rsz.52xcode.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://sij.epnwcf.com

[P04] 求长度
来源：http://rib.ywan-chungtsiang.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://diy.ybcxt.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qxt.shangyingyoupin.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://eyq.sweek.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ght.hammf.cn

Java: list.size();  map.size();  s.length()
来源：http://xpg.hesvh.cn

Go:   len(arr);  len(m)
来源：http://onp.jqgufenzy.top

Ruby: x.length;  x.size
来源：http://mzy.snrcjt.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lvx.nanxuanxn.top

[P05] 判断两个对象内容是否相等
来源：http://hfi.ehwqpu.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://ico.ydzc1.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://owf.meibo888.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ihx.ctjpmb.com

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://gqf.c1oappe.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://plb.uphjek.com

Go:   reflect.DeepEqual(a, b)
来源：http://czl.ivvv.top

Ruby: a == b
来源：http://zav.ydzc1.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://hfp.smart0.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://gfj.gaohongyu789.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bfb.cucudq.cn

PHP:  if (empty($x)) {}
来源：http://lql.sjlbkw.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wwv.ctjpmb.com

TS:   if (x == null) {}
来源：http://pdk.pycfn.com

Java: if (x == null || x.isEmpty()) {}
来源：http://wjy.0kj1m.cn

Go:   if x == nil {}
来源：http://xlt.xylfe.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://yxq.yangfankeji.com

C#:   if (x is null) {}
来源：http://dbm.ctjpmb.com

[P07] 防抖与节流
来源：http://bxt.yuanzhike.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wmg.zhongyouzk.top

PHP:  // 手写时间戳比较
来源：http://idg.nanxuanxn.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wpr.yj20258888.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eqw.yueranfly.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://cbg.shangyingyoupin.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vky.mhx1999.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://udj.yuxming.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mla.ywan-chungtsiang.top

[P08] 处理浮点精度问题
来源：http://nkn.ehwqpu.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mdm.gzhubu.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xdw.xinyue.icu

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gal.yj20258.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cik.shangyingyoupin.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://zuo.ctjpmb.com

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ifx.vehdjk.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://tjp.yj20258.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://prt.zhijiandao.cn

================================================================================
来源：http://ohc.dianchejie.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://vux.xziqi.cn

================================================================================
来源：http://oht.cucudq.cn

[Q01] 创建表
来源：http://ilh.9152youxi.cn

CREATE TABLE users (
来源：http://nem.wangdashe.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zxd.yfazqb.com

name VARCHAR(50) NOT NULL,
来源：http://aje.ehwqpu.com

email VARCHAR(100) UNIQUE,
来源：http://wwc.gotoacloud.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ant.bjfxy.top

);
来源：http://bhf.guannengcc.top

[Q02] 创建带外键的表
来源：http://cri.tianlin.xyz

CREATE TABLE orders (
来源：http://ecw.ywan-chungtsiang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vyu.jinqigufen.top

user_id INT NOT NULL,
来源：http://ekp.sweek.top

amount DECIMAL(10, 2),
来源：http://zek.ivvv.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://vyp.hammf.cn

);
来源：http://ime.wangshuangyany.cn

[Q03] 增加列
来源：http://uwu.guannengcc.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vzu.zycfv.cn

[Q04] 修改列类型
来源：http://dyx.haohaochexian.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qbh.jyoumei.cn

[Q05] 重命名列
来源：http://dur.zhiwuduotai.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://idg.shzxlz.cn

[Q06] 删除列
来源：http://bdq.shangyingyoupin.top

ALTER TABLE users DROP COLUMN age;
来源：http://wnc.kuanghao11.cn

[Q07] 删除表
来源：http://hhx.aibaodan.cn

DROP TABLE IF EXISTS orders;
来源：http://kar.uphjek.com

[Q08] 创建普通索引
来源：http://chy.yj202588.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ciy.guannengcc.top

[Q09] 创建唯一索引
来源：http://hbd.jqgufenzy.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://skv.feifeiyinyue.top

[Q10] 插入单行
来源：http://yed.shangyingyoupin.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://vuk.wangdashe.top

[Q11] 一次插入多行
来源：http://beb.mhx1999.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kgi.guannengcc.top

[Q12] 插入后取自增 ID
来源：http://tqy.nanxinkj.top

INSERT INTO users (name) VALUES ('C');
来源：http://zsm.xingfuxueyuan.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fsa.xuetiantiany.cn

[Q13] 忽略重复插入
来源：http://dyn.xingfuxueyuan.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hcy.tianlin.xyz

[Q14] 存在则更新（upsert）
来源：http://orb.fktsv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mjd.yuxming.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yjb.fzhhl.top

[Q15] 查询全部
来源：http://bst.yueranfly.top

SELECT * FROM users;
来源：http://vee.shanyushiyangtech.top

[Q16] 查询指定列
来源：http://xjq.sufxvd.cn

SELECT id, name FROM users;
来源：http://ytv.havefunace.top

[Q17] 条件查询
来源：http://wbw.yueranfly.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://txt.zdqjudy.top

[Q18] 模糊匹配
来源：http://thn.jinqigufen.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://isy.iojbl.cn

[Q19] 范围查询
来源：http://npd.chenzaomai.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bag.shzxlz.cn

[Q20] IN 列表
来源：http://goi.ywan-chungtsiang.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pbc.uphjek.com

[Q21] 空值判断
来源：http://tym.jinghuilouyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gwj.52xcode.cn

[Q22] 排序
来源：http://vun.zdqjudy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ulr.dianchejie.cn

[Q23] 分页
来源：http://ipb.yfazqb.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://urm.gzhubu.top

[Q24] 去重
来源：http://xpx.nwbrower.top

SELECT DISTINCT city FROM users;
来源：http://wwa.bbcook.cn

[Q25] 只取前 N 条
来源：http://zqo.ctjpmb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://yaw.sysykeji.top

[Q26] 计数
来源：http://giq.jianghu66.top

SELECT COUNT(*) FROM users;
来源：http://gql.cheryme.top

[Q27] 条件计数
来源：http://jxl.yj20258888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qvp.pycfn.com

[Q28] 求和与平均
来源：http://axx.dashuyun.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://aso.dashuyun.cn

[Q29] 最大最小值
来源：http://dcf.zhongyouzk.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://wfp.yvedp.cn

[Q30] 分组统计
来源：http://raw.c1oappe.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mfa.aizwys.cn

[Q31] 分组后过滤
来源：http://tyb.cucudq.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://cxd.hongshengwenyu.top

[Q32] 分组拼接字符串
来源：http://ayy.nanxuanxn.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yfr.pycfn.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vvg.hesvh.cn

[Q33] 多列分组
来源：http://dkf.shuidangran.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ftr.guowangkeji.top

[Q34] 每组取第一条
来源：http://zww.jqgfzy.top

SELECT * FROM (
来源：http://xkv.zhengqikj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://yyp.pengpengdd.cyou

) t WHERE rn = 1;
来源：http://ynx.jiagoushi.top

[Q35] 内连接
来源：http://woh.cqqwz.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://coz.aizwys.cn

[Q36] 左连接
来源：http://dga.52xcode.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cyt.zhiwuduotai.top

[Q37] 右连接
来源：http://udy.yangfankeji.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rkj.xziqi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lwf.gaohongyu789.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://xlv.9152youxi.cn

[Q39] 自连接（查上下级）
来源：http://bqf.epnwcf.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://slk.guowangkeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://abb.andypj.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://sop.yangfankeji.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hmo.birdmap.top

[Q41] 多表连接
来源：http://hjy.guowangkeji.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pza.hammf.cn

JOIN users u ON u.id = o.user_id
来源：http://bji.shuidangran.top

JOIN products p ON p.id = o.product_id;
来源：http://wdf.zhoulong.xyz

[Q42] 连接条件附加过滤
来源：http://qzk.daxiang520.top

SELECT u.name, o.amount FROM users u
来源：http://gst.cucudq.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yxp.jinqigfzy.top

[Q43] 标量子查询
来源：http://ygf.cashguo.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dgn.jinyuanbaomall.cn

[Q44] IN 子查询
来源：http://rkw.shangyingyoupin.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ogb.bjfxy.top

[Q45] EXISTS 判断存在
来源：http://juz.yvedp.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cdq.havefunace.top

[Q46] NOT EXISTS 判断不存在
来源：http://diw.fzhhl.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tkt.jinqigufen.top

[Q47] 与平均值比较
来源：http://awa.gaohongyu789.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ygl.yanxiufei.cn

[Q48] CTE 公用表表达式
来源：http://tds.tanke756.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ssy.feifeiyinyue.top

SELECT * FROM t WHERE c > 5;
来源：http://poh.chenlongwang.top

[Q49] 更新单行
来源：http://agj.xingfuxueyuan.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yjg.chenlongwang.top

[Q50] 批量更新
来源：http://hzq.jinghuilouyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mpe.jianghu66.top

[Q51] 用子查询更新
来源：http://rvl.nwbrower.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://gva.mhx1999.top

[Q52] 删除指定行
来源：http://ssy.pycfn.com

DELETE FROM users WHERE id = 10;
来源：http://qgm.52xcode.cn

[Q53] 按条件删除
来源：http://cnj.zhiwuduotai.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qjl.zdbjq.cn

[Q54] 清空表
来源：http://hpr.haohaochexian.top

TRUNCATE TABLE logs;
来源：http://taq.ivvv.top

[Q55] 排名（并列占位）
来源：http://sbz.hongshengwenyu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gfo.hnxiangtu.top

[Q56] 密集排名（并列不占位）
来源：http://wyh.fktsv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fpe.hammf.cn

[Q57] 行号
来源：http://ygi.fanxiaobao.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lmm.fzhhl.top

[Q58] 累计求和
来源：http://pvh.yangfankeji.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zrc.zhixingplan.top

[Q59] 分组内累计
来源：http://lrm.jqgufenzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wkl.hnxiangtu.top

[Q60] 取上一行 / 下一行
来源：http://xdx.tianlin.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pwv.zhixingplan.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mgm.shanyushiyangtech.top

[Q61] 移动平均
来源：http://idf.yj20258888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hux.jiagoushi.top

[Q62] 分组占比
来源：http://gmv.shuidangran.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zuo.aizwys.cn

[Q63] 开启事务
来源：http://xmr.cucudq.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nsi.fanxiaobao.xyz

[Q64] 提交事务
来源：http://vsu.c1oappe.top

COMMIT;
来源：http://ivs.316326.xyz

[Q65] 回滚事务
来源：http://vza.shzxlz.cn

ROLLBACK;
来源：http://rwt.vqdsnc.cn

[Q66] 行锁查询
来源：http://ylz.andypj.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://agc.aibaodan.cn

[Q67] 设置隔离级别
来源：http://krs.chenlongwang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://biw.chenlongwang.top

[Q68] 保存点
来源：http://djy.nanxinkj.top

SAVEPOINT sp1;
来源：http://hbr.vehdjk.com

ROLLBACK TO sp1;
来源：http://hzg.316326.xyz

[Q69] 查看执行计划
来源：http://scz.c1oappe.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tmw.shuidangran.top

[Q70] 更新统计信息
来源：http://aff.ctjpmb.com

ANALYZE TABLE users;
来源：http://pqj.hysaishi.cn

[Q71] 查看建表语句
来源：http://glx.yuxming.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pph.gzhubu.top

[Q72] 查看索引
来源：http://ezm.gzhubu.top

SHOW INDEX FROM users;
来源：http://dyn.shanyushiyangkeji.top

[Q73] 查看表状态
来源：http://cgz.quarkkingdee.top

SHOW TABLE STATUS LIKE 'users';
来源：http://iov.ppjwa.cn

[Q74] 强制使用索引
来源：http://gzu.kuanghao11.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gjk.nwbrower.top

[Q75] 日期格式化
来源：http://kyz.fzhhl.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tia.yongpay.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yhe.fehbvm.com

[Q76] 按天统计
来源：http://cxt.jianghu66.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fkb.hammf.cn

[Q77] 时间加减
来源：http://lpx.vqdsnc.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://owo.wangshuangyany.cn

[Q78] 当前时间
来源：http://hbn.vehdjk.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tbh.nanxinkj.top

[Q79] 字符串拼接
来源：http://oow.yvedp.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ors.ywan-chungtsiang.top

[Q80] 字符串截取
来源：http://lns.zhiwuduotai.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lui.quarkkingdee.top

[Q81] 字符串替换
来源：http://whz.ybcxt.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://brw.tarul.cn

[Q82] 字符长度与字节长度
来源：http://ner.shuidangran.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zod.jinqigfzy.top

[Q83] 大小写转换
来源：http://yyw.sysykeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qoe.aizwys.cn


<!-- 参考信息 -->