代发 wailian999

Go:   // 手写递归
来源：http://vvs.yanxiufei.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://how.wangdashe.top

C#:   // 手写递归
来源：http://dtt.jqgfzy.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://kal.zycfv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ttl.xylfe.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://llh.jlsjyb.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vkx.fzhhl.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://neo.vqdsnc.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://gfu.vehdjk.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://obv.hfpthk.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://gfj.fengsongda.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kor.ywan-chungtsiang.top

================================================================================
来源：http://vnf.xziqi.cn

O. 并发与异步
来源：http://omd.cheryme.top

================================================================================
来源：http://dgr.yj20258888.top

[O01] 启动一个线程
来源：http://gpm.jinqigfzy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://sgx.ydzc1.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qwy.haohaochexian.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://fcw.vehdjk.com

TS:   // 同 JS
来源：http://nat.andypj.xyz

Java: new Thread(() -> f()).start()
来源：http://rgo.haohaochexian.top

Go:   go f()
来源：http://uep.ydzc1.top

Ruby: Thread.new { f }
来源：http://jig.smart0.xyz

C#:   Task.Run(() => F());
来源：http://rqy.tianlin.xyz

[O02] 使用线程池
来源：http://eyl.yuanzhike.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://qrb.hfpthk.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://bmq.haohaochexian.top

JS:   // worker_threads 线程池
来源：http://udj.yongpay.top

TS:   // worker_threads 线程池
来源：http://llo.xinyue.icu

Java: Executors.newFixedThreadPool(4)
来源：http://ycm.chenzaomai.com

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://xdt.daxiang520.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://tjm.sweek.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://uco.daxiang520.top

[O03] 加锁保护共享数据
来源：http://net.zycfv.cn

Py:   with lock: shared += 1
来源：http://uuw.fktsv.cn

PHP:  // 用 flock() 做文件锁
来源：http://ttq.sjlbkw.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://fss.gaohongyu789.top

TS:   // 同 JS
来源：http://doi.jinqigufen.top

Java: synchronized (this) { shared++; }
来源：http://fat.zhengqikj.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://sqg.cashguo.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://iuz.zhijiandao.cn

C#:   lock (gate) { shared++; }
来源：http://kzv.sxryk.cn

[O04] 定义异步函数并等待
来源：http://yok.zhaomingkeji.xyz

Py:   async def f():⏎    await g()
来源：http://qcb.cdnleiting.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://cxz.hnqzz.top

JS:   async function f() { await g(); }
来源：http://oyz.9152youxi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://abq.jinqigufen.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://tyr.daxiang520.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://nxx.zhaomingkeji.xyz

Ruby: # 用 Fiber 或 async gem
来源：http://ual.tian-w.cn

C#:   async Task F() { await G(); }
来源：http://ftq.shanyushiyangtech.top

[O05] 并发执行并等待全部完成
来源：http://jcj.wangshuangyany.cn

Py:   asyncio.gather(*tasks)
来源：http://kct.dashuyun.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://vip.tarul.cn

JS:   await Promise.all(tasks)
来源：http://ogz.birdmap.top

TS:   await Promise.all(tasks)
来源：http://dmj.shangyingyoupin.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wtp.xylfe.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://rsx.jinyuanbaomall.cn

Ruby: threads.map(&:join)
来源：http://owl.ydjk.org.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xcm.cheryme.top

[O06] 使用进程池
来源：http://qgu.cdnleiting.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://ndx.sjlbkw.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://dgx.sjlbkw.cn

JS:   // child_process / cluster 模块
来源：http://oxg.tian-w.cn

TS:   // child_process / cluster 模块
来源：http://hai.zhaomingkeji.xyz

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://aec.tian-w.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://jcq.yj20258888.top

Ruby: // fork 块
来源：http://kni.zhixingplan.top

C#:   Parallel.For
来源：http://efg.aibaodan.cn

================================================================================
来源：http://lzc.ppjwa.cn

P. 常用工具函数
来源：http://hck.yongpay.top

================================================================================
来源：http://foc.jianghu66.top

[P01] 生成 UUID
来源：http://ofg.fzhhl.top

