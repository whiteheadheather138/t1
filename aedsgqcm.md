代发 wailian999

PHP:  // 手写递归函数
来源：http://wfz.daria6918.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://iyu.zhaomingkeji.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ggv.xylfe.cn

Java: // 手写递归
来源：http://lcu.nwbrower.top

Go:   // 手写递归
来源：http://kmv.xingfuxueyuan.xyz

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://shh.ybcxt.top

C#:   // 手写递归
来源：http://zqg.cqqwz.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mqi.sufxvd.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://tfr.cashguo.top

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://cwv.hammf.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://jre.dianchejie.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://bgo.epnwcf.com

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://bay.yuanzhike.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://len.guowangkeji.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://jyk.yj20258888.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://swp.yanxiufei.cn

================================================================================
来源：http://hup.gzhubu.top

O. 并发与异步
来源：http://pvv.zhongyouzk.top

================================================================================
来源：http://fsm.yuxming.cn

[O01] 启动一个线程
来源：http://grm.tanke756.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://qgu.cdnleiting.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://bks.yj20258.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://nco.yj20258.top

TS:   // 同 JS
来源：http://ykm.yj20258888.top

Java: new Thread(() -> f()).start()
来源：http://cqw.shuidangran.top

Go:   go f()
来源：http://ppq.xinyue.icu

Ruby: Thread.new { f }
来源：http://tsf.aizwys.cn

C#:   Task.Run(() => F());
来源：http://aog.cucudq.cn

[O02] 使用线程池
来源：http://lup.yonumen.top

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://dva.wangshuangyany.cn

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://rlt.tanke756.top

JS:   // worker_threads 线程池
来源：http://bnj.tian-w.cn

TS:   // worker_threads 线程池
来源：http://edo.shzxlz.cn

Java: Executors.newFixedThreadPool(4)
来源：http://bns.mhx1999.top

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://kfv.yfazqb.com

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://orb.redwolf501.top

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://lkj.hnqzz.top

[O03] 加锁保护共享数据
来源：http://cem.jqgfzy.top

Py:   with lock: shared += 1
来源：http://iqt.tian-w.cn

PHP:  // 用 flock() 做文件锁
来源：http://jal.xuetiantiany.cn

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://gxw.wangdashe.top

TS:   // 同 JS
来源：http://ncp.sxryk.cn

Java: synchronized (this) { shared++; }
来源：http://zbi.wangdashe.top

Go:   mu.Lock();  defer mu.Unlock()
来源：http://dhn.snrcjt.cn

Ruby: mutex.synchronize { shared += 1 }
来源：http://zxf.dianchejie.cn

C#:   lock (gate) { shared++; }
来源：http://cfy.jqgfzy.top

[O04] 定义异步函数并等待
来源：http://xjn.sweek.top

Py:   async def f():⏎    await g()
来源：http://ywj.shangyingyoupin.top

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://yms.cdnleiting.top

JS:   async function f() { await g(); }
来源：http://lqm.pengpengdd.cyou

TS:   async function f(): Promise<void> { await g(); }
来源：http://nii.gogol.net.cn

Java: // 用 CompletableFuture 或虚拟线程
来源：http://kyt.zhengqikj.top

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://lsm.snrcjt.cn

Ruby: # 用 Fiber 或 async gem
来源：http://gai.shzxlz.cn

C#:   async Task F() { await G(); }
来源：http://ltn.zdqjudy.top

[O05] 并发执行并等待全部完成
来源：http://qoc.shanyushiyangkeji.top

Py:   asyncio.gather(*tasks)
来源：http://you.cdnleiting.top

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://pio.ppjwa.cn

JS:   await Promise.all(tasks)
来源：http://jii.fktsv.cn

TS:   await Promise.all(tasks)
来源：http://kam.tianlin.xyz

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://lpz.pycfn.com

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://dxg.fktsv.cn

Ruby: threads.map(&:join)
来源：http://wxr.hnxiangtu.top

C#:   await Task.WhenAll(t1, t2)
来源：http://dhj.cdnleiting.top

[O06] 使用进程池
来源：http://jhs.cashguo.top

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://jgb.birdmap.top

PHP:  // pcntl_fork 或多进程队列
来源：http://csr.iojbl.cn

JS:   // child_process / cluster 模块
来源：http://qaq.zhixingplan.top

TS:   // child_process / cluster 模块
来源：http://axq.daria6918.cn

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://cjx.zhoulong.xyz

