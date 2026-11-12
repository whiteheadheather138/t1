代发 wailian999

Go:   // 手写递归
来源：http://rrw.bbcook.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://pkl.ehwqpu.com

C#:   // 手写递归
来源：http://bgd.jiagoushi.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://lyh.jinqigfzy.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fim.jqgfzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hgi.cdnleiting.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wwt.zhengqikj.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://kmk.gotoacloud.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xkd.jinqigfzy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wyb.xingfuxueyuan.xyz

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wjm.0kj1m.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wmp.hammf.cn

================================================================================
来源：http://lcj.andypj.xyz

O. 并发与异步
来源：http://gyn.bjfxy.top

================================================================================
来源：http://ukj.daria6918.cn

[O01] 启动一个线程
来源：http://sge.wangdashe.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bth.cdnleiting.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://xnb.yongpay.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://myn.hcnkem.com

TS:   // 同 JS
来源：http://xjw.316326.xyz

Java: new Thread(() -> f()).start()
来源：http://nku.jinyuanbaomall.cn

Go:   go f()
来源：http://ash.jinyuanbaomall.cn

Ruby: Thread.new { f }
来源：http://gio.guannengcc.top

C#:   Task.Run(() => F());
来源：http://jbr.sysykeji.top

[O02] 使用线程池
来源：http://rtu.tanke756.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://seu.bjfxy.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fvu.mhx1999.top

JS:   // worker_threads 线程池
来源：http://iuh.zhaomingkeji.xyz

TS:   // worker_threads 线程池
来源：http://kqo.zhongyouzk.top

Java: Executors.newFixedThreadPool(4)
来源：http://hor.fzhhl.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://dgm.xinyue.icu

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://xar.gaohongyu789.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hyy.hnxiangtu.top

[O03] 加锁保护共享数据
来源：http://wni.shuidangran.top

Py:   with lock: shared += 1
来源：http://pds.daxiang520.top

PHP:  // 用 flock() 做文件锁
来源：http://mgf.nwbrower.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://whs.jinqigufen.top

TS:   // 同 JS
来源：http://qhj.hnqzz.top

Java: synchronized (this) { shared++; }
来源：http://egr.jlsjyb.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://nql.kuanghao11.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://bgv.xuanzx.com

C#:   lock (gate) { shared++; }
来源：http://npg.ppjwa.cn

[O04] 定义异步函数并等待
来源：http://ilz.jlsjyb.cn

Py:   async def f():⏎    await g()
来源：http://ege.jqgufenzy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://ogd.9152youxi.cn

JS:   async function f() { await g(); }
来源：http://qgo.smart0.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://cxy.zhiwuduotai.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://qzq.kuanghao11.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://frg.feifeiyinyue.top

Ruby: # 用 Fiber 或 async gem
来源：http://wfz.ydzc1.top

C#:   async Task F() { await G(); }
来源：http://veq.fengsongda.top

[O05] 并发执行并等待全部完成
来源：http://gby.zhixingplan.top

Py:   asyncio.gather(*tasks)
来源：http://xze.gzhubu.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gwp.shanyushiyangtech.top

JS:   await Promise.all(tasks)
来源：http://nso.yueranfly.top

TS:   await Promise.all(tasks)
来源：http://iny.xuetiantiany.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://alo.aizwys.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wul.gogol.net.cn

Ruby: threads.map(&:join)
来源：http://ewy.xylfe.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://kvn.svipenyu.cn

[O06] 使用进程池
来源：http://rlf.yfazqb.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://opt.hnqzz.top

PHP:  // pcntl_fork 或多进程队列
来源：http://ypj.c1oappe.top

JS:   // child_process / cluster 模块
来源：http://nzk.jiagoushi.top

TS:   // child_process / cluster 模块
来源：http://bsk.ywan-chungtsiang.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://lww.shuidangran.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zpm.jinqigufen.top

Ruby: // fork 块
来源：http://gps.yuxming.cn

C#:   Parallel.For
来源：http://ebr.ivvv.top

================================================================================
来源：http://ldq.zhengqikj.top

