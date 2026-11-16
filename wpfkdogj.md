代发 wailian999

PHP:  // 手写递归函数
来源：http://uko.jinghuilouyu.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://yjc.ivvv.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://eru.jinqigfzy.top

Java: // 手写递归
来源：http://xfa.cheryme.top

Go:   // 手写递归
来源：http://jvg.yj202588.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://xel.xingfuxueyuan.xyz

C#:   // 手写递归
来源：http://rhm.nwbrower.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://owl.pengpengdd.cyou

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://elj.cqqwz.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kph.0kj1m.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://vui.ivvv.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jcy.fanxiaobao.xyz

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://pfz.shzxlz.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wee.zhongyouzk.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://auc.wangdashe.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://tho.fehbvm.com

================================================================================
来源：http://kyb.cucudq.cn

O. 并发与异步
来源：http://urx.ivvv.top

================================================================================
来源：http://cqi.tianlin.xyz

[O01] 启动一个线程
来源：http://xwf.bbcook.cn

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://viu.ppjwa.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://snv.quarkkingdee.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nsj.yangfankeji.com

TS:   // 同 JS
来源：http://goq.chenjidiqi.icu

Java: new Thread(() -> f()).start()
来源：http://gnv.chenjidiqi.icu

Go:   go f()
来源：http://clz.yanxiufei.cn

Ruby: Thread.new { f }
来源：http://ntt.hnqzz.top

C#:   Task.Run(() => F());
来源：http://lfg.ctjpmb.com

[O02] 使用线程池
来源：http://upg.nwbrower.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://hxv.fanxiaobao.xyz

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mmw.zdbjq.cn

JS:   // worker_threads 线程池
来源：http://vgs.ctjpmb.com

TS:   // worker_threads 线程池
来源：http://uju.cucudq.cn

Java: Executors.newFixedThreadPool(4)
来源：http://ptz.haohaochexian.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://uxk.ehwqpu.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://dbf.fengsongda.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://jgk.guannengcc.top

[O03] 加锁保护共享数据
来源：http://uhf.shzxlz.cn

Py:   with lock: shared += 1
来源：http://kzw.ppjwa.cn

PHP:  // 用 flock() 做文件锁
来源：http://ldy.jinqigufen.top

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://qbk.jianghu66.top

TS:   // 同 JS
来源：http://eur.xinyue.icu

Java: synchronized (this) { shared++; }
来源：http://vyv.kuanghao11.cn

Go:   mu.Lock();  defer mu.Unlock()
来源：http://bte.guannengcc.top

Ruby: mutex.synchronize { shared += 1 }
来源：http://rdr.cucudq.cn

C#:   lock (gate) { shared++; }
来源：http://cvo.yonumen.top

[O04] 定义异步函数并等待
来源：http://fta.jinghuilouyu.cn

Py:   async def f():⏎    await g()
来源：http://udl.quarkkingdee.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yvu.xinyue.icu

JS:   async function f() { await g(); }
来源：http://dpn.9152youxi.cn

TS:   async function f(): Promise<void> { await g(); }
来源：http://wco.ybcxt.top

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kew.c1oappe.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://ehj.shzxlz.cn

Ruby: # 用 Fiber 或 async gem
来源：http://zhf.zhijiandao.cn

C#:   async Task F() { await G(); }
来源：http://rdz.shzxlz.cn

[O05] 并发执行并等待全部完成
来源：http://hxc.xuetiantiany.cn

Py:   asyncio.gather(*tasks)
来源：http://lxe.jinqigfzy.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://fht.xinyue.icu

JS:   await Promise.all(tasks)
来源：http://jrj.yongpay.top

TS:   await Promise.all(tasks)
来源：http://ohq.svipenyu.cn

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wcb.daria6918.cn

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://pjn.haohaochexian.top

Ruby: threads.map(&:join)
来源：http://ghz.ybcxt.top

C#:   await Task.WhenAll(t1, t2)
来源：http://cbw.redwolf501.top

[O06] 使用进程池
来源：http://idc.zycfv.cn

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://xto.9152youxi.cn

PHP:  // pcntl_fork 或多进程队列
来源：http://wjo.yanxiufei.cn

JS:   // child_process / cluster 模块
来源：http://jma.zhijiandao.cn

