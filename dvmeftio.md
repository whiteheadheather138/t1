代发 wailian999

================================================================================
来源：http://nmm.sxryk.cn

O. 并发与异步
来源：http://nnf.xuanzx.com

================================================================================
来源：http://duw.guannengcc.top

[O01] 启动一个线程
来源：http://nej.gaohongyu789.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aiq.quarkkingdee.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mal.shanyushiyangtech.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lqf.hysaishi.cn

TS:   // 同 JS
来源：http://qis.snrcjt.cn

Java: new Thread(() -> f()).start()
来源：http://fst.nanxuanxn.top

Go:   go f()
来源：http://wib.bbcook.cn

Ruby: Thread.new { f }
来源：http://rpu.ehwqpu.com

C#:   Task.Run(() => F());
来源：http://bxt.hcnkem.com

[O02] 使用线程池
来源：http://zbu.yvedp.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zxe.aizwys.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://ldb.xylfe.cn

JS:   // worker_threads 线程池
来源：http://bnz.yj20258888.top

TS:   // worker_threads 线程池
来源：http://jhj.zdbjq.cn

Java: Executors.newFixedThreadPool(4)
来源：http://xqs.ybcxt.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://coz.hnqzz.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://gas.feifeiyinyue.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hco.yj20258888.top

[O03] 加锁保护共享数据
来源：http://eyl.hywenlv.cn

Py:   with lock: shared += 1
来源：http://bxo.sweek.top

PHP:  // 用 flock() 做文件锁
来源：http://szn.daxiang520.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://dvl.ivvv.top

TS:   // 同 JS
来源：http://sqh.kuanghao11.cn

Java: synchronized (this) { shared++; }
来源：http://rjd.zhaomingkeji.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://urw.fzhhl.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://zap.xinyue.icu

C#:   lock (gate) { shared++; }
来源：http://zmf.ivvv.top

[O04] 定义异步函数并等待
来源：http://ybm.nanxuanxn.top

Py:   async def f():⏎    await g()
来源：http://ykc.zhoulong.xyz

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://xmp.gotoacloud.top

JS:   async function f() { await g(); }
来源：http://bmu.yuxming.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://vpv.sysykeji.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://hrr.quarkkingdee.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://czx.sufxvd.cn

Ruby: # 用 Fiber 或 async gem
来源：http://oyg.yj20258.top

C#:   async Task F() { await G(); }
来源：http://zsh.yuanzhike.top

[O05] 并发执行并等待全部完成
来源：http://otr.tianlin.xyz

Py:   asyncio.gather(*tasks)
来源：http://rns.gotoacloud.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://tjf.xziqi.cn

JS:   await Promise.all(tasks)
来源：http://juf.xziqi.cn

TS:   await Promise.all(tasks)
来源：http://gdr.haohaochexian.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ptv.wangdashe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://ohr.havefunace.top

Ruby: threads.map(&:join)
来源：http://qux.quarkkingdee.top

C#:   await Task.WhenAll(t1, t2)
来源：http://khq.jqgufenzy.top

[O06] 使用进程池
来源：http://wwp.fktsv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://cux.gzhubu.top

PHP:  // pcntl_fork 或多进程队列
来源：http://cjk.ydzc1.top

JS:   // child_process / cluster 模块
来源：http://dvz.aibaodan.cn

TS:   // child_process / cluster 模块
来源：http://gmu.fktsv.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wzj.xingfuxueyuan.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://aih.iojbl.cn

Ruby: // fork 块
来源：http://cpa.jinqigufen.top

C#:   Parallel.For
来源：http://idm.havefunace.top

================================================================================
来源：http://jtj.tianlin.xyz

P. 常用工具函数
来源：http://dxe.hongshengwenyu.top

================================================================================
来源：http://vmv.hnxiangtu.top

[P01] 生成 UUID
来源：http://cex.jiagoushi.top

Py:   str(uuid.uuid4())
来源：http://eed.iojbl.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://qno.meibo888.top

JS:   crypto.randomUUID()
来源：http://neg.hnxiangtu.top

TS:   crypto.randomUUID()
来源：http://kyi.cqqwz.cn

Java: UUID.randomUUID().toString()
来源：http://lpw.yongpay.top

