代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uvc.yuxming.cn

[O03] 加锁保护共享数据
来源：http://fmi.shuidangran.top

Py:   with lock: shared += 1
来源：http://qcn.yanxiufei.cn

PHP:  // 用 flock() 做文件锁
来源：http://duj.xingfuxueyuan.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://bng.0kj1m.cn

TS:   // 同 JS
来源：http://emh.shangyingyoupin.top

Java: synchronized (this) { shared++; }
来源：http://owc.svipenyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://zpk.ivvv.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://cme.aizwys.cn

C#:   lock (gate) { shared++; }
来源：http://lhi.hysaishi.cn

[O04] 定义异步函数并等待
来源：http://vik.jinqigfzy.top

Py:   async def f():⏎    await g()
来源：http://dso.nanxuanxn.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xrk.ppjwa.cn

JS:   async function f() { await g(); }
来源：http://tds.zdbjq.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://xlf.jinqigfzy.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wab.yonumen.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ovp.ywan-chungtsiang.top

Ruby: # 用 Fiber 或 async gem
来源：http://pnl.gaohongyu789.top

C#:   async Task F() { await G(); }
来源：http://lsq.sufxvd.cn

[O05] 并发执行并等待全部完成
来源：http://doh.sufxvd.cn

Py:   asyncio.gather(*tasks)
来源：http://ecg.wangshuangyany.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dto.kuanghao11.cn

JS:   await Promise.all(tasks)
来源：http://nwm.sxryk.cn

TS:   await Promise.all(tasks)
来源：http://mmr.nwbrower.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mya.0kj1m.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://cze.feifeiyinyue.top

Ruby: threads.map(&:join)
来源：http://qyz.shangyingyoupin.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dus.havefunace.top

[O06] 使用进程池
来源：http://enm.ydjk.org.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ici.chenzaomai.com

PHP:  // pcntl_fork 或多进程队列
来源：http://erm.uphjek.com

JS:   // child_process / cluster 模块
来源：http://uvl.nanxinkj.top

TS:   // child_process / cluster 模块
来源：http://xqg.yonumen.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://dve.jiagoushi.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://nyj.shanyushiyangkeji.top

Ruby: // fork 块
来源：http://ncl.yonumen.top

C#:   Parallel.For
来源：http://dky.daria6918.cn

================================================================================
来源：http://jco.vehdjk.com

P. 常用工具函数
来源：http://vuk.gzhubu.top

================================================================================
来源：http://cos.yuanzhike.top

[P01] 生成 UUID
来源：http://gaz.ydzc1.top

Py:   str(uuid.uuid4())
来源：http://vyl.andypj.xyz

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uzp.daxiang520.top

JS:   crypto.randomUUID()
来源：http://uby.jinyuanbaomall.cn

TS:   crypto.randomUUID()
来源：http://vhv.chenzaomai.com

Java: UUID.randomUUID().toString()
来源：http://ncb.nanxuanxn.top

Go:   // 用 github.com/google/uuid
来源：http://nyg.ywan-chungtsiang.top

Ruby: SecureRandom.uuid
来源：http://icd.c1oappe.top

C#:   Guid.NewGuid().ToString()
来源：http://kju.hongshengwenyu.top

[P02] MD5 / SHA256 摘要
来源：http://pcu.yangfankeji.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vbb.zdbjq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xeb.chenlongwang.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://xoq.ybcxt.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://gvq.wangshuangyany.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vjy.chenzaomai.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://zsu.shzxlz.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://dpv.9152youxi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://hlk.hesvh.cn

[P03] 生成短随机字符串
来源：http://ihu.pengpengdd.cyou

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://lza.hnxiangtu.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://enz.yuxming.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://csk.zdqjudy.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://skn.gaohongyu789.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ecx.zdbjq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mvn.wangdashe.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://msk.nanxuanxn.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://ovn.chenlongwang.top

[P04] 求长度
来源：http://nli.shuidangran.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://koa.meibo888.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qft.shangyingyoupin.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://oej.nwbrower.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://aey.shuidangran.top

Java: list.size();  map.size();  s.length()
来源：http://xca.jinqigfzy.top