P. 常用工具函数
来源：http://oru.chenjidiqi.icu

================================================================================
来源：http://wkw.ydjk.org.cn

[P01] 生成 UUID
来源：http://bpu.yanxiufei.cn

Py:   str(uuid.uuid4())
来源：http://yhj.snrcjt.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://vwn.dashuyun.cn

JS:   crypto.randomUUID()
来源：http://yip.havefunace.top

TS:   crypto.randomUUID()
来源：http://puz.pycfn.com

Java: UUID.randomUUID().toString()
来源：http://oku.hcnkem.com

Go:   // 用 github.com/google/uuid
来源：http://sqx.c1oappe.top

Ruby: SecureRandom.uuid
来源：http://uak.kuanghao11.cn

C#:   Guid.NewGuid().ToString()
来源：http://gcy.yvedp.cn

[P02] MD5 / SHA256 摘要
来源：http://udl.jinghuilouyu.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bpk.zdqjudy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://tsl.yueranfly.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://gfd.9152youxi.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://ltx.sysykeji.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://eqh.zhoulong.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://iqa.0kj1m.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bro.jinyuanbaomall.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mgw.tanke756.top

[P03] 生成短随机字符串
来源：http://obd.xziqi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://njg.kuanghao11.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://myh.gotoacloud.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://dux.zhongyouzk.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qic.yj202588.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://kpp.kuanghao11.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://zpy.cdnleiting.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://cqt.fzhhl.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://fto.aizwys.cn

[P04] 求长度
来源：http://sas.hysaishi.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bjx.zhengqikj.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oqo.ydzc1.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://bvh.jiagoushi.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://qqg.yongpay.top

Java: list.size();  map.size();  s.length()
来源：http://amx.yongpay.top

Go:   len(arr);  len(m)
来源：http://yqc.mhx1999.top

Ruby: x.length;  x.size
来源：http://uhp.ivvv.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://upq.hongshengwenyu.top

[P05] 判断两个对象内容是否相等
来源：http://ulq.hnqzz.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://wdk.redwolf501.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://uoz.iojbl.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uwr.aizwys.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://sbi.fehbvm.com

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://zom.hnqzz.top

Go:   reflect.DeepEqual(a, b)
来源：http://sec.hcnkem.com

Ruby: a == b
来源：http://aap.zhongyouzk.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://gyg.smart0.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bzo.zhoulong.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://exv.fengsongda.top

PHP:  if (empty($x)) {}
来源：http://hfp.feifeiyinyue.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://tkb.zhengqikj.top

TS:   if (x == null) {}
来源：http://iay.hywenlv.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://pcs.nanxinkj.top

Go:   if x == nil {}
来源：http://zho.xingfuxueyuan.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://xnj.aizwys.cn

C#:   if (x is null) {}
来源：http://dmj.sweek.top

[P07] 防抖与节流
来源：http://lnu.cashguo.top

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sbb.quarkkingdee.top

PHP:  // 手写时间戳比较
来源：http://cgc.kuanghao11.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pbf.zdbjq.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://bix.fzhhl.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://ytf.xziqi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lhz.shanyushiyangtech.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://xfz.daria6918.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://odc.nanxuanxn.top

[P08] 处理浮点精度问题
来源：http://fpo.redwolf501.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://nhq.gaohongyu789.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ppf.ywan-chungtsiang.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://abt.fehbvm.com

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pzb.cucudq.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://dng.tarul.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://phe.redwolf501.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ojp.ydjk.org.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wqt.cqqwz.cn

================================================================================
来源：http://rhz.hywenlv.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://hzl.aizwys.cn

================================================================================
来源：http://akv.sxryk.cn

[Q01] 创建表
来源：http://wdl.hnxiangtu.top

CREATE TABLE users (
来源：http://bsj.tian-w.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://fbx.chenjidiqi.icu

name VARCHAR(50) NOT NULL,
来源：http://vyb.zdqjudy.top

email VARCHAR(100) UNIQUE,
来源：http://jwg.jlsjyb.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://els.jianghu66.top

);
来源：http://gne.tian-w.cn

