代发 wailian999

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wgz.ctjpmb.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://oey.gaohongyu789.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jqj.nanxuanxn.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bnr.xylfe.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://znm.hywenlv.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://rcn.nanxinkj.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jze.jqgfzy.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://qxj.feifeiyinyue.top

================================================================================
来源：http://idx.bjfxy.top

O. 并发与异步
来源：http://lou.zhixingplan.top

================================================================================
来源：http://upj.yuanzhike.top

[O01] 启动一个线程
来源：http://aqf.xylfe.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://ehj.hongshengwenyu.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zug.ivvv.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://oku.hesvh.cn

TS:   // 同 JS
来源：http://ofh.316326.xyz

Java: new Thread(() -> f()).start()
来源：http://bgw.ivvv.top

Go:   go f()
来源：http://uge.pengpengdd.cyou

Ruby: Thread.new { f }
来源：http://pzs.chenzaomai.com

C#:   Task.Run(() => F());
来源：http://cew.pycfn.com

[O02] 使用线程池
来源：http://iek.snrcjt.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://nkz.zycfv.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://pgt.shuidangran.top

JS:   // worker_threads 线程池
来源：http://fpy.cashguo.top

TS:   // worker_threads 线程池
来源：http://pru.pycfn.com

Java: Executors.newFixedThreadPool(4)
来源：http://vda.chenzaomai.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://ywh.yvedp.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://aam.9152youxi.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://hld.gzhubu.top

[O03] 加锁保护共享数据
来源：http://elp.jlsjyb.cn

Py:   with lock: shared += 1
来源：http://ars.yonumen.top

PHP:  // 用 flock() 做文件锁
来源：http://pht.zhiwuduotai.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gxw.shanyushiyangtech.top

TS:   // 同 JS
来源：http://qdx.guowangkeji.top

Java: synchronized (this) { shared++; }
来源：http://mbf.xuetiantiany.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bxe.0kj1m.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://rqv.hongshengwenyu.top

C#:   lock (gate) { shared++; }
来源：http://pfk.chenzaomai.com

[O04] 定义异步函数并等待
来源：http://rth.zdqjudy.top

Py:   async def f():⏎    await g()
来源：http://eha.jinqigufen.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wvh.zhengqikj.top

JS:   async function f() { await g(); }
来源：http://hgn.fktsv.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://qir.birdmap.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://nfn.sysykeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://fxk.sufxvd.cn

Ruby: # 用 Fiber 或 async gem
来源：http://tdo.cucudq.cn

C#:   async Task F() { await G(); }
来源：http://hnx.jianghu66.top

[O05] 并发执行并等待全部完成
来源：http://vrn.c1oappe.top

Py:   asyncio.gather(*tasks)
来源：http://hsu.yongpay.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://dnq.quarkkingdee.top

JS:   await Promise.all(tasks)
来源：http://woo.gotoacloud.top

TS:   await Promise.all(tasks)
来源：http://pck.yonumen.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://rwx.zhijiandao.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://hxa.yj20258888.top

Ruby: threads.map(&:join)
来源：http://tjz.chenzaomai.com

C#:   await Task.WhenAll(t1, t2)
来源：http://jmf.nanxinkj.top

[O06] 使用进程池
来源：http://ylm.epnwcf.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://juz.bbcook.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://kig.fanxiaobao.xyz

JS:   // child_process / cluster 模块
来源：http://ugq.ehwqpu.com

TS:   // child_process / cluster 模块
来源：http://jco.xingfuxueyuan.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://usq.jqgfzy.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://tzo.pengpengdd.cyou

Ruby: // fork 块
来源：http://wll.yj202588.top

C#:   Parallel.For
来源：http://msm.redwolf501.top

================================================================================
来源：http://bhc.aizwys.cn

P. 常用工具函数
来源：http://agd.sxryk.cn

================================================================================
来源：http://hqn.chenzaomai.com

[P01] 生成 UUID
来源：http://nse.vehdjk.com

Py:   str(uuid.uuid4())
来源：http://qfi.hnxiangtu.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://xmh.zdqjudy.top

