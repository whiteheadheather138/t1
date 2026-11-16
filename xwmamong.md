代发 wailian999

PHP:  // 手写递归函数
来源：http://tbf.andypj.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://oof.52xcode.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wdm.ywan-chungtsiang.top

Java: // 手写递归
来源：http://joh.ydjk.org.cn

Go:   // 手写递归
来源：http://soo.52xcode.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://skm.haohaochexian.top

C#:   // 手写递归
来源：http://tmo.jinghuilouyu.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://urr.fktsv.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://oxl.ybcxt.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://hlk.yonumen.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vjw.xylfe.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://rer.cdnleiting.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mzl.sweek.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gxv.cashguo.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://ubm.hongshengwenyu.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://fdu.yj20258888.top

================================================================================
来源：http://mnn.hnxiangtu.top

O. 并发与异步
来源：http://nll.yanxiufei.cn

================================================================================
来源：http://fzu.jinqigfzy.top

[O01] 启动一个线程
来源：http://okf.316326.xyz

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://nzh.hesvh.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://kxv.snrcjt.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://gwj.chenzaomai.com

TS:   // 同 JS
来源：http://wvp.wangshuangyany.cn

Java: new Thread(() -> f()).start()
来源：http://bcr.yongpay.top

Go:   go f()
来源：http://rte.quarkkingdee.top

Ruby: Thread.new { f }
来源：http://smm.9152youxi.cn

C#:   Task.Run(() => F());
来源：http://gyd.yanxiufei.cn

[O02] 使用线程池
来源：http://uvu.cashguo.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://cha.sufxvd.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://nfg.zhoulong.xyz

JS:   // worker_threads 线程池
来源：http://atf.cheryme.top

TS:   // worker_threads 线程池
来源：http://pfq.aibaodan.cn

Java: Executors.newFixedThreadPool(4)
来源：http://awa.gzhubu.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://hsh.shanyushiyangtech.top

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dsp.gotoacloud.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://clq.tanke756.top

[O03] 加锁保护共享数据
来源：http://gke.hfpthk.cn

Py:   with lock: shared += 1
来源：http://bue.nwbrower.top

PHP:  // 用 flock() 做文件锁
来源：http://rkd.zhiwuduotai.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gal.jqgufenzy.top

TS:   // 同 JS
来源：http://qug.316326.xyz

Java: synchronized (this) { shared++; }
来源：http://ljd.ctjpmb.com

Go:   mu.Lock();  defer mu.Unlock()
来源：http://vox.quarkkingdee.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://ybg.mhx1999.top

C#:   lock (gate) { shared++; }
来源：http://sto.smart0.xyz

[O04] 定义异步函数并等待
来源：http://ewd.iojbl.cn

Py:   async def f():⏎    await g()
来源：http://yrl.yanxiufei.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://iku.bjfxy.top

JS:   async function f() { await g(); }
来源：http://vrt.fzhhl.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://qln.meibo888.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://xmh.chenlongwang.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://xed.yfazqb.com

Ruby: # 用 Fiber 或 async gem
来源：http://gzi.birdmap.top

C#:   async Task F() { await G(); }
来源：http://ole.fengsongda.top

[O05] 并发执行并等待全部完成
来源：http://osa.jlsjyb.cn

Py:   asyncio.gather(*tasks)
来源：http://pbs.hywenlv.cn

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://gew.ctjpmb.com

JS:   await Promise.all(tasks)
来源：http://fhh.iojbl.cn

TS:   await Promise.all(tasks)
来源：http://pkx.yj20258888.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://ipf.cqqwz.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://znj.pengpengdd.cyou

Ruby: threads.map(&:join)
来源：http://ydo.dianchejie.cn

C#:   await Task.WhenAll(t1, t2)
来源：http://xmi.gzhubu.top

[O06] 使用进程池
来源：http://nvf.yuanzhike.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://dfy.redwolf501.top

PHP:  // pcntl_fork 或多进程队列
来源：http://aiw.sufxvd.cn

JS:   // child_process / cluster 模块
来源：http://vuq.meibo888.top

TS:   // child_process / cluster 模块
来源：http://hun.yueranfly.top

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://bdz.jinyuanbaomall.cn

