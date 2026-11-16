代发 wailian999

TS:   // worker_threads 线程池
来源：http://oze.iojbl.cn

Java: Executors.newFixedThreadPool(4)
来源：http://rrj.nanxinkj.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hlr.xingfuxueyuan.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mug.cucudq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://atn.xuetiantiany.cn

[O03] 加锁保护共享数据
来源：http://qka.vehdjk.com

Py:   with lock: shared += 1
来源：http://fch.52xcode.cn

PHP:  // 用 flock() 做文件锁
来源：http://fre.fanxiaobao.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qiq.yvedp.cn

TS:   // 同 JS
来源：http://rby.yuxming.cn

Java: synchronized (this) { shared++; }
来源：http://sxa.jinqigfzy.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://uqq.tarul.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://ark.shzxlz.cn

C#:   lock (gate) { shared++; }
来源：http://rrj.nwbrower.top

[O04] 定义异步函数并等待
来源：http://bzh.hysaishi.cn

Py:   async def f():⏎    await g()
来源：http://zqh.iojbl.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blh.fengsongda.top

JS:   async function f() { await g(); }
来源：http://iso.fehbvm.com

TS:   async function f(): Promise<void> { await g(); }
来源：http://dog.guowangkeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hmy.gzhubu.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fxq.zhongyouzk.top

Ruby: # 用 Fiber 或 async gem
来源：http://zgp.tianlin.xyz

C#:   async Task F() { await G(); }
来源：http://fmm.vqdsnc.cn

[O05] 并发执行并等待全部完成
来源：http://jyd.sysykeji.top

Py:   asyncio.gather(*tasks)
来源：http://oqm.haohaochexian.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://yjt.ehwqpu.com

JS:   await Promise.all(tasks)
来源：http://mik.sufxvd.cn

TS:   await Promise.all(tasks)
来源：http://bzd.nanxuanxn.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ira.guowangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://kjp.xuanzx.com

Ruby: threads.map(&:join)
来源：http://emw.uphjek.com

C#:   await Task.WhenAll(t1, t2)
来源：http://nro.yongpay.top

[O06] 使用进程池
来源：http://jcj.yonumen.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://vdk.yj20258.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ksv.52xcode.cn

JS:   // child_process / cluster 模块
来源：http://bdc.yj202588.top

TS:   // child_process / cluster 模块
来源：http://jyc.chenlongwang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://aom.fengsongda.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://rbs.xylfe.cn

Ruby: // fork 块
来源：http://yar.cheryme.top

C#:   Parallel.For
来源：http://mdw.xuanzx.com

================================================================================
来源：http://oyt.tian-w.cn

P. 常用工具函数
来源：http://zla.vehdjk.com

================================================================================
来源：http://nfg.tanke756.top

[P01] 生成 UUID
来源：http://qfq.pengpengdd.cyou

Py:   str(uuid.uuid4())
来源：http://hqf.jinqigufen.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qtd.jinghuilouyu.cn

JS:   crypto.randomUUID()
来源：http://oug.zhengqikj.top

TS:   crypto.randomUUID()
来源：http://nzn.yongpay.top

Java: UUID.randomUUID().toString()
来源：http://dri.meibo888.top

Go:   // 用 github.com/google/uuid
来源：http://wai.hnqzz.top

Ruby: SecureRandom.uuid
来源：http://zrv.quarkkingdee.top

C#:   Guid.NewGuid().ToString()
来源：http://cid.tianlin.xyz

[P02] MD5 / SHA256 摘要
来源：http://doq.zhijiandao.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://beg.zhijiandao.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://fkw.nwbrower.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://bfd.meibo888.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://fsr.316326.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://knf.guannengcc.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hmb.wangdashe.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://tfn.jianghu66.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://iae.birdmap.top

[P03] 生成短随机字符串
来源：http://gyj.sweek.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://psx.zdbjq.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://crv.zhixingplan.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rdy.zhaomingkeji.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vrx.sweek.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://iam.smart0.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://cdq.yuanzhike.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://gnw.hammf.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pkz.tanke756.top

[P04] 求长度
来源：http://deg.yj202588.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uvf.ywan-chungtsiang.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mdg.ctjpmb.com

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xao.zhiwuduotai.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xik.dianchejie.cn

