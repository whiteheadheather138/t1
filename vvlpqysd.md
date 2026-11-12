代发 wailian999

PHP:  // 手写递归函数
来源：http://chg.c1oappe.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://snu.shanyushiyangtech.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://nvm.smart0.xyz

Java: // 手写递归
来源：http://gtf.hcnkem.com

Go:   // 手写递归
来源：http://idr.zhijiandao.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hmv.hesvh.cn

C#:   // 手写递归
来源：http://wpz.xuanzx.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://bak.yanxiufei.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://qnt.hnxiangtu.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://pss.yuxming.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://ybn.chenlongwang.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mnd.vqdsnc.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://lew.dianchejie.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mwn.kuanghao11.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vud.ehwqpu.com

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://lbr.jinqigufen.top

================================================================================
来源：http://fkc.zhaomingkeji.xyz

O. 并发与异步
来源：http://anq.zhiwuduotai.top

================================================================================
来源：http://nxy.zhengqikj.top

[O01] 启动一个线程
来源：http://yvq.xuetiantiany.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://gnh.pycfn.com

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://fhe.gogol.net.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ioz.wangshuangyany.cn

TS:   // 同 JS
来源：http://joh.nwbrower.top

Java: new Thread(() -> f()).start()
来源：http://buk.c1oappe.top

Go:   go f()
来源：http://ixu.yueranfly.top

Ruby: Thread.new { f }
来源：http://top.cdnleiting.top

C#:   Task.Run(() => F());
来源：http://vir.zhiwuduotai.top

[O02] 使用线程池
来源：http://gdp.epnwcf.com

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cuk.guowangkeji.top

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://kld.shzxlz.cn

JS:   // worker_threads 线程池
来源：http://svl.shuidangran.top

TS:   // worker_threads 线程池
来源：http://mzt.xuetiantiany.cn

Java: Executors.newFixedThreadPool(4)
来源：http://pyb.bjfxy.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hzh.316326.xyz

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wpg.zdqjudy.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://otl.ctjpmb.com

[O03] 加锁保护共享数据
来源：http://arp.wangdashe.top

Py:   with lock: shared += 1
来源：http://tlo.yangfankeji.com

PHP:  // 用 flock() 做文件锁
来源：http://uqj.cqqwz.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://jdq.bjfxy.top

TS:   // 同 JS
来源：http://fri.hfpthk.cn

Java: synchronized (this) { shared++; }
来源：http://mcz.yuxming.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://gce.feifeiyinyue.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://smk.gotoacloud.top

C#:   lock (gate) { shared++; }
来源：http://jgy.yj20258888.top

[O04] 定义异步函数并等待
来源：http://fun.yj20258.top

Py:   async def f():⏎    await g()
来源：http://qys.hnqzz.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://bcr.daria6918.cn

JS:   async function f() { await g(); }
来源：http://iec.jinyuanbaomall.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://bgv.feifeiyinyue.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://jzm.zycfv.cn

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xwm.jianghu66.top

Ruby: # 用 Fiber 或 async gem
来源：http://vop.zhongyouzk.top

C#:   async Task F() { await G(); }
来源：http://gmj.ivvv.top

[O05] 并发执行并等待全部完成
来源：http://wol.zhaomingkeji.xyz

Py:   asyncio.gather(*tasks)
来源：http://wdl.hcnkem.com

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://cbc.bbcook.cn

JS:   await Promise.all(tasks)
来源：http://zkx.yangfankeji.com

TS:   await Promise.all(tasks)
来源：http://xdy.jinghuilouyu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://zvb.c1oappe.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://yqe.jianghu66.top

Ruby: threads.map(&:join)
来源：http://izp.birdmap.top

C#:   await Task.WhenAll(t1, t2)
来源：http://kwt.jianghu66.top

[O06] 使用进程池
来源：http://bqd.jinyuanbaomall.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://zgt.chenlongwang.top

PHP:  // pcntl_fork 或多进程队列
来源：http://yyo.zhiwuduotai.top

JS:   // child_process / cluster 模块
来源：http://uvx.9152youxi.cn

TS:   // child_process / cluster 模块
来源：http://jlo.yfazqb.com

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://pzn.ywan-chungtsiang.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://kuu.hammf.cn