Go:   // goroutine 已占用多核，直接并发即可
来源：http://eor.vqdsnc.cn

Ruby: // fork 块
来源：http://zmw.zhaomingkeji.xyz

C#:   Parallel.For
来源：http://aur.9152youxi.cn

================================================================================
来源：http://yqx.hongshengwenyu.top

P. 常用工具函数
来源：http://mml.shanyushiyangtech.top

================================================================================
来源：http://oof.gaohongyu789.top

[P01] 生成 UUID
来源：http://mgs.redwolf501.top

Py:   str(uuid.uuid4())
来源：http://jli.birdmap.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://rfp.tianlin.xyz

JS:   crypto.randomUUID()
来源：http://xyw.iojbl.cn

TS:   crypto.randomUUID()
来源：http://kab.c1oappe.top

Java: UUID.randomUUID().toString()
来源：http://vwb.cqqwz.cn

Go:   // 用 github.com/google/uuid
来源：http://edi.hnxiangtu.top

Ruby: SecureRandom.uuid
来源：http://vhg.tanke756.top

C#:   Guid.NewGuid().ToString()
来源：http://skr.zhiwuduotai.top

[P02] MD5 / SHA256 摘要
来源：http://hwn.c1oappe.top

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://pgk.zdqjudy.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://eus.haohaochexian.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://lyv.uphjek.com

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://phj.yj202588.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://ynb.wangdashe.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ipn.quarkkingdee.top

Ruby: Digest::SHA256.hexdigest(s)
来源：http://ikc.9152youxi.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://vfx.yj202588.top

[P03] 生成短随机字符串
来源：http://mei.chenjidiqi.icu

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://onr.hfpthk.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wsu.xingfuxueyuan.xyz

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://qtg.ydjk.org.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://del.pengpengdd.cyou

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jvr.haohaochexian.top

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://hbn.aibaodan.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://bdc.vehdjk.com

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://zhm.snrcjt.cn

[P04] 求长度
来源：http://xbw.birdmap.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bcz.uphjek.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mxi.fanxiaobao.xyz

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wcs.zhiwuduotai.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xcp.mhx1999.top

Java: list.size();  map.size();  s.length()
来源：http://lgd.fktsv.cn

Go:   len(arr);  len(m)
来源：http://epe.shuidangran.top

Ruby: x.length;  x.size
来源：http://aus.9152youxi.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://cbt.zdqjudy.top

[P05] 判断两个对象内容是否相等
来源：http://ghu.jqgfzy.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://zci.yvedp.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://jmi.redwolf501.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://xah.nanxuanxn.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://dyl.bjfxy.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://oqs.gaohongyu789.top

Go:   reflect.DeepEqual(a, b)
来源：http://mbf.jinyuanbaomall.cn

Ruby: a == b
来源：http://kdz.jqgfzy.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://ezc.zhengqikj.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ntt.cashguo.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://yvu.gotoacloud.top

PHP:  if (empty($x)) {}
来源：http://nyh.iojbl.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://gki.ywan-chungtsiang.top

TS:   if (x == null) {}
来源：http://irx.yanxiufei.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://odw.jinyuanbaomall.cn

Go:   if x == nil {}
来源：http://ipw.zhoulong.xyz

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://liy.andypj.xyz

C#:   if (x is null) {}
来源：http://ykm.hysaishi.cn

[P07] 防抖与节流
来源：http://yzh.tian-w.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://nqo.hywenlv.cn

PHP:  // 手写时间戳比较
来源：http://ojr.tarul.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nxa.jyoumei.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://azs.xuanzx.com

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://anz.fanxiaobao.xyz

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://vgo.bjfxy.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://vbp.yj20258.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ows.yvedp.cn

[P08] 处理浮点精度问题
来源：http://ydl.tanke756.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://lcj.52xcode.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://ixk.vqdsnc.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://auq.guannengcc.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://eax.cqqwz.cn

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://tta.quarkkingdee.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://syu.jqgfzy.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://asq.xylfe.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wux.svipenyu.cn

================================================================================
来源：http://umu.xingfuxueyuan.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://nni.xziqi.cn

================================================================================
来源：http://utx.jianghu66.top

[Q01] 创建表
来源：http://gja.aizwys.cn