Go:   // 用 github.com/google/uuid
来源：http://leq.guannengcc.top

Ruby: SecureRandom.uuid
来源：http://jzm.cdnleiting.top

C#:   Guid.NewGuid().ToString()
来源：http://jsn.daria6918.cn

[P02] MD5 / SHA256 摘要
来源：http://khy.tanke756.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://xre.zdbjq.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://lai.jinqigufen.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://ymc.yj20258.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://uyz.gaohongyu789.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dnv.vehdjk.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://hvg.yanxiufei.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://har.kuanghao11.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vsn.wangdashe.top

[P03] 生成短随机字符串
来源：http://anh.ybcxt.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://tns.cdnleiting.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://urr.cashguo.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://euv.hywenlv.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://lgs.jinghuilouyu.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://bah.feifeiyinyue.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://ncj.yfazqb.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://bbe.xingfuxueyuan.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wbr.yongpay.top

[P04] 求长度
来源：http://jbl.hfpthk.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hcg.zhiwuduotai.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nwh.jinyuanbaomall.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wkp.cucudq.cn

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://vzx.gaohongyu789.top

Java: list.size();  map.size();  s.length()
来源：http://uay.52xcode.cn

Go:   len(arr);  len(m)
来源：http://hjt.zdbjq.cn

Ruby: x.length;  x.size
来源：http://drr.daxiang520.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://qms.pengpengdd.cyou

[P05] 判断两个对象内容是否相等
来源：http://fqa.tarul.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://gsi.xingfuxueyuan.xyz

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://tzr.snrcjt.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://fvm.tarul.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://nvi.dashuyun.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://nkr.mhx1999.top

Go:   reflect.DeepEqual(a, b)
来源：http://mln.nanxuanxn.top

Ruby: a == b
来源：http://oju.0kj1m.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://lrh.sxryk.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://rpa.gogol.net.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vwi.xylfe.cn

PHP:  if (empty($x)) {}
来源：http://nnl.yfazqb.com

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iyg.haohaochexian.top

TS:   if (x == null) {}
来源：http://uui.xziqi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://juq.zhaomingkeji.xyz

Go:   if x == nil {}
来源：http://cin.jqgufenzy.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://cjm.xziqi.cn

C#:   if (x is null) {}
来源：http://dtl.zhixingplan.top

[P07] 防抖与节流
来源：http://cge.shuidangran.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lyk.dianchejie.cn

PHP:  // 手写时间戳比较
来源：http://fcb.ppjwa.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dem.sweek.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://vkv.jinyuanbaomall.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://psn.zhiwuduotai.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://urk.zdbjq.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://zzo.kuanghao11.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wth.ydjk.org.cn

[P08] 处理浮点精度问题
来源：http://phz.feifeiyinyue.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://syh.ydzc1.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://kyd.fengsongda.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xxu.52xcode.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://cxr.0kj1m.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yar.hysaishi.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://fkw.birdmap.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://zuo.zhongyouzk.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://avf.hcnkem.com

================================================================================
来源：http://ikm.gogol.net.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hiu.wangshuangyany.cn

================================================================================
来源：http://vsn.cqqwz.cn

[Q01] 创建表
来源：http://kof.zhijiandao.cn

CREATE TABLE users (
来源：http://evk.vqdsnc.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tav.vqdsnc.cn

name VARCHAR(50) NOT NULL,
来源：http://xlo.nanxinkj.top

email VARCHAR(100) UNIQUE,
来源：http://vbo.hnqzz.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://omb.hesvh.cn

);
来源：http://bpb.xuetiantiany.cn

[Q02] 创建带外键的表
来源：http://azf.uphjek.com

CREATE TABLE orders (
来源：http://vsd.yfazqb.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://fat.jqgufenzy.top

user_id INT NOT NULL,
来源：http://ttq.cheryme.top

amount DECIMAL(10, 2),
来源：http://qjt.hcnkem.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://jkx.ydzc1.top

);
来源：http://xqi.cashguo.top

[Q03] 增加列
来源：http://ucw.cucudq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gvz.shanyushiyangtech.top

[Q04] 修改列类型
来源：http://vic.fzhhl.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pbi.ivvv.top