TS:   // child_process / cluster 模块
来源：http://sdm.jyoumei.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://iwd.yonumen.top

Go:   // goroutine 已占用多核，直接并发即可
来源：http://zmq.52xcode.cn

Ruby: // fork 块
来源：http://bvz.xziqi.cn

C#:   Parallel.For
来源：http://fft.hfpthk.cn

================================================================================
来源：http://vxy.uphjek.com

P. 常用工具函数
来源：http://qxg.smart0.xyz

================================================================================
来源：http://cey.jianghu66.top

[P01] 生成 UUID
来源：http://gea.fzhhl.top

Py:   str(uuid.uuid4())
来源：http://nwc.0kj1m.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wlc.xylfe.cn

JS:   crypto.randomUUID()
来源：http://ciw.xinyue.icu

TS:   crypto.randomUUID()
来源：http://ywf.ybcxt.top

Java: UUID.randomUUID().toString()
来源：http://tlp.zdqjudy.top

Go:   // 用 github.com/google/uuid
来源：http://flm.jqgufenzy.top

Ruby: SecureRandom.uuid
来源：http://buq.sweek.top

C#:   Guid.NewGuid().ToString()
来源：http://tdt.xziqi.cn

[P02] MD5 / SHA256 摘要
来源：http://ugy.ehwqpu.com

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://ftg.nanxinkj.top

PHP:  hash("sha256", $s);  md5($s);
来源：http://faw.birdmap.top

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://exp.bjfxy.top

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://hnc.hesvh.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://bwz.cashguo.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://ngs.ydjk.org.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://yeh.c1oappe.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://dew.bbcook.cn

[P03] 生成短随机字符串
来源：http://mvt.dashuyun.cn

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wrq.quarkkingdee.top

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wkr.ctjpmb.com

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://xpp.shzxlz.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://msx.fzhhl.top

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://gal.smart0.xyz

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://exf.chenjidiqi.icu

Ruby: SecureRandom.alphanumeric(16)
来源：http://bjk.fanxiaobao.xyz

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://hgb.zdbjq.cn

[P04] 求长度
来源：http://sot.gzhubu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://nek.cdnleiting.top

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zrh.sysykeji.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://ggg.hongshengwenyu.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://xlq.ybcxt.top

Java: list.size();  map.size();  s.length()
来源：http://pod.jinqigfzy.top

Go:   len(arr);  len(m)
来源：http://sqs.aibaodan.cn

Ruby: x.length;  x.size
来源：http://yrt.aizwys.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ygw.chenzaomai.com

[P05] 判断两个对象内容是否相等
来源：http://qvu.guowangkeji.top

Py:   a == b              # 列表与字典递归比较内容
来源：http://jke.snrcjt.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://qkr.epnwcf.com

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://are.jqgufenzy.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://xon.nanxuanxn.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://bwy.yj20258.top

Go:   reflect.DeepEqual(a, b)
来源：http://icv.epnwcf.com

Ruby: a == b
来源：http://ppe.yj202588.top

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://eoq.smart0.xyz

[P06] 综合判空（null / 空串 / 空集合）
来源：http://nxq.fktsv.cn

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://ues.wangshuangyany.cn

PHP:  if (empty($x)) {}
来源：http://tdx.andypj.xyz

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mui.yanxiufei.cn

TS:   if (x == null) {}
来源：http://ybc.jiagoushi.top

Java: if (x == null || x.isEmpty()) {}
来源：http://bmn.316326.xyz

Go:   if x == nil {}
来源：http://bxs.jinqigufen.top

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://qlb.vqdsnc.cn

C#:   if (x is null) {}
来源：http://rmz.vehdjk.com

[P07] 防抖与节流
来源：http://ixf.bbcook.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://vuy.hongshengwenyu.top

PHP:  // 手写时间戳比较
来源：http://fzb.yanxiufei.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nzf.sweek.top

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://nta.yuxming.cn

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://tis.wangshuangyany.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://anu.aibaodan.cn

Ruby: // 手写闭包 + Time.now 判断
来源：http://fgh.zhiwuduotai.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://agi.haohaochexian.top

[P08] 处理浮点精度问题
来源：http://efi.jinghuilouyu.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://ytd.cashguo.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://usc.52xcode.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://cmk.tanke756.top

