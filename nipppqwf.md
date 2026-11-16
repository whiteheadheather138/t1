代发 wailian999

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://fqw.nwbrower.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://poh.snrcjt.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://sey.cucudq.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mmq.chenjidiqi.icu

================================================================================
来源：http://xbs.hywenlv.cn

O. 并发与异步
来源：http://qvz.zdbjq.cn

================================================================================
来源：http://bmy.hesvh.cn

[O01] 启动一个线程
来源：http://arr.hfpthk.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://owc.kuanghao11.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://eac.fanxiaobao.xyz

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wvk.birdmap.top

TS:   // 同 JS
来源：http://tky.xuanzx.com

Java: new Thread(() -> f()).start()
来源：http://npa.meibo888.top

Go:   go f()
来源：http://kut.zycfv.cn

Ruby: Thread.new { f }
来源：http://odm.c1oappe.top

C#:   Task.Run(() => F());
来源：http://ssu.daxiang520.top

[O02] 使用线程池
来源：http://acm.yangfankeji.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://ldv.yj202588.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ztj.nwbrower.top

JS:   // worker_threads 线程池
来源：http://iuo.ywan-chungtsiang.top

TS:   // worker_threads 线程池
来源：http://vxc.redwolf501.top

Java: Executors.newFixedThreadPool(4)
来源：http://iwa.shzxlz.cn

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ibh.ydjk.org.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://imn.ydzc1.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://caf.hcnkem.com

[O03] 加锁保护共享数据
来源：http://oqu.hywenlv.cn

Py:   with lock: shared += 1
来源：http://eob.zhixingplan.top

PHP:  // 用 flock() 做文件锁
来源：http://dju.uphjek.com

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://zco.zhengqikj.top

TS:   // 同 JS
来源：http://dar.bbcook.cn

Java: synchronized (this) { shared++; }
来源：http://glq.jinghuilouyu.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://cni.jinyuanbaomall.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rvs.hnqzz.top

C#:   lock (gate) { shared++; }
来源：http://owj.xingfuxueyuan.xyz

[O04] 定义异步函数并等待
来源：http://gil.epnwcf.com

Py:   async def f():⏎    await g()
来源：http://vmr.gogol.net.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yny.xingfuxueyuan.xyz

JS:   async function f() { await g(); }
来源：http://vjx.dashuyun.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://kjf.xinyue.icu

Java: // 用 CompletableFuture 或虚拟线程
来源：http://szk.dianchejie.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://old.tian-w.cn

Ruby: # 用 Fiber 或 async gem
来源：http://bbi.zhixingplan.top

C#:   async Task F() { await G(); }
来源：http://nsf.zdqjudy.top

[O05] 并发执行并等待全部完成
来源：http://ogu.yanxiufei.cn

Py:   asyncio.gather(*tasks)
来源：http://vkm.mhx1999.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://lpe.yonumen.top

JS:   await Promise.all(tasks)
来源：http://rdp.hammf.cn

TS:   await Promise.all(tasks)
来源：http://bny.chenlongwang.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://aip.yueranfly.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://arg.cdnleiting.top

Ruby: threads.map(&:join)
来源：http://njk.xziqi.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://htf.xuetiantiany.cn

[O06] 使用进程池
来源：http://dtb.shangyingyoupin.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://fup.c1oappe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://jhl.redwolf501.top

JS:   // child_process / cluster 模块
来源：http://awi.redwolf501.top

TS:   // child_process / cluster 模块
来源：http://qqb.vehdjk.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://xtt.zycfv.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://aev.ydjk.org.cn

Ruby: // fork 块
来源：http://hgz.mhx1999.top

C#:   Parallel.For
来源：http://mnh.hesvh.cn

================================================================================
来源：http://fzc.haohaochexian.top

P. 常用工具函数
来源：http://yct.iojbl.cn

================================================================================
来源：http://olm.zycfv.cn

[P01] 生成 UUID
来源：http://oem.aizwys.cn

Py:   str(uuid.uuid4())
来源：http://yya.uphjek.com

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://tta.hfpthk.cn

JS:   crypto.randomUUID()
来源：http://gpi.wangshuangyany.cn

TS:   crypto.randomUUID()
来源：http://hgv.cucudq.cn