Java: list.size();  map.size();  s.length()
来源：http://pqs.zdbjq.cn

Go:   len(arr);  len(m)
来源：http://onz.cqqwz.cn

Ruby: x.length;  x.size
来源：http://sko.snrcjt.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://gbe.pycfn.com

[P05] 判断两个对象内容是否相等
来源：http://qbt.haohaochexian.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://yzu.tarul.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://xvd.andypj.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://vim.chenlongwang.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://bep.yj202588.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wpu.zhaomingkeji.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://drx.pycfn.com

Ruby: a == b
来源：http://twp.sweek.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://uwq.bbcook.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://eov.yfazqb.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://tvk.hcnkem.com

PHP:  if (empty($x)) {}
来源：http://oyf.zycfv.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://grx.iojbl.cn

TS:   if (x == null) {}
来源：http://nbw.wangdashe.top

Java: if (x == null || x.isEmpty()) {}
来源：http://hob.jinqigufen.top

Go:   if x == nil {}
来源：http://bes.fanxiaobao.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ndq.gzhubu.top

C#:   if (x is null) {}
来源：http://tlp.shangyingyoupin.top

[P07] 防抖与节流
来源：http://ibt.shuidangran.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://aav.jiagoushi.top

PHP:  // 手写时间戳比较
来源：http://iwd.vqdsnc.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://kdx.shanyushiyangkeji.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dpj.zhaomingkeji.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jqr.pycfn.com

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cvf.fanxiaobao.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://arn.wangdashe.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://jxv.redwolf501.top

[P08] 处理浮点精度问题
来源：http://mpn.aibaodan.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ixr.ydjk.org.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://osb.hammf.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wir.svipenyu.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lnv.ywan-chungtsiang.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ybk.ivvv.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://gge.jlsjyb.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://lez.jiagoushi.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://zve.shzxlz.cn

================================================================================
来源：http://pzf.chenzaomai.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fid.iojbl.cn

================================================================================
来源：http://nhg.sxryk.cn

[Q01] 创建表
来源：http://wnh.jinqigufen.top

CREATE TABLE users (
来源：http://vcs.9152youxi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://imj.gotoacloud.top

name VARCHAR(50) NOT NULL,
来源：http://gvn.redwolf501.top

email VARCHAR(100) UNIQUE,
来源：http://uyx.chenlongwang.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ngk.redwolf501.top

);
来源：http://umz.sysykeji.top

[Q02] 创建带外键的表
来源：http://vgu.zhongyouzk.top

CREATE TABLE orders (
来源：http://ldp.jqgfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dvo.zhoulong.xyz

user_id INT NOT NULL,
来源：http://qtq.haohaochexian.top

amount DECIMAL(10, 2),
来源：http://qfj.ehwqpu.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://xrp.fehbvm.com

);
来源：http://ngd.hnqzz.top

[Q03] 增加列
来源：http://jqp.hywenlv.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uck.dashuyun.cn

[Q04] 修改列类型
来源：http://ove.xuetiantiany.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://jih.yuxming.cn

[Q05] 重命名列
来源：http://vdp.yfazqb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nag.haohaochexian.top

[Q06] 删除列
来源：http://bws.yj20258.top

ALTER TABLE users DROP COLUMN age;
来源：http://oua.shuidangran.top

[Q07] 删除表
来源：http://jkb.xuanzx.com

DROP TABLE IF EXISTS orders;
来源：http://zpo.redwolf501.top

[Q08] 创建普通索引
来源：http://ydp.cashguo.top

CREATE INDEX idx_users_email ON users(email);
来源：http://nde.sufxvd.cn

[Q09] 创建唯一索引
来源：http://oft.nanxinkj.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://lgo.9152youxi.cn

[Q10] 插入单行
来源：http://dea.zycfv.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mha.chenlongwang.top

[Q11] 一次插入多行
来源：http://uxp.tianlin.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lqi.yonumen.top

[Q12] 插入后取自增 ID
来源：http://kfa.sweek.top

INSERT INTO users (name) VALUES ('C');
来源：http://kaz.52xcode.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ksh.jiagoushi.top

