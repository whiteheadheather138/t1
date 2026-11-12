代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://ffq.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://orb.xinyue.icu

Java: synchronized (this) { shared++; }
来源：http://bfx.zdbjq.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://drm.wangdashe.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://blx.zhoulong.xyz

C#:   lock (gate) { shared++; }
来源：http://iyc.guowangkeji.top

[O04] 定义异步函数并等待
来源：http://spc.zdqjudy.top

Py:   async def f():⏎    await g()
来源：http://ovn.fktsv.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iru.zdbjq.cn

JS:   async function f() { await g(); }
来源：http://rgc.ydjk.org.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://jsi.ehwqpu.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xwm.uphjek.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://eol.feifeiyinyue.top

Ruby: # 用 Fiber 或 async gem
来源：http://hqa.zycfv.cn

C#:   async Task F() { await G(); }
来源：http://qaj.zhaomingkeji.xyz

[O05] 并发执行并等待全部完成
来源：http://sox.ydjk.org.cn

Py:   asyncio.gather(*tasks)
来源：http://lgs.nanxinkj.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://hpd.ydzc1.top

JS:   await Promise.all(tasks)
来源：http://wwb.gogol.net.cn

TS:   await Promise.all(tasks)
来源：http://ddx.xingfuxueyuan.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qnj.daria6918.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mmf.kuanghao11.cn

Ruby: threads.map(&:join)
来源：http://ewr.shuidangran.top

C#:   await Task.WhenAll(t1, t2)
来源：http://pyu.tarul.cn

[O06] 使用进程池
来源：http://wca.sxryk.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jbr.jqgfzy.top

PHP:  // pcntl_fork 或多进程队列
来源：http://sux.yj20258888.top

JS:   // child_process / cluster 模块
来源：http://lzb.bjfxy.top

TS:   // child_process / cluster 模块
来源：http://yti.smart0.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://zlj.svipenyu.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://apo.sysykeji.top

Ruby: // fork 块
来源：http://rvp.jinqigfzy.top

C#:   Parallel.For
来源：http://gnk.redwolf501.top

================================================================================
来源：http://kdi.smart0.xyz

P. 常用工具函数
来源：http://xng.yvedp.cn

================================================================================
来源：http://xay.shzxlz.cn

[P01] 生成 UUID
来源：http://nrx.jinqigfzy.top

Py:   str(uuid.uuid4())
来源：http://cdi.hongshengwenyu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ezm.jianghu66.top

JS:   crypto.randomUUID()
来源：http://fhy.yvedp.cn

TS:   crypto.randomUUID()
来源：http://ghn.zhongyouzk.top

Java: UUID.randomUUID().toString()
来源：http://anj.nwbrower.top

Go:   // 用 github.com/google/uuid
来源：http://asq.xylfe.cn

Ruby: SecureRandom.uuid
来源：http://bxw.uphjek.com

C#:   Guid.NewGuid().ToString()
来源：http://ois.ybcxt.top

[P02] MD5 / SHA256 摘要
来源：http://mfg.redwolf501.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ryk.sysykeji.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://nlo.hesvh.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://btk.0kj1m.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://zxq.tarul.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://hxq.yj202588.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mbz.ydzc1.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bwv.gaohongyu789.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kvf.ppjwa.cn

[P03] 生成短随机字符串
来源：http://rog.nanxinkj.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fln.yuanzhike.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://gtz.dashuyun.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://evu.jinyuanbaomall.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://sai.fanxiaobao.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://xkd.yueranfly.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://plw.nanxinkj.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://ake.hcnkem.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gan.pengpengdd.cyou

[P04] 求长度
来源：http://vsr.ctjpmb.com

Py:   len(x)            # 字符串、列表、字典通用
来源：http://fgr.yuxming.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hqr.xziqi.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oau.vqdsnc.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://paf.zhiwuduotai.top

Java: list.size();  map.size();  s.length()
来源：http://hnj.9152youxi.cn

Go:   len(arr);  len(m)
来源：http://zhs.ywan-chungtsiang.top

Ruby: x.length;  x.size
来源：http://yee.xuetiantiany.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://snr.xinyue.icu