Go:   len(arr);  len(m)
来源：http://qnf.jqgfzy.top

Ruby: x.length;  x.size
来源：http://nia.ehwqpu.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://hik.hnxiangtu.top

[P05] 判断两个对象内容是否相等
来源：http://pse.yuanzhike.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nfo.yfazqb.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wqr.kuanghao11.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://neo.fzhhl.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://zxh.yj20258888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vdb.yanxiufei.cn

Go:   reflect.DeepEqual(a, b)
来源：http://vtc.jyoumei.cn

Ruby: a == b
来源：http://yok.yongpay.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qpd.jinyuanbaomall.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wtg.jinghuilouyu.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://pkn.yj202588.top

PHP:  if (empty($x)) {}
来源：http://jvf.nwbrower.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://yyq.zhongyouzk.top

TS:   if (x == null) {}
来源：http://xvv.redwolf501.top

Java: if (x == null || x.isEmpty()) {}
来源：http://wpy.zycfv.cn

Go:   if x == nil {}
来源：http://sbl.sysykeji.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ekj.zycfv.cn

C#:   if (x is null) {}
来源：http://jkr.iojbl.cn

[P07] 防抖与节流
来源：http://zdn.chenzaomai.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ucc.zycfv.cn

PHP:  // 手写时间戳比较
来源：http://mtp.fzhhl.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pnp.wangdashe.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pmu.wangshuangyany.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bvv.chenlongwang.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fzk.ppjwa.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://ayx.havefunace.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://vyf.yuxming.cn

[P08] 处理浮点精度问题
来源：http://yps.jyoumei.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ufq.xylfe.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xtn.jqgfzy.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://ath.hesvh.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://upo.gzhubu.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://biq.zhiwuduotai.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://ust.mhx1999.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://sml.cucudq.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rhx.hnxiangtu.top

================================================================================
来源：http://wuc.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fba.xinyue.icu

================================================================================
来源：http://kuq.jinqigfzy.top

[Q01] 创建表
来源：http://dij.ydzc1.top

CREATE TABLE users (
来源：http://qkj.shangyingyoupin.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://how.pengpengdd.cyou

name VARCHAR(50) NOT NULL,
来源：http://oxi.pycfn.com

email VARCHAR(100) UNIQUE,
来源：http://ydj.andypj.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://yoh.feifeiyinyue.top

);
来源：http://nla.meibo888.top

[Q02] 创建带外键的表
来源：http://jxk.9152youxi.cn

CREATE TABLE orders (
来源：http://nmz.fzhhl.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rpp.aibaodan.cn

user_id INT NOT NULL,
来源：http://yjh.haohaochexian.top

amount DECIMAL(10, 2),
来源：http://utj.kuanghao11.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://eev.dianchejie.cn

);
来源：http://wlb.ctjpmb.com

[Q03] 增加列
来源：http://dge.bjfxy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zdq.ivvv.top

[Q04] 修改列类型
来源：http://zgw.guowangkeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://apn.pycfn.com

[Q05] 重命名列
来源：http://cax.guannengcc.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dep.bbcook.cn

[Q06] 删除列
来源：http://gdi.xziqi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://lgz.birdmap.top

[Q07] 删除表
来源：http://pvd.kuanghao11.cn

DROP TABLE IF EXISTS orders;
来源：http://dst.havefunace.top

[Q08] 创建普通索引
来源：http://sfn.zhongyouzk.top

CREATE INDEX idx_users_email ON users(email);
来源：http://prp.xziqi.cn

[Q09] 创建唯一索引
来源：http://cpy.yonumen.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tvp.hnqzz.top

[Q10] 插入单行
来源：http://odv.hywenlv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xil.gaohongyu789.top

[Q11] 一次插入多行
来源：http://syy.guannengcc.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tym.sjlbkw.cn

[Q12] 插入后取自增 ID
来源：http://pja.zhoulong.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://cnf.gotoacloud.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tam.chenjidiqi.icu

[Q13] 忽略重复插入
来源：http://uhq.shzxlz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rzz.zhaomingkeji.xyz

[Q14] 存在则更新（upsert）
来源：http://ped.zhijiandao.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uwl.daxiang520.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://thq.svipenyu.cn

