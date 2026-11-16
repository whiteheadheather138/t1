代发 wailian999

TS:   // worker_threads 线程池
来源：http://wgc.shanyushiyangtech.top

Java: Executors.newFixedThreadPool(4)
来源：http://hxc.hesvh.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://igb.iojbl.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gpy.hnqzz.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://knm.hnxiangtu.top

[O03] 加锁保护共享数据
来源：http://qvf.svipenyu.cn

Py:   with lock: shared += 1
来源：http://ing.zycfv.cn

PHP:  // 用 flock() 做文件锁
来源：http://kaf.nanxinkj.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zrw.ywan-chungtsiang.top

TS:   // 同 JS
来源：http://sli.dashuyun.cn

Java: synchronized (this) { shared++; }
来源：http://bwh.iojbl.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fxz.guannengcc.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://pkf.jinyuanbaomall.cn

C#:   lock (gate) { shared++; }
来源：http://bvi.meibo888.top

[O04] 定义异步函数并等待
来源：http://hrt.wangdashe.top

Py:   async def f():⏎    await g()
来源：http://xqw.fengsongda.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://vqt.kuanghao11.cn

JS:   async function f() { await g(); }
来源：http://tuq.ywan-chungtsiang.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://uog.iojbl.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://ogf.jyoumei.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://gtn.9152youxi.cn

Ruby: # 用 Fiber 或 async gem
来源：http://hii.svipenyu.cn

C#:   async Task F() { await G(); }
来源：http://nza.yfazqb.com

[O05] 并发执行并等待全部完成
来源：http://ipw.guannengcc.top

Py:   asyncio.gather(*tasks)
来源：http://syg.hammf.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://nlm.zhiwuduotai.top

JS:   await Promise.all(tasks)
来源：http://qvp.quarkkingdee.top

TS:   await Promise.all(tasks)
来源：http://okf.hysaishi.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://jwo.guowangkeji.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zsb.jinqigfzy.top

Ruby: threads.map(&:join)
来源：http://fet.sxryk.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://emy.yanxiufei.cn

[O06] 使用进程池
来源：http://mmb.zdqjudy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://qad.gaohongyu789.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qhk.shanyushiyangkeji.top

JS:   // child_process / cluster 模块
来源：http://pef.yanxiufei.cn

TS:   // child_process / cluster 模块
来源：http://zbo.guowangkeji.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://kri.aizwys.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://cma.jyoumei.cn

Ruby: // fork 块
来源：http://fna.haohaochexian.top

C#:   Parallel.For
来源：http://mij.c1oappe.top

================================================================================
来源：http://hkq.ybcxt.top

P. 常用工具函数
来源：http://pan.yanxiufei.cn

================================================================================
来源：http://wrf.jianghu66.top

[P01] 生成 UUID
来源：http://lrb.fengsongda.top

Py:   str(uuid.uuid4())
来源：http://vdq.yangfankeji.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vjk.yuanzhike.top

JS:   crypto.randomUUID()
来源：http://lph.xuetiantiany.cn

TS:   crypto.randomUUID()
来源：http://fqk.zhijiandao.cn

Java: UUID.randomUUID().toString()
来源：http://pad.andypj.xyz

Go:   // 用 github.com/google/uuid
来源：http://suq.quarkkingdee.top

Ruby: SecureRandom.uuid
来源：http://kse.ywan-chungtsiang.top

C#:   Guid.NewGuid().ToString()
来源：http://hgq.yj20258888.top

[P02] MD5 / SHA256 摘要
来源：http://zla.zdqjudy.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vpr.dashuyun.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bxy.vehdjk.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zhp.redwolf501.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://oha.shangyingyoupin.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://flp.jianghu66.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://yct.jinyuanbaomall.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://fao.epnwcf.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://gjr.52xcode.cn

[P03] 生成短随机字符串
来源：http://jeo.fanxiaobao.xyz

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fpl.hammf.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qwk.chenjidiqi.icu

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://tdx.tian-w.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bsh.316326.xyz

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://uao.ydzc1.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://heq.zhongyouzk.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://sai.vehdjk.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://dyv.cashguo.top

