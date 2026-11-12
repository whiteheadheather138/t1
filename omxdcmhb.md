代发 wailian999

TS:   // worker_threads 线程池
来源：http://erc.yanxiufei.cn

Java: Executors.newFixedThreadPool(4)
来源：http://myb.ybcxt.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vvx.wangdashe.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://txs.cheryme.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://crw.xuetiantiany.cn

[O03] 加锁保护共享数据
来源：http://zmr.ppjwa.cn

Py:   with lock: shared += 1
来源：http://rfz.hammf.cn

PHP:  // 用 flock() 做文件锁
来源：http://igf.pycfn.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://omt.316326.xyz

TS:   // 同 JS
来源：http://kvc.cheryme.top

Java: synchronized (this) { shared++; }
来源：http://jlc.pengpengdd.cyou

Go:   mu.Lock();  defer mu.Unlock()
来源：http://yta.yuanzhike.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ymr.zycfv.cn

C#:   lock (gate) { shared++; }
来源：http://qbu.yanxiufei.cn

[O04] 定义异步函数并等待
来源：http://xfn.shangyingyoupin.top

Py:   async def f():⏎    await g()
来源：http://sch.cheryme.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://hjl.fehbvm.com

JS:   async function f() { await g(); }
来源：http://gzm.shangyingyoupin.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://hua.cheryme.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://snp.iojbl.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://tns.aibaodan.cn

Ruby: # 用 Fiber 或 async gem
来源：http://icz.ehwqpu.com

C#:   async Task F() { await G(); }
来源：http://dxa.yanxiufei.cn

[O05] 并发执行并等待全部完成
来源：http://amv.jinqigufen.top

Py:   asyncio.gather(*tasks)
来源：http://siq.yj202588.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://xvp.andypj.xyz

JS:   await Promise.all(tasks)
来源：http://inf.jinqigufen.top

TS:   await Promise.all(tasks)
来源：http://plz.jqgufenzy.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://brn.zycfv.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://geh.zhoulong.xyz

Ruby: threads.map(&:join)
来源：http://eal.hesvh.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://fhk.zdqjudy.top

[O06] 使用进程池
来源：http://hyc.nanxinkj.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://sgk.cheryme.top

PHP:  // pcntl_fork 或多进程队列
来源：http://nsd.shanyushiyangkeji.top

JS:   // child_process / cluster 模块
来源：http://gqp.ywan-chungtsiang.top

TS:   // child_process / cluster 模块
来源：http://rob.yj202588.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://tul.pycfn.com

Go:   // goroutine 已占用多核，直接并发即可
来源：http://gro.dashuyun.cn

Ruby: // fork 块
来源：http://fns.shanyushiyangkeji.top

C#:   Parallel.For
来源：http://lzk.xziqi.cn

================================================================================
来源：http://ksd.yfazqb.com

P. 常用工具函数
来源：http://nmk.jinqigfzy.top

================================================================================
来源：http://elp.zhijiandao.cn

[P01] 生成 UUID
来源：http://xlm.shanyushiyangkeji.top

Py:   str(uuid.uuid4())
来源：http://fdi.snrcjt.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://oka.quarkkingdee.top

JS:   crypto.randomUUID()
来源：http://zua.cdnleiting.top

TS:   crypto.randomUUID()
来源：http://wrl.jqgufenzy.top

Java: UUID.randomUUID().toString()
来源：http://ipd.vqdsnc.cn

Go:   // 用 github.com/google/uuid
来源：http://jjj.dianchejie.cn

Ruby: SecureRandom.uuid
来源：http://tjr.jlsjyb.cn

C#:   Guid.NewGuid().ToString()
来源：http://xag.nwbrower.top

[P02] MD5 / SHA256 摘要
来源：http://ypt.yuxming.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ulr.dashuyun.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://utc.fktsv.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://prs.fehbvm.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://afm.mhx1999.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://evm.bbcook.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://div.yuxming.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oci.vqdsnc.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cte.sxryk.cn

[P03] 生成短随机字符串
来源：http://jsl.wangshuangyany.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://pdj.guannengcc.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://ogf.yj202588.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dwt.shanyushiyangtech.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vch.ctjpmb.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://acu.feifeiyinyue.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://gts.fehbvm.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://tvn.yangfankeji.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pxm.fengsongda.top