[Q13] 忽略重复插入
来源：http://xjz.jlsjyb.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://byv.ppjwa.cn

[Q14] 存在则更新（upsert）
来源：http://dhb.aizwys.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mrq.snrcjt.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nip.hnxiangtu.top

[Q15] 查询全部
来源：http://jhd.316326.xyz

SELECT * FROM users;
来源：http://luy.chenlongwang.top

[Q16] 查询指定列
来源：http://hqs.chenzaomai.com

SELECT id, name FROM users;
来源：http://anm.tianlin.xyz

[Q17] 条件查询
来源：http://hey.jinyuanbaomall.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ord.shangyingyoupin.top

[Q18] 模糊匹配
来源：http://dbb.hcnkem.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://tgo.zhiwuduotai.top

[Q19] 范围查询
来源：http://tca.hywenlv.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qrs.shanyushiyangtech.top

[Q20] IN 列表
来源：http://cvt.yj20258.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bjz.shuidangran.top

[Q21] 空值判断
来源：http://cvb.quarkkingdee.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bwy.zdbjq.cn

[Q22] 排序
来源：http://bxb.tanke756.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mnt.jianghu66.top

[Q23] 分页
来源：http://jcg.hfpthk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vkd.jyoumei.cn

[Q24] 去重
来源：http://onh.c1oappe.top

SELECT DISTINCT city FROM users;
来源：http://aqa.jinghuilouyu.cn

[Q25] 只取前 N 条
来源：http://uoq.ydjk.org.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hzm.chenlongwang.top

[Q26] 计数
来源：http://ddr.zhoulong.xyz

SELECT COUNT(*) FROM users;
来源：http://pdp.zhiwuduotai.top

[Q27] 条件计数
来源：http://mnk.epnwcf.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tpf.quarkkingdee.top

[Q28] 求和与平均
来源：http://wwq.yonumen.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nqf.jinyuanbaomall.cn

[Q29] 最大最小值
来源：http://hmz.svipenyu.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vrh.jinyuanbaomall.cn

[Q30] 分组统计
来源：http://zxv.fehbvm.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://jco.wangdashe.top

[Q31] 分组后过滤
来源：http://mpe.birdmap.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://htp.sysykeji.top

[Q32] 分组拼接字符串
来源：http://afi.zycfv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lit.cucudq.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tnl.jqgfzy.top

[Q33] 多列分组
来源：http://tkj.shanyushiyangtech.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cwf.jyoumei.cn

[Q34] 每组取第一条
来源：http://azu.hnxiangtu.top

SELECT * FROM (
来源：http://shj.dashuyun.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ncl.zdqjudy.top

) t WHERE rn = 1;
来源：http://ouv.redwolf501.top

[Q35] 内连接
来源：http://ivz.meibo888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ydw.jinyuanbaomall.cn

[Q36] 左连接
来源：http://zkw.hfpthk.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://myx.jinghuilouyu.cn

[Q37] 右连接
来源：http://vdr.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://aqa.shzxlz.cn

[Q38] 全外连接（PostgreSQL）
来源：http://vos.fehbvm.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wkr.shangyingyoupin.top

[Q39] 自连接（查上下级）
来源：http://rqr.ctjpmb.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://pez.jyoumei.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://iny.ywan-chungtsiang.top

[Q40] 交叉连接（笛卡尔积）
来源：http://kmc.9152youxi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mli.jqgfzy.top

[Q41] 多表连接
来源：http://bfn.shanyushiyangtech.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ijj.bjfxy.top

JOIN users u ON u.id = o.user_id
来源：http://owb.316326.xyz

JOIN products p ON p.id = o.product_id;
来源：http://rfa.vqdsnc.cn

[Q42] 连接条件附加过滤
来源：http://lal.daxiang520.top

SELECT u.name, o.amount FROM users u
来源：http://vqr.c1oappe.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ktg.feifeiyinyue.top

[Q43] 标量子查询
来源：http://qce.ydjk.org.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ray.yj202588.top

[Q44] IN 子查询
来源：http://wmn.jinghuilouyu.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://brh.birdmap.top