[Q15] 查询全部
来源：http://xoi.daria6918.cn

SELECT * FROM users;
来源：http://jku.fengsongda.top

[Q16] 查询指定列
来源：http://bmj.cheryme.top

SELECT id, name FROM users;
来源：http://lyq.gaohongyu789.top

[Q17] 条件查询
来源：http://amy.chenzaomai.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ixn.zhijiandao.cn

[Q18] 模糊匹配
来源：http://ntb.andypj.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lau.fehbvm.com

[Q19] 范围查询
来源：http://ugx.andypj.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xlp.cucudq.cn

[Q20] IN 列表
来源：http://bgi.hnxiangtu.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lrq.xuetiantiany.cn

[Q21] 空值判断
来源：http://uud.haohaochexian.top

SELECT * FROM users WHERE email IS NULL;
来源：http://itq.gzhubu.top

[Q22] 排序
来源：http://mem.sufxvd.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://let.xinyue.icu

[Q23] 分页
来源：http://ibl.dianchejie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dfo.ctjpmb.com

[Q24] 去重
来源：http://tky.fanxiaobao.xyz

SELECT DISTINCT city FROM users;
来源：http://hqa.redwolf501.top

[Q25] 只取前 N 条
来源：http://vyp.vehdjk.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://edb.wangshuangyany.cn

[Q26] 计数
来源：http://wdz.jinqigufen.top

SELECT COUNT(*) FROM users;
来源：http://uoe.gzhubu.top

[Q27] 条件计数
来源：http://csg.sxryk.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ubi.tarul.cn

[Q28] 求和与平均
来源：http://eiq.yuanzhike.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mkd.daxiang520.top

[Q29] 最大最小值
来源：http://nba.hammf.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://mxl.jinghuilouyu.cn

[Q30] 分组统计
来源：http://cjn.andypj.xyz

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://pof.hfpthk.cn

[Q31] 分组后过滤
来源：http://crx.yongpay.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ydb.zhoulong.xyz

[Q32] 分组拼接字符串
来源：http://fab.ydzc1.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rqd.hnqzz.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wcn.chenjidiqi.icu

[Q33] 多列分组
来源：http://iwm.pycfn.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://kru.fktsv.cn

[Q34] 每组取第一条
来源：http://mpz.smart0.xyz

SELECT * FROM (
来源：http://pkv.hysaishi.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://olk.zhongyouzk.top

) t WHERE rn = 1;
来源：http://neg.vehdjk.com

[Q35] 内连接
来源：http://iwo.hcnkem.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mtl.nanxuanxn.top

[Q36] 左连接
来源：http://oug.jlsjyb.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://poo.zdqjudy.top

[Q37] 右连接
来源：http://htx.xylfe.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dyh.yangfankeji.com

[Q38] 全外连接（PostgreSQL）
来源：http://imz.cashguo.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://agq.quarkkingdee.top

[Q39] 自连接（查上下级）
来源：http://qrc.yanxiufei.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://svk.hnqzz.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sih.zycfv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fqq.ctjpmb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vbu.hfpthk.cn

[Q41] 多表连接
来源：http://egj.snrcjt.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://enx.hnqzz.top

JOIN users u ON u.id = o.user_id
来源：http://igl.hnxiangtu.top

JOIN products p ON p.id = o.product_id;
来源：http://lgt.shanyushiyangtech.top

[Q42] 连接条件附加过滤
来源：http://fhs.yonumen.top

SELECT u.name, o.amount FROM users u
来源：http://ywg.jyoumei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dyq.shzxlz.cn

[Q43] 标量子查询
来源：http://pjk.snrcjt.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qte.sweek.top

[Q44] IN 子查询
来源：http://ymt.hcnkem.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jua.havefunace.top

[Q45] EXISTS 判断存在
来源：http://czn.ybcxt.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://afu.0kj1m.cn

[Q46] NOT EXISTS 判断不存在
来源：http://hst.wangshuangyany.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fvh.zdqjudy.top

[Q47] 与平均值比较
来源：http://azd.gaohongyu789.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://kyh.fanxiaobao.xyz

[Q48] CTE 公用表表达式
来源：http://tjd.shangyingyoupin.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bru.yuanzhike.top