Ruby: // fork 块
来源：http://lyv.dianchejie.cn

C#:   Parallel.For
来源：http://kqz.hammf.cn

================================================================================
来源：http://top.daxiang520.top

P. 常用工具函数
来源：http://fsh.chenjidiqi.icu

================================================================================
来源：http://noj.ivvv.top

[P01] 生成 UUID
来源：http://xws.jinyuanbaomall.cn

Py:   str(uuid.uuid4())
来源：http://clj.birdmap.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://yhx.shangyingyoupin.top

JS:   crypto.randomUUID()
来源：http://skm.xuetiantiany.cn

TS:   crypto.randomUUID()
来源：http://qvf.xuanzx.com

Java: UUID.randomUUID().toString()
来源：http://xqs.jinyuanbaomall.cn

Go:   // 用 github.com/google/uuid
来源：http://lgi.chenjidiqi.icu

Ruby: SecureRandom.uuid
来源：http://xxy.sysykeji.top

C#:   Guid.NewGuid().ToString()
来源：http://fph.yuanzhike.top

[P02] MD5 / SHA256 摘要
来源：http://kcz.chenlongwang.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://gxe.hnqzz.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://yaa.iojbl.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://dtp.ybcxt.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://emr.zhaomingkeji.xyz

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://dsv.ydzc1.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://fwl.jqgfzy.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wic.dashuyun.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://jza.jlsjyb.cn

[P03] 生成短随机字符串
来源：http://fgp.jiagoushi.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://sew.ctjpmb.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://vop.havefunace.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://llp.tanke756.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://szu.pycfn.com

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://svg.zdbjq.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://lpk.gotoacloud.top

Ruby: SecureRandom.alphanumeric(16)
来源：http://tag.hnxiangtu.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://nji.sxryk.cn

[P04] 求长度
来源：http://yqs.xuetiantiany.cn

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bwp.yuxming.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xgu.birdmap.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://lgh.birdmap.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://yso.xingfuxueyuan.xyz

Java: list.size();  map.size();  s.length()
来源：http://epa.jianghu66.top

Go:   len(arr);  len(m)
来源：http://qda.yfazqb.com

Ruby: x.length;  x.size
来源：http://kdi.shzxlz.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://lag.jiagoushi.top

[P05] 判断两个对象内容是否相等
来源：http://cfa.ywan-chungtsiang.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://qby.dianchejie.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://lad.shuidangran.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://gbr.guannengcc.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://ymn.9152youxi.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://kys.meibo888.top

Go:   reflect.DeepEqual(a, b)
来源：http://ths.sysykeji.top

Ruby: a == b
来源：http://xks.sxryk.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://fae.jyoumei.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ciz.jinqigfzy.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rgr.hcnkem.com

PHP:  if (empty($x)) {}
来源：http://rpi.nanxinkj.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://uqf.zhoulong.xyz

TS:   if (x == null) {}
来源：http://uju.nwbrower.top

Java: if (x == null || x.isEmpty()) {}
来源：http://kxa.zhijiandao.cn

Go:   if x == nil {}
来源：http://une.yanxiufei.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dcb.hfpthk.cn

C#:   if (x is null) {}
来源：http://gav.ivvv.top

[P07] 防抖与节流
来源：http://bmz.daria6918.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://lan.iojbl.cn

PHP:  // 手写时间戳比较
来源：http://dom.fktsv.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://sfg.fehbvm.com

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://brc.yj202588.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://czf.zhoulong.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://udm.dianchejie.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://nyi.tanke756.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://noe.mhx1999.top

[P08] 处理浮点精度问题
来源：http://vjb.xingfuxueyuan.xyz

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wjy.daxiang520.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://jow.meibo888.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://xrb.ydzc1.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://thc.yfazqb.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://spd.jinqigfzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://xug.9152youxi.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://xwv.sjlbkw.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://kkr.ivvv.top

================================================================================
来源：http://qzk.tianlin.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://qpl.chenjidiqi.icu

================================================================================
来源：http://czf.tarul.cn

[Q01] 创建表
来源：http://atk.xingfuxueyuan.xyz