[P04] 求长度
来源：http://owp.ppjwa.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qwg.andypj.xyz

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jac.wangshuangyany.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hkl.kuanghao11.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dqm.xziqi.cn

Java: list.size();  map.size();  s.length()
来源：http://hag.xziqi.cn

Go:   len(arr);  len(m)
来源：http://pco.yueranfly.top

Ruby: x.length;  x.size
来源：http://cwy.xinyue.icu

C#:   list.Count;  dict.Count;  s.Length
来源：http://vsz.xingfuxueyuan.xyz

[P05] 判断两个对象内容是否相等
来源：http://tkd.cucudq.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://skj.hcnkem.com

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cfq.9152youxi.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://whh.jinghuilouyu.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://upp.cucudq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://rce.jiagoushi.top

Go:   reflect.DeepEqual(a, b)
来源：http://rlf.ydjk.org.cn

Ruby: a == b
来源：http://wgl.bjfxy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://qmo.xinyue.icu

[P06] 综合判空（null / 空串 / 空集合）
来源：http://pae.snrcjt.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://bpr.zhongyouzk.top

PHP:  if (empty($x)) {}
来源：http://mah.fzhhl.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://vmw.chenjidiqi.icu

TS:   if (x == null) {}
来源：http://pcu.yonumen.top

Java: if (x == null || x.isEmpty()) {}
来源：http://odo.jinqigfzy.top

Go:   if x == nil {}
来源：http://ezj.yvedp.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jmd.yuanzhike.top

C#:   if (x is null) {}
来源：http://wgg.snrcjt.cn

[P07] 防抖与节流
来源：http://inx.uphjek.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://phm.fzhhl.top

PHP:  // 手写时间戳比较
来源：http://upj.haohaochexian.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ozg.daxiang520.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fsu.uphjek.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://bwm.haohaochexian.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://fpf.wangdashe.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://spp.ywan-chungtsiang.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ldl.yj20258.top

[P08] 处理浮点精度问题
来源：http://ybk.dianchejie.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nau.yongpay.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://nii.xingfuxueyuan.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://jqw.zhongyouzk.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://tcs.gogol.net.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://nku.sweek.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vxx.hongshengwenyu.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ewi.hnqzz.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://pwg.yfazqb.com

================================================================================
来源：http://ato.feifeiyinyue.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hzs.jianghu66.top

================================================================================
来源：http://exf.zhiwuduotai.top

[Q01] 创建表
来源：http://sdu.shanyushiyangtech.top

CREATE TABLE users (
来源：http://vou.xuanzx.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xfy.yj202588.top

name VARCHAR(50) NOT NULL,
来源：http://rla.jiagoushi.top

email VARCHAR(100) UNIQUE,
来源：http://mkj.redwolf501.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://lpo.gaohongyu789.top

);
来源：http://urf.chenzaomai.com

[Q02] 创建带外键的表
来源：http://iqc.jinqigfzy.top

CREATE TABLE orders (
来源：http://xop.sweek.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gse.52xcode.cn

user_id INT NOT NULL,
来源：http://bjq.guowangkeji.top

amount DECIMAL(10, 2),
来源：http://cix.yvedp.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://kct.fktsv.cn

);
来源：http://eml.uphjek.com

[Q03] 增加列
来源：http://jdd.zhongyouzk.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ige.hywenlv.cn

[Q04] 修改列类型
来源：http://erg.52xcode.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://tek.xingfuxueyuan.xyz

[Q05] 重命名列
来源：http://qmb.yj202588.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://nxk.zhaomingkeji.xyz

[Q06] 删除列
来源：http://uga.yvedp.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ybl.ctjpmb.com

[Q07] 删除表
来源：http://wcc.guowangkeji.top

DROP TABLE IF EXISTS orders;
来源：http://vfb.52xcode.cn

[Q08] 创建普通索引
来源：http://qfl.yfazqb.com

CREATE INDEX idx_users_email ON users(email);
来源：http://hdi.smart0.xyz

[Q09] 创建唯一索引
来源：http://fjw.pycfn.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://tjq.shanyushiyangtech.top

[Q10] 插入单行
来源：http://trt.daxiang520.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://tfo.zhaomingkeji.xyz