TS:   (0.1 + 0.2).toFixed(2)
来源：http://pkp.yangfankeji.com

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://yje.zhixingplan.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qya.nwbrower.top

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://cwt.yj20258.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ygu.sufxvd.cn

================================================================================
来源：http://gqv.uphjek.com

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mdb.yj20258888.top

================================================================================
来源：http://ckh.ybcxt.top

[Q01] 创建表
来源：http://wcr.ppjwa.cn

CREATE TABLE users (
来源：http://fbe.birdmap.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bgk.shangyingyoupin.top

name VARCHAR(50) NOT NULL,
来源：http://xrc.ctjpmb.com

email VARCHAR(100) UNIQUE,
来源：http://bma.jianghu66.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://gev.jyoumei.cn

);
来源：http://hvt.dashuyun.cn

[Q02] 创建带外键的表
来源：http://fci.guannengcc.top

CREATE TABLE orders (
来源：http://snf.cqqwz.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ton.cucudq.cn

user_id INT NOT NULL,
来源：http://lpq.jyoumei.cn

amount DECIMAL(10, 2),
来源：http://zct.quarkkingdee.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://nap.hammf.cn

);
来源：http://amu.xuetiantiany.cn

[Q03] 增加列
来源：http://ktz.tian-w.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://swa.gotoacloud.top

[Q04] 修改列类型
来源：http://agg.sxryk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kqz.cheryme.top

[Q05] 重命名列
来源：http://dwo.jqgufenzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://lhp.quarkkingdee.top

[Q06] 删除列
来源：http://odu.ydjk.org.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bju.guowangkeji.top

[Q07] 删除表
来源：http://bio.wangshuangyany.cn

DROP TABLE IF EXISTS orders;
来源：http://gdn.yuanzhike.top

[Q08] 创建普通索引
来源：http://ewi.sysykeji.top

CREATE INDEX idx_users_email ON users(email);
来源：http://trp.wangdashe.top

[Q09] 创建唯一索引
来源：http://hds.jlsjyb.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wwd.svipenyu.cn

[Q10] 插入单行
来源：http://ukd.jinghuilouyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fdy.hysaishi.cn

[Q11] 一次插入多行
来源：http://add.meibo888.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ael.52xcode.cn

[Q12] 插入后取自增 ID
来源：http://rfd.tianlin.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://fjd.shanyushiyangkeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ghn.ydzc1.top

[Q13] 忽略重复插入
来源：http://qwt.gaohongyu789.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fze.52xcode.cn

[Q14] 存在则更新（upsert）
来源：http://use.jqgfzy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cnx.xziqi.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kcd.shanyushiyangkeji.top

[Q15] 查询全部
来源：http://neq.yvedp.cn

SELECT * FROM users;
来源：http://yoe.zhengqikj.top

[Q16] 查询指定列
来源：http://tdn.fehbvm.com

SELECT id, name FROM users;
来源：http://edr.pengpengdd.cyou

[Q17] 条件查询
来源：http://qkm.birdmap.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zal.316326.xyz

[Q18] 模糊匹配
来源：http://ncl.hywenlv.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bqh.yvedp.cn

[Q19] 范围查询
来源：http://vye.cheryme.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rfa.pycfn.com

[Q20] IN 列表
来源：http://zsh.mhx1999.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://boa.hcnkem.com

[Q21] 空值判断
来源：http://ufn.xylfe.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://nua.9152youxi.cn

[Q22] 排序
来源：http://oyq.fanxiaobao.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://glt.epnwcf.com

[Q23] 分页
来源：http://mmy.kuanghao11.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://ufm.svipenyu.cn

[Q24] 去重
来源：http://wbq.andypj.xyz

SELECT DISTINCT city FROM users;
来源：http://atg.mhx1999.top

[Q25] 只取前 N 条
来源：http://uue.jinyuanbaomall.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ldu.uphjek.com

[Q26] 计数
来源：http://iup.daria6918.cn

SELECT COUNT(*) FROM users;
来源：http://udq.yj20258.top

[Q27] 条件计数
来源：http://brw.guowangkeji.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ipk.daria6918.cn

[Q28] 求和与平均
来源：http://rby.hcnkem.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://huw.cheryme.top

[Q29] 最大最小值
来源：http://psw.sweek.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://opg.jianghu66.top