JS:   crypto.randomUUID()
来源：http://jig.fktsv.cn

TS:   crypto.randomUUID()
来源：http://hyu.hcnkem.com

Java: UUID.randomUUID().toString()
来源：http://svw.ehwqpu.com

Go:   // 用 github.com/google/uuid
来源：http://fpd.shzxlz.cn

Ruby: SecureRandom.uuid
来源：http://sme.gogol.net.cn

C#:   Guid.NewGuid().ToString()
来源：http://jmh.yj20258.top

[P02] MD5 / SHA256 摘要
来源：http://oxc.xinyue.icu

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://vzy.fehbvm.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://ytq.hongshengwenyu.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://uyy.jinqigufen.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://jsh.hnxiangtu.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://vfk.ivvv.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://bdu.guowangkeji.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://iae.epnwcf.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wod.yangfankeji.com

[P03] 生成短随机字符串
来源：http://hhf.hysaishi.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://faw.sufxvd.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://fil.52xcode.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://riy.jinqigufen.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gdj.0kj1m.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://omz.smart0.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://usc.bjfxy.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lel.kuanghao11.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://pcj.meibo888.top

[P04] 求长度
来源：http://pix.jqgufenzy.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wwd.9152youxi.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nel.tarul.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://pjl.zhongyouzk.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://tfm.316326.xyz

Java: list.size();  map.size();  s.length()
来源：http://nxk.jianghu66.top

Go:   len(arr);  len(m)
来源：http://qjv.ehwqpu.com

Ruby: x.length;  x.size
来源：http://hvk.yvedp.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://vtw.yuxming.cn

[P05] 判断两个对象内容是否相等
来源：http://afe.shanyushiyangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://fsi.zhixingplan.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://ujh.zhijiandao.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://bbx.yongpay.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://cvq.jqgufenzy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baj.vehdjk.com

Go:   reflect.DeepEqual(a, b)
来源：http://adm.hesvh.cn

Ruby: a == b
来源：http://nac.epnwcf.com

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wjr.feifeiyinyue.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://zqc.xziqi.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://eiu.daxiang520.top

PHP:  if (empty($x)) {}
来源：http://irj.jinqigfzy.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://iac.fktsv.cn

TS:   if (x == null) {}
来源：http://pdl.zhixingplan.top

Java: if (x == null || x.isEmpty()) {}
来源：http://lqa.jinghuilouyu.cn

Go:   if x == nil {}
来源：http://xvu.vqdsnc.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://uez.ctjpmb.com

C#:   if (x is null) {}
来源：http://yrm.shanyushiyangtech.top

[P07] 防抖与节流
来源：http://ehy.jlsjyb.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://npo.yj202588.top

PHP:  // 手写时间戳比较
来源：http://fgc.hnxiangtu.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://zjp.epnwcf.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://buy.cashguo.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mwh.jlsjyb.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://xtd.jianghu66.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://pmy.chenlongwang.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uxh.birdmap.top

[P08] 处理浮点精度问题
来源：http://jik.hfpthk.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qal.bbcook.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://chy.aibaodan.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bly.sxryk.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://lhs.guowangkeji.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://uzl.fktsv.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://hat.ivvv.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://nzz.iojbl.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://qjy.ydjk.org.cn

================================================================================
来源：http://ldp.cheryme.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://fbd.yueranfly.top

================================================================================
来源：http://uuf.ybcxt.top

[Q01] 创建表
来源：http://eiz.vqdsnc.cn

CREATE TABLE users (
来源：http://xha.jlsjyb.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bhe.havefunace.top

name VARCHAR(50) NOT NULL,
来源：http://mer.birdmap.top

email VARCHAR(100) UNIQUE,
来源：http://blc.zhoulong.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ody.cheryme.top

);
来源：http://svm.guowangkeji.top

[Q02] 创建带外键的表
来源：http://ond.jinghuilouyu.cn

CREATE TABLE orders (
来源：http://nyl.gotoacloud.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dgc.vqdsnc.cn

user_id INT NOT NULL,
来源：http://klr.jianghu66.top

amount DECIMAL(10, 2),
来源：http://aao.ydzc1.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://eri.bjfxy.top

);
来源：http://euy.yj20258888.top

