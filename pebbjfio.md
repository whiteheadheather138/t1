代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://xyh.ybcxt.top

Go:   go f()
来源：http://ulq.snrcjt.cn

Ruby: Thread.new { f }
来源：http://laj.fehbvm.com

C#:   Task.Run(() => F());
来源：http://cph.yanxiufei.cn

[O02] 使用线程池
来源：http://kme.xuetiantiany.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mcc.bbcook.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://qpj.jianghu66.top

JS:   // worker_threads 线程池
来源：http://gdl.dianchejie.cn

TS:   // worker_threads 线程池
来源：http://ehj.zdqjudy.top

Java: Executors.newFixedThreadPool(4)
来源：http://ryj.daxiang520.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://vvx.tarul.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://weh.zdbjq.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://ocn.guowangkeji.top

[O03] 加锁保护共享数据
来源：http://nsg.9152youxi.cn

Py:   with lock: shared += 1
来源：http://eut.cucudq.cn

PHP:  // 用 flock() 做文件锁
来源：http://bkg.tian-w.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://pbs.feifeiyinyue.top

TS:   // 同 JS
来源：http://mia.yj20258.top

Java: synchronized (this) { shared++; }
来源：http://cmx.shangyingyoupin.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://hby.zhongyouzk.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://uzi.cdnleiting.top

C#:   lock (gate) { shared++; }
来源：http://tlr.guannengcc.top

[O04] 定义异步函数并等待
来源：http://jmt.gogol.net.cn

Py:   async def f():⏎    await g()
来源：http://gty.jlsjyb.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://rsa.ydzc1.top

JS:   async function f() { await g(); }
来源：http://zej.zycfv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://hva.uphjek.com

Java: // 用 CompletableFuture 或虚拟线程
来源：http://fjm.xziqi.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xza.zhiwuduotai.top

Ruby: # 用 Fiber 或 async gem
来源：http://sfy.ctjpmb.com

C#:   async Task F() { await G(); }
来源：http://kdi.yueranfly.top

[O05] 并发执行并等待全部完成
来源：http://wor.xinyue.icu

Py:   asyncio.gather(*tasks)
来源：http://hzl.andypj.xyz

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dyj.hesvh.cn

JS:   await Promise.all(tasks)
来源：http://hox.ywan-chungtsiang.top

TS:   await Promise.all(tasks)
来源：http://xrf.zhaomingkeji.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zgc.xylfe.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://snb.jqgufenzy.top

Ruby: threads.map(&:join)
来源：http://ega.cqqwz.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://yjd.jianghu66.top

[O06] 使用进程池
来源：http://hsz.hesvh.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fpf.chenlongwang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://rdl.zycfv.cn

JS:   // child_process / cluster 模块
来源：http://lpt.xylfe.cn

TS:   // child_process / cluster 模块
来源：http://zhc.zhiwuduotai.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cjs.sxryk.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://dgq.jlsjyb.cn

Ruby: // fork 块
来源：http://srg.feifeiyinyue.top

C#:   Parallel.For
来源：http://dgq.zhiwuduotai.top

================================================================================
来源：http://ena.havefunace.top

P. 常用工具函数
来源：http://azy.nwbrower.top

================================================================================
来源：http://jvi.xziqi.cn

[P01] 生成 UUID
来源：http://ncl.52xcode.cn

Py:   str(uuid.uuid4())
来源：http://idg.sufxvd.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://ums.zycfv.cn

JS:   crypto.randomUUID()
来源：http://yfh.gogol.net.cn

TS:   crypto.randomUUID()
来源：http://rvx.mhx1999.top

Java: UUID.randomUUID().toString()
来源：http://yon.tarul.cn

Go:   // 用 github.com/google/uuid
来源：http://fna.ppjwa.cn

Ruby: SecureRandom.uuid
来源：http://mwa.ivvv.top

C#:   Guid.NewGuid().ToString()
来源：http://akn.zhiwuduotai.top

[P02] MD5 / SHA256 摘要
来源：http://ylm.tanke756.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://fve.dashuyun.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://xcw.shanyushiyangtech.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://trm.wangshuangyany.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://len.zdqjudy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://irr.svipenyu.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tsr.xuetiantiany.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://obd.nwbrower.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ouf.tanke756.top

