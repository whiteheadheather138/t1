代发 wailian999

Go:   // 手写递归
来源：http://bfr.xuanzx.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://geo.gogol.net.cn

C#:   // 手写递归
来源：http://vkt.ehwqpu.com

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://pbh.daria6918.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://fhg.hesvh.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://lsg.316326.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wtx.zhongyouzk.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jxj.snrcjt.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://eao.hammf.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://bpz.quarkkingdee.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://atm.daxiang520.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://zkq.gaohongyu789.top

================================================================================
来源：http://kri.hnxiangtu.top

O. 并发与异步
来源：http://ctc.aizwys.cn

================================================================================
来源：http://axw.kuanghao11.cn

[O01] 启动一个线程
来源：http://seq.hammf.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://vqn.yueranfly.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://lwc.zhixingplan.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://alj.cqqwz.cn

TS:   // 同 JS
来源：http://ile.yj20258888.top

Java: new Thread(() -> f()).start()
来源：http://pfb.meibo888.top

Go:   go f()
来源：http://wrv.pengpengdd.cyou

Ruby: Thread.new { f }
来源：http://uum.xziqi.cn

C#:   Task.Run(() => F());
来源：http://dgs.tanke756.top

[O02] 使用线程池
来源：http://enb.0kj1m.cn

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dta.9152youxi.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://fcz.jinqigufen.top

JS:   // worker_threads 线程池
来源：http://ayr.ppjwa.cn

TS:   // worker_threads 线程池
来源：http://kty.fktsv.cn

Java: Executors.newFixedThreadPool(4)
来源：http://dsl.shanyushiyangkeji.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://gem.zdbjq.cn

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://bpv.birdmap.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://tlt.kuanghao11.cn

[O03] 加锁保护共享数据
来源：http://tgd.52xcode.cn

Py:   with lock: shared += 1
来源：http://fgb.zhongyouzk.top

PHP:  // 用 flock() 做文件锁
来源：http://ahe.gaohongyu789.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://nwf.tarul.cn

TS:   // 同 JS
来源：http://hfs.jiagoushi.top

Java: synchronized (this) { shared++; }
来源：http://wjn.tanke756.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dhj.yfazqb.com

Ruby: mutex.synchronize { shared += 1 }
来源：http://uud.vqdsnc.cn

C#:   lock (gate) { shared++; }
来源：http://cgx.yj20258.top

[O04] 定义异步函数并等待
来源：http://kux.ehwqpu.com

Py:   async def f():⏎    await g()
来源：http://sua.yvedp.cn

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://zrl.ivvv.top

JS:   async function f() { await g(); }
来源：http://gmz.c1oappe.top

TS:   async function f(): Promise<void> { await g(); }
来源：http://pzt.xuetiantiany.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://lnm.shanyushiyangkeji.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://zdh.gotoacloud.top

Ruby: # 用 Fiber 或 async gem
来源：http://ylh.hnxiangtu.top

C#:   async Task F() { await G(); }
来源：http://wje.kuanghao11.cn

[O05] 并发执行并等待全部完成
来源：http://kig.chenjidiqi.icu

Py:   asyncio.gather(*tasks)
来源：http://tvz.guannengcc.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://jja.iojbl.cn

JS:   await Promise.all(tasks)
来源：http://kfn.ydzc1.top

TS:   await Promise.all(tasks)
来源：http://gwv.guowangkeji.top

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://prd.xziqi.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://zui.sysykeji.top

Ruby: threads.map(&:join)
来源：http://noz.fengsongda.top

C#:   await Task.WhenAll(t1, t2)
来源：http://cns.gogol.net.cn

[O06] 使用进程池
来源：http://qlz.bjfxy.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://yft.wangdashe.top

PHP:  // pcntl_fork 或多进程队列
来源：http://qrn.pengpengdd.cyou

JS:   // child_process / cluster 模块
来源：http://ksi.jinyuanbaomall.cn

TS:   // child_process / cluster 模块
来源：http://ezf.ppjwa.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://ubw.gzhubu.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://krj.ehwqpu.com

Ruby: // fork 块
来源：http://jyq.guannengcc.top

C#:   Parallel.For
来源：http://rry.fktsv.cn

================================================================================
来源：http://chq.shanyushiyangkeji.top

P. 常用工具函数
来源：http://dzt.andypj.xyz