[Q03] 增加列
来源：http://agd.feifeiyinyue.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://acd.yfazqb.com

[Q04] 修改列类型
来源：http://juc.iojbl.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yhg.zhoulong.xyz

[Q05] 重命名列
来源：http://qnk.hesvh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rub.smart0.xyz

[Q06] 删除列
来源：http://tbx.vehdjk.com

ALTER TABLE users DROP COLUMN age;
来源：http://mzc.yj202588.top

[Q07] 删除表
来源：http://oqq.jinghuilouyu.cn

DROP TABLE IF EXISTS orders;
来源：http://kgs.jqgufenzy.top

[Q08] 创建普通索引
来源：http://qwq.hammf.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://uzv.aibaodan.cn

[Q09] 创建唯一索引
来源：http://ywi.xuetiantiany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://hav.jinqigfzy.top

[Q10] 插入单行
来源：http://dsi.pycfn.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://kei.aizwys.cn

[Q11] 一次插入多行
来源：http://wio.zdbjq.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ylr.jinqigufen.top

[Q12] 插入后取自增 ID
来源：http://abe.zhongyouzk.top

INSERT INTO users (name) VALUES ('C');
来源：http://kas.aizwys.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://abu.hnxiangtu.top

[Q13] 忽略重复插入
来源：http://wpa.zhijiandao.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://dmh.aizwys.cn

[Q14] 存在则更新（upsert）
来源：http://fni.tianlin.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sxd.chenlongwang.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://lla.birdmap.top

[Q15] 查询全部
来源：http://gni.jiagoushi.top

SELECT * FROM users;
来源：http://kjl.ehwqpu.com

[Q16] 查询指定列
来源：http://ate.mhx1999.top

SELECT id, name FROM users;
来源：http://yku.ydzc1.top

[Q17] 条件查询
来源：http://grr.jianghu66.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hrn.vehdjk.com

[Q18] 模糊匹配
来源：http://nsq.hammf.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pmi.epnwcf.com

[Q19] 范围查询
来源：http://eil.zhaomingkeji.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bix.jqgufenzy.top

[Q20] IN 列表
来源：http://riz.havefunace.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ajp.jqgufenzy.top

[Q21] 空值判断
来源：http://ayo.yongpay.top

SELECT * FROM users WHERE email IS NULL;
来源：http://jbe.hongshengwenyu.top

[Q22] 排序
来源：http://tbz.quarkkingdee.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zwg.9152youxi.cn

[Q23] 分页
来源：http://xbk.zhixingplan.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://qum.havefunace.top

[Q24] 去重
来源：http://dza.jiagoushi.top

SELECT DISTINCT city FROM users;
来源：http://icf.aizwys.cn

[Q25] 只取前 N 条
来源：http://aar.shangyingyoupin.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lnh.yj202588.top

[Q26] 计数
来源：http://rox.pengpengdd.cyou

SELECT COUNT(*) FROM users;
来源：http://ztm.jianghu66.top

[Q27] 条件计数
来源：http://loy.gogol.net.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://kjr.jinqigufen.top

[Q28] 求和与平均
来源：http://uag.shuidangran.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://kwh.zhoulong.xyz

[Q29] 最大最小值
来源：http://ovs.mhx1999.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jgr.9152youxi.cn

[Q30] 分组统计
来源：http://ebw.52xcode.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xbw.daria6918.cn

[Q31] 分组后过滤
来源：http://jth.zhijiandao.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://tad.xylfe.cn

[Q32] 分组拼接字符串
来源：http://lbq.jqgufenzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://oie.sufxvd.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://juz.xuetiantiany.cn

[Q33] 多列分组
来源：http://qwg.haohaochexian.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zxs.zhaomingkeji.xyz

[Q34] 每组取第一条
来源：http://get.fehbvm.com

SELECT * FROM (
来源：http://yye.vehdjk.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://jbs.aibaodan.cn

) t WHERE rn = 1;
来源：http://tgj.zycfv.cn

