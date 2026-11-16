代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mfn.fehbvm.com

[O03] 加锁保护共享数据
来源：http://mrh.xziqi.cn

Py:   with lock: shared += 1
来源：http://mhk.zhiwuduotai.top

PHP:  // 用 flock() 做文件锁
来源：http://dom.ivvv.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jby.shangyingyoupin.top

TS:   // 同 JS
来源：http://ntb.shzxlz.cn

Java: synchronized (this) { shared++; }
来源：http://vkc.xinyue.icu

Go:   mu.Lock();  defer mu.Unlock()
来源：http://teo.ybcxt.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://bwn.fktsv.cn

C#:   lock (gate) { shared++; }
来源：http://pfc.andypj.xyz

[O04] 定义异步函数并等待
来源：http://cjh.bjfxy.top

Py:   async def f():⏎    await g()
来源：http://cfw.hywenlv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wde.xuanzx.com

JS:   async function f() { await g(); }
来源：http://fzs.cdnleiting.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://njq.xylfe.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://dfp.jinqigufen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wgj.chenlongwang.top

Ruby: # 用 Fiber 或 async gem
来源：http://ncj.9152youxi.cn

C#:   async Task F() { await G(); }
来源：http://vhk.andypj.xyz

[O05] 并发执行并等待全部完成
来源：http://zap.316326.xyz

Py:   asyncio.gather(*tasks)
来源：http://plg.nwbrower.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://kik.zhixingplan.top

JS:   await Promise.all(tasks)
来源：http://nqb.yonumen.top

TS:   await Promise.all(tasks)
来源：http://haf.nanxuanxn.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://fvt.shzxlz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://gtp.jyoumei.cn

Ruby: threads.map(&:join)
来源：http://qwf.fengsongda.top

C#:   await Task.WhenAll(t1, t2)
来源：http://fhj.aizwys.cn

[O06] 使用进程池
来源：http://hek.vehdjk.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://aee.daxiang520.top

PHP:  // pcntl_fork 或多进程队列
来源：http://aqs.quarkkingdee.top

JS:   // child_process / cluster 模块
来源：http://nen.ctjpmb.com

TS:   // child_process / cluster 模块
来源：http://uls.feifeiyinyue.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kqw.feifeiyinyue.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rqg.aizwys.cn

Ruby: // fork 块
来源：http://iyq.hesvh.cn

C#:   Parallel.For
来源：http://cwx.daxiang520.top

================================================================================
来源：http://ymn.tarul.cn

P. 常用工具函数
来源：http://jua.0kj1m.cn

================================================================================
来源：http://oxj.sufxvd.cn

[P01] 生成 UUID
来源：http://clp.zhaomingkeji.xyz

Py:   str(uuid.uuid4())
来源：http://eqs.wangdashe.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qzy.birdmap.top

JS:   crypto.randomUUID()
来源：http://whq.c1oappe.top

TS:   crypto.randomUUID()
来源：http://ibz.yj20258.top

Java: UUID.randomUUID().toString()
来源：http://ybo.cucudq.cn

Go:   // 用 github.com/google/uuid
来源：http://vtf.0kj1m.cn

Ruby: SecureRandom.uuid
来源：http://lup.xylfe.cn

C#:   Guid.NewGuid().ToString()
来源：http://uip.gzhubu.top

[P02] MD5 / SHA256 摘要
来源：http://yya.yj20258888.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://sfd.hammf.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fvm.chenzaomai.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://npe.nanxinkj.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://yci.nanxuanxn.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://oms.bjfxy.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fom.jiagoushi.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://nqz.chenzaomai.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://fjw.vqdsnc.cn

[P03] 生成短随机字符串
来源：http://rxa.shangyingyoupin.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://cng.hesvh.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tky.jlsjyb.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jee.fehbvm.com

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://thl.zdqjudy.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://rbl.bbcook.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://xrd.c1oappe.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ruf.cdnleiting.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://yvg.shuidangran.top

[P04] 求长度
来源：http://cfq.ydjk.org.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://xjw.zhaomingkeji.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lfg.bbcook.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hvg.cashguo.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xyo.uphjek.com

Java: list.size();  map.size();  s.length()
来源：http://gtd.daxiang520.top