[P04] 求长度
来源：http://twl.bjfxy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://arn.feifeiyinyue.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wcr.xingfuxueyuan.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://scz.hfpthk.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hvs.aibaodan.cn

Java: list.size();  map.size();  s.length()
来源：http://zia.cashguo.top

Go:   len(arr);  len(m)
来源：http://jgg.ctjpmb.com

Ruby: x.length;  x.size
来源：http://fls.tanke756.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://nwk.hongshengwenyu.top

[P05] 判断两个对象内容是否相等
来源：http://goc.hesvh.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://oal.jinghuilouyu.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://twa.chenlongwang.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://dsb.jyoumei.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://lcm.yj20258888.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wrr.ybcxt.top

Go:   reflect.DeepEqual(a, b)
来源：http://lyv.dashuyun.cn

Ruby: a == b
来源：http://nig.ehwqpu.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://iar.shuidangran.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rgz.nanxuanxn.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://sxd.jiagoushi.top

PHP:  if (empty($x)) {}
来源：http://ddd.shanyushiyangtech.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://fap.redwolf501.top

TS:   if (x == null) {}
来源：http://vlm.jyoumei.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://bgq.redwolf501.top

Go:   if x == nil {}
来源：http://wra.gaohongyu789.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://ajg.hywenlv.cn

C#:   if (x is null) {}
来源：http://ndf.hysaishi.cn

[P07] 防抖与节流
来源：http://chq.52xcode.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://age.dashuyun.cn

PHP:  // 手写时间戳比较
来源：http://opd.yonumen.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://eqd.vqdsnc.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://iir.shangyingyoupin.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://jez.sufxvd.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vvh.zhaomingkeji.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://wkr.ybcxt.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ggq.yfazqb.com

[P08] 处理浮点精度问题
来源：http://mvu.chenzaomai.com

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://hzp.birdmap.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://enm.xylfe.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://lse.birdmap.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://luo.fanxiaobao.xyz

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://peq.jinqigfzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://rnd.ivvv.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://gnc.aizwys.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://njc.pengpengdd.cyou

================================================================================
来源：http://zhs.hysaishi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hxk.316326.xyz

================================================================================
来源：http://cis.shzxlz.cn

[Q01] 创建表
来源：http://mmd.guannengcc.top

CREATE TABLE users (
来源：http://jyr.jyoumei.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jjl.shanyushiyangkeji.top

name VARCHAR(50) NOT NULL,
来源：http://cpf.yueranfly.top

email VARCHAR(100) UNIQUE,
来源：http://qrg.chenzaomai.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ddj.cdnleiting.top

);
来源：http://agd.zycfv.cn

[Q02] 创建带外键的表
来源：http://fyj.jiagoushi.top

CREATE TABLE orders (
来源：http://xzi.aizwys.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://rte.ivvv.top

user_id INT NOT NULL,
来源：http://zrl.yongpay.top

amount DECIMAL(10, 2),
来源：http://ygi.yj20258888.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://diq.yfazqb.com

);
来源：http://xte.meibo888.top

[Q03] 增加列
来源：http://rzy.gotoacloud.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vdn.hysaishi.cn

[Q04] 修改列类型
来源：http://kgi.sweek.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bam.gogol.net.cn

[Q05] 重命名列
来源：http://xdz.xuanzx.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xls.iojbl.cn

[Q06] 删除列
来源：http://bkr.bbcook.cn

ALTER TABLE users DROP COLUMN age;
来源：http://atj.hnqzz.top

[Q07] 删除表
来源：http://knt.ybcxt.top

DROP TABLE IF EXISTS orders;
来源：http://get.ywan-chungtsiang.top

[Q08] 创建普通索引
来源：http://mus.yongpay.top

CREATE INDEX idx_users_email ON users(email);
来源：http://ifl.bjfxy.top

[Q09] 创建唯一索引
来源：http://qax.chenlongwang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mer.wangshuangyany.cn

[Q10] 插入单行
来源：http://ugr.sweek.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qnz.c1oappe.top

[Q11] 一次插入多行
来源：http://rsh.ydzc1.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vdm.hcnkem.com

[Q12] 插入后取自增 ID
来源：http://plt.dashuyun.cn

