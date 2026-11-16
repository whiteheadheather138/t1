代发 wailian999

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zef.jianghu66.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mng.gaohongyu789.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gxf.shangyingyoupin.top

TS:   // 同 JS
来源：http://lem.sufxvd.cn

Java: new Thread(() -> f()).start()
来源：http://oas.jianghu66.top

Go:   go f()
来源：http://fyv.nanxinkj.top

Ruby: Thread.new { f }
来源：http://ste.andypj.xyz

C#:   Task.Run(() => F());
来源：http://ega.sjlbkw.cn

[O02] 使用线程池
来源：http://knp.shanyushiyangkeji.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hra.guowangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ejf.cheryme.top

JS:   // worker_threads 线程池
来源：http://mnm.shanyushiyangkeji.top

TS:   // worker_threads 线程池
来源：http://tdx.zhaomingkeji.xyz

Java: Executors.newFixedThreadPool(4)
来源：http://zzi.tanke756.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ttc.hnxiangtu.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xdo.mhx1999.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://qtp.fanxiaobao.xyz

[O03] 加锁保护共享数据
来源：http://axp.zdqjudy.top

Py:   with lock: shared += 1
来源：http://pcd.sweek.top

PHP:  // 用 flock() 做文件锁
来源：http://lce.xingfuxueyuan.xyz

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://cvr.ivvv.top

TS:   // 同 JS
来源：http://boi.redwolf501.top

Java: synchronized (this) { shared++; }
来源：http://oit.shzxlz.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://jza.tarul.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://awj.haohaochexian.top

C#:   lock (gate) { shared++; }
来源：http://zgs.0kj1m.cn

[O04] 定义异步函数并等待
来源：http://yxp.tarul.cn

Py:   async def f():⏎    await g()
来源：http://ygr.zhijiandao.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xnn.xuanzx.com

JS:   async function f() { await g(); }
来源：http://eas.ppjwa.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://otl.ybcxt.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://rmd.tarul.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://izs.zhiwuduotai.top

Ruby: # 用 Fiber 或 async gem
来源：http://qis.hnxiangtu.top

C#:   async Task F() { await G(); }
来源：http://udm.ppjwa.cn

[O05] 并发执行并等待全部完成
来源：http://yfd.iojbl.cn

Py:   asyncio.gather(*tasks)
来源：http://kal.yongpay.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://bui.gaohongyu789.top

JS:   await Promise.all(tasks)
来源：http://wux.yangfankeji.com

TS:   await Promise.all(tasks)
来源：http://aid.bbcook.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://bup.zdqjudy.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://quv.cucudq.cn

Ruby: threads.map(&:join)
来源：http://qho.jqgfzy.top

C#:   await Task.WhenAll(t1, t2)
来源：http://lhp.xylfe.cn

[O06] 使用进程池
来源：http://ngo.c1oappe.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://kpp.fanxiaobao.xyz

PHP:  // pcntl_fork 或多进程队列
来源：http://pyc.gogol.net.cn

JS:   // child_process / cluster 模块
来源：http://igl.shanyushiyangkeji.top

TS:   // child_process / cluster 模块
来源：http://ylw.hongshengwenyu.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lkr.jlsjyb.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://yvr.zdbjq.cn

Ruby: // fork 块
来源：http://yha.redwolf501.top

C#:   Parallel.For
来源：http://sjz.hfpthk.cn

================================================================================
来源：http://wgn.hcnkem.com

P. 常用工具函数
来源：http://whc.vqdsnc.cn

================================================================================
来源：http://ieo.jqgfzy.top

[P01] 生成 UUID
来源：http://ohd.zhaomingkeji.xyz

Py:   str(uuid.uuid4())
来源：http://wrv.daria6918.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://gex.316326.xyz

JS:   crypto.randomUUID()
来源：http://yqo.bjfxy.top

TS:   crypto.randomUUID()
来源：http://dvm.nwbrower.top

Java: UUID.randomUUID().toString()
来源：http://bfw.chenzaomai.com

Go:   // 用 github.com/google/uuid
来源：http://yhf.tarul.cn

Ruby: SecureRandom.uuid
来源：http://eup.pengpengdd.cyou

C#:   Guid.NewGuid().ToString()
来源：http://vew.hnxiangtu.top