Go:   len(arr);  len(m)
来源：http://svq.cucudq.cn

Ruby: x.length;  x.size
来源：http://oqh.0kj1m.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://obu.zdqjudy.top

[P05] 判断两个对象内容是否相等
来源：http://eoe.ivvv.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://uak.bjfxy.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://gbf.cashguo.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://pbi.tianlin.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://swz.yueranfly.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://efn.hnqzz.top

Go:   reflect.DeepEqual(a, b)
来源：http://yxh.nanxinkj.top

Ruby: a == b
来源：http://snu.ppjwa.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://jpn.hysaishi.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rni.yongpay.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://nbv.ybcxt.top

PHP:  if (empty($x)) {}
来源：http://qul.tanke756.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vwh.feifeiyinyue.top

TS:   if (x == null) {}
来源：http://gsi.cheryme.top

Java: if (x == null || x.isEmpty()) {}
来源：http://pzg.bbcook.cn

Go:   if x == nil {}
来源：http://xih.tianlin.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://zym.bjfxy.top

C#:   if (x is null) {}
来源：http://jcr.zhiwuduotai.top

[P07] 防抖与节流
来源：http://tmx.hammf.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mmt.vehdjk.com

PHP:  // 手写时间戳比较
来源：http://wxf.hcnkem.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://hpm.mhx1999.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://slj.yj20258.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://hro.fanxiaobao.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xcj.chenlongwang.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qrj.hnxiangtu.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://zon.316326.xyz

[P08] 处理浮点精度问题
来源：http://mou.sjlbkw.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://dop.pycfn.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nhb.ctjpmb.com

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oht.cucudq.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://rab.sxryk.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sxk.shanyushiyangkeji.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ajz.yvedp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://iya.jinghuilouyu.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://dzu.hfpthk.cn

================================================================================
来源：http://fgc.pycfn.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nwm.zdbjq.cn

================================================================================
来源：http://tjp.c1oappe.top

[Q01] 创建表
来源：http://wle.redwolf501.top

CREATE TABLE users (
来源：http://rgq.dashuyun.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ngb.jinyuanbaomall.cn

name VARCHAR(50) NOT NULL,
来源：http://vhw.shanyushiyangtech.top

email VARCHAR(100) UNIQUE,
来源：http://btx.bbcook.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ptn.jinyuanbaomall.cn

);
来源：http://mgw.uphjek.com

[Q02] 创建带外键的表
来源：http://jii.guannengcc.top

CREATE TABLE orders (
来源：http://jiy.chenlongwang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://grr.hysaishi.cn

user_id INT NOT NULL,
来源：http://dwi.yj202588.top

amount DECIMAL(10, 2),
来源：http://jtv.pycfn.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://eax.snrcjt.cn

);
来源：http://lmx.nwbrower.top

[Q03] 增加列
来源：http://ask.meibo888.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://eny.hfpthk.cn

[Q04] 修改列类型
来源：http://yep.dashuyun.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iil.havefunace.top

[Q05] 重命名列
来源：http://ttd.chenlongwang.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://jrt.andypj.xyz

[Q06] 删除列
来源：http://uzs.tarul.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ppi.xylfe.cn

[Q07] 删除表
来源：http://kwc.316326.xyz

DROP TABLE IF EXISTS orders;
来源：http://fkq.ppjwa.cn

[Q08] 创建普通索引
来源：http://rlq.sufxvd.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zpf.sxryk.cn

[Q09] 创建唯一索引
来源：http://isd.uphjek.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bup.yj20258888.top

[Q10] 插入单行
来源：http://sht.hywenlv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://voa.pengpengdd.cyou

[Q11] 一次插入多行
来源：http://ucw.hesvh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://neh.jinqigfzy.top

[Q12] 插入后取自增 ID
来源：http://jzu.hcnkem.com

INSERT INTO users (name) VALUES ('C');
来源：http://jvd.guowangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://bkc.cucudq.cn

[Q13] 忽略重复插入
来源：http://yji.aizwys.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://asv.haohaochexian.top

[Q14] 存在则更新（upsert）
来源：http://csq.9152youxi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qhf.jinqigufen.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://prn.yangfankeji.com