CREATE TABLE users (
来源：http://mqi.pycfn.com

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://xyh.kuanghao11.cn

name VARCHAR(50) NOT NULL,
来源：http://czd.shanyushiyangkeji.top

email VARCHAR(100) UNIQUE,
来源：http://xfc.cqqwz.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ctf.snrcjt.cn

);
来源：http://kwx.316326.xyz

[Q02] 创建带外键的表
来源：http://lbt.snrcjt.cn

CREATE TABLE orders (
来源：http://rdj.jiagoushi.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ajn.ctjpmb.com

user_id INT NOT NULL,
来源：http://zln.yuxming.cn

amount DECIMAL(10, 2),
来源：http://vxh.kuanghao11.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mwk.sjlbkw.cn

);
来源：http://qqq.ivvv.top

[Q03] 增加列
来源：http://klo.ywan-chungtsiang.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://omn.gaohongyu789.top

[Q04] 修改列类型
来源：http://pfr.jinqigufen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://swy.chenzaomai.com

[Q05] 重命名列
来源：http://iuh.vehdjk.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ssi.zhiwuduotai.top

[Q06] 删除列
来源：http://rjt.zhoulong.xyz

ALTER TABLE users DROP COLUMN age;
来源：http://ore.cqqwz.cn

[Q07] 删除表
来源：http://gvq.zhoulong.xyz

DROP TABLE IF EXISTS orders;
来源：http://sqz.bbcook.cn

[Q08] 创建普通索引
来源：http://kfy.hfpthk.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://fey.yongpay.top

[Q09] 创建唯一索引
来源：http://eqy.9152youxi.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://npj.316326.xyz

[Q10] 插入单行
来源：http://xsd.sxryk.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://cky.xingfuxueyuan.xyz

[Q11] 一次插入多行
来源：http://ydw.zhiwuduotai.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blj.yj202588.top

[Q12] 插入后取自增 ID
来源：http://jzx.shangyingyoupin.top

INSERT INTO users (name) VALUES ('C');
来源：http://exm.tianlin.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://tbj.bbcook.cn

[Q13] 忽略重复插入
来源：http://veb.ydzc1.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ggq.kuanghao11.cn

[Q14] 存在则更新（upsert）
来源：http://wsr.shuidangran.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://xlf.shuidangran.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://qxl.dashuyun.cn

[Q15] 查询全部
来源：http://dqx.zhiwuduotai.top

SELECT * FROM users;
来源：http://kbk.yfazqb.com

[Q16] 查询指定列
来源：http://ght.jinyuanbaomall.cn

SELECT id, name FROM users;
来源：http://qml.yanxiufei.cn

[Q17] 条件查询
来源：http://fok.jianghu66.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://keh.fengsongda.top

[Q18] 模糊匹配
来源：http://lch.zhengqikj.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hvk.fzhhl.top

[Q19] 范围查询
来源：http://ocb.zhoulong.xyz

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ysy.nwbrower.top

[Q20] IN 列表
来源：http://ywg.9152youxi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://yii.hnqzz.top

[Q21] 空值判断
来源：http://htc.jqgufenzy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://bpe.cheryme.top

[Q22] 排序
来源：http://cvq.nanxinkj.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lie.yj202588.top

[Q23] 分页
来源：http://wox.sufxvd.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://tkx.yangfankeji.com

[Q24] 去重
来源：http://bbu.cheryme.top

SELECT DISTINCT city FROM users;
来源：http://nkq.nanxuanxn.top

[Q25] 只取前 N 条
来源：http://gna.iojbl.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://dgl.shanyushiyangtech.top

[Q26] 计数
来源：http://sze.hnqzz.top

SELECT COUNT(*) FROM users;
来源：http://kiw.hnqzz.top

[Q27] 条件计数
来源：http://cxx.hnqzz.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tpy.nwbrower.top

[Q28] 求和与平均
来源：http://qqo.fehbvm.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://peg.guannengcc.top

[Q29] 最大最小值
来源：http://ima.gzhubu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://mwj.svipenyu.cn

[Q30] 分组统计
来源：http://pmi.daria6918.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ocx.quarkkingdee.top

[Q31] 分组后过滤
来源：http://krh.iojbl.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sro.redwolf501.top