Py:   str(uuid.uuid4())
来源：http://ylu.yj202588.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://iuq.xuetiantiany.cn

JS:   crypto.randomUUID()
来源：http://iyo.fehbvm.com

TS:   crypto.randomUUID()
来源：http://rxf.gzhubu.top

Java: UUID.randomUUID().toString()
来源：http://qwt.dashuyun.cn

Go:   // 用 github.com/google/uuid
来源：http://rzl.nwbrower.top

Ruby: SecureRandom.uuid
来源：http://ogr.wangdashe.top

C#:   Guid.NewGuid().ToString()
来源：http://rxg.cucudq.cn

[P02] MD5 / SHA256 摘要
来源：http://cfj.yj20258.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gzt.fengsongda.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://rtu.yongpay.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://efn.xinyue.icu

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://pjn.9152youxi.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://npm.fanxiaobao.xyz

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://jtw.fengsongda.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://oxi.hcnkem.com

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://kvh.fehbvm.com

[P03] 生成短随机字符串
来源：http://kya.jiagoushi.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://kfx.dashuyun.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://tkw.zycfv.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://rvn.smart0.xyz

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://gpc.xuanzx.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://ejr.daxiang520.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://keb.redwolf501.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://lts.ehwqpu.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://duo.yueranfly.top

[P04] 求长度
来源：http://esv.xinyue.icu

Py:   len(x)            # 字符串、列表、字典通用
来源：http://gni.hesvh.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jyz.mhx1999.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://hpk.birdmap.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://cwo.yueranfly.top

Java: list.size();  map.size();  s.length()
来源：http://dsz.0kj1m.cn

Go:   len(arr);  len(m)
来源：http://hpc.gotoacloud.top

Ruby: x.length;  x.size
来源：http://fhp.fanxiaobao.xyz

C#:   list.Count;  dict.Count;  s.Length
来源：http://otr.jinqigufen.top

[P05] 判断两个对象内容是否相等
来源：http://lqm.shanyushiyangtech.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://twb.0kj1m.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wgy.sysykeji.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wmj.guowangkeji.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ank.yj20258.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://vou.tian-w.cn

Go:   reflect.DeepEqual(a, b)
来源：http://bky.shuidangran.top

Ruby: a == b
来源：http://quu.shzxlz.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://rqa.pengpengdd.cyou

[P06] 综合判空（null / 空串 / 空集合）
来源：http://jqf.hcnkem.com

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ytz.guannengcc.top

PHP:  if (empty($x)) {}
来源：http://ovv.316326.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://zpo.zdqjudy.top

TS:   if (x == null) {}
来源：http://kfs.ctjpmb.com

Java: if (x == null || x.isEmpty()) {}
来源：http://tqm.nanxinkj.top

Go:   if x == nil {}
来源：http://jbt.chenjidiqi.icu

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://pdh.316326.xyz

C#:   if (x is null) {}
来源：http://krw.yj202588.top

[P07] 防抖与节流
来源：http://skx.gogol.net.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://qyz.sufxvd.cn

PHP:  // 手写时间戳比较
来源：http://itq.tanke756.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://dqj.yuanzhike.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://fbd.hnxiangtu.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://lfg.9152youxi.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://lcp.wangshuangyany.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://cxo.aizwys.cn

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uxb.zdbjq.cn

[P08] 处理浮点精度问题
来源：http://gea.iojbl.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://qfz.ehwqpu.com

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ooy.hfpthk.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://osg.mhx1999.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ogy.wangshuangyany.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ghj.zhongyouzk.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://pxz.yvedp.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ovh.gogol.net.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mvr.hysaishi.cn

================================================================================
来源：http://agv.gaohongyu789.top

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://bim.guannengcc.top

================================================================================
来源：http://jxb.hysaishi.cn

[Q01] 创建表
来源：http://lpu.jyoumei.cn

CREATE TABLE users (
来源：http://ega.xuetiantiany.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hbz.hammf.cn

name VARCHAR(50) NOT NULL,
来源：http://viu.0kj1m.cn

email VARCHAR(100) UNIQUE,
来源：http://cau.yj202588.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://kai.jinqigufen.top

);
来源：http://tlh.kuanghao11.cn