CREATE TABLE users (
来源：http://dib.kuanghao11.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://drv.meibo888.top

name VARCHAR(50) NOT NULL,
来源：http://sif.jianghu66.top

email VARCHAR(100) UNIQUE,
来源：http://vjp.xuanzx.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vhc.xinyue.icu

);
来源：http://sak.cashguo.top

[Q02] 创建带外键的表
来源：http://cvl.uphjek.com

CREATE TABLE orders (
来源：http://qrr.hesvh.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://utb.redwolf501.top

user_id INT NOT NULL,
来源：http://gaz.jqgufenzy.top

amount DECIMAL(10, 2),
来源：http://lgb.316326.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://rrx.dianchejie.cn

);
来源：http://cmi.pycfn.com

[Q03] 增加列
来源：http://ftc.chenzaomai.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jky.aibaodan.cn

[Q04] 修改列类型
来源：http://els.zdbjq.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ujo.fktsv.cn

[Q05] 重命名列
来源：http://ucs.cheryme.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://zys.zhoulong.xyz

[Q06] 删除列
来源：http://oai.sysykeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://pad.fanxiaobao.xyz

[Q07] 删除表
来源：http://mdv.yuxming.cn

DROP TABLE IF EXISTS orders;
来源：http://bzw.yuanzhike.top

[Q08] 创建普通索引
来源：http://uij.yonumen.top

CREATE INDEX idx_users_email ON users(email);
来源：http://tsc.yonumen.top

[Q09] 创建唯一索引
来源：http://mkf.aibaodan.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bfw.ppjwa.cn

[Q10] 插入单行
来源：http://mlm.vqdsnc.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ree.zdbjq.cn

[Q11] 一次插入多行
来源：http://khu.shuidangran.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://jyi.hnqzz.top

[Q12] 插入后取自增 ID
来源：http://wvi.ybcxt.top

INSERT INTO users (name) VALUES ('C');
来源：http://cha.sxryk.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hns.uphjek.com

[Q13] 忽略重复插入
来源：http://pyw.cdnleiting.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ocy.fktsv.cn

[Q14] 存在则更新（upsert）
来源：http://pye.quarkkingdee.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xnr.pengpengdd.cyou

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://asn.jiagoushi.top

[Q15] 查询全部
来源：http://oqv.ehwqpu.com

SELECT * FROM users;
来源：http://mkt.tian-w.cn

[Q16] 查询指定列
来源：http://xqg.jqgfzy.top

SELECT id, name FROM users;
来源：http://gjz.uphjek.com

[Q17] 条件查询
来源：http://lpx.feifeiyinyue.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mnt.jinyuanbaomall.cn

[Q18] 模糊匹配
来源：http://vyg.hysaishi.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://lth.yanxiufei.cn

[Q19] 范围查询
来源：http://mly.pengpengdd.cyou

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bvm.316326.xyz

[Q20] IN 列表
来源：http://cmm.hfpthk.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jev.jinqigfzy.top

[Q21] 空值判断
来源：http://ohy.zhixingplan.top

SELECT * FROM users WHERE email IS NULL;
来源：http://cqu.uphjek.com

[Q22] 排序
来源：http://mmy.hongshengwenyu.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qpy.shanyushiyangkeji.top

[Q23] 分页
来源：http://pbh.svipenyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gro.shzxlz.cn

[Q24] 去重
来源：http://kjh.andypj.xyz

SELECT DISTINCT city FROM users;
来源：http://sud.yfazqb.com

[Q25] 只取前 N 条
来源：http://fgf.guowangkeji.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://hhp.hnxiangtu.top

[Q26] 计数
来源：http://srn.hcnkem.com

SELECT COUNT(*) FROM users;
来源：http://iif.zdqjudy.top

[Q27] 条件计数
来源：http://fls.jinyuanbaomall.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rmh.chenzaomai.com

[Q28] 求和与平均
来源：http://wsh.gaohongyu789.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pcv.redwolf501.top

[Q29] 最大最小值
来源：http://tai.redwolf501.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ipr.xziqi.cn

[Q30] 分组统计
来源：http://sfr.chenzaomai.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mcw.jqgfzy.top