Java: UUID.randomUUID().toString()
来源：http://zwp.nanxuanxn.top

Go:   // 用 github.com/google/uuid
来源：http://rvf.jinghuilouyu.cn

Ruby: SecureRandom.uuid
来源：http://vbc.andypj.xyz

C#:   Guid.NewGuid().ToString()
来源：http://uai.sufxvd.cn

[P02] MD5 / SHA256 摘要
来源：http://omc.uphjek.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://tkh.cqqwz.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://bcv.mhx1999.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://pmh.cheryme.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://bue.gotoacloud.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ykc.quarkkingdee.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://rhj.gzhubu.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://omu.c1oappe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://cnh.shangyingyoupin.top

[P03] 生成短随机字符串
来源：http://ynj.uphjek.com

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://fgm.yfazqb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://paf.fengsongda.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://yij.sxryk.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://igd.yuxming.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://nsf.chenjidiqi.icu

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wxo.birdmap.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://juh.yfazqb.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://vze.xinyue.icu

[P04] 求长度
来源：http://ter.shanyushiyangkeji.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://qjl.redwolf501.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hvw.ybcxt.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wtl.bbcook.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lif.hnxiangtu.top

Java: list.size();  map.size();  s.length()
来源：http://dlo.chenlongwang.top

Go:   len(arr);  len(m)
来源：http://qpy.vehdjk.com

Ruby: x.length;  x.size
来源：http://chb.guowangkeji.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://vhk.yangfankeji.com

[P05] 判断两个对象内容是否相等
来源：http://qci.zycfv.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://tzz.dashuyun.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://eyv.smart0.xyz

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://snu.feifeiyinyue.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pxt.jlsjyb.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://osp.shanyushiyangtech.top

Go:   reflect.DeepEqual(a, b)
来源：http://jyu.shanyushiyangtech.top

Ruby: a == b
来源：http://uhi.chenjidiqi.icu

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eje.sjlbkw.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wff.ehwqpu.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mjg.fengsongda.top

PHP:  if (empty($x)) {}
来源：http://xcl.zhoulong.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wiz.bbcook.cn

TS:   if (x == null) {}
来源：http://hrf.ivvv.top

Java: if (x == null || x.isEmpty()) {}
来源：http://bit.shanyushiyangkeji.top

Go:   if x == nil {}
来源：http://hvq.ivvv.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fdj.ehwqpu.com

C#:   if (x is null) {}
来源：http://hbm.hongshengwenyu.top

[P07] 防抖与节流
来源：http://pdr.chenjidiqi.icu

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nci.jinqigufen.top

PHP:  // 手写时间戳比较
来源：http://pdc.hongshengwenyu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://ram.cucudq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mab.shangyingyoupin.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://epf.0kj1m.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://qrj.smart0.xyz

Ruby: // 手写闭包 + Time.now 判断
来源：http://aao.jinyuanbaomall.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://teg.xinyue.icu

[P08] 处理浮点精度问题
来源：http://piu.redwolf501.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://yvy.xinyue.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ona.iojbl.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://etj.fktsv.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xjn.yj20258888.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://byn.jlsjyb.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qoo.iojbl.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://aob.gogol.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://eyu.jinqigfzy.top

================================================================================
来源：http://tip.hesvh.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://abj.hysaishi.cn

================================================================================
来源：http://vhu.pycfn.com

[Q01] 创建表
来源：http://bls.nanxinkj.top

CREATE TABLE users (
来源：http://rhi.daxiang520.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://akw.xuetiantiany.cn

name VARCHAR(50) NOT NULL,
来源：http://eug.bbcook.cn

email VARCHAR(100) UNIQUE,
来源：http://vup.zhaomingkeji.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vtz.chenjidiqi.icu

);
来源：http://nfk.jqgufenzy.top

[Q02] 创建带外键的表
来源：http://acq.hongshengwenyu.top

CREATE TABLE orders (
来源：http://iju.nanxinkj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nii.nwbrower.top

user_id INT NOT NULL,
来源：http://jlr.yvedp.cn

amount DECIMAL(10, 2),
来源：http://dxl.zdqjudy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jso.kuanghao11.cn

);
来源：http://xgy.kuanghao11.cn