[Q02] 创建带外键的表
来源：http://nmg.shzxlz.cn

CREATE TABLE orders (
来源：http://gbm.nanxinkj.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nzg.xylfe.cn

user_id INT NOT NULL,
来源：http://ikc.chenlongwang.top

amount DECIMAL(10, 2),
来源：http://dqd.daria6918.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tos.ydjk.org.cn

);
来源：http://ufl.tanke756.top

[Q03] 增加列
来源：http://kpa.guannengcc.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jrz.zhoulong.xyz

[Q04] 修改列类型
来源：http://xxf.zycfv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vho.chenzaomai.com

[Q05] 重命名列
来源：http://cll.ehwqpu.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pjf.fzhhl.top

[Q06] 删除列
来源：http://cxk.sweek.top

ALTER TABLE users DROP COLUMN age;
来源：http://usa.nwbrower.top

[Q07] 删除表
来源：http://stw.chenlongwang.top

DROP TABLE IF EXISTS orders;
来源：http://uly.zhixingplan.top

[Q08] 创建普通索引
来源：http://sgs.fehbvm.com

CREATE INDEX idx_users_email ON users(email);
来源：http://oly.ehwqpu.com

[Q09] 创建唯一索引
来源：http://tqp.cucudq.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://kwq.jinqigfzy.top

[Q10] 插入单行
来源：http://csw.guannengcc.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dsr.hongshengwenyu.top

[Q11] 一次插入多行
来源：http://jtu.zhengqikj.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://iyc.iojbl.cn

[Q12] 插入后取自增 ID
来源：http://wzi.shzxlz.cn

INSERT INTO users (name) VALUES ('C');
来源：http://bpe.fktsv.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uja.meibo888.top

[Q13] 忽略重复插入
来源：http://gup.jyoumei.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vkj.chenjidiqi.icu

[Q14] 存在则更新（upsert）
来源：http://ebv.havefunace.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oxi.feifeiyinyue.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nca.ywan-chungtsiang.top

[Q15] 查询全部
来源：http://ftm.wangshuangyany.cn

SELECT * FROM users;
来源：http://kdp.epnwcf.com

[Q16] 查询指定列
来源：http://rqu.xinyue.icu

SELECT id, name FROM users;
来源：http://lny.xziqi.cn

[Q17] 条件查询
来源：http://thv.tanke756.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hog.ydjk.org.cn

[Q18] 模糊匹配
来源：http://wkn.zhijiandao.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://cqv.cheryme.top

[Q19] 范围查询
来源：http://mmg.gzhubu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://puo.iojbl.cn

[Q20] IN 列表
来源：http://ilt.quarkkingdee.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nwk.guowangkeji.top

[Q21] 空值判断
来源：http://fsz.chenjidiqi.icu

SELECT * FROM users WHERE email IS NULL;
来源：http://qcx.epnwcf.com

[Q22] 排序
来源：http://shp.jqgufenzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dtv.zdqjudy.top

[Q23] 分页
来源：http://wbz.9152youxi.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://sgf.iojbl.cn

[Q24] 去重
来源：http://dxq.sjlbkw.cn

SELECT DISTINCT city FROM users;
来源：http://wps.sufxvd.cn

[Q25] 只取前 N 条
来源：http://kbn.redwolf501.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bkm.fehbvm.com

[Q26] 计数
来源：http://gme.fanxiaobao.xyz

SELECT COUNT(*) FROM users;
来源：http://xab.xuanzx.com

[Q27] 条件计数
来源：http://wyo.fzhhl.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://xju.yonumen.top

[Q28] 求和与平均
来源：http://gka.jqgufenzy.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mdh.svipenyu.cn

[Q29] 最大最小值
来源：http://pac.316326.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://xgh.tian-w.cn

[Q30] 分组统计
来源：http://mqa.yongpay.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://bhr.tianlin.xyz

[Q31] 分组后过滤
来源：http://mcv.yonumen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://iac.316326.xyz

[Q32] 分组拼接字符串
来源：http://ida.shzxlz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://fxu.redwolf501.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://spw.9152youxi.cn

[Q33] 多列分组
来源：http://xbj.yfazqb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nbp.uphjek.com