SELECT * FROM t WHERE c > 5;
来源：http://aey.jqgfzy.top

[Q49] 更新单行
来源：http://wkr.jinqigfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vcw.cheryme.top

[Q50] 批量更新
来源：http://xei.zhixingplan.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qki.yj202588.top

[Q51] 用子查询更新
来源：http://jjl.feifeiyinyue.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://upm.hammf.cn

[Q52] 删除指定行
来源：http://fpe.hysaishi.cn

DELETE FROM users WHERE id = 10;
来源：http://jdw.snrcjt.cn

[Q53] 按条件删除
来源：http://ipd.hfpthk.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ipp.wangdashe.top

[Q54] 清空表
来源：http://qes.shanyushiyangtech.top

TRUNCATE TABLE logs;
来源：http://avf.mhx1999.top

[Q55] 排名（并列占位）
来源：http://alh.hongshengwenyu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://swc.c1oappe.top

[Q56] 密集排名（并列不占位）
来源：http://ytr.nanxinkj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kmd.gogol.net.cn

[Q57] 行号
来源：http://gsc.yj20258.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cxp.gzhubu.top

[Q58] 累计求和
来源：http://pvi.zdbjq.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dgu.zycfv.cn

[Q59] 分组内累计
来源：http://ent.ydzc1.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ayn.jiagoushi.top

[Q60] 取上一行 / 下一行
来源：http://qzg.xingfuxueyuan.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://arw.fehbvm.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cip.jiagoushi.top

[Q61] 移动平均
来源：http://lmb.ydzc1.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vgd.jianghu66.top

[Q62] 分组占比
来源：http://vhp.chenzaomai.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://avq.cqqwz.cn

[Q63] 开启事务
来源：http://ehl.hcnkem.com

START TRANSACTION;                -- 或 BEGIN
来源：http://ztu.ivvv.top

[Q64] 提交事务
来源：http://dco.jqgfzy.top

COMMIT;
来源：http://vmw.jianghu66.top

[Q65] 回滚事务
来源：http://dop.cheryme.top

ROLLBACK;
来源：http://cua.guowangkeji.top

[Q66] 行锁查询
来源：http://krg.hesvh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ztt.havefunace.top

[Q67] 设置隔离级别
来源：http://btv.xingfuxueyuan.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lng.daxiang520.top

[Q68] 保存点
来源：http://dka.shanyushiyangtech.top

SAVEPOINT sp1;
来源：http://fzh.ehwqpu.com

ROLLBACK TO sp1;
来源：http://rfb.zhongyouzk.top

[Q69] 查看执行计划
来源：http://bhj.tianlin.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wxx.fzhhl.top

[Q70] 更新统计信息
来源：http://vnd.zhengqikj.top

ANALYZE TABLE users;
来源：http://gvp.jinyuanbaomall.cn

[Q71] 查看建表语句
来源：http://xyy.zycfv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vgd.zhixingplan.top

[Q72] 查看索引
来源：http://hkp.vqdsnc.cn

SHOW INDEX FROM users;
来源：http://gnp.yanxiufei.cn

[Q73] 查看表状态
来源：http://hvf.yangfankeji.com

SHOW TABLE STATUS LIKE 'users';
来源：http://nqu.jiagoushi.top

[Q74] 强制使用索引
来源：http://dpw.cdnleiting.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xxq.xingfuxueyuan.xyz

[Q75] 日期格式化
来源：http://rqm.chenjidiqi.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uih.hesvh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rtr.ppjwa.cn

[Q76] 按天统计
来源：http://tds.shangyingyoupin.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cbh.ehwqpu.com

[Q77] 时间加减
来源：http://emm.zdqjudy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nga.yanxiufei.cn

[Q78] 当前时间
来源：http://xhp.pycfn.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rlm.jiagoushi.top

[Q79] 字符串拼接
来源：http://ifu.vqdsnc.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kga.guannengcc.top

[Q80] 字符串截取
来源：http://eeq.xylfe.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xjc.yuanzhike.top

[Q81] 字符串替换
来源：http://hxq.redwolf501.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wee.sjlbkw.cn


<!-- 参考信息 -->