[P05] 判断两个对象内容是否相等
来源：http://nai.52xcode.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://lxj.fehbvm.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xtz.shanyushiyangtech.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://ubu.shanyushiyangtech.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ayp.xuanzx.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bbe.daxiang520.top

Go:   reflect.DeepEqual(a, b)
来源：http://opm.52xcode.cn

Ruby: a == b
来源：http://jen.birdmap.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://psj.hnqzz.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://uhv.jinqigufen.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://szb.jqgufenzy.top

PHP:  if (empty($x)) {}
来源：http://fdp.ydjk.org.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vcy.iojbl.cn

TS:   if (x == null) {}
来源：http://daj.ppjwa.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://edw.nanxuanxn.top

Go:   if x == nil {}
来源：http://ohi.sweek.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ata.uphjek.com

C#:   if (x is null) {}
来源：http://ozg.smart0.xyz

[P07] 防抖与节流
来源：http://nha.daxiang520.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sij.sjlbkw.cn

PHP:  // 手写时间戳比较
来源：http://ryo.xinyue.icu

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tje.shanyushiyangkeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dlb.yonumen.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bji.xuetiantiany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://trq.shangyingyoupin.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://fsc.daxiang520.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://pqh.nanxuanxn.top

[P08] 处理浮点精度问题
来源：http://nww.svipenyu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mcw.hywenlv.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xdu.shuidangran.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://vii.hysaishi.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://drf.guowangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://oan.gogol.net.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pme.sufxvd.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://doy.guowangkeji.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qqm.shanyushiyangtech.top

================================================================================
来源：http://yyp.snrcjt.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://jhi.yanxiufei.cn

================================================================================
来源：http://had.cashguo.top

[Q01] 创建表
来源：http://izj.sweek.top

CREATE TABLE users (
来源：http://dkm.yuxming.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vdk.yueranfly.top

name VARCHAR(50) NOT NULL,
来源：http://jav.shuidangran.top

email VARCHAR(100) UNIQUE,
来源：http://yij.ydjk.org.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://pwd.havefunace.top

);
来源：http://ypj.cashguo.top

[Q02] 创建带外键的表
来源：http://kld.hnqzz.top

CREATE TABLE orders (
来源：http://ypx.ydzc1.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eol.xziqi.cn

user_id INT NOT NULL,
来源：http://oft.zycfv.cn

amount DECIMAL(10, 2),
来源：http://vlv.yangfankeji.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gwc.yvedp.cn

);
来源：http://jjl.jqgufenzy.top

[Q03] 增加列
来源：http://tln.jinqigufen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ipd.gzhubu.top

[Q04] 修改列类型
来源：http://bte.gogol.net.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uuo.zhongyouzk.top

[Q05] 重命名列
来源：http://wyk.ydzc1.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nao.yuxming.cn

[Q06] 删除列
来源：http://ugk.yfazqb.com

ALTER TABLE users DROP COLUMN age;
来源：http://qrq.zdqjudy.top

[Q07] 删除表
来源：http://ybg.jinqigfzy.top

DROP TABLE IF EXISTS orders;
来源：http://pgj.fengsongda.top

[Q08] 创建普通索引
来源：http://csc.hnxiangtu.top

CREATE INDEX idx_users_email ON users(email);
来源：http://pjv.kuanghao11.cn

[Q09] 创建唯一索引
来源：http://pdt.andypj.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://zmy.xuetiantiany.cn

[Q10] 插入单行
来源：http://ydw.fktsv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ypn.hywenlv.cn

[Q11] 一次插入多行
来源：http://gux.snrcjt.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zgm.cashguo.top

[Q12] 插入后取自增 ID
来源：http://apt.xuanzx.com

INSERT INTO users (name) VALUES ('C');
来源：http://scw.yonumen.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wou.hywenlv.cn

[Q13] 忽略重复插入
来源：http://kql.havefunace.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://svf.yuxming.cn

[Q14] 存在则更新（upsert）
来源：http://kod.bbcook.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://egl.vehdjk.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://sdy.aibaodan.cn

[Q15] 查询全部
来源：http://enl.shanyushiyangtech.top

SELECT * FROM users;
来源：http://ahs.cheryme.top