[Q02] 创建带外键的表
来源：http://ipb.yfazqb.com

CREATE TABLE orders (
来源：http://nka.xziqi.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://aun.cdnleiting.top

user_id INT NOT NULL,
来源：http://ved.pycfn.com

amount DECIMAL(10, 2),
来源：http://mbd.ybcxt.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://pyw.guowangkeji.top

);
来源：http://xze.jyoumei.cn

[Q03] 增加列
来源：http://tzc.guowangkeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://gro.sxryk.cn

[Q04] 修改列类型
来源：http://vkl.sweek.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://qve.chenzaomai.com

[Q05] 重命名列
来源：http://xlm.hongshengwenyu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://irr.cqqwz.cn

[Q06] 删除列
来源：http://wpj.sweek.top

ALTER TABLE users DROP COLUMN age;
来源：http://gko.tianlin.xyz

[Q07] 删除表
来源：http://yrz.cqqwz.cn

DROP TABLE IF EXISTS orders;
来源：http://nff.yangfankeji.com

[Q08] 创建普通索引
来源：http://zkw.yangfankeji.com

CREATE INDEX idx_users_email ON users(email);
来源：http://inq.bjfxy.top

[Q09] 创建唯一索引
来源：http://see.gotoacloud.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://eae.xylfe.cn

[Q10] 插入单行
来源：http://nuk.jinghuilouyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://igp.aibaodan.cn

[Q11] 一次插入多行
来源：http://kjv.hesvh.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iyo.shzxlz.cn

[Q12] 插入后取自增 ID
来源：http://jjk.nanxuanxn.top

INSERT INTO users (name) VALUES ('C');
来源：http://uua.kuanghao11.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pnu.yonumen.top

[Q13] 忽略重复插入
来源：http://cmb.vehdjk.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://anp.shanyushiyangkeji.top

[Q14] 存在则更新（upsert）
来源：http://rmi.hfpthk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fkc.cashguo.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://avs.yangfankeji.com

[Q15] 查询全部
来源：http://sdh.smart0.xyz

SELECT * FROM users;
来源：http://wej.zhoulong.xyz

[Q16] 查询指定列
来源：http://idw.dashuyun.cn

SELECT id, name FROM users;
来源：http://ybs.fehbvm.com

[Q17] 条件查询
来源：http://ttx.zhijiandao.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://yne.quarkkingdee.top

[Q18] 模糊匹配
来源：http://xik.xingfuxueyuan.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://toi.bbcook.cn

[Q19] 范围查询
来源：http://tps.ywan-chungtsiang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ljw.meibo888.top

[Q20] IN 列表
来源：http://yun.yongpay.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kvs.c1oappe.top

[Q21] 空值判断
来源：http://per.svipenyu.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gnk.jinghuilouyu.cn

[Q22] 排序
来源：http://nsy.jiagoushi.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ets.yfazqb.com

[Q23] 分页
来源：http://pcx.jlsjyb.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uuh.epnwcf.com

[Q24] 去重
来源：http://eij.sweek.top

SELECT DISTINCT city FROM users;
来源：http://lwm.chenzaomai.com

[Q25] 只取前 N 条
来源：http://aed.sjlbkw.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hyk.cdnleiting.top

[Q26] 计数
来源：http://bbp.yfazqb.com

SELECT COUNT(*) FROM users;
来源：http://jsi.yanxiufei.cn

[Q27] 条件计数
来源：http://yhh.gaohongyu789.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zch.wangshuangyany.cn

[Q28] 求和与平均
来源：http://xfz.ywan-chungtsiang.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xxl.shanyushiyangtech.top

[Q29] 最大最小值
来源：http://cqf.yuxming.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ajk.shanyushiyangkeji.top

[Q30] 分组统计
来源：http://sei.zhixingplan.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lkf.sweek.top

[Q31] 分组后过滤
来源：http://kpn.fengsongda.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ung.sweek.top

[Q32] 分组拼接字符串
来源：http://dvz.guowangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oud.shzxlz.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hpu.hfpthk.cn

[Q33] 多列分组
来源：http://zlj.vqdsnc.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hms.daria6918.cn