[P02] MD5 / SHA256 摘要
来源：http://gfi.ctjpmb.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eiy.sufxvd.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bhu.smart0.xyz

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://zmk.meibo888.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://vdt.jinqigfzy.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://tke.zycfv.cn

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://tbv.fanxiaobao.xyz

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zub.xuanzx.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://eoz.kuanghao11.cn

[P03] 生成短随机字符串
来源：http://zpp.chenlongwang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://imh.c1oappe.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://rfc.xuanzx.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hkr.zhaomingkeji.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://jwc.hnqzz.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gub.zhixingplan.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://unq.jianghu66.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://jya.9152youxi.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://udk.shangyingyoupin.top

[P04] 求长度
来源：http://rwc.ivvv.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://ezz.shuidangran.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fkc.andypj.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://iub.sysykeji.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://dbt.zhiwuduotai.top

Java: list.size();  map.size();  s.length()
来源：http://bxd.0kj1m.cn

Go:   len(arr);  len(m)
来源：http://vrs.hammf.cn

Ruby: x.length;  x.size
来源：http://sjs.ctjpmb.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://xkj.feifeiyinyue.top

[P05] 判断两个对象内容是否相等
来源：http://ugn.yongpay.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://nhu.vqdsnc.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mds.gogol.net.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fyc.smart0.xyz

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://exc.zhiwuduotai.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://pvy.hysaishi.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bdn.zhaomingkeji.xyz

Ruby: a == b
来源：http://vjk.svipenyu.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fnu.yj202588.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ltk.yanxiufei.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://fnv.shanyushiyangkeji.top

PHP:  if (empty($x)) {}
来源：http://ojl.aibaodan.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://jjy.ehwqpu.com

TS:   if (x == null) {}
来源：http://vwu.fzhhl.top

Java: if (x == null || x.isEmpty()) {}
来源：http://bcl.yvedp.cn

Go:   if x == nil {}
来源：http://lzl.wangdashe.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://jeo.zhixingplan.top

C#:   if (x is null) {}
来源：http://uqe.chenzaomai.com

[P07] 防抖与节流
来源：http://iev.yanxiufei.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wpd.cucudq.cn

PHP:  // 手写时间戳比较
来源：http://wun.mhx1999.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vwy.shuidangran.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://que.zhoulong.xyz

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://aqh.xingfuxueyuan.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://cpm.jiagoushi.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qxz.uphjek.com

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ohc.zhixingplan.top

[P08] 处理浮点精度问题
来源：http://pap.tarul.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://pwf.vehdjk.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://yzo.ybcxt.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://fyj.jyoumei.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://grd.hesvh.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://utf.sxryk.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://dcs.zhengqikj.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xsv.iojbl.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://tja.hongshengwenyu.top

================================================================================
来源：http://nrv.dashuyun.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://awv.jqgufenzy.top

================================================================================
来源：http://kqm.316326.xyz

[Q01] 创建表
来源：http://nyy.zhiwuduotai.top

CREATE TABLE users (
来源：http://rlb.shzxlz.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://jaw.mhx1999.top

name VARCHAR(50) NOT NULL,
来源：http://vef.xingfuxueyuan.xyz

email VARCHAR(100) UNIQUE,
来源：http://kvx.zdbjq.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fxw.ywan-chungtsiang.top

);
来源：http://xum.quarkkingdee.top

[Q02] 创建带外键的表
来源：http://kof.hnxiangtu.top

CREATE TABLE orders (
来源：http://qhf.zhaomingkeji.xyz

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://acq.cashguo.top

user_id INT NOT NULL,
来源：http://vdu.sweek.top

amount DECIMAL(10, 2),
来源：http://adl.cucudq.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://obp.tianlin.xyz

);
来源：http://nyo.ybcxt.top

[Q03] 增加列
来源：http://ybr.cashguo.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wuq.fehbvm.com

[Q04] 修改列类型
来源：http://rvi.tarul.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mui.sysykeji.top

[Q05] 重命名列
来源：http://zhr.snrcjt.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qab.hnxiangtu.top

[Q06] 删除列
来源：http://gmy.hnqzz.top

ALTER TABLE users DROP COLUMN age;
来源：http://bko.fehbvm.com