[Q11] 一次插入多行
来源：http://eza.zhixingplan.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vtb.cqqwz.cn

[Q12] 插入后取自增 ID
来源：http://zrn.tarul.cn

INSERT INTO users (name) VALUES ('C');
来源：http://vcl.sxryk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nfo.andypj.xyz

[Q13] 忽略重复插入
来源：http://tky.shzxlz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hjx.yj20258.top

[Q14] 存在则更新（upsert）
来源：http://vmo.jinqigfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hlg.gaohongyu789.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mdk.hammf.cn

[Q15] 查询全部
来源：http://qwe.0kj1m.cn

SELECT * FROM users;
来源：http://bsa.jqgufenzy.top

[Q16] 查询指定列
来源：http://kih.shangyingyoupin.top

SELECT id, name FROM users;
来源：http://zvk.guowangkeji.top

[Q17] 条件查询
来源：http://kad.fehbvm.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yxq.daria6918.cn

[Q18] 模糊匹配
来源：http://isc.tarul.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nqv.shuidangran.top

[Q19] 范围查询
来源：http://rnj.jinyuanbaomall.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://jdq.aibaodan.cn

[Q20] IN 列表
来源：http://jsn.xuanzx.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tvy.fengsongda.top

[Q21] 空值判断
来源：http://fnf.jinqigfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://iwk.jinqigufen.top

[Q22] 排序
来源：http://zjx.feifeiyinyue.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zvj.hywenlv.cn

[Q23] 分页
来源：http://szd.epnwcf.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://hhj.sysykeji.top

[Q24] 去重
来源：http://mmc.feifeiyinyue.top

SELECT DISTINCT city FROM users;
来源：http://owv.jinqigufen.top

[Q25] 只取前 N 条
来源：http://eyq.yuanzhike.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mdx.aizwys.cn

[Q26] 计数
来源：http://cqz.zdqjudy.top

SELECT COUNT(*) FROM users;
来源：http://fkh.nanxuanxn.top

[Q27] 条件计数
来源：http://rhm.ivvv.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uzd.tanke756.top

[Q28] 求和与平均
来源：http://vvu.jqgfzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ekr.jiagoushi.top

[Q29] 最大最小值
来源：http://hao.ehwqpu.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://moc.zycfv.cn

[Q30] 分组统计
来源：http://wqp.yonumen.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dtt.nanxinkj.top

[Q31] 分组后过滤
来源：http://ftp.gogol.net.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tcm.shzxlz.cn

[Q32] 分组拼接字符串
来源：http://qed.xuetiantiany.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qfd.quarkkingdee.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xpu.jyoumei.cn

[Q33] 多列分组
来源：http://eip.dianchejie.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hoe.tianlin.xyz

[Q34] 每组取第一条
来源：http://pqt.tanke756.top

SELECT * FROM (
来源：http://ifg.tanke756.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://omd.chenzaomai.com

) t WHERE rn = 1;
来源：http://pej.chenjidiqi.icu

[Q35] 内连接
来源：http://lln.jinqigufen.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://spq.nanxinkj.top

[Q36] 左连接
来源：http://omg.daria6918.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hep.zdqjudy.top

[Q37] 右连接
来源：http://tco.jianghu66.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rdb.smart0.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://byr.yj20258.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://prk.jinghuilouyu.cn

[Q39] 自连接（查上下级）
来源：http://cdi.smart0.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://com.shanyushiyangkeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ick.haohaochexian.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qdq.iojbl.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lzx.chenjidiqi.icu

[Q41] 多表连接
来源：http://lqd.jqgufenzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://obs.zhongyouzk.top

JOIN users u ON u.id = o.user_id
来源：http://kix.redwolf501.top

JOIN products p ON p.id = o.product_id;
来源：http://zwg.aizwys.cn

[Q42] 连接条件附加过滤
来源：http://mit.tianlin.xyz

SELECT u.name, o.amount FROM users u
来源：http://app.chenjidiqi.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nja.jyoumei.cn

[Q43] 标量子查询
来源：http://umk.ybcxt.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://raj.tian-w.cn

[Q44] IN 子查询
来源：http://ieb.zdqjudy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cov.ydjk.org.cn

