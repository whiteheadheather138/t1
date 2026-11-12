代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://qyz.pycfn.com

C#:   class Node { public int V; public Node? Next; }
来源：http://ydr.yj202588.top

[N11] 二叉树中序遍历
来源：http://zvu.jinqigufen.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://lqj.vqdsnc.cn

PHP:  // 手写递归函数
来源：http://mzt.gaohongyu789.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yqc.hongshengwenyu.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://rkc.sxryk.cn

Java: // 手写递归
来源：http://hvi.hesvh.cn

Go:   // 手写递归
来源：http://jmv.ydjk.org.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://ukw.tanke756.top

C#:   // 手写递归
来源：http://jkk.nwbrower.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://ckq.shuidangran.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://njz.jqgufenzy.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://clc.zdqjudy.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://uve.cashguo.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fnh.hnxiangtu.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://xhd.gogol.net.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://qsj.haohaochexian.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://pqi.yj202588.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://spw.xingfuxueyuan.xyz

================================================================================
来源：http://eyx.svipenyu.cn

O. 并发与异步
来源：http://rak.gzhubu.top

================================================================================
来源：http://jkt.fzhhl.top

[O01] 启动一个线程
来源：http://qvi.yj20258.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://bsn.fktsv.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kwe.daria6918.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://cjq.zhengqikj.top

TS:   // 同 JS
来源：http://ted.gotoacloud.top

Java: new Thread(() -> f()).start()
来源：http://mct.tarul.cn

Go:   go f()
来源：http://sln.zdqjudy.top

Ruby: Thread.new { f }
来源：http://xca.ivvv.top

C#:   Task.Run(() => F());
来源：http://pal.52xcode.cn

[O02] 使用线程池
来源：http://ffp.gzhubu.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://zgb.hesvh.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://cmy.zhongyouzk.top

JS:   // worker_threads 线程池
来源：http://buo.nanxinkj.top

TS:   // worker_threads 线程池
来源：http://yfy.cheryme.top

Java: Executors.newFixedThreadPool(4)
来源：http://uir.c1oappe.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://lea.haohaochexian.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://swx.shzxlz.cn

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://fnc.yanxiufei.cn

[O03] 加锁保护共享数据
来源：http://qel.sxryk.cn

Py:   with lock: shared += 1
来源：http://cnj.svipenyu.cn

PHP:  // 用 flock() 做文件锁
来源：http://xdb.hesvh.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gct.sweek.top

TS:   // 同 JS
来源：http://ldi.zhoulong.xyz

Java: synchronized (this) { shared++; }
来源：http://axb.xingfuxueyuan.xyz

Go:   mu.Lock();  defer mu.Unlock()
来源：http://fse.ydjk.org.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://obv.pengpengdd.cyou

C#:   lock (gate) { shared++; }
来源：http://wcu.cucudq.cn

[O04] 定义异步函数并等待
来源：http://aat.c1oappe.top

Py:   async def f():⏎    await g()
来源：http://hus.bjfxy.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://lsd.yvedp.cn

JS:   async function f() { await g(); }
来源：http://cph.andypj.xyz

TS:   async function f(): Promise<void> { await g(); }
来源：http://uwo.yonumen.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://trn.xuanzx.com

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://bui.nwbrower.top

Ruby: # 用 Fiber 或 async gem
来源：http://yia.shanyushiyangtech.top

C#:   async Task F() { await G(); }
来源：http://vrv.shangyingyoupin.top

[O05] 并发执行并等待全部完成
来源：http://lrk.yuanzhike.top

Py:   asyncio.gather(*tasks)
来源：http://vys.jinqigfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://ood.mhx1999.top

JS:   await Promise.all(tasks)
来源：http://xpf.shzxlz.cn

TS:   await Promise.all(tasks)
来源：http://bcu.chenzaomai.com

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://qzt.ybcxt.top

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://sua.gzhubu.top

Ruby: threads.map(&:join)
来源：http://jzg.haohaochexian.top

C#:   await Task.WhenAll(t1, t2)
来源：http://jlj.feifeiyinyue.top

[O06] 使用进程池
来源：http://lfe.hcnkem.com

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wwq.pycfn.com

PHP:  // pcntl_fork 或多进程队列
来源：http://zlx.smart0.xyz