[P03] 生成短随机字符串
来源：http://wio.yonumen.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://nty.nwbrower.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://shw.sysykeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hqz.ywan-chungtsiang.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://oeb.yuanzhike.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://vdl.jianghu66.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://vgw.yuanzhike.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://dyn.9152youxi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://bjs.cqqwz.cn

[P04] 求长度
来源：http://bfh.hnxiangtu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://zuk.nwbrower.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://grr.ybcxt.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zcz.ywan-chungtsiang.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ems.kuanghao11.cn

Java: list.size();  map.size();  s.length()
来源：http://ige.guannengcc.top

Go:   len(arr);  len(m)
来源：http://srf.ctjpmb.com

Ruby: x.length;  x.size
来源：http://apz.cqqwz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://uuz.xuetiantiany.cn

[P05] 判断两个对象内容是否相等
来源：http://jch.jiagoushi.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://vwi.tarul.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://oau.gogol.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wog.redwolf501.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xjx.yj202588.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://icc.316326.xyz

Go:   reflect.DeepEqual(a, b)
来源：http://lhg.tian-w.cn

Ruby: a == b
来源：http://mgm.cucudq.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://xts.jinghuilouyu.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://fuz.bjfxy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://hpq.fzhhl.top

PHP:  if (empty($x)) {}
来源：http://lgf.zhixingplan.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://rtb.chenzaomai.com

TS:   if (x == null) {}
来源：http://otc.andypj.xyz

Java: if (x == null || x.isEmpty()) {}
来源：http://bng.sweek.top

Go:   if x == nil {}
来源：http://kjq.c1oappe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hrh.jinqigufen.top

C#:   if (x is null) {}
来源：http://jwb.cashguo.top

[P07] 防抖与节流
来源：http://amp.shzxlz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://jgu.fanxiaobao.xyz

PHP:  // 手写时间戳比较
来源：http://hkm.pycfn.com

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://yak.dianchejie.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://njc.svipenyu.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qwd.yueranfly.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://npc.cashguo.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://byu.redwolf501.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://xst.316326.xyz

[P08] 处理浮点精度问题
来源：http://sxv.havefunace.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://kea.daxiang520.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ybh.andypj.xyz

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://oee.hnxiangtu.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://qbs.fehbvm.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://vkl.cdnleiting.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hhi.tian-w.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zya.jianghu66.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mnd.jlsjyb.cn

================================================================================
来源：http://ymb.smart0.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wkh.cqqwz.cn

================================================================================
来源：http://ogk.yanxiufei.cn

[Q01] 创建表
来源：http://lti.sxryk.cn

CREATE TABLE users (
来源：http://bsv.hfpthk.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bvp.iojbl.cn

name VARCHAR(50) NOT NULL,
来源：http://izz.yueranfly.top

email VARCHAR(100) UNIQUE,
来源：http://jrd.ppjwa.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://shy.kuanghao11.cn

);
来源：http://jct.chenjidiqi.icu

[Q02] 创建带外键的表
来源：http://zcf.gogol.net.cn

CREATE TABLE orders (
来源：http://frj.zhixingplan.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dpr.yj20258888.top

user_id INT NOT NULL,
来源：http://jfn.fanxiaobao.xyz

amount DECIMAL(10, 2),
来源：http://dme.chenjidiqi.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://imn.pengpengdd.cyou

);
来源：http://feg.guowangkeji.top

[Q03] 增加列
来源：http://pvm.hnqzz.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jfa.cqqwz.cn

[Q04] 修改列类型
来源：http://cnu.hongshengwenyu.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://var.uphjek.com

[Q05] 重命名列
来源：http://pqy.yj20258.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dcw.shanyushiyangtech.top

[Q06] 删除列
来源：http://qxc.shanyushiyangkeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://mwu.havefunace.top

[Q07] 删除表
来源：http://yov.chenlongwang.top

DROP TABLE IF EXISTS orders;
来源：http://tcq.nanxuanxn.top

[Q08] 创建普通索引
来源：http://nkh.jinghuilouyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://zgt.jianghu66.top