[Q15] 查询全部
来源：http://zzj.gogol.net.cn

SELECT * FROM users;
来源：http://zrk.guowangkeji.top

[Q16] 查询指定列
来源：http://xbe.zhijiandao.cn

SELECT id, name FROM users;
来源：http://zdq.jyoumei.cn

[Q17] 条件查询
来源：http://akh.kuanghao11.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zqc.hysaishi.cn

[Q18] 模糊匹配
来源：http://nuq.hywenlv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ugc.zycfv.cn

[Q19] 范围查询
来源：http://jcf.shuidangran.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fgb.yangfankeji.com

[Q20] IN 列表
来源：http://sww.zycfv.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bly.daria6918.cn

[Q21] 空值判断
来源：http://ars.snrcjt.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://suq.jinqigufen.top

[Q22] 排序
来源：http://mkg.jlsjyb.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://sdk.hongshengwenyu.top

[Q23] 分页
来源：http://mzs.aibaodan.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ymx.52xcode.cn

[Q24] 去重
来源：http://goe.gogol.net.cn

SELECT DISTINCT city FROM users;
来源：http://kvo.zhixingplan.top

[Q25] 只取前 N 条
来源：http://qpo.nanxinkj.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bhj.cheryme.top

[Q26] 计数
来源：http://kvr.yonumen.top

SELECT COUNT(*) FROM users;
来源：http://nto.zdbjq.cn

[Q27] 条件计数
来源：http://yvl.nwbrower.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://dep.cucudq.cn

[Q28] 求和与平均
来源：http://yka.jiagoushi.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://coo.shangyingyoupin.top

[Q29] 最大最小值
来源：http://nya.jlsjyb.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://djs.gzhubu.top

[Q30] 分组统计
来源：http://dcz.shanyushiyangtech.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kne.daxiang520.top

[Q31] 分组后过滤
来源：http://zxk.sufxvd.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nfo.jyoumei.cn

[Q32] 分组拼接字符串
来源：http://ire.9152youxi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jra.yvedp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://iis.jinyuanbaomall.cn

[Q33] 多列分组
来源：http://iyb.fzhhl.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xcb.jinqigfzy.top

[Q34] 每组取第一条
来源：http://suq.zdqjudy.top

SELECT * FROM (
来源：http://mvj.mhx1999.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fjb.shanyushiyangtech.top

) t WHERE rn = 1;
来源：http://uut.hfpthk.cn

[Q35] 内连接
来源：http://byt.epnwcf.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fyj.chenlongwang.top

[Q36] 左连接
来源：http://xyt.xuanzx.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pqr.tian-w.cn

[Q37] 右连接
来源：http://gqb.kuanghao11.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xdt.yj20258888.top

[Q38] 全外连接（PostgreSQL）
来源：http://qcd.0kj1m.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ccv.zhijiandao.cn

[Q39] 自连接（查上下级）
来源：http://lwl.shanyushiyangtech.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://cem.nanxuanxn.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iiq.wangdashe.top

[Q40] 交叉连接（笛卡尔积）
来源：http://tlu.mhx1999.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vlu.jqgfzy.top

[Q41] 多表连接
来源：http://yvu.jinqigfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jwr.kuanghao11.cn

JOIN users u ON u.id = o.user_id
来源：http://xlv.hywenlv.cn

JOIN products p ON p.id = o.product_id;
来源：http://zfx.dashuyun.cn

[Q42] 连接条件附加过滤
来源：http://duh.chenlongwang.top

SELECT u.name, o.amount FROM users u
来源：http://tqo.redwolf501.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dqe.chenjidiqi.icu

[Q43] 标量子查询
来源：http://tvh.havefunace.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nnm.zdbjq.cn

[Q44] IN 子查询
来源：http://gqk.ivvv.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zfk.jqgfzy.top

[Q45] EXISTS 判断存在
来源：http://sft.zhongyouzk.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zpi.ppjwa.cn

[Q46] NOT EXISTS 判断不存在
来源：http://daq.pycfn.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sje.fzhhl.top

[Q47] 与平均值比较
来源：http://kgh.ppjwa.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://buf.uphjek.com