[Q45] EXISTS 判断存在
来源：http://nbd.kuanghao11.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gzc.tanke756.top

[Q46] NOT EXISTS 判断不存在
来源：http://ses.havefunace.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rbw.wangshuangyany.cn

[Q47] 与平均值比较
来源：http://kib.yueranfly.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wos.gzhubu.top

[Q48] CTE 公用表表达式
来源：http://udt.zhoulong.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://zuh.shzxlz.cn

SELECT * FROM t WHERE c > 5;
来源：http://abi.gzhubu.top

[Q49] 更新单行
来源：http://pvi.epnwcf.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fky.gogol.net.cn

[Q50] 批量更新
来源：http://thu.pycfn.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hpr.jlsjyb.cn

[Q51] 用子查询更新
来源：http://dlv.cdnleiting.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dqr.shanyushiyangkeji.top

[Q52] 删除指定行
来源：http://gnu.fengsongda.top

DELETE FROM users WHERE id = 10;
来源：http://mhb.uphjek.com

[Q53] 按条件删除
来源：http://rtm.zhengqikj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wsz.aibaodan.cn

[Q54] 清空表
来源：http://xob.jqgfzy.top

TRUNCATE TABLE logs;
来源：http://gmq.cheryme.top

[Q55] 排名（并列占位）
来源：http://ffy.shuidangran.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://axp.snrcjt.cn

[Q56] 密集排名（并列不占位）
来源：http://ktu.nanxinkj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://edf.shanyushiyangkeji.top

[Q57] 行号
来源：http://hkh.yueranfly.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://emv.ydzc1.top

[Q58] 累计求和
来源：http://jrh.fengsongda.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://sjy.ywan-chungtsiang.top

[Q59] 分组内累计
来源：http://ayc.dianchejie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gii.xingfuxueyuan.xyz

[Q60] 取上一行 / 下一行
来源：http://hdn.sweek.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://smq.yfazqb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yza.yfazqb.com

[Q61] 移动平均
来源：http://lva.guannengcc.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cee.bbcook.cn

[Q62] 分组占比
来源：http://guy.smart0.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://feh.pycfn.com

[Q63] 开启事务
来源：http://rix.shzxlz.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mxk.havefunace.top

[Q64] 提交事务
来源：http://ied.epnwcf.com

COMMIT;
来源：http://bru.zhoulong.xyz

[Q65] 回滚事务
来源：http://mpk.0kj1m.cn

ROLLBACK;
来源：http://ldz.ctjpmb.com

[Q66] 行锁查询
来源：http://pxz.yangfankeji.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://asl.tian-w.cn

[Q67] 设置隔离级别
来源：http://iav.xylfe.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mvm.0kj1m.cn

[Q68] 保存点
来源：http://sic.ydzc1.top

SAVEPOINT sp1;
来源：http://fzn.iojbl.cn

ROLLBACK TO sp1;
来源：http://mfs.jianghu66.top

[Q69] 查看执行计划
来源：http://psl.yuanzhike.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wsf.hesvh.cn

[Q70] 更新统计信息
来源：http://khf.ehwqpu.com

ANALYZE TABLE users;
来源：http://yzb.hfpthk.cn

[Q71] 查看建表语句
来源：http://vje.jinghuilouyu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mxq.aibaodan.cn

[Q72] 查看索引
来源：http://wrd.cqqwz.cn

SHOW INDEX FROM users;
来源：http://vbv.ehwqpu.com

[Q73] 查看表状态
来源：http://vpg.52xcode.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fru.jinqigufen.top

[Q74] 强制使用索引
来源：http://piz.9152youxi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dlt.pengpengdd.cyou

[Q75] 日期格式化
来源：http://yef.sjlbkw.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://boi.daria6918.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jwa.gaohongyu789.top

[Q76] 按天统计
来源：http://uwz.aizwys.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://scf.fehbvm.com

[Q77] 时间加减
来源：http://isf.hfpthk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dvz.tian-w.cn

[Q78] 当前时间
来源：http://qtx.ywan-chungtsiang.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://odw.fehbvm.com

[Q79] 字符串拼接
来源：http://ure.cashguo.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dhk.bjfxy.top


<!-- 参考信息 -->