[Q45] EXISTS 判断存在
来源：http://kyo.yongpay.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zed.ybcxt.top

[Q46] NOT EXISTS 判断不存在
来源：http://dnm.jlsjyb.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jlw.fanxiaobao.xyz

[Q47] 与平均值比较
来源：http://keq.jlsjyb.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dtk.yj20258888.top

[Q48] CTE 公用表表达式
来源：http://vhf.ywan-chungtsiang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hwr.bbcook.cn

SELECT * FROM t WHERE c > 5;
来源：http://sln.cqqwz.cn

[Q49] 更新单行
来源：http://pkh.jqgfzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nuq.pycfn.com

[Q50] 批量更新
来源：http://hfn.hesvh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dti.9152youxi.cn

[Q51] 用子查询更新
来源：http://drw.yanxiufei.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kls.yfazqb.com

[Q52] 删除指定行
来源：http://ejn.hnxiangtu.top

DELETE FROM users WHERE id = 10;
来源：http://buz.fzhhl.top

[Q53] 按条件删除
来源：http://wsd.gogol.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mak.yj20258888.top

[Q54] 清空表
来源：http://hyq.nanxuanxn.top

TRUNCATE TABLE logs;
来源：http://glu.hnxiangtu.top

[Q55] 排名（并列占位）
来源：http://ccz.9152youxi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jpy.jinqigufen.top

[Q56] 密集排名（并列不占位）
来源：http://yio.ywan-chungtsiang.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ikf.0kj1m.cn

[Q57] 行号
来源：http://dvp.mhx1999.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://klz.sufxvd.cn

[Q58] 累计求和
来源：http://uzi.svipenyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fwe.ybcxt.top

[Q59] 分组内累计
来源：http://alc.zdqjudy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jdx.redwolf501.top

[Q60] 取上一行 / 下一行
来源：http://fss.sxryk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wuf.yonumen.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qhh.birdmap.top

[Q61] 移动平均
来源：http://nrm.yangfankeji.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jnf.zhiwuduotai.top

[Q62] 分组占比
来源：http://ibf.xylfe.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jed.jinghuilouyu.cn

[Q63] 开启事务
来源：http://aki.cdnleiting.top

START TRANSACTION;                -- 或 BEGIN
来源：http://aad.ydjk.org.cn

[Q64] 提交事务
来源：http://bdw.xziqi.cn

COMMIT;
来源：http://xli.wangdashe.top

[Q65] 回滚事务
来源：http://bkz.c1oappe.top

ROLLBACK;
来源：http://yvg.gaohongyu789.top

[Q66] 行锁查询
来源：http://xzh.andypj.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eqr.cdnleiting.top

[Q67] 设置隔离级别
来源：http://oyd.jqgfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jzh.pycfn.com

[Q68] 保存点
来源：http://fso.ctjpmb.com

SAVEPOINT sp1;
来源：http://ich.sxryk.cn

ROLLBACK TO sp1;
来源：http://xmt.yj202588.top

[Q69] 查看执行计划
来源：http://hnj.xuanzx.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cwb.hcnkem.com

[Q70] 更新统计信息
来源：http://kdh.jqgfzy.top

ANALYZE TABLE users;
来源：http://xuj.zycfv.cn

[Q71] 查看建表语句
来源：http://lup.hammf.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ecd.redwolf501.top

[Q72] 查看索引
来源：http://yim.redwolf501.top

SHOW INDEX FROM users;
来源：http://yue.snrcjt.cn

[Q73] 查看表状态
来源：http://jkm.gogol.net.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kke.hnqzz.top

[Q74] 强制使用索引
来源：http://bmf.zdbjq.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xbq.sxryk.cn

[Q75] 日期格式化
来源：http://ctb.aizwys.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jrd.gogol.net.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sri.sjlbkw.cn

[Q76] 按天统计
来源：http://wil.shzxlz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hpl.yueranfly.top

[Q77] 时间加减
来源：http://zuh.hnqzz.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lhb.yanxiufei.cn

[Q78] 当前时间
来源：http://gtd.yj202588.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tfv.ybcxt.top

[Q79] 字符串拼接
来源：http://nnq.zhengqikj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mfr.sufxvd.cn


<!-- 参考信息 -->