JS:   // child_process / cluster 模块
来源：http://buh.bbcook.cn

TS:   // child_process / cluster 模块
来源：http://qxs.xylfe.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://soh.meibo888.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://vbn.jlsjyb.cn

Ruby: // fork 块
来源：http://syc.xylfe.cn

C#:   Parallel.For
来源：http://ume.feifeiyinyue.top

================================================================================
来源：http://yep.hesvh.cn

P. 常用工具函数
来源：http://qwe.jqgfzy.top

================================================================================
来源：http://vmh.shanyushiyangtech.top

[P01] 生成 UUID
来源：http://rin.yj20258.top

Py:   str(uuid.uuid4())
来源：http://fmb.tian-w.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mvi.kuanghao11.cn

JS:   crypto.randomUUID()
来源：http://lyt.shzxlz.cn

TS:   crypto.randomUUID()
来源：http://bkl.tianlin.xyz

Java: UUID.randomUUID().toString()
来源：http://ofm.haohaochexian.top

Go:   // 用 github.com/google/uuid
来源：http://idg.9152youxi.cn

Ruby: SecureRandom.uuid
来源：http://wld.quarkkingdee.top

C#:   Guid.NewGuid().ToString()
来源：http://uar.gotoacloud.top

[P02] MD5 / SHA256 摘要
来源：http://bwa.zhengqikj.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ybr.yangfankeji.com

PHP:  hash("sha256", $s);  md5($s);
来源：http://wpp.epnwcf.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://vrh.tarul.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://muc.yongpay.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blq.zhongyouzk.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://cgm.yuanzhike.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://zqt.meibo888.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://eyo.ehwqpu.com

[P03] 生成短随机字符串
来源：http://ziz.chenlongwang.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://xhz.haohaochexian.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://bbv.svipenyu.cn

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hjv.redwolf501.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://bhi.shzxlz.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://zja.tian-w.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://iyp.sxryk.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tay.xinyue.icu

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://xue.jinqigufen.top

[P04] 求长度
来源：http://dzi.nanxinkj.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://uyl.shuidangran.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zmk.tian-w.cn

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://kan.ivvv.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://zpv.cheryme.top

Java: list.size();  map.size();  s.length()
来源：http://jtm.wangshuangyany.cn

Go:   len(arr);  len(m)
来源：http://rdm.yueranfly.top

Ruby: x.length;  x.size
来源：http://tcu.fehbvm.com

C#:   list.Count;  dict.Count;  s.Length
来源：http://bma.xuetiantiany.cn

[P05] 判断两个对象内容是否相等
来源：http://wqr.tarul.cn

Py:   a == b              # 列表与字典递归比较内容
来源：http://bwg.zhijiandao.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://cjy.cheryme.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://izm.gzhubu.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://pyj.shuidangran.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mme.snrcjt.cn

Go:   reflect.DeepEqual(a, b)
来源：http://aiz.zhijiandao.cn

Ruby: a == b
来源：http://uyj.tianlin.xyz

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://smf.dianchejie.cn

[P06] 综合判空（null / 空串 / 空集合）
来源：http://aql.tianlin.xyz

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://vrv.chenzaomai.com

PHP:  if (empty($x)) {}
来源：http://bdl.tian-w.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://qla.xuetiantiany.cn

TS:   if (x == null) {}
来源：http://azm.9152youxi.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://nvg.jlsjyb.cn

Go:   if x == nil {}
来源：http://akr.shanyushiyangtech.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://fck.zdqjudy.top

C#:   if (x is null) {}
来源：http://qfp.sufxvd.cn

[P07] 防抖与节流
来源：http://nra.fehbvm.com

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://ddq.jinqigufen.top

PHP:  // 手写时间戳比较
来源：http://ccn.cdnleiting.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://tvu.xziqi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://oes.jiagoushi.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://yhv.mhx1999.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://uyy.birdmap.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://qhh.zhongyouzk.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://uyy.sysykeji.top

[P08] 处理浮点精度问题
来源：http://zxo.ppjwa.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://bmk.xuetiantiany.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ubb.cheryme.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://gdf.yonumen.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://vap.zhengqikj.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ixn.jinyuanbaomall.cn

Go:   math/big.Float，或全部换算成整数分再算
来源：http://vuw.zdqjudy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://ttb.redwolf501.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://rjz.jiagoushi.top