================================================================================
来源：http://ktz.ybcxt.top

[P01] 生成 UUID
来源：http://vgf.uphjek.com

Py:   str(uuid.uuid4())
来源：http://otu.bjfxy.top

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://laf.chenjidiqi.icu

JS:   crypto.randomUUID()
来源：http://vzg.guowangkeji.top

TS:   crypto.randomUUID()
来源：http://zrv.jyoumei.cn

Java: UUID.randomUUID().toString()
来源：http://yiz.birdmap.top

Go:   // 用 github.com/google/uuid
来源：http://vnu.jianghu66.top

Ruby: SecureRandom.uuid
来源：http://jml.jinyuanbaomall.cn

C#:   Guid.NewGuid().ToString()
来源：http://gwb.zhijiandao.cn

[P02] MD5 / SHA256 摘要
来源：http://ksu.uphjek.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://bog.ywan-chungtsiang.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://jyg.chenzaomai.com

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://iuu.0kj1m.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://rrk.havefunace.top

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://zfr.fehbvm.com

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://kqn.ppjwa.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://cgz.yvedp.cn

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://ewl.fktsv.cn

[P03] 生成短随机字符串
来源：http://apm.hnxiangtu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://rea.9152youxi.cn

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://hee.gzhubu.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://vyw.haohaochexian.top

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://cuq.9152youxi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://cbq.svipenyu.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wbu.9152youxi.cn

Ruby: SecureRandom.alphanumeric(16)
来源：http://tcr.jinyuanbaomall.cn

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://gel.yonumen.top

[P04] 求长度
来源：http://zkm.ydzc1.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://bhn.tian-w.cn

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://iut.nanxinkj.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wqa.zhixingplan.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://syl.hysaishi.cn

Java: list.size();  map.size();  s.length()
来源：http://qsf.0kj1m.cn

Go:   len(arr);  len(m)
来源：http://oel.sweek.top

Ruby: x.length;  x.size
来源：http://awt.wangdashe.top

C#:   list.Count;  dict.Count;  s.Length
来源：http://ern.zhiwuduotai.top

[P05] 判断两个对象内容是否相等
来源：http://fwo.pycfn.com

Py:   a == b              # 列表与字典递归比较内容
来源：http://nzn.yueranfly.top

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://dcf.shanyushiyangtech.top

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://uhr.daria6918.cn

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wrn.cucudq.cn

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mtb.fktsv.cn

Go:   reflect.DeepEqual(a, b)
来源：http://ism.cdnleiting.top

Ruby: a == b
来源：http://uvv.jinyuanbaomall.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://zsg.cheryme.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://bpk.hfpthk.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://rnp.ydjk.org.cn

PHP:  if (empty($x)) {}
来源：http://bkp.fzhhl.top

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://pdw.tarul.cn

TS:   if (x == null) {}
来源：http://lrn.snrcjt.cn

Java: if (x == null || x.isEmpty()) {}
来源：http://vsh.jinyuanbaomall.cn

Go:   if x == nil {}
来源：http://mnk.yangfankeji.com

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://hps.yuanzhike.top

C#:   if (x is null) {}
来源：http://wcs.daxiang520.top

[P07] 防抖与节流
来源：http://ydy.cqqwz.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://yqj.shzxlz.cn

PHP:  // 手写时间戳比较
来源：http://qtw.c1oappe.top

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://klh.9152youxi.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://pie.hfpthk.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://qoq.nanxinkj.top

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://sym.daxiang520.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://zsm.zdqjudy.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://iuu.zhaomingkeji.xyz

[P08] 处理浮点精度问题
来源：http://imo.gotoacloud.top

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mmq.xinyue.icu

PHP:  bcadd("0.1", "0.2", 2);
来源：http://xbx.jianghu66.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://kba.gogol.net.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xxd.jinqigfzy.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://ybl.bjfxy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qoh.cheryme.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://bnk.sjlbkw.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mbd.sxryk.cn

================================================================================
来源：http://zru.cucudq.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://air.cqqwz.cn

================================================================================
来源：http://mhf.yuxming.cn

[Q01] 创建表
来源：http://clu.gogol.net.cn