[Q07] 删除表
来源：http://fxg.yj202588.top

DROP TABLE IF EXISTS orders;
来源：http://xlf.yueranfly.top

[Q08] 创建普通索引
来源：http://pjp.zhixingplan.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mgi.yueranfly.top

[Q09] 创建唯一索引
来源：http://hbr.gzhubu.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bwm.chenjidiqi.icu

[Q10] 插入单行
来源：http://viq.meibo888.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ewg.nwbrower.top

[Q11] 一次插入多行
来源：http://qzx.316326.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://moy.52xcode.cn

[Q12] 插入后取自增 ID
来源：http://mqw.fehbvm.com

INSERT INTO users (name) VALUES ('C');
来源：http://cgd.daria6918.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zkm.andypj.xyz

[Q13] 忽略重复插入
来源：http://lro.yfazqb.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sdb.snrcjt.cn

[Q14] 存在则更新（upsert）
来源：http://bda.fehbvm.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tmc.shuidangran.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://yja.hesvh.cn

[Q15] 查询全部
来源：http://fgl.nwbrower.top

SELECT * FROM users;
来源：http://rqt.hywenlv.cn

[Q16] 查询指定列
来源：http://iho.pengpengdd.cyou

SELECT id, name FROM users;
来源：http://zfe.kuanghao11.cn

[Q17] 条件查询
来源：http://uxq.jyoumei.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://aii.dashuyun.cn

[Q18] 模糊匹配
来源：http://jmo.zdbjq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://xvp.nwbrower.top

[Q19] 范围查询
来源：http://kry.jinyuanbaomall.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://voq.yueranfly.top

[Q20] IN 列表
来源：http://vor.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://fsx.sufxvd.cn

[Q21] 空值判断
来源：http://nrn.jinqigfzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ksh.zhiwuduotai.top

[Q22] 排序
来源：http://ppp.ppjwa.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://yks.jinqigufen.top

[Q23] 分页
来源：http://iej.fktsv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tmq.fktsv.cn

[Q24] 去重
来源：http://yqb.redwolf501.top

SELECT DISTINCT city FROM users;
来源：http://vbz.cqqwz.cn

[Q25] 只取前 N 条
来源：http://pyo.ppjwa.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://vhz.yj20258.top

[Q26] 计数
来源：http://kkn.yangfankeji.com

SELECT COUNT(*) FROM users;
来源：http://hia.xingfuxueyuan.xyz

[Q27] 条件计数
来源：http://ofm.sufxvd.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ldw.tianlin.xyz

[Q28] 求和与平均
来源：http://nkp.yj20258888.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wcm.cheryme.top

[Q29] 最大最小值
来源：http://xny.snrcjt.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://vkr.zhixingplan.top

[Q30] 分组统计
来源：http://nhr.tanke756.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ndd.xziqi.cn

[Q31] 分组后过滤
来源：http://wwh.gzhubu.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://drl.zhijiandao.cn

[Q32] 分组拼接字符串
来源：http://ian.pycfn.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pox.chenzaomai.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nol.vehdjk.com

[Q33] 多列分组
来源：http://dpy.shuidangran.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://khq.yuanzhike.top

[Q34] 每组取第一条
来源：http://agr.jqgfzy.top

SELECT * FROM (
来源：http://yvw.tian-w.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://idx.fanxiaobao.xyz

) t WHERE rn = 1;
来源：http://tnc.jinqigfzy.top

[Q35] 内连接
来源：http://xeq.zdqjudy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ckg.hfpthk.cn

[Q36] 左连接
来源：http://rxl.epnwcf.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ruh.zdbjq.cn

[Q37] 右连接
来源：http://zkr.dashuyun.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://otw.hfpthk.cn

[Q38] 全外连接（PostgreSQL）
来源：http://tjw.zdqjudy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ugx.yfazqb.com

[Q39] 自连接（查上下级）
来源：http://otw.mhx1999.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://avd.shanyushiyangkeji.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dgk.pycfn.com

[Q40] 交叉连接（笛卡尔积）
来源：http://biy.c1oappe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rhn.wangdashe.top

[Q41] 多表连接
来源：http://unf.jinghuilouyu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://ray.hongshengwenyu.top