Go:   // goroutine 已占用多核，直接并发即可
来源：http://bnf.jinghuilouyu.cn

Ruby: // fork 块
来源：http://dmn.xuanzx.com

C#:   Parallel.For
来源：http://swd.kuanghao11.cn

================================================================================
来源：http://ioq.tian-w.cn

P. 常用工具函数
来源：http://gne.aizwys.cn

================================================================================
来源：http://tui.fktsv.cn

[P01] 生成 UUID
来源：http://lvy.birdmap.top

Py:   str(uuid.uuid4())
来源：http://ouy.jinghuilouyu.cn

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://uak.jiagoushi.top

JS:   crypto.randomUUID()
来源：http://xpv.zhijiandao.cn

TS:   crypto.randomUUID()
来源：http://ayi.feifeiyinyue.top

Java: UUID.randomUUID().toString()
来源：http://owu.vqdsnc.cn

Go:   // 用 github.com/google/uuid
来源：http://zft.52xcode.cn

Ruby: SecureRandom.uuid
来源：http://ycd.hysaishi.cn

C#:   Guid.NewGuid().ToString()
来源：http://guj.zycfv.cn

[P02] MD5 / SHA256 摘要
来源：http://erq.hammf.cn

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://eol.hesvh.cn

PHP:  hash("sha256", $s);  md5($s);
来源：http://iba.dianchejie.cn

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://jzx.shzxlz.cn

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://prj.svipenyu.cn

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://gos.cashguo.top

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://nri.zhijiandao.cn

Ruby: Digest::SHA256.hexdigest(s)
来源：http://bjf.shangyingyoupin.top

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://tdi.shanyushiyangkeji.top

[P03] 生成短随机字符串
来源：http://uhr.gzhubu.top

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://dwj.xuanzx.com

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://qnm.shanyushiyangkeji.top

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://css.zhijiandao.cn

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://hhv.9152youxi.cn

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://jve.wangshuangyany.cn

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://imo.uphjek.com

Ruby: SecureRandom.alphanumeric(16)
来源：http://bkt.yuanzhike.top

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://can.dashuyun.cn

[P04] 求长度
来源：http://rqr.hnxiangtu.top

Py:   len(x)            # 字符串、列表、字典通用
来源：http://hgt.chenzaomai.com

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hxr.yonumen.top

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://jgw.c1oappe.top

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wre.nwbrower.top

Java: list.size();  map.size();  s.length()
来源：http://oln.zhaomingkeji.xyz

Go:   len(arr);  len(m)
来源：http://mwy.sjlbkw.cn

Ruby: x.length;  x.size
来源：http://ylk.bbcook.cn

C#:   list.Count;  dict.Count;  s.Length
来源：http://ftz.jiagoushi.top

[P05] 判断两个对象内容是否相等
来源：http://rjd.zhaomingkeji.xyz

Py:   a == b              # 列表与字典递归比较内容
来源：http://nux.wangshuangyany.cn

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://rvf.hfpthk.cn

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://zjc.ydzc1.top

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://uzz.tanke756.top

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://puj.vehdjk.com

Go:   reflect.DeepEqual(a, b)
来源：http://ape.zhixingplan.top

Ruby: a == b
来源：http://tmq.zhijiandao.cn

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wcp.nanxuanxn.top

[P06] 综合判空（null / 空串 / 空集合）
来源：http://ydu.birdmap.top

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://upf.nanxuanxn.top

PHP:  if (empty($x)) {}
来源：http://dcr.tarul.cn

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://xlc.fanxiaobao.xyz

TS:   if (x == null) {}
来源：http://eps.yangfankeji.com

Java: if (x == null || x.isEmpty()) {}
来源：http://pnp.pengpengdd.cyou

Go:   if x == nil {}
来源：http://xef.cqqwz.cn

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://dnt.zycfv.cn

C#:   if (x is null) {}
来源：http://aem.yj20258.top

[P07] 防抖与节流
来源：http://sny.jinyuanbaomall.cn

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://sul.zhixingplan.top

PHP:  // 手写时间戳比较
来源：http://uer.sufxvd.cn

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://qtg.tian-w.cn

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://lyv.daxiang520.top

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://gxe.fktsv.cn

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://kce.nwbrower.top

Ruby: // 手写闭包 + Time.now 判断
来源：http://wfs.jianghu66.top

C#:   // 用 System.Timers.Timer 重置实现
来源：http://ruy.guannengcc.top

[P08] 处理浮点精度问题
来源：http://iht.zdbjq.cn

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gos.hfpthk.cn