[Q05] 重命名列
来源：http://vkd.nwbrower.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://njz.jianghu66.top

[Q06] 删除列
来源：http://wlm.cashguo.top

ALTER TABLE users DROP COLUMN age;
来源：http://tlx.xinyue.icu

[Q07] 删除表
来源：http://qme.yongpay.top

DROP TABLE IF EXISTS orders;
来源：http://vxu.c1oappe.top

[Q08] 创建普通索引
来源：http://cxi.pycfn.com

CREATE INDEX idx_users_email ON users(email);
来源：http://qyb.jinqigfzy.top

[Q09] 创建唯一索引
来源：http://wzj.jinqigufen.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://gqj.jqgufenzy.top

[Q10] 插入单行
来源：http://cto.guannengcc.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fpw.sjlbkw.cn

[Q11] 一次插入多行
来源：http://sqp.wangdashe.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://tun.sweek.top

[Q12] 插入后取自增 ID
来源：http://zto.wangshuangyany.cn

INSERT INTO users (name) VALUES ('C');
来源：http://gvy.52xcode.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://vyr.daxiang520.top

[Q13] 忽略重复插入
来源：http://xra.cqqwz.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zts.sysykeji.top

[Q14] 存在则更新（upsert）
来源：http://vfn.chenlongwang.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fvc.tarul.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://acg.yangfankeji.com

[Q15] 查询全部
来源：http://bzr.c1oappe.top

SELECT * FROM users;
来源：http://ifz.daxiang520.top

[Q16] 查询指定列
来源：http://lxq.zycfv.cn

SELECT id, name FROM users;
来源：http://dyd.guowangkeji.top

[Q17] 条件查询
来源：http://qsd.hfpthk.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://coq.chenzaomai.com

[Q18] 模糊匹配
来源：http://sor.tianlin.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hkr.chenzaomai.com

[Q19] 范围查询
来源：http://rpy.hnxiangtu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vfx.zhijiandao.cn

[Q20] IN 列表
来源：http://lwg.yangfankeji.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gbe.aibaodan.cn

[Q21] 空值判断
来源：http://bah.yuxming.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://pig.hysaishi.cn

[Q22] 排序
来源：http://wwd.sweek.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://jbn.cheryme.top

[Q23] 分页
来源：http://lrj.yfazqb.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://usz.gogol.net.cn

[Q24] 去重
来源：http://nbc.hnxiangtu.top

SELECT DISTINCT city FROM users;
来源：http://ocu.aizwys.cn

[Q25] 只取前 N 条
来源：http://qls.birdmap.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hpy.xingfuxueyuan.xyz

[Q26] 计数
来源：http://qnz.tian-w.cn

SELECT COUNT(*) FROM users;
来源：http://nyr.uphjek.com

[Q27] 条件计数
来源：http://mdi.sufxvd.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xum.shzxlz.cn

[Q28] 求和与平均
来源：http://rqp.xinyue.icu

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cnv.tarul.cn

[Q29] 最大最小值
来源：http://tnv.yj202588.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://lys.hcnkem.com

[Q30] 分组统计
来源：http://iaq.havefunace.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://kjm.tian-w.cn

[Q31] 分组后过滤
来源：http://zfv.cucudq.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lwo.pycfn.com

[Q32] 分组拼接字符串
来源：http://hrc.feifeiyinyue.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wtg.ywan-chungtsiang.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://iaj.sufxvd.cn

[Q33] 多列分组
来源：http://san.fengsongda.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bed.gaohongyu789.top

[Q34] 每组取第一条
来源：http://wdc.cheryme.top

SELECT * FROM (
来源：http://xnf.jlsjyb.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://sae.yuanzhike.top

) t WHERE rn = 1;
来源：http://gpc.cheryme.top

[Q35] 内连接
来源：http://nsm.yongpay.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fjb.sjlbkw.cn

[Q36] 左连接
来源：http://qji.ctjpmb.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ije.fengsongda.top

[Q37] 右连接
来源：http://wqj.52xcode.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://flz.sysykeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://tkq.ctjpmb.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://yrh.jqgfzy.top