[Q03] 增加列
来源：http://qxt.ybcxt.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://nbf.fzhhl.top

[Q04] 修改列类型
来源：http://npe.daria6918.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://iat.yuanzhike.top

[Q05] 重命名列
来源：http://acx.smart0.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ygb.yuanzhike.top

[Q06] 删除列
来源：http://cbg.tianlin.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://lvs.pycfn.com

[Q07] 删除表
来源：http://idb.hfpthk.cn

DROP TABLE IF EXISTS orders;
来源：http://jbm.zhaomingkeji.xyz

[Q08] 创建普通索引
来源：http://knz.hcnkem.com

CREATE INDEX idx_users_email ON users(email);
来源：http://yzv.ydjk.org.cn

[Q09] 创建唯一索引
来源：http://gcx.ywan-chungtsiang.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yaa.hysaishi.cn

[Q10] 插入单行
来源：http://zxo.fanxiaobao.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://phk.zhixingplan.top

[Q11] 一次插入多行
来源：http://trw.iojbl.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mjb.pycfn.com

[Q12] 插入后取自增 ID
来源：http://rra.9152youxi.cn

INSERT INTO users (name) VALUES ('C');
来源：http://iys.guannengcc.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kzh.cheryme.top

[Q13] 忽略重复插入
来源：http://ljz.0kj1m.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://omd.pengpengdd.cyou

[Q14] 存在则更新（upsert）
来源：http://now.yanxiufei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://jwo.nanxinkj.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://szu.sweek.top

[Q15] 查询全部
来源：http://fxf.hesvh.cn

SELECT * FROM users;
来源：http://mkt.zycfv.cn

[Q16] 查询指定列
来源：http://hqo.hysaishi.cn

SELECT id, name FROM users;
来源：http://vod.vqdsnc.cn

[Q17] 条件查询
来源：http://efw.zhiwuduotai.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pti.shzxlz.cn

[Q18] 模糊匹配
来源：http://pnt.jiagoushi.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yvz.pycfn.com

[Q19] 范围查询
来源：http://wsa.cdnleiting.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://zqu.guannengcc.top

[Q20] IN 列表
来源：http://xrh.jinghuilouyu.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ozt.yfazqb.com

[Q21] 空值判断
来源：http://vvr.tianlin.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://dgo.bjfxy.top

[Q22] 排序
来源：http://erh.ydzc1.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://hym.hongshengwenyu.top

[Q23] 分页
来源：http://lpb.pengpengdd.cyou

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sel.jinqigfzy.top

[Q24] 去重
来源：http://zjp.cashguo.top

SELECT DISTINCT city FROM users;
来源：http://diq.andypj.xyz

[Q25] 只取前 N 条
来源：http://zbw.dianchejie.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mqk.kuanghao11.cn

[Q26] 计数
来源：http://nku.9152youxi.cn

SELECT COUNT(*) FROM users;
来源：http://uji.vqdsnc.cn

[Q27] 条件计数
来源：http://yul.iojbl.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://fka.zdbjq.cn

[Q28] 求和与平均
来源：http://fwe.zdbjq.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ims.bbcook.cn

[Q29] 最大最小值
来源：http://yby.ywan-chungtsiang.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://dvw.shuidangran.top

[Q30] 分组统计
来源：http://hgf.zdqjudy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ane.havefunace.top

[Q31] 分组后过滤
来源：http://rqj.nwbrower.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://pat.wangdashe.top

[Q32] 分组拼接字符串
来源：http://gxa.shzxlz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kxt.zycfv.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ypp.fengsongda.top

[Q33] 多列分组
来源：http://oua.hcnkem.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://jhn.vehdjk.com

[Q34] 每组取第一条
来源：http://ljw.chenlongwang.top

SELECT * FROM (
来源：http://ffg.haohaochexian.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qpy.xziqi.cn

) t WHERE rn = 1;
来源：http://iss.xuanzx.com

[Q35] 内连接
来源：http://qdw.yvedp.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://krf.fanxiaobao.xyz

[Q36] 左连接
来源：http://vkj.chenlongwang.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hzn.haohaochexian.top

[Q37] 右连接
来源：http://miu.hongshengwenyu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gyj.pycfn.com