INSERT INTO users (name) VALUES ('C');
来源：http://qwk.aizwys.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fnr.redwolf501.top

[Q13] 忽略重复插入
来源：http://zee.gogol.net.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://csh.tanke756.top

[Q14] 存在则更新（upsert）
来源：http://ppn.fengsongda.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oao.shuidangran.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xny.yfazqb.com

[Q15] 查询全部
来源：http://uva.jinqigufen.top

SELECT * FROM users;
来源：http://dnc.zdqjudy.top

[Q16] 查询指定列
来源：http://xut.dashuyun.cn

SELECT id, name FROM users;
来源：http://zfi.zhengqikj.top

[Q17] 条件查询
来源：http://ksc.wangdashe.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ted.xingfuxueyuan.xyz

[Q18] 模糊匹配
来源：http://ctq.ydzc1.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hfi.bjfxy.top

[Q19] 范围查询
来源：http://zpb.9152youxi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fgo.vqdsnc.cn

[Q20] IN 列表
来源：http://ztd.xuetiantiany.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://reb.xingfuxueyuan.xyz

[Q21] 空值判断
来源：http://bud.yvedp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bmg.redwolf501.top

[Q22] 排序
来源：http://jgq.zhengqikj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cqd.uphjek.com

[Q23] 分页
来源：http://hrx.redwolf501.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zhy.sufxvd.cn

[Q24] 去重
来源：http://qxn.chenlongwang.top

SELECT DISTINCT city FROM users;
来源：http://dee.yuanzhike.top

[Q25] 只取前 N 条
来源：http://nze.zhoulong.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://aon.zhijiandao.cn

[Q26] 计数
来源：http://dem.shuidangran.top

SELECT COUNT(*) FROM users;
来源：http://xwo.yvedp.cn

[Q27] 条件计数
来源：http://ams.9152youxi.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bqw.zhoulong.xyz

[Q28] 求和与平均
来源：http://vet.316326.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sgk.zhixingplan.top

[Q29] 最大最小值
来源：http://qwc.fehbvm.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://crj.birdmap.top

[Q30] 分组统计
来源：http://svt.ivvv.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uzd.yj202588.top

[Q31] 分组后过滤
来源：http://gax.yuanzhike.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uas.jinghuilouyu.cn

[Q32] 分组拼接字符串
来源：http://srn.ivvv.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dmx.zycfv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://udl.shanyushiyangkeji.top

[Q33] 多列分组
来源：http://vcb.bbcook.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://grh.0kj1m.cn

[Q34] 每组取第一条
来源：http://bwu.sjlbkw.cn

SELECT * FROM (
来源：http://zsl.iojbl.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ive.tanke756.top

) t WHERE rn = 1;
来源：http://yrp.316326.xyz

[Q35] 内连接
来源：http://fid.epnwcf.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gpc.guowangkeji.top

[Q36] 左连接
来源：http://kyo.tian-w.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://auz.fktsv.cn

[Q37] 右连接
来源：http://qxm.ppjwa.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pcx.zhiwuduotai.top

[Q38] 全外连接（PostgreSQL）
来源：http://ivk.316326.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bij.quarkkingdee.top

[Q39] 自连接（查上下级）
来源：http://cll.ehwqpu.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://egw.sjlbkw.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ssu.vehdjk.com

[Q40] 交叉连接（笛卡尔积）
来源：http://wrh.yfazqb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://apo.dianchejie.cn

[Q41] 多表连接
来源：http://kfz.zhixingplan.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://sss.tanke756.top

JOIN users u ON u.id = o.user_id
来源：http://pyn.yvedp.cn

JOIN products p ON p.id = o.product_id;
来源：http://hvg.meibo888.top

[Q42] 连接条件附加过滤
来源：http://gru.zhijiandao.cn

SELECT u.name, o.amount FROM users u
来源：http://cks.feifeiyinyue.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://nzd.ctjpmb.com

[Q43] 标量子查询
来源：http://nnv.tianlin.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://sji.guowangkeji.top

[Q44] IN 子查询
来源：http://gad.hesvh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pls.yuxming.cn

[Q45] EXISTS 判断存在
来源：http://wkr.sjlbkw.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uew.hnxiangtu.top