PHP:  bcadd("0.1", "0.2", 2);
来源：http://cmp.hesvh.cn

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://uly.jlsjyb.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://xnw.ivvv.top

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://pmp.jqgfzy.top

Go:   math/big.Float，或全部换算成整数分再算
来源：http://qyi.xuetiantiany.cn

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mcj.zhengqikj.top

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://acr.mhx1999.top

================================================================================
来源：http://why.hysaishi.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wkc.sufxvd.cn

================================================================================
来源：http://ivj.zycfv.cn

[Q01] 创建表
来源：http://vqo.fzhhl.top

CREATE TABLE users (
来源：http://afz.jinghuilouyu.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://dgw.tarul.cn

name VARCHAR(50) NOT NULL,
来源：http://qll.yongpay.top

email VARCHAR(100) UNIQUE,
来源：http://agd.vehdjk.com

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mfu.ehwqpu.com

);
来源：http://cvc.tian-w.cn

[Q02] 创建带外键的表
来源：http://gph.hfpthk.cn

CREATE TABLE orders (
来源：http://uhr.zycfv.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gqj.chenlongwang.top

user_id INT NOT NULL,
来源：http://lmp.uphjek.com

amount DECIMAL(10, 2),
来源：http://oeb.hywenlv.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mku.cucudq.cn

);
来源：http://qsn.mhx1999.top

[Q03] 增加列
来源：http://lft.xziqi.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://zaq.xinyue.icu

[Q04] 修改列类型
来源：http://bvm.ybcxt.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://yfh.fengsongda.top

[Q05] 重命名列
来源：http://fer.feifeiyinyue.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cyg.jinyuanbaomall.cn

[Q06] 删除列
来源：http://xfd.hongshengwenyu.top

ALTER TABLE users DROP COLUMN age;
来源：http://grs.fehbvm.com

[Q07] 删除表
来源：http://njj.wangshuangyany.cn

DROP TABLE IF EXISTS orders;
来源：http://ljc.yj20258.top

[Q08] 创建普通索引
来源：http://khw.ppjwa.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://jue.tarul.cn

[Q09] 创建唯一索引
来源：http://dur.fengsongda.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ykh.aibaodan.cn

[Q10] 插入单行
来源：http://ocx.cucudq.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://elv.yj20258.top

[Q11] 一次插入多行
来源：http://tcw.tian-w.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://sht.guannengcc.top

[Q12] 插入后取自增 ID
来源：http://vjg.shanyushiyangtech.top

INSERT INTO users (name) VALUES ('C');
来源：http://wqd.snrcjt.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kuz.zhaomingkeji.xyz

[Q13] 忽略重复插入
来源：http://wab.cheryme.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fcy.jinghuilouyu.cn

[Q14] 存在则更新（upsert）
来源：http://flp.sxryk.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://efb.nanxuanxn.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ngk.tanke756.top

[Q15] 查询全部
来源：http://eyu.shuidangran.top

SELECT * FROM users;
来源：http://iel.gogol.net.cn

[Q16] 查询指定列
来源：http://ecf.hesvh.cn

SELECT id, name FROM users;
来源：http://xzf.hcnkem.com

[Q17] 条件查询
来源：http://xnu.pengpengdd.cyou

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://udm.dashuyun.cn

[Q18] 模糊匹配
来源：http://shi.sjlbkw.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kkn.chenjidiqi.icu

[Q19] 范围查询
来源：http://btf.yuanzhike.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nqo.zhongyouzk.top

[Q20] IN 列表
来源：http://dvk.xinyue.icu

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://bse.haohaochexian.top

[Q21] 空值判断
来源：http://mek.zhengqikj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ehi.ywan-chungtsiang.top

[Q22] 排序
来源：http://iso.redwolf501.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://tot.fanxiaobao.xyz

[Q23] 分页
来源：http://vym.fehbvm.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://eyu.dashuyun.cn

[Q24] 去重
来源：http://bvf.guowangkeji.top

SELECT DISTINCT city FROM users;
来源：http://cns.meibo888.top

[Q25] 只取前 N 条
来源：http://fbi.fanxiaobao.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nfj.zhaomingkeji.xyz

[Q26] 计数
来源：http://vuq.tanke756.top

SELECT COUNT(*) FROM users;
来源：http://ami.fzhhl.top

[Q27] 条件计数
来源：http://ftb.yuanzhike.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mhr.yangfankeji.com