================================================================================
来源：http://dyc.xuetiantiany.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://gsr.jinqigufen.top

================================================================================
来源：http://fyb.sufxvd.cn

[Q01] 创建表
来源：http://uwr.daxiang520.top

CREATE TABLE users (
来源：http://xvv.sxryk.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://zsb.jlsjyb.cn

name VARCHAR(50) NOT NULL,
来源：http://utt.jyoumei.cn

email VARCHAR(100) UNIQUE,
来源：http://drp.dashuyun.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://qpc.xuanzx.com

);
来源：http://zyw.zhoulong.xyz

[Q02] 创建带外键的表
来源：http://ugx.feifeiyinyue.top

CREATE TABLE orders (
来源：http://upm.yvedp.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://liy.chenjidiqi.icu

user_id INT NOT NULL,
来源：http://igg.zhongyouzk.top

amount DECIMAL(10, 2),
来源：http://hve.nanxinkj.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ejt.smart0.xyz

);
来源：http://rwv.yuanzhike.top

[Q03] 增加列
来源：http://znt.redwolf501.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://kyn.havefunace.top

[Q04] 修改列类型
来源：http://ity.ctjpmb.com

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://cvp.vehdjk.com

[Q05] 重命名列
来源：http://qfk.hongshengwenyu.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://tjh.gogol.net.cn

[Q06] 删除列
来源：http://voc.shangyingyoupin.top

ALTER TABLE users DROP COLUMN age;
来源：http://swv.jyoumei.cn

[Q07] 删除表
来源：http://yhx.feifeiyinyue.top

DROP TABLE IF EXISTS orders;
来源：http://ddf.nanxuanxn.top

[Q08] 创建普通索引
来源：http://oqf.cdnleiting.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hfz.quarkkingdee.top

[Q09] 创建唯一索引
来源：http://qkz.jinqigufen.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rsh.tian-w.cn

[Q10] 插入单行
来源：http://oii.daxiang520.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://qgl.0kj1m.cn

[Q11] 一次插入多行
来源：http://tbx.ehwqpu.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wjr.andypj.xyz

[Q12] 插入后取自增 ID
来源：http://waq.jinqigfzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://gop.jinqigfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://hsa.nwbrower.top

[Q13] 忽略重复插入
来源：http://plh.hysaishi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oho.gotoacloud.top

[Q14] 存在则更新（upsert）
来源：http://nzy.uphjek.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tej.redwolf501.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wvp.wangshuangyany.cn

[Q15] 查询全部
来源：http://qkw.zhiwuduotai.top

SELECT * FROM users;
来源：http://qll.zhoulong.xyz

[Q16] 查询指定列
来源：http://sre.hongshengwenyu.top

SELECT id, name FROM users;
来源：http://esp.cucudq.cn

[Q17] 条件查询
来源：http://mdk.bjfxy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://umd.ctjpmb.com

[Q18] 模糊匹配
来源：http://oxx.xingfuxueyuan.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vkp.cucudq.cn

[Q19] 范围查询
来源：http://rtm.hesvh.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wps.havefunace.top

[Q20] IN 列表
来源：http://vas.zdbjq.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bfw.fzhhl.top

[Q21] 空值判断
来源：http://hfz.nanxuanxn.top

SELECT * FROM users WHERE email IS NULL;
来源：http://kvn.zhixingplan.top

[Q22] 排序
来源：http://lvg.chenzaomai.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://nib.shangyingyoupin.top

[Q23] 分页
来源：http://kwz.fzhhl.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ahv.ppjwa.cn

[Q24] 去重
来源：http://jvq.zhoulong.xyz

SELECT DISTINCT city FROM users;
来源：http://law.hesvh.cn

[Q25] 只取前 N 条
来源：http://pnj.zhoulong.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zqj.dianchejie.cn

[Q26] 计数
来源：http://vxx.hcnkem.com

SELECT COUNT(*) FROM users;
来源：http://vvy.ivvv.top

[Q27] 条件计数
来源：http://iju.fktsv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qbs.zdqjudy.top

[Q28] 求和与平均
来源：http://tkw.0kj1m.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://sgg.xuetiantiany.cn

[Q29] 最大最小值
来源：http://jgg.guowangkeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://azx.sxryk.cn