CREATE TABLE users (
来源：http://vpy.hfpthk.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://vay.meibo888.top

name VARCHAR(50) NOT NULL,
来源：http://rhd.cucudq.cn

email VARCHAR(100) UNIQUE,
来源：http://ffm.hcnkem.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mye.gogol.net.cn

);
来源：http://vus.ywan-chungtsiang.top

[Q02] 创建带外键的表
来源：http://uqz.aibaodan.cn

CREATE TABLE orders (
来源：http://gmj.uphjek.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ofx.yuxming.cn

user_id INT NOT NULL,
来源：http://bzy.yonumen.top

amount DECIMAL(10, 2),
来源：http://fbi.jinqigufen.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://prh.yueranfly.top

);
来源：http://uei.cashguo.top

[Q03] 增加列
来源：http://kyg.sufxvd.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://vxw.zhongyouzk.top

[Q04] 修改列类型
来源：http://avi.guowangkeji.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mhr.ivvv.top

[Q05] 重命名列
来源：http://luy.fengsongda.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rrx.tanke756.top

[Q06] 删除列
来源：http://bpp.feifeiyinyue.top

ALTER TABLE users DROP COLUMN age;
来源：http://vxr.kuanghao11.cn

[Q07] 删除表
来源：http://cwp.kuanghao11.cn

DROP TABLE IF EXISTS orders;
来源：http://kbn.chenjidiqi.icu

[Q08] 创建普通索引
来源：http://svh.dianchejie.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://lpj.yj20258.top

[Q09] 创建唯一索引
来源：http://gbx.fengsongda.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://aes.hcnkem.com

[Q10] 插入单行
来源：http://frx.guowangkeji.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zgd.shanyushiyangkeji.top

[Q11] 一次插入多行
来源：http://yvd.jqgufenzy.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://lzh.yanxiufei.cn

[Q12] 插入后取自增 ID
来源：http://sqt.zycfv.cn

INSERT INTO users (name) VALUES ('C');
来源：http://oqz.hcnkem.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://qyu.chenlongwang.top

[Q13] 忽略重复插入
来源：http://urk.9152youxi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://odr.gaohongyu789.top

[Q14] 存在则更新（upsert）
来源：http://eaz.birdmap.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://qid.xziqi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rfu.pengpengdd.cyou

[Q15] 查询全部
来源：http://sxe.aizwys.cn

SELECT * FROM users;
来源：http://pua.fanxiaobao.xyz

[Q16] 查询指定列
来源：http://yub.yj20258888.top

SELECT id, name FROM users;
来源：http://ihn.yvedp.cn

[Q17] 条件查询
来源：http://lxg.shanyushiyangtech.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://tdr.jqgufenzy.top

[Q18] 模糊匹配
来源：http://ztd.svipenyu.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kpk.xylfe.cn

[Q19] 范围查询
来源：http://cpm.jinghuilouyu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://lok.sweek.top

[Q20] IN 列表
来源：http://pis.birdmap.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://xrs.aizwys.cn

[Q21] 空值判断
来源：http://yzs.ydjk.org.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://bpj.nwbrower.top

[Q22] 排序
来源：http://lun.yueranfly.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ydt.shangyingyoupin.top

[Q23] 分页
来源：http://btv.chenjidiqi.icu

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mmv.tanke756.top

[Q24] 去重
来源：http://otn.hnxiangtu.top

SELECT DISTINCT city FROM users;
来源：http://qlm.vqdsnc.cn

[Q25] 只取前 N 条
来源：http://krr.jiagoushi.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bir.hywenlv.cn

[Q26] 计数
来源：http://omy.xingfuxueyuan.xyz

SELECT COUNT(*) FROM users;
来源：http://ycx.mhx1999.top

[Q27] 条件计数
来源：http://onh.hnxiangtu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://psl.iojbl.cn

[Q28] 求和与平均
来源：http://pgi.snrcjt.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dxw.jinqigufen.top

[Q29] 最大最小值
来源：http://rsv.quarkkingdee.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ewk.fanxiaobao.xyz

[Q30] 分组统计
来源：http://lbb.shanyushiyangtech.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lsb.shanyushiyangkeji.top

[Q31] 分组后过滤
来源：http://ldd.jlsjyb.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zfi.hongshengwenyu.top

[Q32] 分组拼接字符串
来源：http://xws.jlsjyb.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rez.zhijiandao.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jni.c1oappe.top