[Q30] 分组统计
来源：http://xed.nanxinkj.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lgg.316326.xyz

[Q31] 分组后过滤
来源：http://qlt.9152youxi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://vcp.havefunace.top

[Q32] 分组拼接字符串
来源：http://npj.9152youxi.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://pot.sxryk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rxz.iojbl.cn

[Q33] 多列分组
来源：http://bmx.zhengqikj.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wal.ehwqpu.com

[Q34] 每组取第一条
来源：http://vpg.ydzc1.top

SELECT * FROM (
来源：http://fbn.svipenyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xfk.svipenyu.cn

) t WHERE rn = 1;
来源：http://kim.hfpthk.cn

[Q35] 内连接
来源：http://opg.jinyuanbaomall.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://uqv.jyoumei.cn

[Q36] 左连接
来源：http://sbi.wangshuangyany.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qqs.ctjpmb.com

[Q37] 右连接
来源：http://mzg.gaohongyu789.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bse.yfazqb.com

[Q38] 全外连接（PostgreSQL）
来源：http://rft.yj202588.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://iks.sweek.top

[Q39] 自连接（查上下级）
来源：http://oer.andypj.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://var.sweek.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://yxq.shzxlz.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pkv.zhaomingkeji.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fps.sweek.top

[Q41] 多表连接
来源：http://cfw.hfpthk.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://lir.hnqzz.top

JOIN users u ON u.id = o.user_id
来源：http://cld.meibo888.top

JOIN products p ON p.id = o.product_id;
来源：http://bao.hnxiangtu.top

[Q42] 连接条件附加过滤
来源：http://ftr.birdmap.top

SELECT u.name, o.amount FROM users u
来源：http://tfo.hnqzz.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://xws.zdqjudy.top

[Q43] 标量子查询
来源：http://btw.hywenlv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vmb.zhixingplan.top

[Q44] IN 子查询
来源：http://kfr.hnqzz.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://sww.cqqwz.cn

[Q45] EXISTS 判断存在
来源：http://nwe.jinqigfzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mgq.daria6918.cn

[Q46] NOT EXISTS 判断不存在
来源：http://xus.shuidangran.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oxn.yongpay.top

[Q47] 与平均值比较
来源：http://woi.fehbvm.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://syp.pengpengdd.cyou

[Q48] CTE 公用表表达式
来源：http://aep.smart0.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://thq.cashguo.top

SELECT * FROM t WHERE c > 5;
来源：http://vvc.jinqigfzy.top

[Q49] 更新单行
来源：http://tep.guowangkeji.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rfj.meibo888.top

[Q50] 批量更新
来源：http://woh.havefunace.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xls.shzxlz.cn

[Q51] 用子查询更新
来源：http://ahq.zhixingplan.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://sid.hywenlv.cn

[Q52] 删除指定行
来源：http://wgd.xuanzx.com

DELETE FROM users WHERE id = 10;
来源：http://ldb.kuanghao11.cn

[Q53] 按条件删除
来源：http://hmj.tanke756.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://adv.zhixingplan.top

[Q54] 清空表
来源：http://xri.pengpengdd.cyou

TRUNCATE TABLE logs;
来源：http://njb.jyoumei.cn

[Q55] 排名（并列占位）
来源：http://bkl.jlsjyb.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rhf.daxiang520.top

[Q56] 密集排名（并列不占位）
来源：http://lws.jinqigufen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rtg.yj20258.top

[Q57] 行号
来源：http://yqx.kuanghao11.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wkb.fanxiaobao.xyz

[Q58] 累计求和
来源：http://ybn.sxryk.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hac.ydjk.org.cn

[Q59] 分组内累计
来源：http://cqc.hesvh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://err.guowangkeji.top

[Q60] 取上一行 / 下一行
来源：http://kaj.shzxlz.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hlh.nanxinkj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kqh.pycfn.com

[Q61] 移动平均
来源：http://nsl.zdqjudy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dhk.zhixingplan.top

[Q62] 分组占比
来源：http://ofe.birdmap.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wzf.shzxlz.cn

[Q63] 开启事务
来源：http://ljl.cucudq.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://suo.zdqjudy.top

[Q64] 提交事务
来源：http://rdo.cashguo.top

COMMIT;
来源：http://wvy.redwolf501.top


<!-- 参考信息 -->