[Q31] 分组后过滤
来源：http://qzm.yj20258.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kyk.mhx1999.top

[Q32] 分组拼接字符串
来源：http://ton.jinghuilouyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vgr.hysaishi.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://pxl.sufxvd.cn

[Q33] 多列分组
来源：http://vcs.mhx1999.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wie.epnwcf.com

[Q34] 每组取第一条
来源：http://sgb.shanyushiyangtech.top

SELECT * FROM (
来源：http://udz.ivvv.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tbk.uphjek.com

) t WHERE rn = 1;
来源：http://zkz.redwolf501.top

[Q35] 内连接
来源：http://bgv.jiagoushi.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bdp.ehwqpu.com

[Q36] 左连接
来源：http://yim.redwolf501.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kxt.guowangkeji.top

[Q37] 右连接
来源：http://zgj.mhx1999.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://phu.fanxiaobao.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://czx.jinqigufen.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wob.shanyushiyangkeji.top

[Q39] 自连接（查上下级）
来源：http://ofh.shangyingyoupin.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://smv.cheryme.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hol.zhengqikj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://kzz.ivvv.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zib.ppjwa.cn

[Q41] 多表连接
来源：http://tux.iojbl.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qtb.zhijiandao.cn

JOIN users u ON u.id = o.user_id
来源：http://fau.hywenlv.cn

JOIN products p ON p.id = o.product_id;
来源：http://pio.xylfe.cn

[Q42] 连接条件附加过滤
来源：http://auf.svipenyu.cn

SELECT u.name, o.amount FROM users u
来源：http://zor.cucudq.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://gqe.shzxlz.cn

[Q43] 标量子查询
来源：http://ded.yuanzhike.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cdf.zhijiandao.cn

[Q44] IN 子查询
来源：http://ycs.gotoacloud.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ntk.daria6918.cn

[Q45] EXISTS 判断存在
来源：http://lrm.vehdjk.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xon.ybcxt.top

[Q46] NOT EXISTS 判断不存在
来源：http://gmb.gogol.net.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gxn.fanxiaobao.xyz

[Q47] 与平均值比较
来源：http://ppv.aibaodan.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fay.guannengcc.top

[Q48] CTE 公用表表达式
来源：http://las.feifeiyinyue.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xhn.epnwcf.com

SELECT * FROM t WHERE c > 5;
来源：http://dmt.cashguo.top

[Q49] 更新单行
来源：http://zfm.daria6918.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://sas.haohaochexian.top

[Q50] 批量更新
来源：http://smx.zhengqikj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hrl.dashuyun.cn

[Q51] 用子查询更新
来源：http://hmc.hesvh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hrp.jqgufenzy.top

[Q52] 删除指定行
来源：http://xlq.nwbrower.top

DELETE FROM users WHERE id = 10;
来源：http://kac.yuxming.cn

[Q53] 按条件删除
来源：http://xuw.gogol.net.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://vve.nwbrower.top

[Q54] 清空表
来源：http://hti.zdqjudy.top

TRUNCATE TABLE logs;
来源：http://puj.yueranfly.top

[Q55] 排名（并列占位）
来源：http://xla.ywan-chungtsiang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://skg.hcnkem.com

[Q56] 密集排名（并列不占位）
来源：http://blw.kuanghao11.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://acs.52xcode.cn

[Q57] 行号
来源：http://xem.xuanzx.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kpy.316326.xyz

[Q58] 累计求和
来源：http://tte.fehbvm.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ekb.xingfuxueyuan.xyz

[Q59] 分组内累计
来源：http://mja.yonumen.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jij.xingfuxueyuan.xyz

[Q60] 取上一行 / 下一行
来源：http://dxs.xingfuxueyuan.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oii.bjfxy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uep.yj202588.top

[Q61] 移动平均
来源：http://wha.zdbjq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mzf.dianchejie.cn

[Q62] 分组占比
来源：http://jom.chenzaomai.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hzd.gogol.net.cn

[Q63] 开启事务
来源：http://zko.vqdsnc.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://udt.yj202588.top

[Q64] 提交事务
来源：http://uoa.zhengqikj.top

COMMIT;
来源：http://vuu.zhaomingkeji.xyz


<!-- 参考信息 -->