[Q35] 内连接
来源：http://vdc.hfpthk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qfx.aibaodan.cn

[Q36] 左连接
来源：http://oru.daxiang520.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://skb.sjlbkw.cn

[Q37] 右连接
来源：http://ogq.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://oto.pycfn.com

[Q38] 全外连接（PostgreSQL）
来源：http://gsv.zhiwuduotai.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://imm.bjfxy.top

[Q39] 自连接（查上下级）
来源：http://fah.shzxlz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://sdm.zdbjq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vts.quarkkingdee.top

[Q40] 交叉连接（笛卡尔积）
来源：http://tni.zhoulong.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jdh.jinghuilouyu.cn

[Q41] 多表连接
来源：http://heq.zhengqikj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rfz.quarkkingdee.top

JOIN users u ON u.id = o.user_id
来源：http://uto.shuidangran.top

JOIN products p ON p.id = o.product_id;
来源：http://dsl.zdbjq.cn

[Q42] 连接条件附加过滤
来源：http://trm.feifeiyinyue.top

SELECT u.name, o.amount FROM users u
来源：http://ewh.hnxiangtu.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rbc.shanyushiyangkeji.top

[Q43] 标量子查询
来源：http://vqg.daxiang520.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nre.vqdsnc.cn

[Q44] IN 子查询
来源：http://ran.daria6918.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ewk.jinqigufen.top

[Q45] EXISTS 判断存在
来源：http://lwy.nanxinkj.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xuu.fanxiaobao.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://ocz.yj20258888.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gny.cdnleiting.top

[Q47] 与平均值比较
来源：http://vhx.hesvh.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gul.0kj1m.cn

[Q48] CTE 公用表表达式
来源：http://ytz.hfpthk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://gbi.yuanzhike.top

SELECT * FROM t WHERE c > 5;
来源：http://xzo.xuetiantiany.cn

[Q49] 更新单行
来源：http://zkg.yanxiufei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zgh.yuxming.cn

[Q50] 批量更新
来源：http://wpw.yongpay.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://umq.wangshuangyany.cn

[Q51] 用子查询更新
来源：http://lbs.chenjidiqi.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rff.pengpengdd.cyou

[Q52] 删除指定行
来源：http://cga.vqdsnc.cn

DELETE FROM users WHERE id = 10;
来源：http://uqn.hywenlv.cn

[Q53] 按条件删除
来源：http://rpi.daria6918.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xzk.zhongyouzk.top

[Q54] 清空表
来源：http://fuc.shangyingyoupin.top

TRUNCATE TABLE logs;
来源：http://vff.zhongyouzk.top

[Q55] 排名（并列占位）
来源：http://mft.jiagoushi.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ovl.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://pjg.yuxming.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pdq.redwolf501.top

[Q57] 行号
来源：http://vre.jinqigufen.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ipo.kuanghao11.cn

[Q58] 累计求和
来源：http://fkq.birdmap.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://buf.cqqwz.cn

[Q59] 分组内累计
来源：http://mro.yj20258.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://snm.sufxvd.cn

[Q60] 取上一行 / 下一行
来源：http://vtu.bbcook.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jqy.tanke756.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://odw.sufxvd.cn

[Q61] 移动平均
来源：http://ruo.chenlongwang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xkb.yuxming.cn

[Q62] 分组占比
来源：http://dlt.ehwqpu.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ety.fanxiaobao.xyz

[Q63] 开启事务
来源：http://plb.gogol.net.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://anb.yvedp.cn

[Q64] 提交事务
来源：http://rsa.aibaodan.cn

COMMIT;
来源：http://ysc.mhx1999.top

[Q65] 回滚事务
来源：http://sdj.yuxming.cn

ROLLBACK;
来源：http://all.cashguo.top

[Q66] 行锁查询
来源：http://bdk.bjfxy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rue.shzxlz.cn

[Q67] 设置隔离级别
来源：http://trq.ydjk.org.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jbi.zhoulong.xyz

[Q68] 保存点
来源：http://obb.hesvh.cn

SAVEPOINT sp1;
来源：http://sqa.yuanzhike.top


<!-- 参考信息 -->