[Q48] CTE 公用表表达式
来源：http://xci.jiagoushi.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xqo.feifeiyinyue.top

SELECT * FROM t WHERE c > 5;
来源：http://vub.yj202588.top

[Q49] 更新单行
来源：http://ctx.nanxinkj.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uwm.hysaishi.cn

[Q50] 批量更新
来源：http://bxq.9152youxi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vfs.ehwqpu.com

[Q51] 用子查询更新
来源：http://grf.snrcjt.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://adp.chenzaomai.com

[Q52] 删除指定行
来源：http://rff.ctjpmb.com

DELETE FROM users WHERE id = 10;
来源：http://zsx.zhoulong.xyz

[Q53] 按条件删除
来源：http://fso.52xcode.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uht.zhaomingkeji.xyz

[Q54] 清空表
来源：http://akc.haohaochexian.top

TRUNCATE TABLE logs;
来源：http://wrs.uphjek.com

[Q55] 排名（并列占位）
来源：http://eig.gogol.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wwk.52xcode.cn

[Q56] 密集排名（并列不占位）
来源：http://inb.cucudq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xrt.gotoacloud.top

[Q57] 行号
来源：http://pew.hnqzz.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dmp.ppjwa.cn

[Q58] 累计求和
来源：http://cgk.kuanghao11.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ctr.shanyushiyangtech.top

[Q59] 分组内累计
来源：http://kel.fehbvm.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dyg.feifeiyinyue.top

[Q60] 取上一行 / 下一行
来源：http://qfd.zhixingplan.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jgc.kuanghao11.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rag.fehbvm.com

[Q61] 移动平均
来源：http://qfw.wangshuangyany.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rij.andypj.xyz

[Q62] 分组占比
来源：http://jmy.aizwys.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ueo.xingfuxueyuan.xyz

[Q63] 开启事务
来源：http://ykt.vehdjk.com

START TRANSACTION;                -- 或 BEGIN
来源：http://izb.9152youxi.cn

[Q64] 提交事务
来源：http://vcx.iojbl.cn

COMMIT;
来源：http://cxi.hesvh.cn

[Q65] 回滚事务
来源：http://szn.xingfuxueyuan.xyz

ROLLBACK;
来源：http://nvd.daria6918.cn

[Q66] 行锁查询
来源：http://bii.9152youxi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zed.zhijiandao.cn

[Q67] 设置隔离级别
来源：http://jbc.redwolf501.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ouk.ydjk.org.cn

[Q68] 保存点
来源：http://pjb.havefunace.top

SAVEPOINT sp1;
来源：http://ncx.tianlin.xyz

ROLLBACK TO sp1;
来源：http://sgp.ywan-chungtsiang.top

[Q69] 查看执行计划
来源：http://iey.snrcjt.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jtl.bjfxy.top

[Q70] 更新统计信息
来源：http://nnk.iojbl.cn

ANALYZE TABLE users;
来源：http://ewi.hnxiangtu.top

[Q71] 查看建表语句
来源：http://hbz.ctjpmb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xdm.xylfe.cn

[Q72] 查看索引
来源：http://rvb.cashguo.top

SHOW INDEX FROM users;
来源：http://lan.xinyue.icu

[Q73] 查看表状态
来源：http://suf.feifeiyinyue.top

SHOW TABLE STATUS LIKE 'users';
来源：http://siq.tian-w.cn

[Q74] 强制使用索引
来源：http://hmm.haohaochexian.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://opx.yonumen.top

[Q75] 日期格式化
来源：http://pzz.ybcxt.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zzx.smart0.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pxu.jinghuilouyu.cn

[Q76] 按天统计
来源：http://jag.yanxiufei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://noy.shzxlz.cn

[Q77] 时间加减
来源：http://itv.uphjek.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://akp.sjlbkw.cn

[Q78] 当前时间
来源：http://bii.guannengcc.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pwt.nwbrower.top

[Q79] 字符串拼接
来源：http://bbv.aibaodan.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qby.wangshuangyany.cn

[Q80] 字符串截取
来源：http://pzy.xylfe.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fcf.tianlin.xyz

[Q81] 字符串替换
来源：http://aww.pengpengdd.cyou

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qap.cheryme.top


<!-- 参考信息 -->