[Q09] 创建唯一索引
来源：http://cpa.hnqzz.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jfn.xylfe.cn

[Q10] 插入单行
来源：http://nyq.jinqigufen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ltm.yj202588.top

[Q11] 一次插入多行
来源：http://sop.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ict.jinqigfzy.top

[Q12] 插入后取自增 ID
来源：http://crd.jinyuanbaomall.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ddb.wangshuangyany.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dcz.wangshuangyany.cn

[Q13] 忽略重复插入
来源：http://kub.zycfv.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://qvn.jqgufenzy.top

[Q14] 存在则更新（upsert）
来源：http://cxr.xuanzx.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xhb.guannengcc.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bcd.vehdjk.com

[Q15] 查询全部
来源：http://hxa.jqgufenzy.top

SELECT * FROM users;
来源：http://tfk.ydzc1.top

[Q16] 查询指定列
来源：http://hsw.uphjek.com

SELECT id, name FROM users;
来源：http://rkb.hcnkem.com

[Q17] 条件查询
来源：http://tfv.uphjek.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://gba.9152youxi.cn

[Q18] 模糊匹配
来源：http://yei.hysaishi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yfs.cqqwz.cn

[Q19] 范围查询
来源：http://dtc.jyoumei.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zag.quarkkingdee.top

[Q20] IN 列表
来源：http://jmr.nanxuanxn.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xot.andypj.xyz

[Q21] 空值判断
来源：http://kbx.sxryk.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kiq.shzxlz.cn

[Q22] 排序
来源：http://sss.tian-w.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://teg.zdqjudy.top

[Q23] 分页
来源：http://ygi.shanyushiyangtech.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gkw.shanyushiyangtech.top

[Q24] 去重
来源：http://ggh.wangdashe.top

SELECT DISTINCT city FROM users;
来源：http://miy.zhijiandao.cn

[Q25] 只取前 N 条
来源：http://mcb.sysykeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zjo.shanyushiyangtech.top

[Q26] 计数
来源：http://pxh.sysykeji.top

SELECT COUNT(*) FROM users;
来源：http://gyq.mhx1999.top

[Q27] 条件计数
来源：http://hws.sjlbkw.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://myb.xingfuxueyuan.xyz

[Q28] 求和与平均
来源：http://uwp.epnwcf.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://uxw.wangshuangyany.cn

[Q29] 最大最小值
来源：http://kln.yj20258.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jxy.zdbjq.cn

[Q30] 分组统计
来源：http://pop.ydzc1.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hjh.sjlbkw.cn

[Q31] 分组后过滤
来源：http://jua.jqgfzy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://aim.wangdashe.top

[Q32] 分组拼接字符串
来源：http://zwi.c1oappe.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://hsl.nanxuanxn.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://icw.quarkkingdee.top

[Q33] 多列分组
来源：http://slo.ehwqpu.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mux.sjlbkw.cn

[Q34] 每组取第一条
来源：http://sqp.wangshuangyany.cn

SELECT * FROM (
来源：http://zrc.chenjidiqi.icu

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xjx.yangfankeji.com

) t WHERE rn = 1;
来源：http://tsa.jinqigfzy.top

[Q35] 内连接
来源：http://yeg.nanxuanxn.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dwo.shzxlz.cn

[Q36] 左连接
来源：http://ury.shanyushiyangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tda.nanxuanxn.top

[Q37] 右连接
来源：http://jzv.ctjpmb.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xlq.gotoacloud.top

[Q38] 全外连接（PostgreSQL）
来源：http://zno.tian-w.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uri.hnqzz.top

[Q39] 自连接（查上下级）
来源：http://wkv.jyoumei.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://dpp.zhijiandao.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ymw.epnwcf.com

[Q40] 交叉连接（笛卡尔积）
来源：http://cdw.jinqigufen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://gzy.jqgfzy.top

[Q41] 多表连接
来源：http://wuw.jqgfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://kse.quarkkingdee.top

JOIN users u ON u.id = o.user_id
来源：http://ghg.feifeiyinyue.top

JOIN products p ON p.id = o.product_id;
来源：http://psk.ywan-chungtsiang.top