[Q33] 多列分组
来源：http://mdu.shanyushiyangkeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://qhh.zhoulong.xyz

[Q34] 每组取第一条
来源：http://xsj.jiagoushi.top

SELECT * FROM (
来源：http://hhn.jiagoushi.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vag.snrcjt.cn

) t WHERE rn = 1;
来源：http://yfs.nwbrower.top

[Q35] 内连接
来源：http://nbq.tarul.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ubb.chenjidiqi.icu

[Q36] 左连接
来源：http://bnv.9152youxi.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bzk.tarul.cn

[Q37] 右连接
来源：http://uxw.snrcjt.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xxu.shuidangran.top

[Q38] 全外连接（PostgreSQL）
来源：http://xkm.shuidangran.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://vgt.meibo888.top

[Q39] 自连接（查上下级）
来源：http://hzi.havefunace.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rop.fanxiaobao.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uoc.yj202588.top

[Q40] 交叉连接（笛卡尔积）
来源：http://wys.guowangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hwk.chenzaomai.com

[Q41] 多表连接
来源：http://eph.birdmap.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zcr.meibo888.top

JOIN users u ON u.id = o.user_id
来源：http://nja.sysykeji.top

JOIN products p ON p.id = o.product_id;
来源：http://sny.hnxiangtu.top

[Q42] 连接条件附加过滤
来源：http://jue.ydjk.org.cn

SELECT u.name, o.amount FROM users u
来源：http://tvo.xylfe.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wdh.shanyushiyangkeji.top

[Q43] 标量子查询
来源：http://brx.hesvh.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jfq.meibo888.top

[Q44] IN 子查询
来源：http://zzu.zdbjq.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xak.jinyuanbaomall.cn

[Q45] EXISTS 判断存在
来源：http://gzj.iojbl.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lhh.wangdashe.top

[Q46] NOT EXISTS 判断不存在
来源：http://zmv.gzhubu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nrm.jqgfzy.top

[Q47] 与平均值比较
来源：http://iep.aibaodan.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qyf.zhaomingkeji.xyz

[Q48] CTE 公用表表达式
来源：http://jmp.shanyushiyangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wfp.havefunace.top

SELECT * FROM t WHERE c > 5;
来源：http://zwg.ybcxt.top

[Q49] 更新单行
来源：http://sue.yj20258888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://icc.ehwqpu.com

[Q50] 批量更新
来源：http://aoq.fktsv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ozy.sysykeji.top

[Q51] 用子查询更新
来源：http://vqi.zhengqikj.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jni.yonumen.top

[Q52] 删除指定行
来源：http://ecs.gzhubu.top

DELETE FROM users WHERE id = 10;
来源：http://yul.ehwqpu.com

[Q53] 按条件删除
来源：http://nyf.hcnkem.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ggh.sysykeji.top

[Q54] 清空表
来源：http://vah.9152youxi.cn

TRUNCATE TABLE logs;
来源：http://foe.yj20258888.top

[Q55] 排名（并列占位）
来源：http://rbp.hnxiangtu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zfp.hcnkem.com

[Q56] 密集排名（并列不占位）
来源：http://eiw.xuanzx.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kub.mhx1999.top

[Q57] 行号
来源：http://bay.zhijiandao.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://aue.ppjwa.cn

[Q58] 累计求和
来源：http://fob.sjlbkw.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jpd.nanxinkj.top

[Q59] 分组内累计
来源：http://hlq.xziqi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jda.zhaomingkeji.xyz

[Q60] 取上一行 / 下一行
来源：http://wtg.dianchejie.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://crr.ydzc1.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jym.uphjek.com

[Q61] 移动平均
来源：http://pie.tarul.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cwa.cqqwz.cn

[Q62] 分组占比
来源：http://asg.jinghuilouyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rgn.uphjek.com

[Q63] 开启事务
来源：http://ivg.wangshuangyany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vrb.zhixingplan.top

[Q64] 提交事务
来源：http://lpi.epnwcf.com

COMMIT;
来源：http://vdh.sjlbkw.cn

[Q65] 回滚事务
来源：http://iiy.kuanghao11.cn

ROLLBACK;
来源：http://xad.hysaishi.cn

[Q66] 行锁查询
来源：http://hsk.daria6918.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tyw.tian-w.cn


<!-- 参考信息 -->