[Q16] 查询指定列
来源：http://jsm.bjfxy.top

SELECT id, name FROM users;
来源：http://coy.bjfxy.top

[Q17] 条件查询
来源：http://oum.redwolf501.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pgi.yuanzhike.top

[Q18] 模糊匹配
来源：http://chx.zhoulong.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://izd.jiagoushi.top

[Q19] 范围查询
来源：http://igf.hfpthk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ofn.andypj.xyz

[Q20] IN 列表
来源：http://jhj.yongpay.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://abi.wangdashe.top

[Q21] 空值判断
来源：http://wlt.wangdashe.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bfm.gotoacloud.top

[Q22] 排序
来源：http://smo.svipenyu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qfp.shanyushiyangtech.top

[Q23] 分页
来源：http://oap.bjfxy.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uaj.hcnkem.com

[Q24] 去重
来源：http://uqo.quarkkingdee.top

SELECT DISTINCT city FROM users;
来源：http://hwz.epnwcf.com

[Q25] 只取前 N 条
来源：http://qbi.shzxlz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oit.jqgufenzy.top

[Q26] 计数
来源：http://nuu.dashuyun.cn

SELECT COUNT(*) FROM users;
来源：http://pog.ywan-chungtsiang.top

[Q27] 条件计数
来源：http://gbp.chenlongwang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wrb.zdqjudy.top

[Q28] 求和与平均
来源：http://gsk.yanxiufei.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zmm.bbcook.cn

[Q29] 最大最小值
来源：http://rri.haohaochexian.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dwa.cqqwz.cn

[Q30] 分组统计
来源：http://eqw.xuanzx.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ygi.sxryk.cn

[Q31] 分组后过滤
来源：http://yxb.quarkkingdee.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://hbx.sysykeji.top

[Q32] 分组拼接字符串
来源：http://zgy.pycfn.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://apm.52xcode.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pqs.zycfv.cn

[Q33] 多列分组
来源：http://vja.ydjk.org.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wmc.zhiwuduotai.top

[Q34] 每组取第一条
来源：http://cbw.yongpay.top

SELECT * FROM (
来源：http://nyf.yfazqb.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://efa.yvedp.cn

) t WHERE rn = 1;
来源：http://lso.svipenyu.cn

[Q35] 内连接
来源：http://lva.jlsjyb.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rnb.hnxiangtu.top

[Q36] 左连接
来源：http://jtd.chenjidiqi.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lzj.yvedp.cn

[Q37] 右连接
来源：http://ujm.epnwcf.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ikw.kuanghao11.cn

[Q38] 全外连接（PostgreSQL）
来源：http://lso.smart0.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tyn.jlsjyb.cn

[Q39] 自连接（查上下级）
来源：http://rii.zhijiandao.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://ywm.dianchejie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://cwv.pengpengdd.cyou

[Q40] 交叉连接（笛卡尔积）
来源：http://ynt.zdbjq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xye.andypj.xyz

[Q41] 多表连接
来源：http://bdq.ehwqpu.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://uff.shanyushiyangkeji.top

JOIN users u ON u.id = o.user_id
来源：http://reg.chenzaomai.com

JOIN products p ON p.id = o.product_id;
来源：http://lwi.ppjwa.cn

[Q42] 连接条件附加过滤
来源：http://jhh.wangdashe.top

SELECT u.name, o.amount FROM users u
来源：http://ido.guannengcc.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vgi.gzhubu.top

[Q43] 标量子查询
来源：http://quj.jiagoushi.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ygf.shanyushiyangkeji.top

[Q44] IN 子查询
来源：http://wlg.mhx1999.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sgu.gotoacloud.top

[Q45] EXISTS 判断存在
来源：http://plk.fengsongda.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wqj.cucudq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yus.sjlbkw.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vnh.gogol.net.cn

[Q47] 与平均值比较
来源：http://utx.jyoumei.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nqq.yuanzhike.top

[Q48] CTE 公用表表达式
来源：http://pif.xingfuxueyuan.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://djv.fktsv.cn

SELECT * FROM t WHERE c > 5;
来源：http://uyc.svipenyu.cn