[Q30] 分组统计
来源：http://rfp.quarkkingdee.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://cgd.ppjwa.cn

[Q31] 分组后过滤
来源：http://ilr.fehbvm.com

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://qfz.zycfv.cn

[Q32] 分组拼接字符串
来源：http://ylp.jyoumei.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://idv.ywan-chungtsiang.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://lpl.chenjidiqi.icu

[Q33] 多列分组
来源：http://kyl.yanxiufei.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cdb.yfazqb.com

[Q34] 每组取第一条
来源：http://muc.gogol.net.cn

SELECT * FROM (
来源：http://kgf.mhx1999.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ail.vehdjk.com

) t WHERE rn = 1;
来源：http://snm.xingfuxueyuan.xyz

[Q35] 内连接
来源：http://wyf.xinyue.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://zqp.gaohongyu789.top

[Q36] 左连接
来源：http://bqi.jinqigufen.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://twc.316326.xyz

[Q37] 右连接
来源：http://aaq.birdmap.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://pkj.zycfv.cn

[Q38] 全外连接（PostgreSQL）
来源：http://udy.kuanghao11.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tpi.jianghu66.top

[Q39] 自连接（查上下级）
来源：http://bgs.jiagoushi.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://awy.hysaishi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://swo.mhx1999.top

[Q40] 交叉连接（笛卡尔积）
来源：http://umb.ctjpmb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bma.jyoumei.cn

[Q41] 多表连接
来源：http://lfv.xingfuxueyuan.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://cvq.ppjwa.cn

JOIN users u ON u.id = o.user_id
来源：http://tlw.andypj.xyz

JOIN products p ON p.id = o.product_id;
来源：http://tdl.xingfuxueyuan.xyz

[Q42] 连接条件附加过滤
来源：http://pcc.shzxlz.cn

SELECT u.name, o.amount FROM users u
来源：http://kph.guowangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hym.ybcxt.top

[Q43] 标量子查询
来源：http://lkp.ppjwa.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hzm.nwbrower.top

[Q44] IN 子查询
来源：http://nzx.gaohongyu789.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pwf.nanxuanxn.top

[Q45] EXISTS 判断存在
来源：http://kgu.pycfn.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dvj.cheryme.top

[Q46] NOT EXISTS 判断不存在
来源：http://etb.ehwqpu.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mno.andypj.xyz

[Q47] 与平均值比较
来源：http://mjs.jqgufenzy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://caa.yangfankeji.com

[Q48] CTE 公用表表达式
来源：http://kma.vehdjk.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uln.yuxming.cn

SELECT * FROM t WHERE c > 5;
来源：http://ndq.cucudq.cn

[Q49] 更新单行
来源：http://ihl.zdbjq.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ggz.yangfankeji.com

[Q50] 批量更新
来源：http://bfm.jinghuilouyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ksh.iojbl.cn

[Q51] 用子查询更新
来源：http://tqu.uphjek.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://eyr.cucudq.cn

[Q52] 删除指定行
来源：http://wms.xziqi.cn

DELETE FROM users WHERE id = 10;
来源：http://mdn.yongpay.top

[Q53] 按条件删除
来源：http://byu.xuetiantiany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xxu.wangshuangyany.cn

[Q54] 清空表
来源：http://gkj.xuanzx.com

TRUNCATE TABLE logs;
来源：http://ngl.xuetiantiany.cn

[Q55] 排名（并列占位）
来源：http://rgd.bbcook.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yxj.fzhhl.top

[Q56] 密集排名（并列不占位）
来源：http://xhr.xinyue.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hsg.daxiang520.top

[Q57] 行号
来源：http://xpn.jlsjyb.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hsd.shanyushiyangkeji.top

[Q58] 累计求和
来源：http://cli.shzxlz.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nsc.jinghuilouyu.cn

[Q59] 分组内累计
来源：http://prr.zhixingplan.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://olv.jinyuanbaomall.cn

[Q60] 取上一行 / 下一行
来源：http://lup.yvedp.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xtl.fengsongda.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qlf.cucudq.cn

[Q61] 移动平均
来源：http://yyo.ybcxt.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nne.hysaishi.cn

[Q62] 分组占比
来源：http://jll.zycfv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://nwj.daxiang520.top


<!-- 参考信息 -->