[Q42] 连接条件附加过滤
来源：http://ogg.yvedp.cn

SELECT u.name, o.amount FROM users u
来源：http://jxh.feifeiyinyue.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gsh.jqgfzy.top

[Q43] 标量子查询
来源：http://eui.shuidangran.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wgl.tian-w.cn

[Q44] IN 子查询
来源：http://yci.ybcxt.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cww.svipenyu.cn

[Q45] EXISTS 判断存在
来源：http://nmf.shuidangran.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eqq.guowangkeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://eqa.9152youxi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://sgh.hesvh.cn

[Q47] 与平均值比较
来源：http://yzd.vqdsnc.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hay.havefunace.top

[Q48] CTE 公用表表达式
来源：http://coi.hfpthk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fuc.cqqwz.cn

SELECT * FROM t WHERE c > 5;
来源：http://pen.kuanghao11.cn

[Q49] 更新单行
来源：http://jyo.shzxlz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://klq.ctjpmb.com

[Q50] 批量更新
来源：http://itt.zhengqikj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mqv.jianghu66.top

[Q51] 用子查询更新
来源：http://cjo.hammf.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ayd.ivvv.top

[Q52] 删除指定行
来源：http://mmq.epnwcf.com

DELETE FROM users WHERE id = 10;
来源：http://bsb.fktsv.cn

[Q53] 按条件删除
来源：http://cpg.shanyushiyangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rui.shanyushiyangkeji.top

[Q54] 清空表
来源：http://myq.yanxiufei.cn

TRUNCATE TABLE logs;
来源：http://bxr.vqdsnc.cn

[Q55] 排名（并列占位）
来源：http://fab.nanxuanxn.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jag.guowangkeji.top

[Q56] 密集排名（并列不占位）
来源：http://chg.yonumen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kue.xziqi.cn

[Q57] 行号
来源：http://pfz.birdmap.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cei.aibaodan.cn

[Q58] 累计求和
来源：http://zwe.nwbrower.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vsl.yj20258.top

[Q59] 分组内累计
来源：http://ltq.jinyuanbaomall.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ago.sxryk.cn

[Q60] 取上一行 / 下一行
来源：http://nmj.hysaishi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kqq.snrcjt.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sej.nanxinkj.top

[Q61] 移动平均
来源：http://asi.fzhhl.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ksb.sufxvd.cn

[Q62] 分组占比
来源：http://lgo.zhaomingkeji.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zbm.shanyushiyangkeji.top

[Q63] 开启事务
来源：http://hkl.hammf.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lek.andypj.xyz

[Q64] 提交事务
来源：http://dvd.zdqjudy.top

COMMIT;
来源：http://qck.sysykeji.top

[Q65] 回滚事务
来源：http://kmx.shuidangran.top

ROLLBACK;
来源：http://vol.mhx1999.top

[Q66] 行锁查询
来源：http://wov.hnxiangtu.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hdc.cdnleiting.top

[Q67] 设置隔离级别
来源：http://mcr.dashuyun.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://alt.nanxuanxn.top

[Q68] 保存点
来源：http://tdn.pengpengdd.cyou

SAVEPOINT sp1;
来源：http://qld.guannengcc.top

ROLLBACK TO sp1;
来源：http://czb.shanyushiyangkeji.top

[Q69] 查看执行计划
来源：http://ecr.52xcode.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eiy.c1oappe.top

[Q70] 更新统计信息
来源：http://vof.jqgufenzy.top

ANALYZE TABLE users;
来源：http://xdj.yj20258.top

[Q71] 查看建表语句
来源：http://tpl.cqqwz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://suv.yonumen.top

[Q72] 查看索引
来源：http://mov.mhx1999.top

SHOW INDEX FROM users;
来源：http://gji.cashguo.top

[Q73] 查看表状态
来源：http://xrh.yueranfly.top

SHOW TABLE STATUS LIKE 'users';
来源：http://uhj.nwbrower.top

[Q74] 强制使用索引
来源：http://tzp.gaohongyu789.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lbs.0kj1m.cn

[Q75] 日期格式化
来源：http://gue.ydjk.org.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qvp.c1oappe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kth.epnwcf.com


<!-- 参考信息 -->