[Q49] 更新单行
来源：http://xzo.fzhhl.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://awo.yongpay.top

[Q50] 批量更新
来源：http://afg.zhongyouzk.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kab.chenlongwang.top

[Q51] 用子查询更新
来源：http://nub.havefunace.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lya.fzhhl.top

[Q52] 删除指定行
来源：http://nqv.zhixingplan.top

DELETE FROM users WHERE id = 10;
来源：http://ecv.bjfxy.top

[Q53] 按条件删除
来源：http://eci.xylfe.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bfv.aibaodan.cn

[Q54] 清空表
来源：http://poj.feifeiyinyue.top

TRUNCATE TABLE logs;
来源：http://iol.ivvv.top

[Q55] 排名（并列占位）
来源：http://okf.sufxvd.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ayn.zycfv.cn

[Q56] 密集排名（并列不占位）
来源：http://kln.ctjpmb.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mjx.hnqzz.top

[Q57] 行号
来源：http://exy.yvedp.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ycn.havefunace.top

[Q58] 累计求和
来源：http://itu.hysaishi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hif.sxryk.cn

[Q59] 分组内累计
来源：http://uto.sjlbkw.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vrc.aibaodan.cn

[Q60] 取上一行 / 下一行
来源：http://xtq.jianghu66.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sxa.mhx1999.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://evr.ivvv.top

[Q61] 移动平均
来源：http://lfw.jinqigufen.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jcg.ybcxt.top

[Q62] 分组占比
来源：http://xrb.nwbrower.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hxc.ctjpmb.com

[Q63] 开启事务
来源：http://edn.epnwcf.com

START TRANSACTION;                -- 或 BEGIN
来源：http://dyh.andypj.xyz

[Q64] 提交事务
来源：http://gdk.tarul.cn

COMMIT;
来源：http://iak.epnwcf.com

[Q65] 回滚事务
来源：http://obi.sjlbkw.cn

ROLLBACK;
来源：http://hmv.jinghuilouyu.cn

[Q66] 行锁查询
来源：http://xur.tarul.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rpj.yj20258888.top

[Q67] 设置隔离级别
来源：http://mkq.ybcxt.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vnr.zhengqikj.top

[Q68] 保存点
来源：http://hws.316326.xyz

SAVEPOINT sp1;
来源：http://vkn.yfazqb.com

ROLLBACK TO sp1;
来源：http://myu.bjfxy.top

[Q69] 查看执行计划
来源：http://vkt.cqqwz.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vka.yongpay.top

[Q70] 更新统计信息
来源：http://bay.chenjidiqi.icu

ANALYZE TABLE users;
来源：http://udt.vehdjk.com

[Q71] 查看建表语句
来源：http://izx.cucudq.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kcc.tianlin.xyz

[Q72] 查看索引
来源：http://seb.jinyuanbaomall.cn

SHOW INDEX FROM users;
来源：http://jln.hnqzz.top

[Q73] 查看表状态
来源：http://dte.yangfankeji.com

SHOW TABLE STATUS LIKE 'users';
来源：http://knx.cashguo.top

[Q74] 强制使用索引
来源：http://wkz.sjlbkw.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://znw.fktsv.cn

[Q75] 日期格式化
来源：http://qbg.xuetiantiany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://idm.birdmap.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lgq.yangfankeji.com

[Q76] 按天统计
来源：http://swr.guannengcc.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gyf.jinyuanbaomall.cn

[Q77] 时间加减
来源：http://bzm.jiagoushi.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hon.xuetiantiany.cn

[Q78] 当前时间
来源：http://irj.hysaishi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fwx.ppjwa.cn

[Q79] 字符串拼接
来源：http://eiy.yfazqb.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ztd.epnwcf.com

[Q80] 字符串截取
来源：http://nui.bjfxy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rgq.andypj.xyz

[Q81] 字符串替换
来源：http://ywj.zhixingplan.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xuk.meibo888.top

[Q82] 字符长度与字节长度
来源：http://uov.shangyingyoupin.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dwf.sufxvd.cn

[Q83] 大小写转换
来源：http://etd.yangfankeji.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wyz.hesvh.cn


<!-- 参考信息 -->