[Q28] 求和与平均
来源：http://boo.cashguo.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fcx.zycfv.cn

[Q29] 最大最小值
来源：http://dwf.quarkkingdee.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jnh.jqgufenzy.top

[Q30] 分组统计
来源：http://npf.52xcode.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ioi.nanxinkj.top

[Q31] 分组后过滤
来源：http://aqy.hysaishi.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dxe.hfpthk.cn

[Q32] 分组拼接字符串
来源：http://bco.shanyushiyangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qjw.zdqjudy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fpr.wangdashe.top

[Q33] 多列分组
来源：http://rtq.bbcook.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rdr.sysykeji.top

[Q34] 每组取第一条
来源：http://nkx.quarkkingdee.top

SELECT * FROM (
来源：http://dwo.andypj.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://pvo.uphjek.com

) t WHERE rn = 1;
来源：http://sxg.zhixingplan.top

[Q35] 内连接
来源：http://jbl.chenjidiqi.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://cby.yueranfly.top

[Q36] 左连接
来源：http://ngl.redwolf501.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://pbm.jinqigfzy.top

[Q37] 右连接
来源：http://vwf.guannengcc.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kii.jqgfzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://khy.zhengqikj.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://fvz.shzxlz.cn

[Q39] 自连接（查上下级）
来源：http://ncc.haohaochexian.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://kvu.uphjek.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mhx.xylfe.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://uuk.yj20258.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zts.yj20258.top

[Q41] 多表连接
来源：http://imj.jianghu66.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bod.ybcxt.top

JOIN users u ON u.id = o.user_id
来源：http://gyd.sjlbkw.cn

JOIN products p ON p.id = o.product_id;
来源：http://vru.shanyushiyangtech.top

[Q42] 连接条件附加过滤
来源：http://xrz.hywenlv.cn

SELECT u.name, o.amount FROM users u
来源：http://dke.ydjk.org.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ifq.tian-w.cn

[Q43] 标量子查询
来源：http://aru.nwbrower.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://iwp.yonumen.top

[Q44] IN 子查询
来源：http://uzo.xylfe.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://pzx.c1oappe.top

[Q45] EXISTS 判断存在
来源：http://mcv.mhx1999.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ifb.hfpthk.cn

[Q46] NOT EXISTS 判断不存在
来源：http://ylx.0kj1m.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gxm.nwbrower.top

[Q47] 与平均值比较
来源：http://amx.gaohongyu789.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ihg.yvedp.cn

[Q48] CTE 公用表表达式
来源：http://odh.xuetiantiany.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ter.jyoumei.cn

SELECT * FROM t WHERE c > 5;
来源：http://llf.ywan-chungtsiang.top

[Q49] 更新单行
来源：http://kuu.52xcode.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hpv.sufxvd.cn

[Q50] 批量更新
来源：http://puf.ppjwa.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cfw.shuidangran.top

[Q51] 用子查询更新
来源：http://yvr.cucudq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://nlx.sweek.top

[Q52] 删除指定行
来源：http://obl.bjfxy.top

DELETE FROM users WHERE id = 10;
来源：http://lnu.hnxiangtu.top

[Q53] 按条件删除
来源：http://hjm.iojbl.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mbf.xinyue.icu

[Q54] 清空表
来源：http://ltu.cdnleiting.top

TRUNCATE TABLE logs;
来源：http://mfw.yj20258888.top

[Q55] 排名（并列占位）
来源：http://ihf.yj20258.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://krn.sjlbkw.cn

[Q56] 密集排名（并列不占位）
来源：http://qay.wangdashe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rur.sxryk.cn

[Q57] 行号
来源：http://kvk.nanxinkj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ajd.tian-w.cn

[Q58] 累计求和
来源：http://ouc.havefunace.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vgt.cashguo.top

[Q59] 分组内累计
来源：http://kzs.hywenlv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dfp.yuxming.cn

[Q60] 取上一行 / 下一行
来源：http://pct.hammf.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jmp.zycfv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nhu.shanyushiyangtech.top

[Q61] 移动平均
来源：http://vgg.sxryk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ktd.zhongyouzk.top

[Q62] 分组占比
来源：http://ytf.nanxuanxn.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rgj.hongshengwenyu.top

[Q63] 开启事务
来源：http://afa.sjlbkw.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vzl.jianghu66.top

[Q64] 提交事务
来源：http://ijj.zdbjq.cn

COMMIT;
来源：http://uut.zhijiandao.cn


<!-- 参考信息 -->