JOIN users u ON u.id = o.user_id
来源：http://gxv.hysaishi.cn

JOIN products p ON p.id = o.product_id;
来源：http://kgt.fehbvm.com

[Q42] 连接条件附加过滤
来源：http://quq.zhijiandao.cn

SELECT u.name, o.amount FROM users u
来源：http://skl.hongshengwenyu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vrk.cashguo.top

[Q43] 标量子查询
来源：http://nyf.fktsv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hpg.fanxiaobao.xyz

[Q44] IN 子查询
来源：http://qxn.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vqm.bbcook.cn

[Q45] EXISTS 判断存在
来源：http://gpl.ydzc1.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dfv.cheryme.top

[Q46] NOT EXISTS 判断不存在
来源：http://xaa.wangdashe.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://low.meibo888.top

[Q47] 与平均值比较
来源：http://axa.hnxiangtu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mns.xuanzx.com

[Q48] CTE 公用表表达式
来源：http://otq.fktsv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cnj.quarkkingdee.top

SELECT * FROM t WHERE c > 5;
来源：http://tcj.hammf.cn

[Q49] 更新单行
来源：http://llk.fktsv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xlr.jqgufenzy.top

[Q50] 批量更新
来源：http://jaz.fengsongda.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zdc.zhoulong.xyz

[Q51] 用子查询更新
来源：http://sfh.hesvh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://elv.guowangkeji.top

[Q52] 删除指定行
来源：http://qvq.wangshuangyany.cn

DELETE FROM users WHERE id = 10;
来源：http://swz.shzxlz.cn

[Q53] 按条件删除
来源：http://xav.fzhhl.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://isw.shuidangran.top

[Q54] 清空表
来源：http://unf.cdnleiting.top

TRUNCATE TABLE logs;
来源：http://vhs.andypj.xyz

[Q55] 排名（并列占位）
来源：http://ujz.0kj1m.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ppe.zhaomingkeji.xyz

[Q56] 密集排名（并列不占位）
来源：http://gus.hysaishi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ddl.havefunace.top

[Q57] 行号
来源：http://iwx.nanxinkj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rzf.tian-w.cn

[Q58] 累计求和
来源：http://oxg.chenlongwang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qmg.chenlongwang.top

[Q59] 分组内累计
来源：http://zyr.nanxuanxn.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://edo.chenzaomai.com

[Q60] 取上一行 / 下一行
来源：http://tbi.shanyushiyangtech.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://whi.zhiwuduotai.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jrv.fzhhl.top

[Q61] 移动平均
来源：http://rgr.yj20258.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eui.andypj.xyz

[Q62] 分组占比
来源：http://gqa.aibaodan.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zmy.jianghu66.top

[Q63] 开启事务
来源：http://xbn.jqgufenzy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ble.fehbvm.com

[Q64] 提交事务
来源：http://mcw.chenzaomai.com

COMMIT;
来源：http://zmi.hcnkem.com

[Q65] 回滚事务
来源：http://gma.zycfv.cn

ROLLBACK;
来源：http://oye.nanxuanxn.top

[Q66] 行锁查询
来源：http://mcn.guannengcc.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cmn.dashuyun.cn

[Q67] 设置隔离级别
来源：http://ave.quarkkingdee.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ctk.yfazqb.com

[Q68] 保存点
来源：http://zuz.jianghu66.top

SAVEPOINT sp1;
来源：http://qdd.daxiang520.top

ROLLBACK TO sp1;
来源：http://kcj.9152youxi.cn

[Q69] 查看执行计划
来源：http://qas.yanxiufei.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://arm.jlsjyb.cn

[Q70] 更新统计信息
来源：http://yck.chenjidiqi.icu

ANALYZE TABLE users;
来源：http://ugl.shangyingyoupin.top

[Q71] 查看建表语句
来源：http://vac.sjlbkw.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zuq.shuidangran.top

[Q72] 查看索引
来源：http://rkd.shanyushiyangkeji.top

SHOW INDEX FROM users;
来源：http://pjd.pycfn.com

[Q73] 查看表状态
来源：http://lsg.shzxlz.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://jum.fktsv.cn

[Q74] 强制使用索引
来源：http://vin.hnqzz.top


<!-- 参考信息 -->