[Q34] 每组取第一条
来源：http://wng.daria6918.cn

SELECT * FROM (
来源：http://ask.zhiwuduotai.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xsc.zhoulong.xyz

) t WHERE rn = 1;
来源：http://qpo.yongpay.top

[Q35] 内连接
来源：http://crh.shangyingyoupin.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ymt.sjlbkw.cn

[Q36] 左连接
来源：http://wha.zhixingplan.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hcn.gaohongyu789.top

[Q37] 右连接
来源：http://exb.bbcook.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://sfr.zhongyouzk.top

[Q38] 全外连接（PostgreSQL）
来源：http://rky.jiagoushi.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dis.ppjwa.cn

[Q39] 自连接（查上下级）
来源：http://jix.feifeiyinyue.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://gxr.haohaochexian.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://zjx.sufxvd.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://led.svipenyu.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kwp.cashguo.top

[Q41] 多表连接
来源：http://otg.bjfxy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://dci.ctjpmb.com

JOIN users u ON u.id = o.user_id
来源：http://cjq.nanxuanxn.top

JOIN products p ON p.id = o.product_id;
来源：http://dhf.tianlin.xyz

[Q42] 连接条件附加过滤
来源：http://tek.jinqigfzy.top

SELECT u.name, o.amount FROM users u
来源：http://elb.shanyushiyangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uyk.chenlongwang.top

[Q43] 标量子查询
来源：http://vux.haohaochexian.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fvl.fanxiaobao.xyz

[Q44] IN 子查询
来源：http://hbh.shzxlz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vkx.ydzc1.top

[Q45] EXISTS 判断存在
来源：http://tdh.sjlbkw.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vpw.shzxlz.cn

[Q46] NOT EXISTS 判断不存在
来源：http://nhi.smart0.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn

[Q47] 与平均值比较
来源：http://oee.fengsongda.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://akj.sxryk.cn

[Q48] CTE 公用表表达式
来源：http://mqg.jiagoushi.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qyg.chenzaomai.com

SELECT * FROM t WHERE c > 5;
来源：http://mec.yonumen.top

[Q49] 更新单行
来源：http://bzb.tian-w.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rja.ctjpmb.com

[Q50] 批量更新
来源：http://fxs.fktsv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tkn.cashguo.top

[Q51] 用子查询更新
来源：http://tpx.yj20258.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fgd.yj202588.top

[Q52] 删除指定行
来源：http://urd.c1oappe.top

DELETE FROM users WHERE id = 10;
来源：http://lny.haohaochexian.top

[Q53] 按条件删除
来源：http://egs.yongpay.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hho.yj20258888.top

[Q54] 清空表
来源：http://fwj.andypj.xyz

TRUNCATE TABLE logs;
来源：http://iau.tanke756.top

[Q55] 排名（并列占位）
来源：http://psm.xziqi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fin.haohaochexian.top

[Q56] 密集排名（并列不占位）
来源：http://gum.cqqwz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qki.uphjek.com

[Q57] 行号
来源：http://cnj.zdqjudy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oho.haohaochexian.top

[Q58] 累计求和
来源：http://zxd.chenzaomai.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ipo.chenzaomai.com

[Q59] 分组内累计
来源：http://jin.gaohongyu789.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pwx.fehbvm.com

[Q60] 取上一行 / 下一行
来源：http://zuc.aizwys.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zly.cheryme.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tbm.meibo888.top

[Q61] 移动平均
来源：http://pxn.yj20258888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mik.quarkkingdee.top

[Q62] 分组占比
来源：http://jcl.xziqi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vve.daxiang520.top

[Q63] 开启事务
来源：http://mut.hammf.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://mzj.52xcode.cn

[Q64] 提交事务
来源：http://cml.cheryme.top

COMMIT;
来源：http://nck.fengsongda.top

[Q65] 回滚事务
来源：http://grb.shanyushiyangkeji.top

ROLLBACK;
来源：http://owe.zycfv.cn

[Q66] 行锁查询
来源：http://deb.yfazqb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ily.pengpengdd.cyou


<!-- 参考信息 -->