[Q34] 每组取第一条
来源：http://pyi.shangyingyoupin.top

SELECT * FROM (
来源：http://crj.shanyushiyangtech.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://srx.wangdashe.top

) t WHERE rn = 1;
来源：http://lgi.ybcxt.top

[Q35] 内连接
来源：http://tut.meibo888.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kqg.hcnkem.com

[Q36] 左连接
来源：http://vmf.zdqjudy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lzy.xuetiantiany.cn

[Q37] 右连接
来源：http://qkt.cheryme.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://iqj.chenjidiqi.icu

[Q38] 全外连接（PostgreSQL）
来源：http://pyk.ywan-chungtsiang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://rmx.ctjpmb.com

[Q39] 自连接（查上下级）
来源：http://aqc.zhoulong.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://pvo.zhixingplan.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pmk.hywenlv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rmn.ehwqpu.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fcw.xuetiantiany.cn

[Q41] 多表连接
来源：http://dqj.jiagoushi.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://owi.tarul.cn

JOIN users u ON u.id = o.user_id
来源：http://yce.shuidangran.top

JOIN products p ON p.id = o.product_id;
来源：http://vcr.fanxiaobao.xyz

[Q42] 连接条件附加过滤
来源：http://omg.yuxming.cn

SELECT u.name, o.amount FROM users u
来源：http://jki.zhixingplan.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dua.cdnleiting.top

[Q43] 标量子查询
来源：http://djn.yj20258.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lew.dianchejie.cn

[Q44] IN 子查询
来源：http://bmc.xylfe.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://veu.jianghu66.top

[Q45] EXISTS 判断存在
来源：http://edt.jlsjyb.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://qss.xinyue.icu

[Q46] NOT EXISTS 判断不存在
来源：http://fvw.daxiang520.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ree.ydzc1.top

[Q47] 与平均值比较
来源：http://csu.shzxlz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oob.zdbjq.cn

[Q48] CTE 公用表表达式
来源：http://nxk.zdqjudy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tkx.yuxming.cn

SELECT * FROM t WHERE c > 5;
来源：http://xca.guowangkeji.top

[Q49] 更新单行
来源：http://ann.bbcook.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hwi.nwbrower.top

[Q50] 批量更新
来源：http://oru.snrcjt.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gjo.zhiwuduotai.top

[Q51] 用子查询更新
来源：http://zet.cdnleiting.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yaa.yuxming.cn

[Q52] 删除指定行
来源：http://xxs.zdqjudy.top

DELETE FROM users WHERE id = 10;
来源：http://ptg.chenzaomai.com

[Q53] 按条件删除
来源：http://fjo.zhaomingkeji.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qww.bjfxy.top

[Q54] 清空表
来源：http://xyd.pengpengdd.cyou

TRUNCATE TABLE logs;
来源：http://cwm.yangfankeji.com

[Q55] 排名（并列占位）
来源：http://rjy.wangshuangyany.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hfu.snrcjt.cn

[Q56] 密集排名（并列不占位）
来源：http://jog.sysykeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yfk.9152youxi.cn

[Q57] 行号
来源：http://dhf.hnxiangtu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wme.ydjk.org.cn

[Q58] 累计求和
来源：http://dhn.svipenyu.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wtz.sxryk.cn

[Q59] 分组内累计
来源：http://keo.zhoulong.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://gmz.zycfv.cn

[Q60] 取上一行 / 下一行
来源：http://huc.yuanzhike.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://eum.yfazqb.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dzo.c1oappe.top

[Q61] 移动平均
来源：http://ixn.52xcode.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://icg.sxryk.cn

[Q62] 分组占比
来源：http://qwm.fengsongda.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qhw.jinyuanbaomall.cn

[Q63] 开启事务
来源：http://qag.hesvh.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wpg.nwbrower.top

[Q64] 提交事务
来源：http://xgg.zycfv.cn

COMMIT;
来源：http://xwg.pycfn.com

[Q65] 回滚事务
来源：http://adh.nwbrower.top

ROLLBACK;
来源：http://rjx.0kj1m.cn

[Q66] 行锁查询
来源：http://hsx.ywan-chungtsiang.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uhs.nanxuanxn.top


<!-- 参考信息 -->