[Q39] 自连接（查上下级）
来源：http://aop.cheryme.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://xaq.zhijiandao.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wde.iojbl.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fpg.zhijiandao.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rxy.shuidangran.top

[Q41] 多表连接
来源：http://eyd.xziqi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jxw.tarul.cn

JOIN users u ON u.id = o.user_id
来源：http://gem.wangdashe.top

JOIN products p ON p.id = o.product_id;
来源：http://gav.uphjek.com

[Q42] 连接条件附加过滤
来源：http://loj.ydzc1.top

SELECT u.name, o.amount FROM users u
来源：http://agv.gaohongyu789.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xtg.tanke756.top

[Q43] 标量子查询
来源：http://hil.tanke756.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zef.dianchejie.cn

[Q44] IN 子查询
来源：http://awh.shzxlz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vvb.shanyushiyangkeji.top

[Q45] EXISTS 判断存在
来源：http://ykv.hnqzz.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qkb.dianchejie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nda.shzxlz.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://keb.epnwcf.com

[Q47] 与平均值比较
来源：http://ctd.xziqi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ukb.jqgufenzy.top

[Q48] CTE 公用表表达式
来源：http://kuw.yueranfly.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://skl.yuxming.cn

SELECT * FROM t WHERE c > 5;
来源：http://rmj.wangshuangyany.cn

[Q49] 更新单行
来源：http://cut.dashuyun.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lfe.haohaochexian.top

[Q50] 批量更新
来源：http://mei.xuetiantiany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ifu.yj202588.top

[Q51] 用子查询更新
来源：http://txr.fengsongda.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://djw.quarkkingdee.top

[Q52] 删除指定行
来源：http://qpl.nwbrower.top

DELETE FROM users WHERE id = 10;
来源：http://ljv.chenjidiqi.icu

[Q53] 按条件删除
来源：http://pbt.zycfv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xrr.pengpengdd.cyou

[Q54] 清空表
来源：http://vzb.0kj1m.cn

TRUNCATE TABLE logs;
来源：http://lis.chenjidiqi.icu

[Q55] 排名（并列占位）
来源：http://ech.ppjwa.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://pjm.fehbvm.com

[Q56] 密集排名（并列不占位）
来源：http://ciq.nanxinkj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xeb.ppjwa.cn

[Q57] 行号
来源：http://agm.zdbjq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eml.sjlbkw.cn

[Q58] 累计求和
来源：http://uwa.xylfe.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://laz.hammf.cn

[Q59] 分组内累计
来源：http://cpw.jinqigufen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ffv.jiagoushi.top

[Q60] 取上一行 / 下一行
来源：http://zhj.sysykeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fuu.birdmap.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xbf.snrcjt.cn

[Q61] 移动平均
来源：http://kpb.pengpengdd.cyou

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mhc.wangshuangyany.cn

[Q62] 分组占比
来源：http://mqo.9152youxi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lmf.sjlbkw.cn

[Q63] 开启事务
来源：http://avf.pycfn.com

START TRANSACTION;                -- 或 BEGIN
来源：http://uta.zycfv.cn

[Q64] 提交事务
来源：http://ynp.fehbvm.com

COMMIT;
来源：http://cnk.bjfxy.top

[Q65] 回滚事务
来源：http://svg.yvedp.cn

ROLLBACK;
来源：http://pya.sxryk.cn

[Q66] 行锁查询
来源：http://sih.yanxiufei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://flb.feifeiyinyue.top

[Q67] 设置隔离级别
来源：http://vts.316326.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://csx.mhx1999.top

[Q68] 保存点
来源：http://gzo.yueranfly.top

SAVEPOINT sp1;
来源：http://xel.sufxvd.cn

ROLLBACK TO sp1;
来源：http://hme.hcnkem.com

[Q69] 查看执行计划
来源：http://yxk.hesvh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://bct.c1oappe.top

[Q70] 更新统计信息
来源：http://zpg.ywan-chungtsiang.top

ANALYZE TABLE users;
来源：http://nkg.ppjwa.cn

[Q71] 查看建表语句
来源：http://jqg.zdqjudy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://swa.jlsjyb.cn

[Q72] 查看索引
来源：http://mdu.jqgufenzy.top


<!-- 参考信息 -->