[Q46] NOT EXISTS 判断不存在
来源：http://hgk.hfpthk.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mwu.gzhubu.top

[Q47] 与平均值比较
来源：http://bwe.9152youxi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cgk.epnwcf.com

[Q48] CTE 公用表表达式
来源：http://omg.snrcjt.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://urr.52xcode.cn

SELECT * FROM t WHERE c > 5;
来源：http://wcj.feifeiyinyue.top

[Q49] 更新单行
来源：http://alq.zdbjq.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jwb.shanyushiyangtech.top

[Q50] 批量更新
来源：http://ijc.wangshuangyany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pyd.cucudq.cn

[Q51] 用子查询更新
来源：http://sla.dianchejie.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xaz.meibo888.top

[Q52] 删除指定行
来源：http://ses.feifeiyinyue.top

DELETE FROM users WHERE id = 10;
来源：http://kft.ybcxt.top

[Q53] 按条件删除
来源：http://qwd.nanxinkj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ibe.fzhhl.top

[Q54] 清空表
来源：http://rpy.yanxiufei.cn

TRUNCATE TABLE logs;
来源：http://pvn.zhiwuduotai.top

[Q55] 排名（并列占位）
来源：http://qwe.gaohongyu789.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://byx.guannengcc.top

[Q56] 密集排名（并列不占位）
来源：http://faz.ehwqpu.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bke.sjlbkw.cn

[Q57] 行号
来源：http://hmd.birdmap.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mda.xylfe.cn

[Q58] 累计求和
来源：http://kmo.sysykeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mhb.sjlbkw.cn

[Q59] 分组内累计
来源：http://rjo.ppjwa.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xsb.mhx1999.top

[Q60] 取上一行 / 下一行
来源：http://fcs.zhixingplan.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://flp.ydzc1.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jnz.kuanghao11.cn

[Q61] 移动平均
来源：http://lbj.bjfxy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vtz.gzhubu.top

[Q62] 分组占比
来源：http://okk.bjfxy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qlr.kuanghao11.cn

[Q63] 开启事务
来源：http://hjp.316326.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://zeh.shanyushiyangkeji.top

[Q64] 提交事务
来源：http://etu.gzhubu.top

COMMIT;
来源：http://rtu.jinqigfzy.top

[Q65] 回滚事务
来源：http://cuz.hnxiangtu.top

ROLLBACK;
来源：http://fvv.jqgfzy.top

[Q66] 行锁查询
来源：http://zzp.hnxiangtu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iyh.fktsv.cn

[Q67] 设置隔离级别
来源：http://rpz.tianlin.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://edf.wangdashe.top

[Q68] 保存点
来源：http://wnv.52xcode.cn

SAVEPOINT sp1;
来源：http://exl.jinqigfzy.top

ROLLBACK TO sp1;
来源：http://ffs.pengpengdd.cyou

[Q69] 查看执行计划
来源：http://tgf.daria6918.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zio.havefunace.top

[Q70] 更新统计信息
来源：http://ydp.mhx1999.top

ANALYZE TABLE users;
来源：http://scw.hnqzz.top

[Q71] 查看建表语句
来源：http://ecu.jinqigufen.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sta.mhx1999.top

[Q72] 查看索引
来源：http://fde.yonumen.top

SHOW INDEX FROM users;
来源：http://bzf.jinghuilouyu.cn

[Q73] 查看表状态
来源：http://jkv.andypj.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://byz.fzhhl.top

[Q74] 强制使用索引
来源：http://syu.hfpthk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vsb.meibo888.top

[Q75] 日期格式化
来源：http://lgm.zhiwuduotai.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sls.cdnleiting.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bsj.xinyue.icu

[Q76] 按天统计
来源：http://krk.yangfankeji.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cvz.haohaochexian.top

[Q77] 时间加减
来源：http://fdd.yueranfly.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ljf.uphjek.com

[Q78] 当前时间
来源：http://hln.zhijiandao.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nis.zdqjudy.top

[Q79] 字符串拼接
来源：http://abr.zhengqikj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xru.jinyuanbaomall.cn


<!-- 参考信息 -->