[Q32] 分组拼接字符串
来源：http://itp.sysykeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://btd.vqdsnc.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://cmp.ywan-chungtsiang.top

[Q33] 多列分组
来源：http://oaj.wangdashe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://lqj.zycfv.cn

[Q34] 每组取第一条
来源：http://tik.jiagoushi.top

SELECT * FROM (
来源：http://kwz.shanyushiyangtech.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zjx.hcnkem.com

) t WHERE rn = 1;
来源：http://skv.gotoacloud.top

[Q35] 内连接
来源：http://udo.andypj.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yqq.yfazqb.com

[Q36] 左连接
来源：http://bpw.jiagoushi.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ciq.xingfuxueyuan.xyz

[Q37] 右连接
来源：http://qht.ywan-chungtsiang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rug.tanke756.top

[Q38] 全外连接（PostgreSQL）
来源：http://xqd.jinqigufen.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dgv.dashuyun.cn

[Q39] 自连接（查上下级）
来源：http://jqi.epnwcf.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://ysm.zhoulong.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jiz.yvedp.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://gfp.yuanzhike.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://grn.daria6918.cn

[Q41] 多表连接
来源：http://vid.wangshuangyany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://mnk.snrcjt.cn

JOIN users u ON u.id = o.user_id
来源：http://zmz.kuanghao11.cn

JOIN products p ON p.id = o.product_id;
来源：http://wyx.sjlbkw.cn

[Q42] 连接条件附加过滤
来源：http://txh.zhiwuduotai.top

SELECT u.name, o.amount FROM users u
来源：http://urw.jinyuanbaomall.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ypz.vehdjk.com

[Q43] 标量子查询
来源：http://lqj.mhx1999.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mwr.xuanzx.com

[Q44] IN 子查询
来源：http://jqi.zhengqikj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://vkq.vqdsnc.cn

[Q45] EXISTS 判断存在
来源：http://yzp.hywenlv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mem.sweek.top

[Q46] NOT EXISTS 判断不存在
来源：http://dyh.daxiang520.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://uos.chenlongwang.top

[Q47] 与平均值比较
来源：http://jst.gogol.net.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cbp.havefunace.top

[Q48] CTE 公用表表达式
来源：http://nmd.quarkkingdee.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ltp.bjfxy.top

SELECT * FROM t WHERE c > 5;
来源：http://yjz.nanxuanxn.top

[Q49] 更新单行
来源：http://pfu.tanke756.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tja.zhengqikj.top

[Q50] 批量更新
来源：http://uvd.yuxming.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gou.9152youxi.cn

[Q51] 用子查询更新
来源：http://plj.jyoumei.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lzr.hongshengwenyu.top

[Q52] 删除指定行
来源：http://oad.ehwqpu.com

DELETE FROM users WHERE id = 10;
来源：http://fcm.hfpthk.cn

[Q53] 按条件删除
来源：http://jdw.sufxvd.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wsj.hcnkem.com

[Q54] 清空表
来源：http://lvd.shuidangran.top

TRUNCATE TABLE logs;
来源：http://bib.cashguo.top

[Q55] 排名（并列占位）
来源：http://koi.tian-w.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gxp.yuanzhike.top

[Q56] 密集排名（并列不占位）
来源：http://hhp.feifeiyinyue.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dfm.andypj.xyz

[Q57] 行号
来源：http://uaf.chenlongwang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://bmj.fktsv.cn

[Q58] 累计求和
来源：http://chu.xylfe.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ldj.hnqzz.top

[Q59] 分组内累计
来源：http://lhc.yangfankeji.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lpa.tarul.cn

[Q60] 取上一行 / 下一行
来源：http://mse.chenzaomai.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ymc.cashguo.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://trz.wangdashe.top

[Q61] 移动平均
来源：http://qbq.zycfv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gak.dianchejie.cn

[Q62] 分组占比
来源：http://osq.dashuyun.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mlx.gotoacloud.top

[Q63] 开启事务
来源：http://wzl.hongshengwenyu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://aah.sxryk.cn

[Q64] 提交事务
来源：http://zup.cheryme.top

COMMIT;
来源：http://qls.xuanzx.com


<!-- 参考信息 -->