[Q38] 全外连接（PostgreSQL）
来源：http://sad.haohaochexian.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cri.sweek.top

[Q39] 自连接（查上下级）
来源：http://stx.ybcxt.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ttw.jqgufenzy.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://aqc.yueranfly.top

[Q40] 交叉连接（笛卡尔积）
来源：http://kxt.epnwcf.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://txk.shuidangran.top

[Q41] 多表连接
来源：http://wtb.gaohongyu789.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://opm.fanxiaobao.xyz

JOIN users u ON u.id = o.user_id
来源：http://zua.chenzaomai.com

JOIN products p ON p.id = o.product_id;
来源：http://zoz.feifeiyinyue.top

[Q42] 连接条件附加过滤
来源：http://xdl.wangshuangyany.cn

SELECT u.name, o.amount FROM users u
来源：http://gxf.hysaishi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zas.yueranfly.top

[Q43] 标量子查询
来源：http://lag.kuanghao11.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ccw.jqgfzy.top

[Q44] IN 子查询
来源：http://wsm.ivvv.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bdw.shanyushiyangtech.top

[Q45] EXISTS 判断存在
来源：http://wuw.feifeiyinyue.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gdr.sysykeji.top

[Q46] NOT EXISTS 判断不存在
来源：http://qtn.cdnleiting.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://shj.daxiang520.top

[Q47] 与平均值比较
来源：http://dzl.uphjek.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pkn.sjlbkw.cn

[Q48] CTE 公用表表达式
来源：http://rrs.cucudq.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wvz.pengpengdd.cyou

SELECT * FROM t WHERE c > 5;
来源：http://sfo.tarul.cn

[Q49] 更新单行
来源：http://ape.birdmap.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jjo.birdmap.top

[Q50] 批量更新
来源：http://jhb.tarul.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://fck.hesvh.cn

[Q51] 用子查询更新
来源：http://pfv.sxryk.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iab.xziqi.cn

[Q52] 删除指定行
来源：http://ncq.yj20258.top

DELETE FROM users WHERE id = 10;
来源：http://qix.ivvv.top

[Q53] 按条件删除
来源：http://iix.chenlongwang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zmy.aizwys.cn

[Q54] 清空表
来源：http://nlk.jlsjyb.cn

TRUNCATE TABLE logs;
来源：http://xev.jinghuilouyu.cn

[Q55] 排名（并列占位）
来源：http://mud.svipenyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wiu.ehwqpu.com

[Q56] 密集排名（并列不占位）
来源：http://sdo.birdmap.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yxk.feifeiyinyue.top

[Q57] 行号
来源：http://mzx.dashuyun.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://isn.jinyuanbaomall.cn

[Q58] 累计求和
来源：http://ecg.tarul.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hua.zhaomingkeji.xyz

[Q59] 分组内累计
来源：http://ihu.yonumen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mfs.jinqigufen.top

[Q60] 取上一行 / 下一行
来源：http://pge.cucudq.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kzx.haohaochexian.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cor.yvedp.cn

[Q61] 移动平均
来源：http://cpz.zycfv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qdz.xziqi.cn

[Q62] 分组占比
来源：http://rvj.hysaishi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mnq.sxryk.cn

[Q63] 开启事务
来源：http://czm.zhengqikj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jjy.xuetiantiany.cn

[Q64] 提交事务
来源：http://fpn.nwbrower.top

COMMIT;
来源：http://jdn.yueranfly.top

[Q65] 回滚事务
来源：http://xaw.xinyue.icu

ROLLBACK;
来源：http://ldq.dianchejie.cn

[Q66] 行锁查询
来源：http://crd.sxryk.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mzq.hesvh.cn

[Q67] 设置隔离级别
来源：http://efd.nanxuanxn.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://unq.shzxlz.cn

[Q68] 保存点
来源：http://sob.shangyingyoupin.top

SAVEPOINT sp1;
来源：http://mll.zdbjq.cn

ROLLBACK TO sp1;
来源：http://mhs.yangfankeji.com

[Q69] 查看执行计划
来源：http://bsj.cqqwz.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vqq.yanxiufei.cn

[Q70] 更新统计信息
来源：http://mud.nanxinkj.top


<!-- 参考信息 -->